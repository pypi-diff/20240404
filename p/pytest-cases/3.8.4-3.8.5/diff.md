# Comparing `tmp/pytest-cases-3.8.4.tar.gz` & `tmp/pytest-cases-3.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-cases-3.8.4.tar", last modified: Sat Mar 16 01:22:45 2024, max compression
+gzip compressed data, was "pytest-cases-3.8.5.tar", last modified: Thu Apr  4 21:28:24 2024, max compression
```

## Comparing `pytest-cases-3.8.4.tar` & `pytest-cases-3.8.5.tar`

### file list

```diff
@@ -1,292 +1,292 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.487744 pytest-cases-3.8.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.439744 pytest-cases-3.8.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.447744 pytest-cases-3.8.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/.github/workflows/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/.github/workflows/updater.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-03-16 01:22:45.487744 pytest-cases-3.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.447744 pytest-cases-3.8.4/ci_tools/
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/ci_tools/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/ci_tools/check_python_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/ci_tools/flake8-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/ci_tools/github_release.py
--rw-r--r--   0 runner    (1001) docker     (127)    30467 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/ci_tools/nox_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.447744 pytest-cases-3.8.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    37751 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/api_reference.md
--rw-r--r--   0 runner    (1001) docker     (127)    50825 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/examples.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.451744 pytest-cases-3.8.4/docs/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)    30199 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/imgs/0_bench_plots_example.png
--rw-r--r--   0 runner    (1001) docker     (127)   125834 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/imgs/0_bench_plots_example2.png
--rw-r--r--   0 runner    (1001) docker     (127)   154533 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/imgs/0_bench_plots_example3.png
--rw-r--r--   0 runner    (1001) docker     (127)   169153 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/imgs/0_bench_plots_example4.png
--rw-r--r--   0 runner    (1001) docker     (127)    21812 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/imgs/0_dummy_bench_results.png
--rw-r--r--   0 runner    (1001) docker     (127)    46959 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/imgs/1_files_overview.png
--rw-r--r--   0 runner    (1001) docker     (127)    48279 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/imgs/2_class_overview.png
--rw-r--r--   0 runner    (1001) docker     (127)    37954 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/imgs/3_fixture_graph_pytest.png
--rw-r--r--   0 runner    (1001) docker     (127)    81311 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/imgs/4_fixture_graph_pytest_closure.png
--rw-r--r--   0 runner    (1001) docker     (127)    44481 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/imgs/5_fixture_graph_union.png
--rw-r--r--   0 runner    (1001) docker     (127)   132008 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/imgs/6_fixture_graph_union_closures.png
--rw-r--r--   0 runner    (1001) docker     (127)    81052 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/imgs/source.pptx
--rw-r--r--   0 runner    (1001) docker     (127)    33122 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/long_description.md
--rw-r--r--   0 runner    (1001) docker     (127)    15700 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/pytest_goodies.md
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/docs/unions_theory.md
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/noxfile-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-16 01:22:45.487744 pytest-cases-3.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.443744 pytest-cases-3.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.455744 pytest-cases-3.8.4/src/pytest_cases/
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-16 01:22:45.000000 pytest-cases-3.8.4/src/pytest_cases/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13986 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/case_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    64296 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/case_parametrizer_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/common_mini_six.py
--rw-r--r--   0 runner    (1001) docker     (127)    22294 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/common_others.py
--rw-r--r--   0 runner    (1001) docker     (127)    34191 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/common_pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)    22901 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/common_pytest_lazy_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    12979 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/common_pytest_marks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/fixture__creation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/fixture_core1_unions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28376 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/fixture_core2.py
--rw-r--r--   0 runner    (1001) docker     (127)    70777 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/fixture_parametrize_plus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/pep380.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/pep492.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/pep525.py
--rw-r--r--   0 runner    (1001) docker     (127)    71963 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/src/pytest_cases/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.487744 pytest-cases-3.8.4/src/pytest_cases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-03-16 01:22:45.000000 pytest-cases-3.8.4/src/pytest_cases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-03-16 01:22:45.000000 pytest-cases-3.8.4/src/pytest_cases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 01:22:45.000000 pytest-cases-3.8.4/src/pytest_cases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-16 01:22:45.000000 pytest-cases-3.8.4/src/pytest_cases.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 01:22:36.000000 pytest-cases-3.8.4/src/pytest_cases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-16 01:22:45.000000 pytest-cases-3.8.4/src/pytest_cases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-16 01:22:45.000000 pytest-cases-3.8.4/src/pytest_cases.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.455744 pytest-cases-3.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.459744 pytest-cases-3.8.4/tests/cases/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.459744 pytest-cases-3.8.4/tests/cases/doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/cases_doc_alternate.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_doc_alternate.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_doc_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_doc_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_doc_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_doc_filters_n_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_doc_filters_n_tags2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_doc_get_current_case_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_doc_get_current_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_doc_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_get_current_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_get_current_cases_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_get_current_cases_negative.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_get_current_cases_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_indirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_joss.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/doc/test_parametrize_alt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.467744 pytest-cases-3.8.4/tests/cases/issues/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.467744 pytest-cases-3.8.4/tests/cases/issues/issue_196/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_196/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_196/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_196/test_issue_196.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.467744 pytest-cases-3.8.4/tests/cases/issues/issue_225/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_225/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_225/cases.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_225/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_225/test_sth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.467744 pytest-cases-3.8.4/tests/cases/issues/issue_258/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_258/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_258/cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_258/cases_issue_258.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_258/cases_other.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_258/test_issue_258.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_258/test_other.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.471744 pytest-cases-3.8.4/tests/cases/issues/issue_309/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_309/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_309/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_309/test_issue_309.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.471744 pytest-cases-3.8.4/tests/cases/issues/issue_311/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_311/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_311/cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_311/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.471744 pytest-cases-3.8.4/tests/cases/issues/issue_311/test_issue_311/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_311/test_issue_311/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_311/test_issue_311/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/issue_311/test_issue_311/test_issue_311.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_117.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_125.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_126.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_126_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_126_2_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_128_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_128_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_142.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_142_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_151.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_152.py
--rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_154.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_158.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_158_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_159.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_165.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_168.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_171.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_179.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_190.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_191.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_193.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_193_bis.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_193_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_202.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_211.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_212.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_230.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_238.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_242.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_246.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_274.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_issue_286.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_py35_issue_176.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_py35_issue_243.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_py35_issue_286.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_py35_issue_287.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/issues/test_py36_issue_286.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.471744 pytest-cases-3.8.4/tests/cases/others/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/others/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/others/test_bound_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/others/test_glob_low_level.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.471744 pytest-cases-3.8.4/tests/cases/so/
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/so/test_so2.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/so/test_so3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/cases/so/test_so4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.471744 pytest-cases-3.8.4/tests/pytest_extension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.471744 pytest-cases-3.8.4/tests/pytest_extension/doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/doc/test_doc_fixture_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/doc/test_doc_fixture_graph_union.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/doc/test_doc_fixture_graph_union_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/doc/test_doc_fixture_graph_union_union.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/doc/test_doc_parametrize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/doc/test_doc_parametrize_customids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.471744 pytest-cases-3.8.4/tests/pytest_extension/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.475744 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixture_unpacking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixture_unpacking2.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixture_unpacking_cls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_parametrize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_parametrize_stereo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_paramfixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_paramfixtures_marks.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_skip_on_paramz_fixture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.475744 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixture_closure_edits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_custom_mark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_setup_teardown.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_setup_teardown2.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_setup_teardown3.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_0simplest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_1simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_2hard.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_3parametrize_plus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_so.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/test_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/test_issue_github_54.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/fixtures/test_so3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.479744 pytest-cases-3.8.4/tests/pytest_extension/issues/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_114.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_115.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_124.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_137.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_138.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_146.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_148.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_149.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_177.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_182.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_199.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_201.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_234.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_269.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_doctests.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_fixture_union1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_fixture_union2.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_indirect_fixture_param.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_pytest_70.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_python2_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_so_76.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_parametrize_with_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/issues/test_pytest_py35_asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.479744 pytest-cases-3.8.4/tests/pytest_extension/meta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.479744 pytest-cases-3.8.4/tests/pytest_extension/meta/raw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/meta/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.479744 pytest-cases-3.8.4/tests/pytest_extension/meta/raw/reorder_skip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/meta/raw/reorder_skip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/meta/raw/reorder_skip/cmdargs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/meta/raw/reorder_skip/reorder_skip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.483744 pytest-cases-3.8.4/tests/pytest_extension/meta/raw/session_optim/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/meta/raw/session_optim/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/meta/raw/session_optim/session_optim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.483744 pytest-cases-3.8.4/tests/pytest_extension/meta/raw/xfail_marker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/meta/raw/xfail_marker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/meta/raw/xfail_marker/cmdargs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/meta/raw/xfail_marker/xfail_marker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/meta/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.483744 pytest-cases-3.8.4/tests/pytest_extension/order/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.483744 pytest-cases-3.8.4/tests/pytest_extension/order/session_optim/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/order/session_optim/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/order/session_optim/test_reorder_default_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/order/test_fixture_order_respects_scope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.483744 pytest-cases-3.8.4/tests/pytest_extension/others/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/others/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/others/test_assert_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:45.487744 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_basics_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic3_tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic4_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom4_tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_getcallspecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value__custom_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value_and_fixture_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value_and_fixture_ref2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value_and_fixture_ref3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value_low_level.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value_so.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_parametrizing_a_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_so2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_so2_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_so2_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_so2_simplified.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/test_plugin_installed.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-16 01:22:14.000000 pytest-cases-3.8.4/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.059785 pytest-cases-3.8.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.011785 pytest-cases-3.8.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.019786 pytest-cases-3.8.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/.github/workflows/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/.github/workflows/updater.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-04 21:28:24.059785 pytest-cases-3.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.019786 pytest-cases-3.8.5/ci_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/ci_tools/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/ci_tools/check_python_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/ci_tools/flake8-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/ci_tools/github_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30467 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/ci_tools/nox_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.019786 pytest-cases-3.8.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    37751 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/api_reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)    51031 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/examples.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.023785 pytest-cases-3.8.5/docs/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)    30199 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/imgs/0_bench_plots_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)   125834 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/imgs/0_bench_plots_example2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   154533 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/imgs/0_bench_plots_example3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   169153 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/imgs/0_bench_plots_example4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21812 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/imgs/0_dummy_bench_results.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46959 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/imgs/1_files_overview.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48279 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/imgs/2_class_overview.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37954 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/imgs/3_fixture_graph_pytest.png
+-rw-r--r--   0 runner    (1001) docker     (127)    81311 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/imgs/4_fixture_graph_pytest_closure.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44481 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/imgs/5_fixture_graph_union.png
+-rw-r--r--   0 runner    (1001) docker     (127)   132008 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/imgs/6_fixture_graph_union_closures.png
+-rw-r--r--   0 runner    (1001) docker     (127)    81052 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/imgs/source.pptx
+-rw-r--r--   0 runner    (1001) docker     (127)    33122 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/long_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15700 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/pytest_goodies.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/docs/unions_theory.md
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/noxfile-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-04 21:28:24.059785 pytest-cases-3.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.015785 pytest-cases-3.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.027785 pytest-cases-3.8.5/src/pytest_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 21:28:23.000000 pytest-cases-3.8.5/src/pytest_cases/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13986 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/case_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64296 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/case_parametrizer_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/common_mini_six.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22294 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/common_others.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34191 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/common_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22901 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/common_pytest_lazy_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/common_pytest_marks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/fixture__creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/fixture_core1_unions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28420 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/fixture_core2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70777 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/fixture_parametrize_plus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/pep380.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/pep492.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/pep525.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71963 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/src/pytest_cases/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.059785 pytest-cases-3.8.5/src/pytest_cases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-04 21:28:23.000000 pytest-cases-3.8.5/src/pytest_cases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-04-04 21:28:24.000000 pytest-cases-3.8.5/src/pytest_cases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:28:23.000000 pytest-cases-3.8.5/src/pytest_cases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 21:28:23.000000 pytest-cases-3.8.5/src/pytest_cases.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:28:17.000000 pytest-cases-3.8.5/src/pytest_cases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 21:28:23.000000 pytest-cases-3.8.5/src/pytest_cases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 21:28:23.000000 pytest-cases-3.8.5/src/pytest_cases.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.027785 pytest-cases-3.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.027785 pytest-cases-3.8.5/tests/cases/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.031785 pytest-cases-3.8.5/tests/cases/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/cases_doc_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_doc_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_doc_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_doc_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_doc_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_doc_filters_n_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_doc_filters_n_tags2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_doc_get_current_case_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_doc_get_current_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_doc_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_get_current_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_get_current_cases_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_get_current_cases_negative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_get_current_cases_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_indirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_joss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/doc/test_parametrize_alt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.039785 pytest-cases-3.8.5/tests/cases/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.039785 pytest-cases-3.8.5/tests/cases/issues/issue_196/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_196/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_196/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_196/test_issue_196.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.039785 pytest-cases-3.8.5/tests/cases/issues/issue_225/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_225/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_225/cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_225/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_225/test_sth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.039785 pytest-cases-3.8.5/tests/cases/issues/issue_258/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_258/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_258/cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_258/cases_issue_258.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_258/cases_other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_258/test_issue_258.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_258/test_other.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.039785 pytest-cases-3.8.5/tests/cases/issues/issue_309/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_309/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_309/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_309/test_issue_309.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.043785 pytest-cases-3.8.5/tests/cases/issues/issue_311/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_311/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_311/cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_311/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.043785 pytest-cases-3.8.5/tests/cases/issues/issue_311/test_issue_311/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_311/test_issue_311/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_311/test_issue_311/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/issue_311/test_issue_311/test_issue_311.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_117.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_125.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_126.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_126_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_126_2_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_128_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_128_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_142.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_142_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_151.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_152.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_154.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_158.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_158_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_159.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_165.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_168.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_171.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_179.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_190.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_191.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_193.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_193_bis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_193_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_202.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_211.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_212.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_230.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_238.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_242.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_246.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_274.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_issue_286.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_py35_issue_176.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_py35_issue_243.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_py35_issue_286.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_py35_issue_287.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/issues/test_py36_issue_286.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.043785 pytest-cases-3.8.5/tests/cases/others/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/others/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/others/test_bound_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/others/test_glob_low_level.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.043785 pytest-cases-3.8.5/tests/cases/so/
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/so/test_so2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/so/test_so3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/cases/so/test_so4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.043785 pytest-cases-3.8.5/tests/pytest_extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.043785 pytest-cases-3.8.5/tests/pytest_extension/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/doc/test_doc_fixture_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/doc/test_doc_fixture_graph_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/doc/test_doc_fixture_graph_union_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/doc/test_doc_fixture_graph_union_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/doc/test_doc_parametrize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/doc/test_doc_parametrize_customids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.043785 pytest-cases-3.8.5/tests/pytest_extension/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.047786 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixture_unpacking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixture_unpacking2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixture_unpacking_cls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_parametrize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_parametrize_stereo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_paramfixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_paramfixtures_marks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_skip_on_paramz_fixture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.047786 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixture_closure_edits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_custom_mark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_setup_teardown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_setup_teardown2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_setup_teardown3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_0simplest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_1simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_2hard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_3parametrize_plus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_so.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/test_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/test_issue_github_54.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/fixtures/test_so3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.051786 pytest-cases-3.8.5/tests/pytest_extension/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_114.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_115.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_124.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_137.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_138.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_146.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_148.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_149.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_177.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_182.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_199.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_201.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_234.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_269.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_fixture_union1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_fixture_union2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_indirect_fixture_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_pytest_70.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_python2_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_so_76.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_parametrize_with_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/issues/test_pytest_py35_asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.051786 pytest-cases-3.8.5/tests/pytest_extension/meta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.051786 pytest-cases-3.8.5/tests/pytest_extension/meta/raw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/meta/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.051786 pytest-cases-3.8.5/tests/pytest_extension/meta/raw/reorder_skip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/meta/raw/reorder_skip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/meta/raw/reorder_skip/cmdargs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/meta/raw/reorder_skip/reorder_skip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.051786 pytest-cases-3.8.5/tests/pytest_extension/meta/raw/session_optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/meta/raw/session_optim/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/meta/raw/session_optim/session_optim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.055786 pytest-cases-3.8.5/tests/pytest_extension/meta/raw/xfail_marker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/meta/raw/xfail_marker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/meta/raw/xfail_marker/cmdargs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/meta/raw/xfail_marker/xfail_marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/meta/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.055786 pytest-cases-3.8.5/tests/pytest_extension/order/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.055786 pytest-cases-3.8.5/tests/pytest_extension/order/session_optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/order/session_optim/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/order/session_optim/test_reorder_default_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/order/test_fixture_order_respects_scope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.055786 pytest-cases-3.8.5/tests/pytest_extension/others/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/others/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/others/test_assert_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:24.059785 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_basics_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic3_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic4_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom4_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_getcallspecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value__custom_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value_and_fixture_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value_and_fixture_ref2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value_and_fixture_ref3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value_low_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value_so.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_parametrizing_a_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_so2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_so2_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_so2_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_so2_simplified.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/test_plugin_installed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-04 21:28:00.000000 pytest-cases-3.8.5/tests/utils.py
```

### Comparing `pytest-cases-3.8.4/.github/workflows/base.yml` & `pytest-cases-3.8.5/.github/workflows/base.yml`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/.github/workflows/updater.yml` & `pytest-cases-3.8.5/.github/workflows/updater.yml`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/.gitignore` & `pytest-cases-3.8.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/.zenodo.json` & `pytest-cases-3.8.5/.zenodo.json`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/LICENSE` & `pytest-cases-3.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/PKG-INFO` & `pytest-cases-3.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pytest-cases
-Version: 3.8.4
+Version: 3.8.5
 Summary: Separate test code from test cases in pytest.
 Home-page: https://github.com/smarie/python-pytest-cases
-Download-URL: https://github.com/smarie/python-pytest-cases/tarball/3.8.4
+Download-URL: https://github.com/smarie/python-pytest-cases/tarball/3.8.5
 Author: Sylvain MARIE <sylvain.marie@se.com>
 Maintainer: Sylvain MARIE <sylvain.marie@se.com>
 License: BSD 3-Clause
 Keywords: pytest test case testcase test-case decorator parametrize parameter data dataset file separate concerns lazy fixture union
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pytest-cases-3.8.4/README.md` & `pytest-cases-3.8.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pytest-cases
 
 Separate test code from test cases in `pytest`.
 
-[![Python versions](https://img.shields.io/pypi/pyversions/pytest-cases.svg)](https://pypi.python.org/pypi/pytest-cases/) ![Pytest versions](https://img.shields.io/badge/pytest-2%20%7C%203%20%7C%204%20%7C%205%20%7C%206%20%7C%207-blue) [![Build Status](https://github.com/smarie/python-pytest-cases/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pytest-cases/actions/workflows/base.yml) [![Tests Status](https://smarie.github.io/python-pytest-cases/reports/junit/junit-badge.svg?dummy=8484744)](https://smarie.github.io/python-pytest-cases/reports/junit/report.html) [![Coverage Status](https://smarie.github.io/python-pytest-cases/reports/coverage/coverage-badge.svg?dummy=8484744)](https://smarie.github.io/python-pytest-cases/reports/coverage/index.html) [![codecov](https://codecov.io/gh/smarie/python-pytest-cases/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pytest-cases) [![Flake8 Status](https://smarie.github.io/python-pytest-cases/reports/flake8/flake8-badge.svg?dummy=8484744)](https://smarie.github.io/python-pytest-cases/reports/flake8/index.html)
+[![Python versions](https://img.shields.io/pypi/pyversions/pytest-cases.svg)](https://pypi.python.org/pypi/pytest-cases/) ![Pytest versions](https://img.shields.io/badge/pytest-3%20%7C%204%20%7C%205%20%7C%206%20%7C%207%20%7C%208-blue) [![Build Status](https://github.com/smarie/python-pytest-cases/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pytest-cases/actions/workflows/base.yml) [![Tests Status](https://smarie.github.io/python-pytest-cases/reports/junit/junit-badge.svg?dummy=8484744)](https://smarie.github.io/python-pytest-cases/reports/junit/report.html) [![Coverage Status](https://smarie.github.io/python-pytest-cases/reports/coverage/coverage-badge.svg?dummy=8484744)](https://smarie.github.io/python-pytest-cases/reports/coverage/index.html) [![codecov](https://codecov.io/gh/smarie/python-pytest-cases/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pytest-cases) [![Flake8 Status](https://smarie.github.io/python-pytest-cases/reports/flake8/flake8-badge.svg?dummy=8484744)](https://smarie.github.io/python-pytest-cases/reports/flake8/index.html)
 
 [![Documentation](https://img.shields.io/badge/doc-latest-blue.svg)](https://smarie.github.io/python-pytest-cases/) [![PyPI](https://img.shields.io/pypi/v/pytest-cases.svg)](https://pypi.python.org/pypi/pytest-cases/) [![Downloads](https://pepy.tech/badge/pytest-cases)](https://pepy.tech/project/pytest-cases) [![Downloads per week](https://pepy.tech/badge/pytest-cases/week)](https://pepy.tech/project/pytest-cases) [![GitHub stars](https://img.shields.io/github/stars/smarie/python-pytest-cases.svg)](https://github.com/smarie/python-pytest-cases/stargazers) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3937829.svg)](https://doi.org/10.5281/zenodo.3937829)
 
 **This is the readme for developers.** The documentation for users is available here: [https://smarie.github.io/python-pytest-cases/](https://smarie.github.io/python-pytest-cases/)
 
 ## Want to contribute ?
```

### Comparing `pytest-cases-3.8.4/ci_tools/.pylintrc` & `pytest-cases-3.8.5/ci_tools/.pylintrc`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/ci_tools/check_python_version.py` & `pytest-cases-3.8.5/ci_tools/check_python_version.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/ci_tools/github_release.py` & `pytest-cases-3.8.5/ci_tools/github_release.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/ci_tools/nox_utils.py` & `pytest-cases-3.8.5/ci_tools/nox_utils.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/api_reference.md` & `pytest-cases-3.8.5/docs/api_reference.md`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/changelog.md` & `pytest-cases-3.8.5/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+### 3.8.5 - Suppressed annoying warning with pytest 8
+
+- Fixed `PytestRemovedIn9Warning: Marks applied to fixtures have no effect`. Fixed
+  [#337](https://github.com/smarie/python-pytest-cases/issues/337)
+
 ### 3.8.4 - Removed debug logs
 
 - Reverted `DEBUG` flag used for pytest 8 compatibility. Fixed
   [#336](https://github.com/smarie/python-pytest-cases/issues/336)
 
 ### 3.8.3 - Support for `pytest` version 8
```

### Comparing `pytest-cases-3.8.4/docs/imgs/0_bench_plots_example.png` & `pytest-cases-3.8.5/docs/imgs/0_bench_plots_example.png`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/imgs/0_bench_plots_example2.png` & `pytest-cases-3.8.5/docs/imgs/0_bench_plots_example2.png`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/imgs/0_bench_plots_example3.png` & `pytest-cases-3.8.5/docs/imgs/0_bench_plots_example3.png`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/imgs/0_bench_plots_example4.png` & `pytest-cases-3.8.5/docs/imgs/0_bench_plots_example4.png`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/imgs/0_dummy_bench_results.png` & `pytest-cases-3.8.5/docs/imgs/0_dummy_bench_results.png`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/imgs/1_files_overview.png` & `pytest-cases-3.8.5/docs/imgs/1_files_overview.png`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/imgs/2_class_overview.png` & `pytest-cases-3.8.5/docs/imgs/2_class_overview.png`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/imgs/3_fixture_graph_pytest.png` & `pytest-cases-3.8.5/docs/imgs/3_fixture_graph_pytest.png`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/imgs/4_fixture_graph_pytest_closure.png` & `pytest-cases-3.8.5/docs/imgs/4_fixture_graph_pytest_closure.png`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/imgs/5_fixture_graph_union.png` & `pytest-cases-3.8.5/docs/imgs/5_fixture_graph_union.png`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/imgs/6_fixture_graph_union_closures.png` & `pytest-cases-3.8.5/docs/imgs/6_fixture_graph_union_closures.png`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/imgs/source.pptx` & `pytest-cases-3.8.5/docs/imgs/source.pptx`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/index.md` & `pytest-cases-3.8.5/docs/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pytest-cases
 
 *Separate test code from test cases in `pytest`.*
 
-[![Python versions](https://img.shields.io/pypi/pyversions/pytest-cases.svg)](https://pypi.python.org/pypi/pytest-cases/) ![Pytest versions](https://img.shields.io/badge/pytest-2%20%7C%203%20%7C%204%20%7C%205%20%7C%206%20%7C%207-blue) [![Build Status](https://github.com/smarie/python-pytest-cases/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pytest-cases/actions/workflows/base.yml)  [![Tests Status](./reports/junit/junit-badge.svg?dummy=8484744)](./reports/junit/report.html) [![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744)](./reports/coverage/index.html) [![codecov](https://codecov.io/gh/smarie/python-pytest-cases/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pytest-cases) [![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744)](./reports/flake8/index.html)
+[![Python versions](https://img.shields.io/pypi/pyversions/pytest-cases.svg)](https://pypi.python.org/pypi/pytest-cases/) ![Pytest versions](https://img.shields.io/badge/pytest-3%20%7C%204%20%7C%205%20%7C%206%20%7C%207%20%7C%208-blue) [![Build Status](https://github.com/smarie/python-pytest-cases/actions/workflows/base.yml/badge.svg)](https://github.com/smarie/python-pytest-cases/actions/workflows/base.yml)  [![Tests Status](./reports/junit/junit-badge.svg?dummy=8484744)](./reports/junit/report.html) [![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744)](./reports/coverage/index.html) [![codecov](https://codecov.io/gh/smarie/python-pytest-cases/branch/main/graph/badge.svg)](https://codecov.io/gh/smarie/python-pytest-cases) [![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744)](./reports/flake8/index.html)
 
 [![Documentation](https://img.shields.io/badge/doc-latest-blue.svg)](https://smarie.github.io/python-pytest-cases/) [![PyPI](https://img.shields.io/pypi/v/pytest-cases.svg)](https://pypi.python.org/pypi/pytest-cases/) [![Downloads](https://pepy.tech/badge/pytest-cases)](https://pepy.tech/project/pytest-cases) [![Downloads per week](https://pepy.tech/badge/pytest-cases/week)](https://pepy.tech/project/pytest-cases) [![GitHub stars](https://img.shields.io/github/stars/smarie/python-pytest-cases.svg)](https://github.com/smarie/python-pytest-cases/stargazers)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3937829.svg)](https://doi.org/10.5281/zenodo.3937829)
 
 !!! success "Slides from the `pytest-cases` presentation at EuroPython 2021 are now [available here](https://ep2021.europython.eu/talks/649sqwq-powerful-tests-and-reproducible-benchmarks-with-pytest-cases/)."
 
 !!! success "New `current_cases` fixture to easily know the current case for each parameter ! See [below](#d-accessing-the-current-case) for details."
```

### Comparing `pytest-cases-3.8.4/docs/long_description.md` & `pytest-cases-3.8.5/docs/long_description.md`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/pytest_goodies.md` & `pytest-cases-3.8.5/docs/pytest_goodies.md`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/docs/unions_theory.md` & `pytest-cases-3.8.5/docs/unions_theory.md`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/mkdocs.yml` & `pytest-cases-3.8.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/noxfile.py` & `pytest-cases-3.8.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/setup.cfg` & `pytest-cases-3.8.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/setup.py` & `pytest-cases-3.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/__init__.py` & `pytest-cases-3.8.5/src/pytest_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/case_funcs.py` & `pytest-cases-3.8.5/src/pytest_cases/case_funcs.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/case_parametrizer_new.py` & `pytest-cases-3.8.5/src/pytest_cases/case_parametrizer_new.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/common_mini_six.py` & `pytest-cases-3.8.5/src/pytest_cases/common_mini_six.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/common_others.py` & `pytest-cases-3.8.5/src/pytest_cases/common_others.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/common_pytest.py` & `pytest-cases-3.8.5/src/pytest_cases/common_pytest.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/common_pytest_lazy_values.py` & `pytest-cases-3.8.5/src/pytest_cases/common_pytest_lazy_values.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/common_pytest_marks.py` & `pytest-cases-3.8.5/src/pytest_cases/common_pytest_marks.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,29 +197,37 @@
         try:
             delattr(f, mark_name)
         except AttributeError:
             pass
     return f
 
 
-def get_pytest_parametrize_marks(f):
+def get_pytest_parametrize_marks(
+    f,
+    pop=False  # type: bool
+):
     """
     Returns the @pytest.mark.parametrize marks associated with a function (and only those)
 
     :param f:
+    :param pop: boolean flag, when True the marks will be removed from f.
     :return: a tuple containing all 'parametrize' marks
     """
     # pytest > 3.2.0
     marks = getattr(f, 'pytestmark', None)
     if marks is not None:
+        if pop:
+            delattr(f, 'pytestmark')
         return tuple(_ParametrizationMark(m) for m in marks if m.name == 'parametrize')
     else:
         # older versions
         mark_info = getattr(f, 'parametrize', None)
         if mark_info is not None:
+            if pop:
+                delattr(f, 'parametrize')
             # mark_info.args contains a list of (name, values)
             if len(mark_info.args) % 2 != 0:
                 raise ValueError("internal pytest compatibility error - please report")
             nb_parametrize_decorations = len(mark_info.args) // 2
             if nb_parametrize_decorations > 1 and len(mark_info.kwargs) > 0:
                 raise ValueError("Unfortunately with this old pytest version it is not possible to have several "
                                  "parametrization decorators while specifying **kwargs, as all **kwargs are "
```

### Comparing `pytest-cases-3.8.4/src/pytest_cases/filters.py` & `pytest-cases-3.8.5/src/pytest_cases/filters.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/fixture__creation.py` & `pytest-cases-3.8.5/src/pytest_cases/fixture__creation.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/fixture_core1_unions.py` & `pytest-cases-3.8.5/src/pytest_cases/fixture_core1_unions.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/fixture_core2.py` & `pytest-cases-3.8.5/src/pytest_cases/fixture_core2.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     from types import ModuleType  # noqa
 except ImportError:
     pass
 
 from .common_pytest_lazy_values import get_lazy_args
 from .common_pytest import get_pytest_parametrize_marks, make_marked_parameter_value, get_param_argnames_as_list, \
     combine_ids, is_marked_parameter_value, pytest_fixture, resolve_ids, extract_parameterset_info, make_test_ids
-from .common_pytest_marks import PYTEST3_OR_GREATER
+from .common_pytest_marks import PYTEST3_OR_GREATER, PYTEST8_OR_GREATER
 from .fixture__creation import get_caller_module, check_name_available, WARN, CHANGE
 from .fixture_core1_unions import ignore_unused, is_used_request, NOT_USED, _make_unpack_fixture
 
 
 def param_fixture(argname,           # type: str
                   argvalues,         # type: Iterable[Any]
                   autouse=False,     # type: bool
@@ -419,15 +419,15 @@
         # get caller module to create the symbols
         caller_module = get_caller_module(frame_offset=_caller_module_offset_when_unpack)
 
         # note that we cannot use in_cls=True since we have no way to assign the unpacked fixtures to the class
         _make_unpack_fixture(caller_module, unpack_into, name, hook=hook, in_cls=False)
 
     # (1) Collect all @pytest.mark.parametrize markers (including those created by usage of @cases_data)
-    parametrizer_marks = get_pytest_parametrize_marks(fixture_func)
+    parametrizer_marks = get_pytest_parametrize_marks(fixture_func, pop=PYTEST8_OR_GREATER)
     if len(parametrizer_marks) < 1:
         # make the fixture union-aware
         wrapped_fixture_func = ignore_unused(fixture_func)
 
         # resolve possibly infinite generators of ids here
         if 'params' in kwargs and 'ids' in kwargs:
             kwargs['ids'] = resolve_ids(kwargs['ids'], kwargs['params'], full_resolve=False)
```

### Comparing `pytest-cases-3.8.4/src/pytest_cases/fixture_parametrize_plus.py` & `pytest-cases-3.8.5/src/pytest_cases/fixture_parametrize_plus.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/pep380.py` & `pytest-cases-3.8.5/src/pytest_cases/pep380.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/pep492.py` & `pytest-cases-3.8.5/src/pytest_cases/pep492.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/pep525.py` & `pytest-cases-3.8.5/src/pytest_cases/pep525.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases/plugin.py` & `pytest-cases-3.8.5/src/pytest_cases/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/src/pytest_cases.egg-info/PKG-INFO` & `pytest-cases-3.8.5/src/pytest_cases.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pytest-cases
-Version: 3.8.4
+Version: 3.8.5
 Summary: Separate test code from test cases in pytest.
 Home-page: https://github.com/smarie/python-pytest-cases
-Download-URL: https://github.com/smarie/python-pytest-cases/tarball/3.8.4
+Download-URL: https://github.com/smarie/python-pytest-cases/tarball/3.8.5
 Author: Sylvain MARIE <sylvain.marie@se.com>
 Maintainer: Sylvain MARIE <sylvain.marie@se.com>
 License: BSD 3-Clause
 Keywords: pytest test case testcase test-case decorator parametrize parameter data dataset file separate concerns lazy fixture union
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pytest-cases-3.8.4/src/pytest_cases.egg-info/SOURCES.txt` & `pytest-cases-3.8.5/src/pytest_cases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/cases_doc_alternate.py` & `pytest-cases-3.8.5/tests/cases/doc/cases_doc_alternate.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_doc.py` & `pytest-cases-3.8.5/tests/cases/doc/test_doc.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_doc_alternate.py` & `pytest-cases-3.8.5/tests/cases/doc/test_doc_alternate.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_doc_cache.py` & `pytest-cases-3.8.5/tests/cases/doc/test_doc_cache.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_doc_debug.py` & `pytest-cases-3.8.5/tests/cases/doc/test_doc_debug.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_doc_filters_n_tags.py` & `pytest-cases-3.8.5/tests/cases/doc/test_doc_filters_n_tags.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_doc_filters_n_tags2.py` & `pytest-cases-3.8.5/tests/cases/doc/test_doc_filters_n_tags2.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_doc_get_current_case_id.py` & `pytest-cases-3.8.5/tests/cases/doc/test_doc_get_current_case_id.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_doc_get_current_cases.py` & `pytest-cases-3.8.5/tests/cases/doc/test_doc_get_current_cases.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_doc_ids.py` & `pytest-cases-3.8.5/tests/cases/doc/test_doc_ids.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_fixtures.py` & `pytest-cases-3.8.5/tests/cases/doc/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_generators.py` & `pytest-cases-3.8.5/tests/cases/doc/test_generators.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_get_current_cases.py` & `pytest-cases-3.8.5/tests/cases/doc/test_get_current_cases.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_get_current_cases_cases.py` & `pytest-cases-3.8.5/tests/cases/doc/test_get_current_cases_cases.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_get_current_cases_negative.py` & `pytest-cases-3.8.5/tests/cases/doc/test_get_current_cases_negative.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_get_current_cases_params.py` & `pytest-cases-3.8.5/tests/cases/doc/test_get_current_cases_params.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_indirect.py` & `pytest-cases-3.8.5/tests/cases/doc/test_indirect.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_joss.py` & `pytest-cases-3.8.5/tests/cases/doc/test_joss.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_nested.py` & `pytest-cases-3.8.5/tests/cases/doc/test_nested.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/doc/test_parametrize_alt.py` & `pytest-cases-3.8.5/tests/cases/doc/test_parametrize_alt.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/issue_258/test_issue_258.py` & `pytest-cases-3.8.5/tests/cases/issues/issue_258/test_issue_258.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/issue_311/test_issue_311/test_issue_311.py` & `pytest-cases-3.8.5/tests/cases/issues/issue_311/test_issue_311/test_issue_311.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_125.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_125.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_126.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_126.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_126_2.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_126_2.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_126_2_cases.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_126_2_cases.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_128_2.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_128_2.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_142.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_142.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_142_2.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_142_2.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_151.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_151.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_154.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_154.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_159.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_159.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_168.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_168.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_171.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_171.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_179.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_179.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_190.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_190.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_191.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_191.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_193.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_193.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_211.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_211.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_212.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_212.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_242.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_242.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_246.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_246.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_issue_274.py` & `pytest-cases-3.8.5/tests/cases/issues/test_issue_274.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_py35_issue_176.py` & `pytest-cases-3.8.5/tests/cases/issues/test_py35_issue_176.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_py35_issue_243.py` & `pytest-cases-3.8.5/tests/cases/issues/test_py35_issue_243.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/issues/test_py35_issue_287.py` & `pytest-cases-3.8.5/tests/cases/issues/test_py35_issue_287.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/others/test_bound_methods.py` & `pytest-cases-3.8.5/tests/cases/others/test_bound_methods.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/others/test_glob_low_level.py` & `pytest-cases-3.8.5/tests/cases/others/test_glob_low_level.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/so/test_so2.py` & `pytest-cases-3.8.5/tests/cases/so/test_so2.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/so/test_so3.py` & `pytest-cases-3.8.5/tests/cases/so/test_so3.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/cases/so/test_so4.py` & `pytest-cases-3.8.5/tests/cases/so/test_so4.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/conftest.py` & `pytest-cases-3.8.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/doc/test_doc_fixture_graph.py` & `pytest-cases-3.8.5/tests/pytest_extension/doc/test_doc_fixture_graph.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/doc/test_doc_fixture_graph_union.py` & `pytest-cases-3.8.5/tests/pytest_extension/doc/test_doc_fixture_graph_union.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/doc/test_doc_fixture_graph_union_normal.py` & `pytest-cases-3.8.5/tests/pytest_extension/doc/test_doc_fixture_graph_union_normal.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/doc/test_doc_fixture_graph_union_union.py` & `pytest-cases-3.8.5/tests/pytest_extension/doc/test_doc_fixture_graph_union_union.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/doc/test_doc_parametrize.py` & `pytest-cases-3.8.5/tests/pytest_extension/doc/test_doc_parametrize.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/doc/test_doc_parametrize_customids.py` & `pytest-cases-3.8.5/tests/pytest_extension/doc/test_doc_parametrize_customids.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixture_unpacking.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixture_unpacking.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixture_unpacking2.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixture_unpacking2.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_parametrize.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_parametrize.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_parametrize_stereo.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_parametrize_stereo.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_paramfixtures.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_paramfixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_paramfixtures_marks.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_fixtures_paramfixtures_marks.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_plus_and_others/test_skip_on_paramz_fixture.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_plus_and_others/test_skip_on_paramz_fixture.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixture_closure_edits.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixture_closure_edits.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_custom_mark.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_custom_mark.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_ids.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_ids.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_setup_teardown.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_setup_teardown.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_setup_teardown2.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_setup_teardown2.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_setup_teardown3.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixture_union_setup_teardown3.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_0simplest.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_0simplest.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_1simple.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_1simple.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_2hard.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_fixtures_union_2hard.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/fixture_unions/test_so.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/fixture_unions/test_so.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/test_hook.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/test_hook.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/fixtures/test_issue_github_54.py` & `pytest-cases-3.8.5/tests/pytest_extension/fixtures/test_issue_github_54.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_124.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_124.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_137.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_137.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_138.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_138.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_148.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_148.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_149.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_149.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_177.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_177.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_182.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_182.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_199.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_199.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_269.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_269.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_classes.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_classes.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_fixture_union1.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_fixture_union1.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_fixture_union2.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_fixture_union2.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_indirect_fixture_param.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_indirect_fixture_param.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_pytest_70.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_pytest_70.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_python2_str.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_python2_str.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_issue_so_76.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_issue_so_76.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/issues/test_parametrize_with_lists.py` & `pytest-cases-3.8.5/tests/pytest_extension/issues/test_parametrize_with_lists.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/meta/raw/session_optim/session_optim.py` & `pytest-cases-3.8.5/tests/pytest_extension/meta/raw/session_optim/session_optim.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/meta/test_all.py` & `pytest-cases-3.8.5/tests/pytest_extension/meta/test_all.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/order/session_optim/conftest.py` & `pytest-cases-3.8.5/tests/pytest_extension/order/session_optim/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/order/session_optim/test_reorder_default_normal.py` & `pytest-cases-3.8.5/tests/pytest_extension/order/session_optim/test_reorder_default_normal.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/order/test_fixture_order_respects_scope.py` & `pytest-cases-3.8.5/tests/pytest_extension/order/test_fixture_order_respects_scope.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/others/test_assert_exception.py` & `pytest-cases-3.8.5/tests/pytest_extension/others/test_assert_exception.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_basics_misc.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_basics_misc.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_filter.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_filter.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic1.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic1.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic2.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic2.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic3_tuples.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic3_tuples.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic4_ids.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_basic4_ids.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom1.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom1.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom2.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom2.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom3.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom3.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom4_tuples.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_fixture_ref_custom4_tuples.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_getcallspecs.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_getcallspecs.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value__custom_ids.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value__custom_ids.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value_and_fixture_ref.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value_and_fixture_ref.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value_and_fixture_ref2.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value_and_fixture_ref2.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value_and_fixture_ref3.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value_and_fixture_ref3.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value_low_level.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value_low_level.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_lazy_value_so.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_lazy_value_so.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_parametrizing_a_class.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_parametrizing_a_class.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_so2.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_so2.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_so2_dynamic.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_so2_dynamic.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_so2_new.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_so2_new.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/pytest_extension/parametrize_plus/test_so2_simplified.py` & `pytest-cases-3.8.5/tests/pytest_extension/parametrize_plus/test_so2_simplified.py`

 * *Files identical despite different names*

### Comparing `pytest-cases-3.8.4/tests/utils.py` & `pytest-cases-3.8.5/tests/utils.py`

 * *Files identical despite different names*

