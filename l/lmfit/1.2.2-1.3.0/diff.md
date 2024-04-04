# Comparing `tmp/lmfit-1.2.2.tar.gz` & `tmp/lmfit-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmfit-1.2.2.tar", last modified: Fri Jul 14 02:56:03 2023, max compression
+gzip compressed data, was "lmfit-1.3.0.tar", last modified: Thu Apr  4 17:31:35 2024, max compression
```

## Comparing `lmfit-1.2.2.tar` & `lmfit-1.3.0.tar`

### file list

```diff
@@ -1,206 +1,213 @@
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.903850 lmfit-1.2.2/
--rw-r--r--   0 Newville   (501) staff       (20)      308 2023-07-14 02:55:52.000000 lmfit-1.2.2/.codecov.yml
--rw-r--r--   0 Newville   (501) staff       (20)      393 2023-07-14 02:55:52.000000 lmfit-1.2.2/.gitattributes
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.876691 lmfit-1.2.2/.github/
--rw-r--r--   0 Newville   (501) staff       (20)     5158 2023-07-14 02:55:52.000000 lmfit-1.2.2/.github/CONTRIBUTING.md
--rw-r--r--   0 Newville   (501) staff       (20)     2901 2023-07-14 02:55:52.000000 lmfit-1.2.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 Newville   (501) staff       (20)     2211 2023-07-14 02:55:52.000000 lmfit-1.2.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 Newville   (501) staff       (20)      502 2023-07-14 02:55:52.000000 lmfit-1.2.2/.github/dependabot.yml
--rw-r--r--   0 Newville   (501) staff       (20)      323 2023-07-14 02:55:52.000000 lmfit-1.2.2/.gitignore
--rw-r--r--   0 Newville   (501) staff       (20)     1676 2023-07-14 02:55:52.000000 lmfit-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 Newville   (501) staff       (20)     3015 2023-07-14 02:55:52.000000 lmfit-1.2.2/AUTHORS.txt
--rw-r--r--   0 Newville   (501) staff       (20)     3670 2023-07-14 02:55:52.000000 lmfit-1.2.2/LICENSE
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.880166 lmfit-1.2.2/NIST_STRD/
--rw-r--r--   0 Newville   (501) staff       (20)     6869 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Bennett5.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1713 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/BoxBOD.dat
--rw-r--r--   0 Newville   (501) staff       (20)     7558 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Chwirut1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3060 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Chwirut2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1990 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/DanWood.dat
--rw-r--r--   0 Newville   (501) staff       (20)     6761 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/ENSO.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2773 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Eckerle4.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8098 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Gauss1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8100 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Gauss2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8102 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Gauss3.dat
--rw-r--r--   0 Newville   (501) staff       (20)     9276 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Hahn1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     5858 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Kirby2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2945 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Lanczos1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2601 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Lanczos2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2574 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Lanczos3.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2305 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/MGH09.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2335 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/MGH10.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3078 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/MGH17.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1853 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Misra1a.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1845 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Misra1b.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1839 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Misra1c.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1843 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Misra1d.dat
--rw-r--r--   0 Newville   (501) staff       (20)     6401 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Models
--rw-r--r--   0 Newville   (501) staff       (20)     7001 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Nelson.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1873 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Rat42.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2072 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Rat43.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2486 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Roszman1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3026 2023-07-14 02:55:52.000000 lmfit-1.2.2/NIST_STRD/Thurber.dat
--rw-r--r--   0 Newville   (501) staff       (20)     7730 2023-07-14 02:56:03.904109 lmfit-1.2.2/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     6229 2023-07-14 02:55:52.000000 lmfit-1.2.2/README.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.880533 lmfit-1.2.2/asv_benchmarking/
--rw-r--r--   0 Newville   (501) staff       (20)       43 2023-07-14 02:55:52.000000 lmfit-1.2.2/asv_benchmarking/README.md
--rw-r--r--   0 Newville   (501) staff       (20)     2793 2023-07-14 02:55:52.000000 lmfit-1.2.2/asv_benchmarking/asv.conf.json
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.880759 lmfit-1.2.2/asv_benchmarking/benchmarks/
--rw-r--r--   0 Newville   (501) staff       (20)        0 2023-07-14 02:55:52.000000 lmfit-1.2.2/asv_benchmarking/benchmarks/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)     4394 2023-07-14 02:55:52.000000 lmfit-1.2.2/asv_benchmarking/benchmarks/benchmarks.py
--rw-r--r--   0 Newville   (501) staff       (20)      350 2023-07-14 02:55:52.000000 lmfit-1.2.2/asv_benchmarking/run_benchmark_code.py
--rw-r--r--   0 Newville   (501) staff       (20)    12176 2023-07-14 02:55:52.000000 lmfit-1.2.2/azure-pipelines.yml
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.883343 lmfit-1.2.2/doc/
--rw-r--r--   0 Newville   (501) staff       (20)     4460 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/Makefile
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.883479 lmfit-1.2.2/doc/_static/
--rw-r--r--   0 Newville   (501) staff       (20)        0 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/_static/empty
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.883586 lmfit-1.2.2/doc/_templates/
--rw-r--r--   0 Newville   (501) staff       (20)      756 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/_templates/indexsidebar.html
--rw-r--r--   0 Newville   (501) staff       (20)     3499 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/bounds.rst
--rw-r--r--   0 Newville   (501) staff       (20)    30647 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/builtin_models.rst
--rw-r--r--   0 Newville   (501) staff       (20)     6527 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/conf.py
--rw-r--r--   0 Newville   (501) staff       (20)    15659 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/confidence.rst
--rw-r--r--   0 Newville   (501) staff       (20)     8110 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/constraints.rst
--rw-r--r--   0 Newville   (501) staff       (20)      223 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/contents.rst
--rwxr-xr-x   0 Newville   (501) staff       (20)     1943 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/doc_examples_to_gallery.py
--rw-r--r--   0 Newville   (501) staff       (20)    12177 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/faq.rst
--rwxr-xr-x   0 Newville   (501) staff       (20)      657 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/filter_spurious_link_from_html.py
--rw-r--r--   0 Newville   (501) staff       (20)    38148 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/fitting.rst
--rw-r--r--   0 Newville   (501) staff       (20)     2915 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/index.rst
--rw-r--r--   0 Newville   (501) staff       (20)     5102 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/installation.rst
--rw-r--r--   0 Newville   (501) staff       (20)     9268 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/intro.rst
--rw-r--r--   0 Newville   (501) staff       (20)      941 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/make.bat
--rw-r--r--   0 Newville   (501) staff       (20)    47467 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/model.rst
--rw-r--r--   0 Newville   (501) staff       (20)     4670 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/parameters.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.883826 lmfit-1.2.2/doc/sphinx/
--rw-r--r--   0 Newville   (501) staff       (20)      460 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/ext_imgmath.py
--rw-r--r--   0 Newville   (501) staff       (20)      407 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/ext_mathjax.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.874288 lmfit-1.2.2/doc/sphinx/theme/
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.884194 lmfit-1.2.2/doc/sphinx/theme/sphinx13/
--rw-r--r--   0 Newville   (501) staff       (20)     7546 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/basic_layout.html
--rw-r--r--   0 Newville   (501) staff       (20)     3080 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/layout.html
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.889679 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/
--rw-r--r--   0 Newville   (501) staff       (20)      429 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/bodybg.png
--rw-r--r--   0 Newville   (501) staff       (20)      180 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/footerbg.png
--rw-r--r--   0 Newville   (501) staff       (20)      189 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/headerbg.png
--rw-r--r--   0 Newville   (501) staff       (20)      149 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/listitem.png
--rw-r--r--   0 Newville   (501) staff       (20)     9907 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/lmfitheader.png
--rw-r--r--   0 Newville   (501) staff       (20)      183 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/relbg.png
--rw-r--r--   0 Newville   (501) staff       (20)     7978 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/sphinx13.css
--rw-r--r--   0 Newville   (501) staff       (20)       72 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/sphinx/theme/sphinx13/theme.conf
--rw-r--r--   0 Newville   (501) staff       (20)     1500 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/support.rst
--rw-r--r--   0 Newville   (501) staff       (20)    28488 2023-07-14 02:55:52.000000 lmfit-1.2.2/doc/whatsnew.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.896318 lmfit-1.2.2/examples/
--rw-r--r--   0 Newville   (501) staff       (20)     8195 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/NIST_Gauss2.dat
--rw-r--r--   0 Newville   (501) staff       (20)      419 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/README.txt
--rw-r--r--   0 Newville   (501) staff       (20)     1419 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_builtinmodels_nistgauss.py
--rw-r--r--   0 Newville   (501) staff       (20)     1010 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_builtinmodels_nistgauss2.py
--rw-r--r--   0 Newville   (501) staff       (20)     1364 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_builtinmodels_peakmodels.py
--rw-r--r--   0 Newville   (501) staff       (20)     1961 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_builtinmodels_splinemodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      784 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_builtinmodels_stepmodel.py
--rw-r--r--   0 Newville   (501) staff       (20)     1964 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_confidence_advanced.py
--rw-r--r--   0 Newville   (501) staff       (20)      481 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_confidence_basic.py
--rw-r--r--   0 Newville   (501) staff       (20)     3850 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_confidence_chi2_maps.py
--rw-r--r--   0 Newville   (501) staff       (20)     3359 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_fitting_emcee.py
--rw-r--r--   0 Newville   (501) staff       (20)      969 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_fitting_withreport.py
--rw-r--r--   0 Newville   (501) staff       (20)     1953 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_composite.py
--rw-r--r--   0 Newville   (501) staff       (20)      651 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_gaussian.py
--rw-r--r--   0 Newville   (501) staff       (20)      774 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_loadmodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      531 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_loadmodelresult.py
--rw-r--r--   0 Newville   (501) staff       (20)      537 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_loadmodelresult2.py
--rw-r--r--   0 Newville   (501) staff       (20)      337 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_savemodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      423 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_savemodelresult.py
--rw-r--r--   0 Newville   (501) staff       (20)      996 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_savemodelresult2.py
--rw-r--r--   0 Newville   (501) staff       (20)      862 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_two_components.py
--rw-r--r--   0 Newville   (501) staff       (20)      834 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_uncertainty.py
--rw-r--r--   0 Newville   (501) staff       (20)     3148 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_uncertainty2.py
--rw-r--r--   0 Newville   (501) staff       (20)     1051 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_with_iter_callback.py
--rw-r--r--   0 Newville   (501) staff       (20)      775 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_model_with_nan_policy.py
--rw-r--r--   0 Newville   (501) staff       (20)     1499 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_parameters_basic.py
--rw-r--r--   0 Newville   (501) staff       (20)     1252 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_parameters_valuesdict.py
--rw-r--r--   0 Newville   (501) staff       (20)     2417 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/doc_uvars_params.py
--rw-r--r--   0 Newville   (501) staff       (20)     7666 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_Model_interface.py
--rw-r--r--   0 Newville   (501) staff       (20)    17926 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_brute.py
--rw-r--r--   0 Newville   (501) staff       (20)     4731 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_complex_resonator_model.py
--rw-r--r--   0 Newville   (501) staff       (20)     4378 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_confidence_interval.py
--rw-r--r--   0 Newville   (501) staff       (20)     3331 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_detect_outliers.py
--rw-r--r--   0 Newville   (501) staff       (20)     1795 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_diffev.py
--rw-r--r--   0 Newville   (501) staff       (20)     4098 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_emcee_Model_interface.py
--rw-r--r--   0 Newville   (501) staff       (20)     1273 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_expression_model.py
--rw-r--r--   0 Newville   (501) staff       (20)     2716 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_fit_multi_datasets.py
--rw-r--r--   0 Newville   (501) staff       (20)     1417 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_fit_with_algebraic_constraint.py
--rw-r--r--   0 Newville   (501) staff       (20)     2161 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_fit_with_bounds.py
--rw-r--r--   0 Newville   (501) staff       (20)     2666 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_fit_with_derivfunc.py
--rw-r--r--   0 Newville   (501) staff       (20)     2190 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_fit_with_inequality.py
--rw-r--r--   0 Newville   (501) staff       (20)     2378 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_reduce_fcn.py
--rw-r--r--   0 Newville   (501) staff       (20)     2915 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_sympy.py
--rw-r--r--   0 Newville   (501) staff       (20)     6112 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_two_dimensional_peak.py
--rw-r--r--   0 Newville   (501) staff       (20)      851 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/example_use_pandas.py
--rw-r--r--   0 Newville   (501) staff       (20)     7776 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/lmfit_emcee_model_selection.py
--rw-r--r--   0 Newville   (501) staff       (20)     2373 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/model1d_gauss.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1987 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/peak.csv
--rw-r--r--   0 Newville   (501) staff       (20)     2464 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/sinedata.dat
--rw-r--r--   0 Newville   (501) staff       (20)     9496 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/test_peak.dat
--rw-r--r--   0 Newville   (501) staff       (20)    11611 2023-07-14 02:55:52.000000 lmfit-1.2.2/examples/test_splinepeak.dat
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.898138 lmfit-1.2.2/lmfit/
--rw-r--r--   0 Newville   (501) staff       (20)     1956 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)    10016 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/_ampgo.py
--rw-r--r--   0 Newville   (501) staff       (20)    21034 2023-04-26 01:48:37.000000 lmfit-1.2.2/lmfit/conf_emcee.py
--rw-r--r--   0 Newville   (501) staff       (20)    15312 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/confidence.py
--rw-r--r--   0 Newville   (501) staff       (20)     5060 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/jsonutils.py
--rw-r--r--   0 Newville   (501) staff       (20)    16913 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/lineshapes.py
--rw-r--r--   0 Newville   (501) staff       (20)   106040 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/minimizer.py
--rw-r--r--   0 Newville   (501) staff       (20)    85772 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/model.py
--rw-r--r--   0 Newville   (501) staff       (20)    68610 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/models.py
--rw-r--r--   0 Newville   (501) staff       (20)    40026 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/parameter.py
--rw-r--r--   0 Newville   (501) staff       (20)    16055 2023-07-14 02:55:52.000000 lmfit-1.2.2/lmfit/printfuncs.py
--rw-r--r--   0 Newville   (501) staff       (20)      160 2023-07-14 02:56:03.000000 lmfit-1.2.2/lmfit/version.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.898758 lmfit-1.2.2/lmfit.egg-info/
--rw-r--r--   0 Newville   (501) staff       (20)     7730 2023-07-14 02:56:03.000000 lmfit-1.2.2/lmfit.egg-info/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     5047 2023-07-14 02:56:03.000000 lmfit-1.2.2/lmfit.egg-info/SOURCES.txt
--rw-r--r--   0 Newville   (501) staff       (20)        1 2023-07-14 02:56:03.000000 lmfit-1.2.2/lmfit.egg-info/dependency_links.txt
--rw-r--r--   0 Newville   (501) staff       (20)      669 2023-07-14 02:56:03.000000 lmfit-1.2.2/lmfit.egg-info/requires.txt
--rw-r--r--   0 Newville   (501) staff       (20)        6 2023-07-14 02:56:03.000000 lmfit-1.2.2/lmfit.egg-info/top_level.txt
--rwxr-xr-x   0 Newville   (501) staff       (20)     1010 2023-07-14 02:55:52.000000 lmfit-1.2.2/publish_docs.sh
--rw-r--r--   0 Newville   (501) staff       (20)      202 2023-07-14 02:55:52.000000 lmfit-1.2.2/pyproject.toml
--rw-r--r--   0 Newville   (501) staff       (20)     2447 2023-07-14 02:56:03.904931 lmfit-1.2.2/setup.cfg
--rw-r--r--   0 Newville   (501) staff       (20)       92 2023-07-14 02:55:52.000000 lmfit-1.2.2/setup.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-07-14 02:56:03.903712 lmfit-1.2.2/tests/
--rw-r--r--   0 Newville   (501) staff       (20)     6109 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/NISTModels.py
--rw-r--r--   0 Newville   (501) staff       (20)        0 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)      893 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/conftest.py
--rw-r--r--   0 Newville   (501) staff       (20)     5656 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/gauss_modelresult_lmfit100.sav
--rw-r--r--   0 Newville   (501) staff       (20)     1374 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_1variable.py
--rw-r--r--   0 Newville   (501) staff       (20)     7097 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_NIST_Strd.py
--rw-r--r--   0 Newville   (501) staff       (20)     4008 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_algebraic_constraint.py
--rw-r--r--   0 Newville   (501) staff       (20)     5063 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_ampgo.py
--rw-r--r--   0 Newville   (501) staff       (20)     1238 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_basicfit.py
--rw-r--r--   0 Newville   (501) staff       (20)     3911 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_basinhopping.py
--rw-r--r--   0 Newville   (501) staff       (20)     1900 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_bounded_jacobian.py
--rw-r--r--   0 Newville   (501) staff       (20)     1413 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_bounds.py
--rw-r--r--   0 Newville   (501) staff       (20)    11428 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_brute.py
--rw-r--r--   0 Newville   (501) staff       (20)    11953 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_builtin_models.py
--rw-r--r--   0 Newville   (501) staff       (20)     9251 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_confidence.py
--rw-r--r--   0 Newville   (501) staff       (20)     9987 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_covariance_matrix.py
--rw-r--r--   0 Newville   (501) staff       (20)     1235 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_custom_independentvar.py
--rw-r--r--   0 Newville   (501) staff       (20)      612 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_default_kws.py
--rw-r--r--   0 Newville   (501) staff       (20)     2595 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_dual_annealing.py
--rw-r--r--   0 Newville   (501) staff       (20)     4292 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_itercb.py
--rw-r--r--   0 Newville   (501) staff       (20)     3066 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_jsonutils.py
--rw-r--r--   0 Newville   (501) staff       (20)     6266 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_least_squares.py
--rw-r--r--   0 Newville   (501) staff       (20)     4780 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_lineshapes.py
--rw-r--r--   0 Newville   (501) staff       (20)      781 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_manypeaks_speed.py
--rw-r--r--   0 Newville   (501) staff       (20)     3689 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_max_nfev.py
--rw-r--r--   0 Newville   (501) staff       (20)     2686 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_minimizer.py
--rw-r--r--   0 Newville   (501) staff       (20)    56579 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_model.py
--rw-r--r--   0 Newville   (501) staff       (20)    10484 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_model_saveload.py
--rw-r--r--   0 Newville   (501) staff       (20)     4354 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_model_uncertainties.py
--rw-r--r--   0 Newville   (501) staff       (20)     4965 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_models.py
--rw-r--r--   0 Newville   (501) staff       (20)     2181 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_multidatasets.py
--rw-r--r--   0 Newville   (501) staff       (20)    24063 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_nose.py
--rw-r--r--   0 Newville   (501) staff       (20)     1168 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_pandas.py
--rw-r--r--   0 Newville   (501) staff       (20)    19779 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_parameter.py
--rw-r--r--   0 Newville   (501) staff       (20)    21303 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_parameters.py
--rw-r--r--   0 Newville   (501) staff       (20)     3169 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_params_uvars.py
--rw-r--r--   0 Newville   (501) staff       (20)    14955 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_printfuncs.py
--rw-r--r--   0 Newville   (501) staff       (20)     4237 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_shgo.py
--rw-r--r--   0 Newville   (501) staff       (20)     1503 2023-07-14 02:55:52.000000 lmfit-1.2.2/tests/test_stepmodel.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.696514 lmfit-1.3.0/
+-rw-r--r--   0 Newville   (501) staff       (20)      308 2024-04-04 17:29:11.000000 lmfit-1.3.0/.codecov.yml
+-rw-r--r--   0 Newville   (501) staff       (20)      393 2024-04-04 17:29:11.000000 lmfit-1.3.0/.gitattributes
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.661185 lmfit-1.3.0/.github/
+-rw-r--r--   0 Newville   (501) staff       (20)     5158 2024-04-04 17:29:11.000000 lmfit-1.3.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2901 2024-04-04 17:29:11.000000 lmfit-1.3.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2211 2024-04-04 17:29:11.000000 lmfit-1.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 Newville   (501) staff       (20)      502 2024-04-04 17:29:11.000000 lmfit-1.3.0/.github/dependabot.yml
+-rw-r--r--   0 Newville   (501) staff       (20)      350 2024-04-04 17:29:11.000000 lmfit-1.3.0/.gitignore
+-rw-r--r--   0 Newville   (501) staff       (20)     1789 2024-04-04 17:29:11.000000 lmfit-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 Newville   (501) staff       (20)     3015 2024-04-04 17:29:11.000000 lmfit-1.3.0/AUTHORS.txt
+-rw-r--r--   0 Newville   (501) staff       (20)     3670 2024-04-04 17:29:11.000000 lmfit-1.3.0/LICENSE
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.665527 lmfit-1.3.0/NIST_STRD/
+-rw-r--r--   0 Newville   (501) staff       (20)     6869 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Bennett5.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1713 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/BoxBOD.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     7558 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Chwirut1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3060 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Chwirut2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1990 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/DanWood.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     6761 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/ENSO.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2773 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Eckerle4.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8098 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Gauss1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8100 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Gauss2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8102 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Gauss3.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     9276 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Hahn1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     5858 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Kirby2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2945 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Lanczos1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2601 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Lanczos2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2574 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Lanczos3.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2305 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/MGH09.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2335 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/MGH10.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3078 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/MGH17.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1853 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Misra1a.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1845 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Misra1b.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1839 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Misra1c.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1843 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Misra1d.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     6401 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Models
+-rw-r--r--   0 Newville   (501) staff       (20)     7001 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Nelson.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1873 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Rat42.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2072 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Rat43.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2486 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Roszman1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3026 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Thurber.dat
+-rw-r--r--   0 Newville   (501) staff       (20)    13054 2024-04-04 17:31:35.696052 lmfit-1.3.0/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     6229 2024-04-04 17:29:11.000000 lmfit-1.3.0/README.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.666163 lmfit-1.3.0/asv_benchmarking/
+-rw-r--r--   0 Newville   (501) staff       (20)       43 2024-04-04 17:29:11.000000 lmfit-1.3.0/asv_benchmarking/README.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2793 2024-04-04 17:29:11.000000 lmfit-1.3.0/asv_benchmarking/asv.conf.json
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.666478 lmfit-1.3.0/asv_benchmarking/benchmarks/
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2024-04-04 17:29:11.000000 lmfit-1.3.0/asv_benchmarking/benchmarks/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4394 2024-04-04 17:29:11.000000 lmfit-1.3.0/asv_benchmarking/benchmarks/benchmarks.py
+-rw-r--r--   0 Newville   (501) staff       (20)      350 2024-04-04 17:29:11.000000 lmfit-1.3.0/asv_benchmarking/run_benchmark_code.py
+-rw-r--r--   0 Newville   (501) staff       (20)    12203 2024-04-04 17:29:11.000000 lmfit-1.3.0/azure-pipelines.yml
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.669610 lmfit-1.3.0/doc/
+-rw-r--r--   0 Newville   (501) staff       (20)     4529 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/Makefile
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.669803 lmfit-1.3.0/doc/_static/
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/_static/empty
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.669947 lmfit-1.3.0/doc/_templates/
+-rw-r--r--   0 Newville   (501) staff       (20)      756 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/_templates/indexsidebar.html
+-rw-r--r--   0 Newville   (501) staff       (20)     3499 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/bounds.rst
+-rw-r--r--   0 Newville   (501) staff       (20)    30647 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/builtin_models.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     6530 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/conf.py
+-rw-r--r--   0 Newville   (501) staff       (20)    16305 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/confidence.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     8110 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/constraints.rst
+-rw-r--r--   0 Newville   (501) staff       (20)      223 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/contents.rst
+-rwxr-xr-x   0 Newville   (501) staff       (20)     1943 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/doc_examples_to_gallery.py
+-rw-r--r--   0 Newville   (501) staff       (20)    12177 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/faq.rst
+-rwxr-xr-x   0 Newville   (501) staff       (20)      657 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/filter_spurious_link_from_html.py
+-rw-r--r--   0 Newville   (501) staff       (20)    40606 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/fitting.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     2915 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/index.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     5143 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/installation.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     9268 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/intro.rst
+-rw-r--r--   0 Newville   (501) staff       (20)      941 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/make.bat
+-rw-r--r--   0 Newville   (501) staff       (20)    50953 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/model.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     4670 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/parameters.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.670382 lmfit-1.3.0/doc/sphinx/
+-rw-r--r--   0 Newville   (501) staff       (20)      460 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/ext_imgmath.py
+-rw-r--r--   0 Newville   (501) staff       (20)      407 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/ext_mathjax.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.658261 lmfit-1.3.0/doc/sphinx/theme/
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.670942 lmfit-1.3.0/doc/sphinx/theme/sphinx13/
+-rw-r--r--   0 Newville   (501) staff       (20)     7586 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/basic_layout.html
+-rw-r--r--   0 Newville   (501) staff       (20)     3080 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/layout.html
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.672040 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/
+-rw-r--r--   0 Newville   (501) staff       (20)      429 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/bodybg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      180 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/footerbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      189 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/headerbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      149 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/listitem.png
+-rw-r--r--   0 Newville   (501) staff       (20)     9907 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/lmfitheader.png
+-rw-r--r--   0 Newville   (501) staff       (20)      183 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/relbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)     7978 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/sphinx13.css
+-rw-r--r--   0 Newville   (501) staff       (20)       72 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/theme.conf
+-rw-r--r--   0 Newville   (501) staff       (20)     1500 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/support.rst
+-rw-r--r--   0 Newville   (501) staff       (20)    30537 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/whatsnew.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.682089 lmfit-1.3.0/examples/
+-rw-r--r--   0 Newville   (501) staff       (20)     8195 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/NIST_Gauss2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)      419 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/README.txt
+-rw-r--r--   0 Newville   (501) staff       (20)   392918 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/discuss_model_eval_uncertainty.ipynb
+-rw-r--r--   0 Newville   (501) staff       (20)     1419 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_builtinmodels_nistgauss.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1010 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_builtinmodels_nistgauss2.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1364 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_builtinmodels_peakmodels.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1961 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_builtinmodels_splinemodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      784 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_builtinmodels_stepmodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1964 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_confidence_advanced.py
+-rw-r--r--   0 Newville   (501) staff       (20)      481 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_confidence_basic.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3795 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_confidence_chi2_maps.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3359 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_fitting_emcee.py
+-rw-r--r--   0 Newville   (501) staff       (20)      969 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_fitting_withreport.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1953 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_composite.py
+-rw-r--r--   0 Newville   (501) staff       (20)      651 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_gaussian.py
+-rw-r--r--   0 Newville   (501) staff       (20)      774 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_loadmodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      531 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_loadmodelresult.py
+-rw-r--r--   0 Newville   (501) staff       (20)      537 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_loadmodelresult2.py
+-rw-r--r--   0 Newville   (501) staff       (20)      337 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_savemodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      423 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_savemodelresult.py
+-rw-r--r--   0 Newville   (501) staff       (20)      996 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_savemodelresult2.py
+-rw-r--r--   0 Newville   (501) staff       (20)      862 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_two_components.py
+-rw-r--r--   0 Newville   (501) staff       (20)      834 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_uncertainty.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3148 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_uncertainty2.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5383 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_uncertainty_pred.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1051 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_with_iter_callback.py
+-rw-r--r--   0 Newville   (501) staff       (20)      775 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_with_nan_policy.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1499 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_parameters_basic.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1252 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_parameters_valuesdict.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2417 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_uvars_params.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7666 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_Model_interface.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1867 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_basinhopping.py
+-rw-r--r--   0 Newville   (501) staff       (20)    17926 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_brute.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4731 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_complex_resonator_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4378 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_confidence_interval.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3331 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_detect_outliers.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1795 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_diffev.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4098 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_emcee_Model_interface.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1273 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_expression_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2716 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_fit_multi_datasets.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1417 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_fit_with_algebraic_constraint.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2161 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_fit_with_bounds.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2666 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_fit_with_derivfunc.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2190 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_fit_with_inequality.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2378 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_reduce_fcn.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2915 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_sympy.py
+-rw-r--r--   0 Newville   (501) staff       (20)     6112 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_two_dimensional_peak.py
+-rw-r--r--   0 Newville   (501) staff       (20)      851 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_use_pandas.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7776 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/lmfit_emcee_model_selection.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2373 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/model1d_gauss.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1987 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/peak.csv
+-rw-r--r--   0 Newville   (501) staff       (20)     2464 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/sinedata.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     9496 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/test_peak.dat
+-rw-r--r--   0 Newville   (501) staff       (20)    11611 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/test_splinepeak.dat
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.685597 lmfit-1.3.0/lmfit/
+-rw-r--r--   0 Newville   (501) staff       (20)     1956 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)    10016 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/_ampgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)    21021 2023-12-31 16:26:04.000000 lmfit-1.3.0/lmfit/conf_emcee.py
+-rw-r--r--   0 Newville   (501) staff       (20)    16981 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/confidence.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5251 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/jsonutils.py
+-rw-r--r--   0 Newville   (501) staff       (20)    16913 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/lineshapes.py
+-rw-r--r--   0 Newville   (501) staff       (20)   105588 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/minimizer.py
+-rw-r--r--   0 Newville   (501) staff       (20)    91579 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/model.py
+-rw-r--r--   0 Newville   (501) staff       (20)    68814 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/models.py
+-rw-r--r--   0 Newville   (501) staff       (20)    40207 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/parameter.py
+-rw-r--r--   0 Newville   (501) staff       (20)    16055 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/printfuncs.py
+-rw-r--r--   0 Newville   (501) staff       (20)      411 2024-04-04 17:31:35.000000 lmfit-1.3.0/lmfit/version.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.693863 lmfit-1.3.0/lmfit.egg-info/
+-rw-r--r--   0 Newville   (501) staff       (20)    13054 2024-04-04 17:31:35.000000 lmfit-1.3.0/lmfit.egg-info/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     5290 2024-04-04 17:31:35.000000 lmfit-1.3.0/lmfit.egg-info/SOURCES.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        1 2024-04-04 17:31:35.000000 lmfit-1.3.0/lmfit.egg-info/dependency_links.txt
+-rw-r--r--   0 Newville   (501) staff       (20)      423 2024-04-04 17:31:35.000000 lmfit-1.3.0/lmfit.egg-info/requires.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        6 2024-04-04 17:31:35.000000 lmfit-1.3.0/lmfit.egg-info/top_level.txt
+-rwxr-xr-x   0 Newville   (501) staff       (20)     1010 2024-04-04 17:29:11.000000 lmfit-1.3.0/publish_docs.sh
+-rw-r--r--   0 Newville   (501) staff       (20)     3056 2024-04-04 17:29:11.000000 lmfit-1.3.0/pyproject.toml
+-rw-r--r--   0 Newville   (501) staff       (20)       38 2024-04-04 17:31:35.696578 lmfit-1.3.0/setup.cfg
+-rw-r--r--   0 Newville   (501) staff       (20)       92 2024-04-04 17:29:11.000000 lmfit-1.3.0/setup.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.692922 lmfit-1.3.0/tests/
+-rw-r--r--   0 Newville   (501) staff       (20)     6109 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/NISTModels.py
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)      893 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/conftest.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5656 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/gauss_modelresult_lmfit100.sav
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.693390 lmfit-1.3.0/tests/saved_models/
+-rw-r--r--   0 Newville   (501) staff       (20)      767 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/saved_models/sinemodel_py310_lm122.sav
+-rw-r--r--   0 Newville   (501) staff       (20)      863 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/saved_models/sinemodel_py311_lm122.sav
+-rw-r--r--   0 Newville   (501) staff       (20)      863 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/saved_models/sinemodel_py312_lm122.sav
+-rw-r--r--   0 Newville   (501) staff       (20)     1374 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_1variable.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7097 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_NIST_Strd.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4008 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_algebraic_constraint.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4640 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_ampgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1238 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_basicfit.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3663 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_basinhopping.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1900 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_bounded_jacobian.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1413 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_bounds.py
+-rw-r--r--   0 Newville   (501) staff       (20)    11428 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_brute.py
+-rw-r--r--   0 Newville   (501) staff       (20)    11953 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_builtin_models.py
+-rw-r--r--   0 Newville   (501) staff       (20)     9251 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_confidence.py
+-rw-r--r--   0 Newville   (501) staff       (20)     9987 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_covariance_matrix.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1235 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_custom_independentvar.py
+-rw-r--r--   0 Newville   (501) staff       (20)      612 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_default_kws.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2259 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_dual_annealing.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4292 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_itercb.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3066 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_jsonutils.py
+-rw-r--r--   0 Newville   (501) staff       (20)     6266 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_least_squares.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4780 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_lineshapes.py
+-rw-r--r--   0 Newville   (501) staff       (20)      781 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_manypeaks_speed.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3689 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_max_nfev.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2686 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_minimizer.py
+-rw-r--r--   0 Newville   (501) staff       (20)    58586 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)    12648 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_model_saveload.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4354 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_model_uncertainties.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4965 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_models.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2181 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_multidatasets.py
+-rw-r--r--   0 Newville   (501) staff       (20)    24062 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_nose.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1168 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_pandas.py
+-rw-r--r--   0 Newville   (501) staff       (20)    19779 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_parameter.py
+-rw-r--r--   0 Newville   (501) staff       (20)    21262 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_parameters.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4367 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_params_uvars.py
+-rw-r--r--   0 Newville   (501) staff       (20)    14955 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_printfuncs.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3999 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_shgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1503 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_stepmodel.py
```

### Comparing `lmfit-1.2.2/.github/CONTRIBUTING.md` & `lmfit-1.3.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/.github/ISSUE_TEMPLATE.md` & `lmfit-1.3.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/.github/PULL_REQUEST_TEMPLATE.md` & `lmfit-1.3.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/.pre-commit-config.yaml` & `lmfit-1.3.0/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 exclude: 'doc/conf.py'
 
 repos:
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.7.0
+    rev: v3.15.2
     hooks:
     -   id: pyupgrade
-        args: [--py37-plus]
+        args: [--py38-plus]
 
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
     -   id: check-ast
     -   id: check-builtin-literals
     -   id: check-case-conflict
     -   id: check-merge-conflict
     -   id: check-toml
     -   id: debug-statements
     -   id: end-of-file-fixer
     -   id: mixed-line-ending
     -   id: trailing-whitespace
     -   id: fix-encoding-pragma
         args: [--remove]
 
 -   repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
-        additional_dependencies: [flake8-deprecated, flake8-mutable]
+        additional_dependencies: [flake8-deprecated, flake8-mutable, Flake8-pyproject]
 
 -   repo: https://github.com/PyCQA/isort/
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
     -   id: isort
 
 -   repo: local
     hooks:
     -   id: rstcheck
         name: rstcheck
@@ -47,20 +47,21 @@
     hooks:
     -   id: rst-backticks
     -   id: rst-directive-colons
     -   id: rst-inline-touching-normal
     -   id: python-check-blanket-noqa
 
 -   repo: https://github.com/codespell-project/codespell
-    rev: v2.2.5
+    rev: v2.2.6
     hooks:
     -   id: codespell
         files: '.py|.rst'
-        exclude: 'doc/doc_examples_to_gallery.py'
+        exclude: 'doc/doc_examples_to_gallery.py|.ipynb'
         # escaped characters currently do not work correctly
         # so \nnumber is considered a spelling error....
         args: ["-L nnumber", "-L mone"]
 
 -   repo: https://github.com/asottile/yesqa
     rev: v1.5.0
     hooks:
     -   id: yesqa
+        additional_dependencies: [flake8-deprecated, flake8-mutable, Flake8-pyproject]
```

### Comparing `lmfit-1.2.2/AUTHORS.txt` & `lmfit-1.3.0/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/LICENSE` & `lmfit-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Bennett5.dat` & `lmfit-1.3.0/NIST_STRD/Bennett5.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/BoxBOD.dat` & `lmfit-1.3.0/NIST_STRD/BoxBOD.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Chwirut1.dat` & `lmfit-1.3.0/NIST_STRD/Chwirut1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Chwirut2.dat` & `lmfit-1.3.0/NIST_STRD/Chwirut2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/DanWood.dat` & `lmfit-1.3.0/NIST_STRD/DanWood.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/ENSO.dat` & `lmfit-1.3.0/NIST_STRD/ENSO.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Eckerle4.dat` & `lmfit-1.3.0/NIST_STRD/Eckerle4.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Gauss1.dat` & `lmfit-1.3.0/NIST_STRD/Gauss1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Gauss2.dat` & `lmfit-1.3.0/NIST_STRD/Gauss2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Gauss3.dat` & `lmfit-1.3.0/NIST_STRD/Gauss3.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Hahn1.dat` & `lmfit-1.3.0/NIST_STRD/Hahn1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Kirby2.dat` & `lmfit-1.3.0/NIST_STRD/Kirby2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Lanczos1.dat` & `lmfit-1.3.0/NIST_STRD/Lanczos1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Lanczos2.dat` & `lmfit-1.3.0/NIST_STRD/Lanczos2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Lanczos3.dat` & `lmfit-1.3.0/NIST_STRD/Lanczos3.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/MGH09.dat` & `lmfit-1.3.0/NIST_STRD/MGH09.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/MGH10.dat` & `lmfit-1.3.0/NIST_STRD/MGH10.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/MGH17.dat` & `lmfit-1.3.0/NIST_STRD/MGH17.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Misra1a.dat` & `lmfit-1.3.0/NIST_STRD/Misra1a.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Misra1b.dat` & `lmfit-1.3.0/NIST_STRD/Misra1b.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Misra1c.dat` & `lmfit-1.3.0/NIST_STRD/Misra1c.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Misra1d.dat` & `lmfit-1.3.0/NIST_STRD/Misra1d.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Models` & `lmfit-1.3.0/NIST_STRD/Models`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Nelson.dat` & `lmfit-1.3.0/NIST_STRD/Nelson.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Rat42.dat` & `lmfit-1.3.0/NIST_STRD/Rat42.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Rat43.dat` & `lmfit-1.3.0/NIST_STRD/Rat43.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Roszman1.dat` & `lmfit-1.3.0/NIST_STRD/Roszman1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/NIST_STRD/Thurber.dat` & `lmfit-1.3.0/NIST_STRD/Thurber.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/PKG-INFO` & `lmfit-1.3.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,7 @@
-Metadata-Version: 2.1
-Name: lmfit
-Version: 1.2.2
-Summary: Least-Squares Minimization with Bounds and Constraints
-Home-page: https://lmfit.github.io//lmfit-py/
-Author: LMFit Development Team
-Author-email: matt.newville@gmail.com
-License: BSD 3-Clause
-Project-URL: Source, https://github.com/lmfit/lmfit-py
-Project-URL: Changelog, https://lmfit.github.io/lmfit-py/whatsnew.html
-Project-URL: Documentation, https://lmfit.github.io/lmfit-py/
-Project-URL: Tracker, https://github.com/lmfit/lmfit-py/issues
-Keywords: curve-fitting,least-squares minimization
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-Provides-Extra: doc
-Provides-Extra: test
-Provides-Extra: all
-License-File: LICENSE
-License-File: AUTHORS.txt
-
 LMfit-py
 ========
 
 .. image:: https://dev.azure.com/lmfit/lmfit-py/_apis/build/status/lmfit.lmfit-py?branchName=master
     :target: https://dev.azure.com/lmfit/lmfit-py/_build/latest?definitionId=1&branchName=master
 
 .. image:: https://codecov.io/gh/lmfit/lmfit-py/branch/master/graph/badge.svg
```

### Comparing `lmfit-1.2.2/asv_benchmarking/asv.conf.json` & `lmfit-1.3.0/asv_benchmarking/asv.conf.json`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/asv_benchmarking/benchmarks/benchmarks.py` & `lmfit-1.3.0/asv_benchmarking/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/azure-pipelines.yml` & `lmfit-1.3.0/azure-pipelines.yml`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     - job: pre_commit
       pool:
         vmImage: 'ubuntu-latest'
 
       steps:
         - task: UsePythonVersion@0
           inputs:
-            versionSpec: '3.11'
+            versionSpec: '3.12'
         - script: |
             python -m pip install --upgrade build pip setuptools wheel
           displayName: 'Install Python build tools and dependencies'
         - script: |
             python -m build
             python -m pip install '.[dev]'
           displayName: 'Build wheel/sdist and install lmfit'
@@ -39,15 +39,15 @@
     - job: build_documentation
       pool:
         vmImage: 'ubuntu-latest'
 
       steps:
         - task: UsePythonVersion@0
           inputs:
-            versionSpec: '3.11'
+            versionSpec: '3.12'
         - script: |
             python -m pip install --upgrade build pip setuptools wheel
           displayName: 'Install Python build tools'
         - script: |
             python -m build
             python -m pip install '.[doc]'
           displayName: 'Build wheel/sdist and install lmfit'
@@ -63,16 +63,14 @@
   condition: succeededOrFailed()
   jobs:
     - job:
       pool:
         vmImage: 'ubuntu-latest'
       strategy:
         matrix:
-          Python37:
-            python.version: '3.7'
           Python38:
             python.version: '3.8'
 
       steps:
         - task: UsePythonVersion@0
           inputs:
             versionSpec: '$(python.version)'
@@ -80,15 +78,15 @@
         - script: |
             sudo apt-get update && sudo apt-get install -yq --no-install-suggests --no-install-recommends \
             libatlas-base-dev liblapack-dev gfortran libgmp-dev libmpfr-dev libsuitesparse-dev ccache \
             swig libmpc-dev
           displayName: 'Install dependencies'
         - script: |
             python -m pip install --upgrade build pip wheel
-            python -m pip install asteval==0.9.28 numpy==1.19.0 scipy==1.6.0 uncertainties==3.1.4
+            python -m pip install asteval==0.9.28 numpy==1.23.0 scipy==1.8.0 uncertainties==3.1.4
           displayName: 'Install minimum required version of dependencies'
         - script: |
             python -m build
             python -m pip install ".[test]"
           displayName: 'Build wheel/sdist and install lmfit'
         - script: |
             python -m pip list
@@ -115,24 +113,24 @@
   condition: succeededOrFailed()
   jobs:
     - job:
       pool:
         vmImage: 'ubuntu-latest'
       strategy:
         matrix:
-          Python37:
-            python.version: '3.7'
           Python38:
             python.version: '3.8'
           Python39:
             python.version: '3.9'
           Python310:
             python.version: '3.10'
           Python311:
             python.version: '3.11'
+          Python312:
+            python.version: '3.12'
 
       steps:
         - task: UsePythonVersion@0
           inputs:
             versionSpec: '$(python.version)'
           displayName: 'Use Python $(python.version)'
         - script: |
@@ -163,26 +161,25 @@
             shasum -a 256 -c codecov.SHA256SUM
             chmod +x codecov
           displayName: 'Download and verify codecov uploader'
         - script: |
             ./codecov -v -f "coverage.xml"
           displayName: 'Upload to codecov.io'
 
-# Python 3.11 on Windows currently fails to build pycairo
 - stage: test_Windows_latest
   dependsOn: check_codestyle
   condition: succeededOrFailed()
   jobs:
     - job:
       pool:
         vmImage: 'windows-latest'
       strategy:
         matrix:
-          Python310:
-            python.version: '3.10'
+          Python312:
+            python.version: '3.12'
 
       steps:
         - task: UsePythonVersion@0
           inputs:
             versionSpec: '$(python.version)'
           displayName: 'Use Python $(python.version)'
         - script: |
@@ -208,16 +205,16 @@
   condition: succeededOrFailed()
   jobs:
     - job:
       pool:
         vmImage: 'macos-latest'
       strategy:
         matrix:
-          Python311:
-            python.version: '3.11'
+          Python312:
+            python.version: '3.12'
 
       steps:
         - task: UsePythonVersion@0
           inputs:
             versionSpec: '$(python.version)'
           displayName: 'Use Python $(python.version)'
         - script: |
@@ -235,66 +232,66 @@
             pytest
           displayName: 'Run test-suite and collect coverage'
 
 - stage: development_version
   dependsOn: check_codestyle
   condition: succeededOrFailed()
   jobs:
-    - job: Python312_dev
+    - job: Python313_dev
       pool:
         vmImage: 'ubuntu-latest'
       steps:
         - script: |
             sudo add-apt-repository ppa:deadsnakes/nightly
-            sudo apt-get update && sudo apt-get install -y --no-install-recommends python3.12-dev python3.12-venv
+            sudo apt-get update && sudo apt-get install -y --no-install-recommends python3.13-dev python3.13-venv
           displayName: Install Python development version from the deadsnakes PPA
         - script: |
             sudo apt-get update && sudo apt-get install -yq --no-install-suggests --no-install-recommends \
             libatlas-base-dev liblapack-dev gfortran libgmp-dev libmpfr-dev libsuitesparse-dev ccache \
             swig libmpc-dev
           displayName: 'Install dependencies'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
-            ##curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
-            ##python3.12 get-pip.py --user
-            python3.12 -m ensurepip --upgrade
-            pip3.12 install -U build pip setuptools wheel pybind11 cython || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
+            python3.13 -m ensurepip --upgrade
+            pip3.13 install -U build pip setuptools wheel pybind11 cython || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install build, pip, setuptools, wheel, pybind11, and cython'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
-            export numpy_version=1.25.0
+            export numpy_version=1.26.4
             wget https://github.com/numpy/numpy/releases/download/v${numpy_version}/numpy-${numpy_version}.tar.gz
             tar xzvf numpy-${numpy_version}.tar.gz
             cd numpy-${numpy_version}
-            python3.12 setup.py install --user || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
+            python3.13 -m build || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
+            python3.13 -m pip install . --user || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install latest available version of NumPy'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
-            pip3.12 install -U pythran || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
+            pip3.13 install -U pythran || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install pythran'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
-            export scipy_version=1.10.1
+            export scipy_version=1.13.0
             wget https://github.com/scipy/scipy/releases/download/v${scipy_version}/scipy-${scipy_version}.tar.gz
             tar xzvf scipy-${scipy_version}.tar.gz
             cd scipy-${scipy_version}
-            python3.12 setup.py install --user || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
+            python3.13 -m build || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
+            python3.13 -m pip install . --user || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install latest available version of SciPy'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
             # remove numdifftools for now as it pulls in statsmodels, that wants to build with NumPy 1.14.5
-            pip3.12 install asteval uncertainties dill emcee flaky pytest pytest-cov || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
+            pip3.13 install asteval uncertainties dill emcee flaky pytest pytest-cov || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install latest available version of Python dependencies'
         - script: |
-            python3.12 -m build
-            python3.12 -m pip install '.[test]' --user || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
+            python3.13 -m build
+            python3.13 -m pip install '.[test]' --user || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Build wheel/sdist and install lmfit'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
-            pip3.12 list || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
+            pip3.13 list || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'List installed Python packages'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
-            pip3.12 install pytest-azurepipelines
+            pip3.13 install pytest-azurepipelines
             cd $(Agent.BuildDirectory)/s/tests
             pytest || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Run test-suite'
```

### Comparing `lmfit-1.2.2/doc/Makefile` & `lmfit-1.3.0/doc/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 .PHONY: help clean html dirhtml pickle json htmlhelp qthelp latex changes linkcheck doctest latexpdf htmlzip
 .PHONY: all pdf gallery debug
 
 html:  gallery
 	cp sphinx/ext_mathjax.py extensions.py
 	$(SPHINXBUILD) -b html $(SPHINX_OUTPUT) $(SPHINX_OPTS) . $(BUILDDIR)/html
+	./filter_spurious_link_from_html.py
 	@echo
 	@echo "html build finished: $(BUILDDIR)/html."
 
 debug:  gallery
 	cp sphinx/ext_mathjax.py extensions.py
 	$(SPHINXBUILD) -b html $(SPHINX_OUTPUT) $(SPHINX_DEBUGOPTS) . $(BUILDDIR)/html
 	./filter_spurious_link_from_html.py
@@ -71,14 +72,15 @@
 clean:
 	-rm -rf $(BUILDDIR)
 	-rm -f extensions.py
 	-rm -f *.dat *.sav *.csv
 	-rm -rf examples/*
 	-rm -rf ../examples/documentation
 	-rm -rf __pycache__
+	-rm -rf sg_execution_times.rst
 
 dirhtml:  gallery
 	$(SPHINXBUILD) -b dirhtml $(SPHINX_OUTPUT) $(SPHINX_OPTS) . $(BUILDDIR)/dirhtml
 	@echo
 	@echo "Build finished. The HTML pages are in $(BUILDDIR)/dirhtml."
 
 pickle:  gallery
```

### Comparing `lmfit-1.2.2/doc/_templates/indexsidebar.html` & `lmfit-1.3.0/doc/_templates/indexsidebar.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/bounds.rst` & `lmfit-1.3.0/doc/bounds.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/builtin_models.rst` & `lmfit-1.3.0/doc/builtin_models.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/conf.py` & `lmfit-1.3.0/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 # shpinx.ext.autodoc settings
 autoclass_content = 'both'
 
 # shpinx.ext.intersphinx settings
 intersphinx_mapping = {'py': ('https://docs.python.org/3', None),
                        'numpy': ('https://numpy.org/doc/stable/', None),
-                       'scipy': ('https://matplotlib.org/stable/', None),
+                       'scipy': ('https://docs.scipy.org/doc/scipy/', None),
                        'matplotlib': ('https://matplotlib.org/stable/', None),
                        'pandas': ('https://pandas.pydata.org/pandas-docs/stable/', None),
                        'sympy': ('https://docs.sympy.org/latest/', None),
                        }
 
 # shpinx.ext.extlinks settings
 extlinks = {
```

### Comparing `lmfit-1.2.2/doc/confidence.rst` & `lmfit-1.3.0/doc/confidence.rst`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 But for some models, the sum of two exponentials for example, the approximation
 begins to fail. For this case, lmfit has the function :func:`conf_interval`
 to calculate confidence intervals directly. This is substantially slower
 than using the errors estimated from the covariance matrix, but the results
 are more robust.
 
+Please note that :func:`conf_interval` is not suited to work with
+fit results obtained by ``emcee``.
 
 Method used for calculating confidence intervals
 ------------------------------------------------
 
 The F-test is used to compare our null model, which is the best fit we have
 found, with an alternate model, where one of the parameters is fixed to a
 specific value. The value is changed until the difference between :math:`\chi^2_0`
@@ -178,15 +180,17 @@
 
 The reports show that we obtained a pretty good fit, and that the automated
 estimates of the uncertainties are actually pretty good -- agreeing to the
 second decimal place.  But we also see that some of the uncertainties do become
 noticeably asymmetric at high :math:`n-\sigma` levels.
 
 We'll plot this data and fit, and then further explore these uncertainties
-using :func:`conf_interval2d`:
+using :func:`conf_interval2d`. Please note that :func:`conf_interval2d` shows the
+confidence intervals obtained considering the standard errors, not those obtained
+by 'conf_interval(out, out, sigmas=sigma_levels)'.
 
 .. jupyter-execute::
 
     #########################
     # plot initial fit
     colors = ('#2030b0', '#b02030', '#207070')
     fig, axes = plt.subplots(2, 3, figsize=(15, 9.5))
@@ -194,40 +198,47 @@
     axes[0, 0].plot(x, y, 'o', markersize=3, label='data', color=colors[0])
     axes[0, 0].plot(x, out.best_fit, label='fit', color=colors[1])
     axes[0, 0].set_xlabel('x')
     axes[0, 0].set_ylabel('y')
     axes[0, 0].legend()
 
     aix, aiy = 0, 0
-    nsamples = 30
+    nsamples = 50
+    explicitly_calculate_sigma = True
+
     for pairs in (('sigma', 'amplitude'), ('intercept', 'amplitude'),
                   ('slope', 'intercept'), ('slope', 'center'), ('sigma', 'center')):
-        xpar, ypar = pairs
-        print("Generating chi-square map for ", pairs)
-        c_x, c_y, dchi2_mat = conf_interval2d(out, out, xpar, ypar,
-                                              nsamples, nsamples,
-                                              nsigma=3.5, chi2_out=True)
-        # sigma matrix: sigma increases chi_square
-        # from  chi_square_best
-        # to    chi_square + sigma**2 * reduced_chi_square
-        # so:   sigma = sqrt(dchi2 / reduced_chi_square)
-        sigma_mat = np.sqrt(abs(dchi2_mat)/out.redchi)
 
-        # you could calculate the matrix of probabilities from sigma as:
-        # prob_mat  = np.erf(sigma_mat/np.sqrt(2))
+        xpar, ypar = pairs
+        if explicitly_calculate_sigma:
+            print(f"Generating chi-square map for {pairs}")
+            c_x, c_y, chi2_mat = conf_interval2d(out, out, xpar, ypar,
+                                                 nsamples, nsamples, nsigma=3.5,
+                                                 chi2_out=True)
+            # explicitly calculate sigma matrix: sigma increases chi_square
+            # from  chi_square_best
+            # to    chi_square + sigma**2 * reduced_chi_square
+            # so:   sigma = sqrt((chi2-chi2_best)/ reduced_chi_square)
+            chi2_min = chi2_mat.min()
+            sigma_mat = np.sqrt((chi2_mat-chi2_min)/out.redchi)
+        else:
+            print(f"Generating sigma map for {pairs}")
+            # or, you could just calculate the matrix of probabilities as:
+            c_x, c_y, sigma_mat = conf_interval2d(out, out, xpar, ypar,
+                                                  nsamples, nsamples, nsigma=3.5)
 
         aix += 1
         if aix == 2:
             aix = 0
             aiy += 1
         ax = axes[aix, aiy]
 
         cnt = ax.contour(c_x, c_y, sigma_mat, levels=sigma_levels, colors=colors,
                          linestyles='-')
-        ax.clabel(cnt, inline=True, fmt="$\sigma=%.0f$", fontsize=13)
+        ax.clabel(cnt, inline=True, fmt=r"$\sigma=%.0f$", fontsize=13)
 
         # draw boxes for estimated uncertaties:
         #  dotted :  scaled stderr from initial fit
         #  dashed :  values found from conf_interval()
         xv = out.params[xpar].value
         xs = out.params[xpar].stderr
         yv = out.params[ypar].value
```

### Comparing `lmfit-1.2.2/doc/constraints.rst` & `lmfit-1.3.0/doc/constraints.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/doc_examples_to_gallery.py` & `lmfit-1.3.0/doc/doc_examples_to_gallery.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/faq.rst` & `lmfit-1.3.0/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/filter_spurious_link_from_html.py` & `lmfit-1.3.0/doc/filter_spurious_link_from_html.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/fitting.rst` & `lmfit-1.3.0/doc/fitting.rst`

 * *Files 2% similar despite different names*

```diff
@@ -326,30 +326,48 @@
 +----------------------+----------------------------------------------------------------------------+
 |    nvarys            | number of variables in fit :math:`N_{\rm varys}`                           |
 +----------------------+----------------------------------------------------------------------------+
 |    ndata             | number of data points: :math:`N`                                           |
 +----------------------+----------------------------------------------------------------------------+
 |    nfree             | degrees of freedom in fit: :math:`N - N_{\rm varys}`                       |
 +----------------------+----------------------------------------------------------------------------+
+|    aborted           | boolean of whether the fit has been aborted.                               |
++----------------------+----------------------------------------------------------------------------+
+|    success           | boolean for a minimal test of whether the fit finished successfully        |
++----------------------+----------------------------------------------------------------------------+
+|    errorbars         | boolean of whether error bars and unccertainty were estimated              |
++----------------------+----------------------------------------------------------------------------+
+|    ier               | integer flag describing message from ``leastsq``.                          |
++----------------------+----------------------------------------------------------------------------+
+|    message           | simple message from ``leastsq``                                            |
++----------------------+----------------------------------------------------------------------------+
+|    method            | name of fitting methods                                                    |
++----------------------+----------------------------------------------------------------------------+
 |    residual          | residual array, returned by the objective function: :math:`\{\rm Resid_i\}`|
 +----------------------+----------------------------------------------------------------------------+
 |    chisqr            | chi-square: :math:`\chi^2 = \sum_i^N [{\rm Resid}_i]^2`                    |
 +----------------------+----------------------------------------------------------------------------+
 |    redchi            | reduced chi-square: :math:`\chi^2_{\nu}= {\chi^2} / {(N - N_{\rm varys})}` |
 +----------------------+----------------------------------------------------------------------------+
 |    aic               | Akaike Information Criterion statistic (see below)                         |
 +----------------------+----------------------------------------------------------------------------+
 |    bic               | Bayesian Information Criterion statistic (see below)                       |
 +----------------------+----------------------------------------------------------------------------+
+|    params            | best-fit parameters after fit, with uncertainties is available             |
++----------------------+----------------------------------------------------------------------------+
 |    var_names         | ordered list of variable parameter names used for init_vals and covar      |
 +----------------------+----------------------------------------------------------------------------+
 |    covar             | covariance matrix (with rows/columns using var_names)                      |
 +----------------------+----------------------------------------------------------------------------+
 |    init_vals         | list of initial values for variable parameters                             |
 +----------------------+----------------------------------------------------------------------------+
+|    init_values       | dictionary of initial values for variable Parameters.                      |
++----------------------+----------------------------------------------------------------------------+
+|    uvars             | dictionary of uncertainties uvalues for all Parameters.                    |
++----------------------+----------------------------------------------------------------------------+
 |    call_kws          | dict of keyword arguments sent to underlying solver                        |
 +----------------------+----------------------------------------------------------------------------+
 
 Note that the calculation of chi-square and reduced chi-square assume
 that the returned residual function is scaled properly to the
 uncertainties in the data. For these statistics to be meaningful, the
 person writing the function to be minimized **must** scale them properly.
@@ -420,23 +438,33 @@
 the Bayesian information criterion is considered the most conservative of
 these statistics.
 
 
 Uncertainties in Variable Parameters, and their Correlations
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+.. _uncertainties:   https://github.com/lebigot/uncertainties/
+
 As mentioned above, when a fit is complete the uncertainties for fitted
-Parameters as well as the correlations between pairs of Parameters are
-usually calculated. This happens automatically either when using the
-default :meth:`leastsq` method, the :meth:`least_squares` method, or for
-most other fitting methods if the highly-recommended ``numdifftools``
-package is available. The estimated standard error (the :math:`1\sigma`
-uncertainty) for each variable Parameter will be contained in the
-:attr:`stderr`, while the :attr:`correl` attribute for each Parameter will
-contain a dictionary of the correlation with each other variable Parameter.
+Parameters as well as the correlations between pairs of Parameters are usually
+calculated. This happens automatically either when using the default
+:meth:`leastsq` method, the :meth:`least_squares` method, or for most other
+fitting methods if the highly-recommended ``numdifftools`` package is
+available. The estimated standard error (the :math:`1\sigma` uncertainty) for
+each variable Parameter will be contained in the :attr:`stderr`, while the
+:attr:`correl` attribute for each Parameter will contain a dictionary of the
+correlation with each other variable Parameter.  These updated parameters with
+uncertainty and correlation information will be placed in
+``MinimizerResult.params``, so that you may access the best fit value, standard
+error and correlation. For a successful fit for which uncertainties and
+correlations can be calculated, the ``MinimizerResult`` will also have a
+``uvars`` attribute that is a dictionary with keynames for each Parameter
+(includnig constraints) and values of ``Ufloats`` from the `uncertainties`_
+package using the best fit values, the standard error and the correlation
+between Parameters.
 
 These estimates of the uncertainties are done by inverting the Hessian
 matrix which represents the second derivative of fit quality for each
 variable parameter. There are situations for which the uncertainties cannot
 be estimated, which generally indicates that this matrix cannot be inverted
 because one of the fit is not actually sensitive to one of the variables.
 This can happen if a Parameter is stuck at an upper or lower bound, if the
```

### Comparing `lmfit-1.2.2/doc/index.rst` & `lmfit-1.3.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/installation.rst` & `lmfit-1.3.0/doc/installation.rst`

 * *Files 3% similar despite different names*

```diff
@@ -28,40 +28,41 @@
 .. _flaky: https://github.com/box/flaky
 .. _SymPy: https://www.sympy.org/
 .. _Latexmk: https://ctan.org/pkg/latexmk/
 
 Prerequisites
 ~~~~~~~~~~~~~
 
-Lmfit works with `Python`_ versions 3.7 and higher. Version
+Lmfit works with `Python`_ versions 3.8 and higher. Version
 0.9.15 is the final version to support Python 2.7.
 
 Lmfit requires the following Python packages, with versions given:
-   * `NumPy`_ version 1.19 or higher.
-   * `SciPy`_ version 1.6 or higher.
+   * `NumPy`_ version 1.23 or higher.
+   * `SciPy`_ version 1.8 or higher.
    * `asteval`_ version 0.9.28 or higher.
    * `uncertainties`_ version 3.1.4 or higher.
+   * `dill`_ version 0.3.4 or higher.
 
 All of these are readily available on PyPI, and are installed
 automatically if installing with ``pip install lmfit``.
 
 In order to run the test suite, the `pytest`_, `pytest-cov`_, and `flaky`_
 packages are required. Some functionality requires the `emcee`_ (version 3+),
-`corner`_, `pandas`_, `Jupyter`_, `matplotlib`_, `dill`_, or `numdifftools`_
+`corner`_, `pandas`_, `Jupyter`_, `matplotlib`_, or `numdifftools`_
 packages. These are not installed automatically, but we highly recommend each
 of them.
 
 For building the documentation and generating the examples gallery, `matplotlib`_,
 `emcee`_ (version 3+), `corner`_, `Sphinx`_, `sphinx-gallery`_, `jupyter_sphinx`_,
 `ipykernel`_, `Pillow`_, and `SymPy`_ are required. For generating the PDF documentation,
 the Python packages `sphinxcontrib-svg2pdfconverter`_ and `cairosvg`_ are also required,
 as well as the LaTex package `Latexmk`_ (which is included by default in some
 LaTex distributions).
 
-Please refer to ``setup.cfg`` under ``options.extras_require`` for a list of all
+Please refer to ``pyproject.toml`` under ``project.optional-dependencies`` for a list of all
 dependencies that are needed if you want to participate in the development of lmfit.
 You can install all these dependencies automatically by doing ``pip install lmfit[all]``,
 or select only a subset (e.g., ``dev```, ``doc``, or ``test``).
 
 Please note: the "original" ``python setup.py install`` is deprecated, but we will
 provide a shim ``setup.py`` file for as long as ``Python`` and/or ``setuptools``
 allow the use of this legacy command.
@@ -96,15 +97,15 @@
 and install using::
 
    pip install --upgrade build pip setuptools wheel
 
 to install the required build dependencies and then do::
 
    python -m build
-   pip install ".[all]'
+   pip install ".[all]"
 
 to generate the wheel and install ``lmfit`` with all its dependencies.
 
 We welcome all contributions to lmfit! If you cloned the repository for this
 purpose, please read `CONTRIBUTING.md`_ for more detailed instructions.
 
 Testing
```

### Comparing `lmfit-1.2.2/doc/intro.rst` & `lmfit-1.3.0/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/make.bat` & `lmfit-1.3.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/model.rst` & `lmfit-1.3.0/doc/model.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,53 +2,53 @@
 
 ===============================
 Modeling Data and Curve Fitting
 ===============================
 
 .. module:: lmfit.model
 
-A common use of least-squares minimization is *curve fitting*, where one
-has a parametrized model function meant to explain some phenomena and wants
-to adjust the numerical values for the model so that it most closely
-matches some data. With :mod:`scipy`, such problems are typically solved
-with :scipydoc:`optimize.curve_fit`, which is a wrapper around
-:scipydoc:`optimize.leastsq`. Since lmfit's
-:func:`~lmfit.minimizer.minimize` is also a high-level wrapper around
-:scipydoc:`optimize.leastsq` it can be used for curve-fitting problems.
-While it offers many benefits over :scipydoc:`optimize.leastsq`, using
-:func:`~lmfit.minimizer.minimize` for many curve-fitting problems still
-requires more effort than using :scipydoc:`optimize.curve_fit`.
-
-The :class:`Model` class in lmfit provides a simple and flexible approach
-to curve-fitting problems. Like :scipydoc:`optimize.curve_fit`, a
-:class:`Model` uses a *model function* -- a function that is meant to
-calculate a model for some phenomenon -- and then uses that to best match
-an array of supplied data. Beyond that similarity, its interface is rather
-different from :scipydoc:`optimize.curve_fit`, for example in that it uses
-:class:`~lmfit.parameter.Parameters`, but also offers several other
-important advantages.
+A common use of least-squares minimization is *curve fitting*, where one has a
+parametrized model function meant to explain some phenomena and wants to adjust
+the numerical values for the model so that it most closely matches some
+data. With :mod:`scipy`, such problems are typically solved with
+:scipydoc:`optimize.curve_fit`, which is a wrapper around
+:scipydoc:`optimize.least_squares`.  While :func:`~lmfit.minimizer.minimize`
+can be used for curve-fitting problems, it is more general and not aimed
+specifically at this common use-case.
+
+
+The :class:`Model` class in lmfit provides a simple and flexible approach to
+curve-fitting problems. Like :scipydoc:`optimize.curve_fit`, a :class:`Model`
+uses a *model function* -- a function that is meant to calculate a model for
+some phenomenon -- and then uses that to best match an array of supplied
+data.  Beyond that similarity, the :class:`Model` interface is rather different
+from :scipydoc:`optimize.curve_fit`.  These differences include a) being
+class-based and so having multiple methods for working with :class:`Model`s,
+b) using :class:`~lmfit.parameter.Parameters`, and all of the advantages they
+provide, and c) being easy to combine into composite models.
+
 
 In addition to allowing you to turn any model function into a curve-fitting
-method, lmfit also provides canonical definitions for many known lineshapes
+model, lmfit also provides canonical definitions for many known line shapes
 such as Gaussian or Lorentzian peaks and Exponential decays that are widely
 used in many scientific domains. These are available in the :mod:`models`
 module that will be discussed in more detail in the next chapter
 (:ref:`builtin_models_chapter`). We mention it here as you may want to
 consult that list before writing your own model. For now, we focus on
 turning Python functions into high-level fitting models with the
 :class:`Model` class, and using these to fit data.
 
 
 Motivation and simple example: Fit data to Gaussian profile
 ===========================================================
 
-Let's start with a simple and common example of fitting data to a Gaussian
-peak. As we will see, there is a built-in :class:`GaussianModel` class that
-can help do this, but here we'll build our own. We start with a simple
-definition of the model function:
+We start with a simple and common example of fitting data to a Gaussian
+peak. As we will see, there is a built-in :class:`GaussianModel` class that can
+help do this, but here we'll build our own. We start with a simple definition
+of the model function:
 
 .. jupyter-execute::
     :hide-code:
 
     import matplotlib as mpl
     mpl.rcParams['figure.dpi'] = 150
     %matplotlib inline
@@ -58,67 +58,68 @@
 
     from numpy import exp, linspace, random
 
 
     def gaussian(x, amp, cen, wid):
         return amp * exp(-(x-cen)**2 / wid)
 
-We want to use this function to fit to data :math:`y(x)` represented by the
+With that function, we can easily calculate a model for our data, and the goal
+here is to use this function to fit to data :math:`y(x)` represented by the
 arrays ``y`` and ``x``.  With :scipydoc:`optimize.curve_fit`, this would be:
 
 .. jupyter-execute::
     :hide-output:
 
     from scipy.optimize import curve_fit
 
     x = linspace(-10, 10, 101)
     y = gaussian(x, 2.33, 0.21, 1.51) + random.normal(0, 0.2, x.size)
 
     init_vals = [1, 0, 1]  # for [amp, cen, wid]
     best_vals, covar = curve_fit(gaussian, x, y, p0=init_vals)
 
-That is, we create data, make an initial guess of the model values, and run
-:scipydoc:`optimize.curve_fit` with the model function, data arrays, and
-initial guesses. The results returned are the optimal values for the
-parameters and the covariance matrix. It's simple and useful, but it
-misses the benefits of lmfit.
+That is, we create data (maybe adding a little noise), make an initial guess of
+the model values, and run :scipydoc:`optimize.curve_fit` with the model
+function, data arrays, and initial guesses. The results returned are the
+optimal values for the parameters and the covariance matrix.
 
 With lmfit, we create a :class:`Model` that wraps the ``gaussian`` model
 function, which automatically generates the appropriate residual function,
 and determines the corresponding parameter names from the function
 signature itself:
 
 .. jupyter-execute::
 
     from lmfit import Model
 
     gmodel = Model(gaussian)
     print(f'parameter names: {gmodel.param_names}')
     print(f'independent variables: {gmodel.independent_vars}')
 
-As you can see, the Model ``gmodel`` determined the names of the parameters
-and the independent variables. By default, the first argument of the
-function is taken as the independent variable, held in
-:attr:`independent_vars`, and the rest of the functions positional
-arguments (and, in certain cases, keyword arguments -- see below) are used
-for Parameter names. Thus, for the ``gaussian`` function above, the
-independent variable is ``x``, and the parameters are named ``amp``,
-``cen``, and ``wid``, and -- all taken directly from the signature of the
-model function. As we will see below, you can modify the default
-assignment of independent variable / arguments and specify yourself what
-the independent variable is and which function arguments should be identified
-as parameter names.
+As you can see, the Model ``gmodel`` determined the names of the parameters and
+the independent variables. By default, the first argument of the function is
+taken as the independent variable, held in :attr:`independent_vars`, and the
+rest of the functions positional arguments (and, in certain cases, keyword
+arguments -- see below) are used for Parameter names. Thus, for the
+``gaussian`` function above, the independent variable is ``x``, and the
+parameters are named ``amp``, ``cen``, and ``wid``.  These are all taken
+directly from the signature of the model function. As discussed below, you can
+modify the default assignment of independent variable / arguments and specify
+yourself what the independent variable.
 
+Although the model determines what the parameters should be named,
 :class:`~lmfit.parameter.Parameters` are *not* created when the model is
-created. The model knows what the parameters should be named, but nothing about
-the scale and range of your data. To help you create Parameters for a Model,
-each model has a :meth:`make_params` method that will generate parameters with
-the expected names. You will have to do this, or make Parameters some other way
-(say, with :func:`~lmfit.parameter.create_params`), and assign initial values
-for all Parameters. You can also assign other attributes when doing this:
+created.  That is, the model knows the parameters names, but nothing about the
+scale and range of your data.  You will have to make Parameters for a Model
+yourself.  To help you create Parameters for a Model, each model has a
+:meth:`make_params` method that will generate parameters with the
+expected names.  You can use this method or create Parameters some other way
+(say, with :func:`~lmfit.parameter.create_params`), but you will have to create
+Parameters and assign initial values for all Parameters. You can also assign
+other attributes when doing this:
 
 .. jupyter-execute::
 
     params = gmodel.make_params()
 
 This creates the :class:`~lmfit.parameter.Parameters` but does not
 automatically give them initial values since it has no idea what the scale
@@ -238,15 +239,15 @@
 
    See :ref:`model_param_hints_section`.
 
 .. automethod:: Model.print_param_hints
 
    See :ref:`model_param_hints_section`.
 
-..  automethod:: Model.post_fit
+.. automethod:: Model.post_fit
 
    See :ref:`modelresult_uvars_postfit_section`.
 
 
 :class:`Model` class Attributes
 -------------------------------
 
@@ -297,29 +298,51 @@
    ``g1_amplitude``, ``g1_center``, and ``g1_sigma``. This can be
    essential to avoid name collision in composite models.
 
 
 Determining parameter names and independent variables for a function
 --------------------------------------------------------------------
 
-The :class:`Model` created from the supplied function ``func`` will create a
-:class:`~lmfit.parameter.Parameters` object, and names are inferred from the
-function` arguments, and a residual function is automatically constructed.
-
-By default, the independent variable is taken as the first argument to the
-function. You can, of course, explicitly set this, and will need to do so
-if the independent variable is not first in the list, or if there is actually
-more than one independent variable.
-
-If not specified, Parameters are constructed from all positional arguments
-and all keyword arguments that have a default value that is numerical, except
-the independent variable, of course. Importantly, the Parameters can be
-modified after creation. In fact, you will have to do this because none of the
-parameters have valid initial values. In addition, one can place bounds and
-constraints on Parameters, or fix their values.
+The :class:`Model` created from the supplied function ``func`` will guess which
+function arguments of the model function should be made into
+:class:`~lmfit.parameter.Parameters` object, and which should be considered
+non-varying **independent variables** that need to be specified when evaluating
+or fitting with the Model.
+
+By convention and by default, the first argument to the model function is taken
+to be the independent variable -- this is often the ``x`` value for the model.
+You can explicitly set this to be a different functional argument, and will
+need to do so if the independent variable is not first in the list, or if there
+is more than one independent variable.  Since curve fitting most commonly fits
+some function :math:`y(x)`, it is common for the independent variable to be a
+numpy float ndarray of the same length as the data to be fit. While this is
+common, it is not actually required.  The independent variable does not not
+need to be an ndarray, and can be any Python data type, and it is fine to
+have multiple independent variables.
+
+.. versionchanged:: 1.2.3
+
+
+By convention and default, the positional arguments (that is, those without
+default values specified in the function signature) other than the first
+argument are marked as being Parameters -- these will have an invalid default
+value (or ``-Inf``) that must be supplied before using the Parameter. Keyword
+arguments to the model function that have numerical values will also be marked
+as being Parameters, and the supplied numerical value will be used as the
+default value for that Parameter.
+
+Keyword arguments to the model function that have non-numerical values
+(including ``None``, ``False``, and ``True``, but also strings) will be marked
+as being independent variables and their default value will be stored and used
+unless overwritten.  There is some ambiguity for function arguments that have a
+value supplied in the function signature of ``None``, ``False``, or ``True``.
+These function arguments are tagged as independent variables, but can be made
+into a Parameter with :meth:`Model.make_params`, in which case, they will be
+treated as variables.  An example is given below.
+
 
 
 Explicitly specifying ``independent_vars``
 ------------------------------------------
 
 As we saw for the Gaussian example above, creating a :class:`Model` from a
 function is fairly easy. Let's try another one:
@@ -338,17 +361,17 @@
     print(f'independent variables: {decay_model.independent_vars}')
 
     params = decay_model.make_params()
     print('\nParameters:')
     for pname, par in params.items():
         print(pname, par)
 
-Here, ``t`` is assumed to be the independent variable because it is the
-first argument to the function. The other function arguments are used to
-create parameters for the model.
+Here, ``t`` is assumed to be the independent variable because it is the first
+argument to the function. The other function arguments are used to create
+parameters for the model.
 
 If you want ``tau`` to be the independent variable in the above example,
 you can say so:
 
 .. jupyter-execute::
 
     decay_model = Model(decay, independent_vars=['tau'])
@@ -366,61 +389,100 @@
 
 independent variable
     A function argument that is not a parameter or otherwise part of the
     model, and that will be required to be explicitly provided as a
     keyword argument for each fit with :meth:`Model.fit` or evaluation
     with :meth:`Model.eval`.
 
-Note that independent variables are not required to be arrays, or even
-floating point numbers.
+Note that independent variables are not required to be arrays, or even floating
+point numbers.  Dictionaries or Objects from user-defined classes can be
+independent variables.
 
 
 Functions with keyword arguments
 --------------------------------
 
 If the model function had keyword parameters, these would be turned into
-Parameters if the supplied default value was a valid number (but not
-``None``, ``True``, or ``False``).
+Parameters if the supplied default value was a valid number:
 
 .. jupyter-execute::
 
     def decay2(t, tau, N=10, check_positive=False):
         if check_positive:
             arg = abs(t)/max(1.e-9, abs(tau))
         else:
             arg = t/tau
         return N*np.exp(arg)
 
 
     mod = Model(decay2)
+    print(f'independent variables: {mod.independent_vars}')
+
     params = mod.make_params()
     print('Parameters:')
     for pname, par in params.items():
         print(pname, par)
 
-Here, even though ``N`` is a keyword argument to the function, it is turned
-into a parameter, with the default numerical value as its initial value.
-By default, it is permitted to be varied in the fit -- the 10 is taken as
-an initial value, not a fixed value. On the other hand, the
-``check_positive`` keyword argument, was not converted to a parameter
-because it has a boolean default value. In some sense,
-``check_positive`` becomes like an independent variable to the model.
-However, because it has a default value it is not required to be given for
-each model evaluation or fit, as independent variables are.
+Here, ``check_positive`` is listed as an independent variable, because it
+has a default value of ``False``.
+
+The function argument ``N`` is expected to be an Parameter, because it has a
+numerical default value. This value will be kept as the default value when
+building the Parameters. Also, note that the default value for ``tau`` is
+``-np.inf``, which will need to be fixed before really be used.
+
+Function arguments with default values of ``None``, ``False``, and ``True`` are
+slightly ambiguous whether they should be considered independent variables or
+Parameters.  That is, in many contexts (including basic arithmetic) ``True``
+acts like the integer 1, and ``False`` acts like 0.  A default value of
+``None`` might be used to signal some default behavior.  For example, the
+builtin :func:`lmfit.lineshapes.voigt` function is defined as
+
+.. jupyter-execute::
+
+
+    def voigt(x, amplitude=1.0, center=0.0, sigma=1.0, gamma=None):
+        """Return a 1-dimensional Voigt function.
+            ...
+        """
+        if gamma is None:
+            gamma = sigma
+        z = (x-center + 1j*gamma) / max(tiny, (sigma*s2))
+        return amplitude*real(wofz(z)) / max(tiny, (sigma*s2pi))
+
+    mod = Model(voigt)
+    print(f'independent variables: {mod.independent_vars}')
+
+    params = mod.make_params(amplitude=10, center=5, sigma=2)
+
+    # or
+    params2 = mod.make_params(amplitude=10, center=5, sigma=2, gamma=1.5)
+
+In this case, ``gamma`` will be listed as an independent variable.  But because
+its default value is ``None`` (or ``True`` or ``False``) it can be made a
+Parameter that can be varied independently as shown above.  Of course, whether
+this makes sense depends on the details of the implementation of the model
+function: it can be sensible (and even intended) for ``gamma`` in the ``voigt``
+function above to be a numerical value that could be a variable Parameter, but
+it is not sensible for the ``check_positive`` argument in ``decay2`` to be
+variable that can take any numeric value.
+
+
+
 
 Defining a ``prefix`` for the Parameters
 ----------------------------------------
 
-As we will see in the next chapter when combining models, it is sometimes
-necessary to decorate the parameter names in the model, but still have them
-be correctly used in the underlying model function. This would be
-necessary, for example, if two parameters in a composite model (see
-:ref:`composite_models_section` or examples in the next chapter) would have
-the same name. To avoid this, we can add a ``prefix`` to the
-:class:`Model` which will automatically do this mapping for us.
+As we will see below when combining models, it is sometimes necessary to
+decorate the parameter names in the model, but still have them be correctly
+used in the underlying model function. This would be necessary, for example, if
+two parameters in a composite model (see :ref:`composite_models_section` or
+examples in the next chapter) would have the same name. To avoid this, we can
+add a ``prefix`` to the :class:`Model` which will automatically do this mapping
+for us.
 
 .. jupyter-execute::
 
     def myfunc(x, amplitude=1, center=0, sigma=1):
         # function definition, for now just ``pass``
         pass
 
@@ -543,14 +605,15 @@
     out = mod.fit(y_sim, pars, x=x, a=3.0, b=0.0)
 
 These approaches to initialization provide many opportunities for setting
 initial values for parameters. The methods can be combined, so that you
 can set parameter hints but then change the initial value explicitly with
 :meth:`Model.fit`.
 
+
 .. _model_param_hints_section:
 
 Using parameter hints
 ---------------------
 
 After a model has been created, but prior to creating parameters with
 :meth:`Model.make_params`, you can define parameter hints for that model. This
@@ -600,59 +663,58 @@
     params = mod.make_params(amp={'value': 10, 'min':0.1, 'max':2000},
                              cen=5.5, wid=1.25)
     params.pretty_print()
 
 With that definition, the value (and uncertainty) of the ``fwhm`` parameter
 will be reported in the output of any fit done with that model.
 
+
 .. _model_data_coercion_section:
 
 Data Types for data  and independent data with ``Model``
--------------------------------------------------------------
+--------------------------------------------------------
 
 The model as defined by your model function will use the independent
-variable(s) you specify to best match the data you provide.  The model is meant
+variable(s) you specify to best match the data you provide. The model is meant
 to be an abstract representation for data, but when you do a fit with
 :meth:`Model.fit`, you really need to pass in values for the data to be modeled
 and the independent data used to calculate that data.
 
-
 As discussed in :ref:`fit-data-label`, the mathematical solvers used by
 ``lmfit`` all work exclusively with 1-dimensional numpy arrays of datatype
-(dtype) "float64".  The value of the calculation ``(model-data)*weights`` using
+(dtype) "float64". The value of the calculation ``(model-data)*weights`` using
 the calculation of your model function, and the data and weights you pass in
 **will always be coerced** to an 1-dimensional ndarray with dtype "float64"
-when it is passed to the solver.  If it cannot be coerced, an error will occur
+when it is passed to the solver. If it cannot be coerced, an error will occur
 and the fit will be aborted.
 
 That coercion will usually work for "array like" data that is not already a
 float64 ndarray.  But, depending on the model function, the calculations within
 the model function may not always work well for some "array like" data types
 - especially independent data that are in list of numbers and ndarrays of type
 "float32" or "int16" or less precision.
 
-
 To be clear, independent data for models using ``Model`` are meant to be truly
 independent, and not **not** required to be strictly numerical or objects that
-are easily converted to arrays of numbers.  The could, for example, be a
+are easily converted to arrays of numbers. The could, for example, be a
 dictionary, an instance of a user-defined class, or other type of structured
-data.  You can use independent data any way you want in your model function.
+data. You can use independent data any way you want in your model function.
 But, as with almost all the examples given here, independent data is often also
 a 1-dimensional array of values, say ``x``, and a simple view of the fit would
-be to plot the data as ``y`` as a function of ``x``.  Again, this is not
+be to plot the data as ``y`` as a function of ``x``. Again, this is not
 required, but it is very common, especially for novice users.
 
 By default, all data and independent data passed to :meth:`Model.fit` that is
 "array like" - a list or tuple of numbers, a ``pandas.Series``, and
 ``h5py.Dataset``, or any object that has an ``__array__()`` method -- will be
-converted to a "float64" ndarray before the fit begins.  If the array-like data
+converted to a "float64" ndarray before the fit begins. If the array-like data
 is complex, it will be converted to a "complex128" ndarray, which will always
-work too.  This conversion before the fit begins ensures that the model
+work too. This conversion before the fit begins ensures that the model
 function sees only "float64 ndarrays", and nearly guarantees that data type
-conversion will not cause problems for the fit.  But it also means that if you
+conversion will not cause problems for the fit. But it also means that if you
 have passed a ``pandas.Series`` as data or independent data, not all of the
 methods or attributes of that ``Series`` will be available by default within
 the model function.
 
 .. versionadded:: 1.2.2
 
 This coercion can be turned of with the ``coerce_farray`` option to
@@ -665,15 +727,14 @@
 types of data to use when fitting data.
 
 .. _model_saveload_sec:
 
 Saving and Loading Models
 -------------------------
 
-
 It is sometimes desirable to save a :class:`Model` for later use outside of
 the code used to define the model. Lmfit provides a :func:`save_model`
 function that will save a :class:`Model` to a file. There is also a
 companion :func:`load_model` function that can read this file and
 reconstruct a :class:`Model` from it.
 
 Saving a model turns out to be somewhat challenging. The main issue is that
@@ -716,14 +777,15 @@
 To load that later, one might do:
 
 .. jupyter-execute:: ../examples/doc_model_loadmodel.py
     :hide-output:
 
 See also :ref:`modelresult_saveload_sec`.
 
+
 The :class:`ModelResult` class
 ==============================
 
 A :class:`ModelResult` (which had been called ``ModelFit`` prior to version
 0.9) is the object returned by :meth:`Model.fit`. It is a subclass of
 :class:`~lmfit.minimizer.Minimizer`, and so contains many of the fit results.
 Of course, it knows the :class:`Model` and the set of
@@ -771,15 +833,14 @@
 
 .. automethod:: ModelResult.plot
 
 .. automethod:: ModelResult.plot_fit
 
 .. automethod:: ModelResult.plot_residuals
 
-
 .. method:: ModelResult.iter_cb
 
    Optional callable function, to be called at each fit iteration. This
    must take take arguments of ``(params, iter, resid, *args, **kws)``, where
    ``params`` will have the current parameter values, ``iter`` the
    iteration, ``resid`` the current residual array, and ``*args`` and
    ``**kws`` as passed to the objective function. See :ref:`fit-itercb-label`.
@@ -794,15 +855,15 @@
 
 A :class:`ModelResult` will take all of the attributes of
 :class:`MinimizerResult`, and several more. Here, we arrange them into
 categories.
 
 
 Parameters and Variables
-~~~~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. attribute:: best_values
 
    Dictionary with parameter names as keys, and best-fit values as values.
 
 .. attribute:: init_params
 
@@ -814,54 +875,61 @@
 
 .. attribute:: init_vals
 
    list of values for the variable parameters.
 
 .. attribute::  params
 
-   Parameters used in fit; will contain the best-fit values.
+   Parameters used in fit; will contain the best-fit values and uncertainties
+   if available.
 
 .. attribute:: uvars
 
    Dictionary of ``uncertainties`` ufloats from Parameters.
 
 .. attribute::   var_names
 
    List of variable Parameter names used in optimization in the
    same order as the values in :attr:`init_vals` and :attr:`covar`.
 
+
 Fit Arrays and Model
-~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~
 
 .. attribute:: best_fit
 
    numpy.ndarray result of model function, evaluated at provided
    independent variables and with best-fit parameters.
 
-
 .. attribute:: covar
 
    numpy.ndarray (square) covariance matrix returned from fit.
 
-
 .. attribute:: data
 
    numpy.ndarray of data to compare to model.
 
 .. attribute:: dely
 
-   numpy.ndarray of estimated uncertainties in the ``y`` values of the model
-   from :meth:`ModelResult.eval_uncertainty`  (see :ref:`eval_uncertainty_sec`).
+   numpy.ndarray of estimated uncertainties or *confidence interval* in the
+   ``y`` values of the model from :meth:`ModelResult.eval_uncertainty` (see
+   :ref:`eval_uncertainty_sec`).
 
 .. attribute:: dely_comps
 
    a dictionary of estimated uncertainties in the ``y`` values of the model
    components, from :meth:`ModelResult.eval_uncertainty` (see
    :ref:`eval_uncertainty_sec`).
 
+.. attribute:: dely_predicted
+
+   numpy.ndarray of estimated expected uncertainties in the data or *predicted
+   interval* in the ``y`` values of the model from
+   :meth:`ModelResult.eval_uncertainty` (see :ref:`eval_uncertainty_sec`).
+
 .. attribute:: init_fit
 
    numpy.ndarray result of model function, evaluated at provided
    independent variables and with initial parameters.
 
 .. attribute::  residual
 
@@ -875,17 +943,16 @@
    least-squares sense.
 
 .. attribute:: components
 
    List of components of the :class:`Model`.
 
 
-
 Fit Status
-~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~
 
 .. attribute:: aborted
 
    Whether the fit was aborted.
 
 .. attribute:: errorbars
 
@@ -930,17 +997,16 @@
    positional arguments passed to :meth:`Model.fit`, a tuple of (``y``, ``weights``)
 
 .. attribute:: userkws
 
    keyword arguments passed to :meth:`Model.fit`, a dict, which will have independent data arrays such as ``x``.
 
 
-
 Fit Statistics
-~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~
 
 .. attribute:: aic
 
    Floating point best-fit Akaike Information Criterion statistic
    (see :ref:`fit-results-label`).
 
 .. attribute:: bic
@@ -969,15 +1035,14 @@
 
    Integer number of free parameters in fit.
 
 .. attribute::  nvarys
 
    Integer number of independent, freely varying variables in fit.
 
-
 .. attribute::  redchi
 
    Floating point reduced chi-square statistic (see :ref:`fit-results-label`).
 
 .. attribute:: rsquared
 
    Floating point :math:`R^2` statistic, defined for data :math:`y` and best-fit model :math:`f` as
@@ -991,15 +1056,14 @@
 
 .. attribute:: success
 
    Boolean value of whether fit succeeded. This is an optimistic
    view of success, meaning that the method finished without error.
 
 
-
 .. _eval_uncertainty_sec:
 
 Calculating uncertainties in the model function
 -----------------------------------------------
 
 We return to the first example above and ask not only for the
 uncertainties in the fitted parameters but for the range of values that
@@ -1015,28 +1079,28 @@
     :hide-code:
 
 .. jupyter-execute::
     :hide-output:
 
     dely = result.eval_uncertainty(sigma=3)
     plt.fill_between(x, result.best_fit-dely, result.best_fit+dely, color="#ABABAB",
-                     label='3-$\sigma$ uncertainty band')
+                     label=r'3-$\sigma$ uncertainty band')
 
 to the example fit to the Gaussian at the beginning of this chapter will
 give 3-:math:`\sigma` bands for the best-fit Gaussian, and produce the
 figure below.
 
 .. jupyter-execute::
     :hide-code:
 
     plt.plot(x, y, 'o')
     plt.plot(x, result.init_fit, '--', label='initial fit')
     plt.plot(x, result.best_fit, '-', label='best fit')
     plt.fill_between(x, result.best_fit-dely, result.best_fit+dely, color="#ABABAB",
-                     label='3-$\sigma$ uncertainty band')
+                     label=r'3-$\sigma$ uncertainty band')
     plt.legend()
     plt.show()
 
 
 .. versionadded:: 1.0.4
 
 If the model is a composite built from multiple components, the
@@ -1047,20 +1111,29 @@
 ``result.dely_comps``, with keys that are the component prefixes.
 
 An example script shows how the uncertainties in components of a composite
 model can be calculated and used:
 
 .. jupyter-execute:: ../examples/doc_model_uncertainty2.py
 
+.. versionadded:: 1.2.3
+
+In addition to the "confidence interval" ``result.dely``, the
+:meth:`ModelResult.eval_uncertainty` method will also estimate the "predicted
+interval" -- the expected range for data matching the model, and hold this in
+``result.dely_predicted``. An example script showing both confidence and
+predicted intervals is shown below:
+
+.. jupyter-execute:: ../examples/doc_model_uncertainty_pred.py
 
 
 .. _modelresult_uvars_postfit_section:
 
 Using uncertainties in the fitted parameters for post-fit calculations
---------------------------------------------------------------------------
+----------------------------------------------------------------------
 
 .. versionadded:: 1.2.2
 
 .. _uncertainties package:   https://pythonhosted.org/uncertainties/
 
 As with the previous section, after a fit is complete, you may want to do some
 further calculations with the resulting Parameter values.  Since these
@@ -1131,14 +1204,15 @@
 To load that later, one might do:
 
 .. jupyter-execute:: ../examples/doc_model_loadmodelresult.py
     :hide-output:
 
 .. index:: Composite models
 
+
 .. _composite_models_section:
 
 Composite Models : adding (or multiplying) Models
 =================================================
 
 One of the more interesting features of the :class:`Model` class is that
 Models can be added together or combined with basic algebraic operations
```

### Comparing `lmfit-1.2.2/doc/parameters.rst` & `lmfit-1.3.0/doc/parameters.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/sphinx/theme/sphinx13/basic_layout.html` & `lmfit-1.3.0/doc/sphinx/theme/sphinx13/basic_layout.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 {#
     basic/layout.html
     ~~~~~~~~~~~~~~~~~
 
     Master layout template for Sphinx themes.
 
-    :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS.
+    :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
     :license: BSD, see LICENSE for details.
 #}
-{%- block doctype -%}{%- if html5_doctype %}
+{%- block doctype -%}
 <!DOCTYPE html>
-{%- else %}
-<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
-  "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
-{%- endif %}{%- endblock %}
+{%- endblock %}
 {%- set reldelim1 = reldelim1 is not defined and ' &#187;' or reldelim1 %}
 {%- set reldelim2 = reldelim2 is not defined and ' |' or reldelim2 %}
 {%- set render_sidebar = (not embedded) and (not theme_nosidebar|tobool) and
                          (sidebars != []) %}
 {# URL root should never be #, then all links are fragments #}
 {%- if not embedded and docstitle %}
   {%- set titlesuffix = " &#8212; "|safe + docstitle|e %}
@@ -76,14 +73,15 @@
             {%- include customsidebar %}
             {%- endif %}
             {%- block sidebarsearch %}
             {%- include "searchbox.html" %}
             {%- endblock %}
           {%- endif %}
         </div>
+        {%- block sidebarextra %}{%- endblock %}
       </div>
       {%- endif %}
 {%- endmacro %}
 
 {%- macro script() %}
     {%- for js in script_files %}
     {{ js_tag(js) }}
@@ -99,25 +97,18 @@
       {%- endif %}
     {%- endfor %}
 {%- endmacro %}
 
 {%- if html_tag %}
 {{ html_tag }}
 {%- else %}
-<html{% if not html5_doctype %} xmlns="http://www.w3.org/1999/xhtml"{% endif %}{% if language is not none %} lang="{{ language }}"{% endif %}>
+<html{% if language is not none %} lang="{{ language }}"{% endif %} data-content_root="{{ content_root }}">
 {%- endif %}
   <head>
-    {%- if not html5_doctype and not skip_ua_compatible %}
-    <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
-    {%- endif %}
-    {%- if use_meta_charset or html5_doctype %}
     <meta charset="{{ encoding }}" />
-    {%- else %}
-    <meta http-equiv="Content-Type" content="text/html; charset={{ encoding }}" />
-    {%- endif %}
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     {{- metatags }}
     {%- block htmltitle %}
     <title>{{ title|striptags|e }}{{ titlesuffix }}</title>
     {%- endblock %}
     {%- block css %}
     {{- css() }}
@@ -131,15 +122,15 @@
     {%- endif %}
     {%- if use_opensearch %}
     <link rel="search" type="application/opensearchdescription+xml"
           title="{% trans docstitle=docstitle|e %}Search within {{ docstitle }}{% endtrans %}"
           href="{{ pathto('_static/opensearch.xml', 1) }}"/>
     {%- endif %}
     {%- if favicon_url %}
-    <link rel="shortcut icon" href="{{ favicon_url|e }}"/>
+    <link rel="icon" href="{{ favicon_url|e }}"/>
     {%- endif %}
     {%- endif %}
 {%- block linktags %}
     {%- if hasdoc('about') %}
     <link rel="author" title="{{ _('About these documents') }}" href="{{ pathto('about') }}" />
     {%- endif %}
     {%- if hasdoc('genindex') %}
@@ -187,22 +178,38 @@
   {%- block sidebar2 %}{{ sidebar() }}{% endblock %}
       <div class="clearer"></div>
     </div>
 {%- endblock %}
 
 {%- block relbar2 %}{{ relbar() }}{% endblock %}
 
+{%- macro copyright_block() %}
+  {%- if hasdoc('copyright') %}
+    {%- set copyright_prefix = '<a href="' + pathto('copyright') + '">' + _('Copyright') + '</a>' -%}
+  {%- else %}
+    {%- set copyright_prefix = _('Copyright') %}
+  {%- endif %}
+  {%- if copyright is iterable and copyright is not string %}
+    {% for copyright_line in copyright %}
+      {% trans trimmed copyright_prefix=copyright_prefix, copyright=copyright_line|e %}
+        &#169; {{ copyright_prefix }} {{ copyright }}.
+      {% endtrans %}
+      {%- if not loop.last %}<br/>{%- endif %}
+    {% endfor %}
+  {%- else %}
+    {% trans trimmed copyright_prefix=copyright_prefix, copyright=copyright|e %}
+      &#169; {{ copyright_prefix }} {{ copyright }}.
+    {% endtrans %}
+  {%- endif %}
+{%- endmacro %}
+
 {%- block footer %}
     <div class="footer" role="contentinfo">
     {%- if show_copyright %}
-      {%- if hasdoc('copyright') %}
-        {% trans path=pathto('copyright'), copyright=copyright|e %}&#169; <a href="{{ path }}">Copyright</a> {{ copyright }}.{% endtrans %}
-      {%- else %}
-        {% trans copyright=copyright|e %}&#169; Copyright {{ copyright }}.{% endtrans %}
-      {%- endif %}
+        {{- copyright_block() -}}
     {%- endif %}
     {%- if last_updated %}
       {% trans last_updated=last_updated|e %}Last updated on {{ last_updated }}.{% endtrans %}
     {%- endif %}
     {%- if show_sphinx %}
       {% trans sphinx_version=sphinx_version|e %}Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> {{ sphinx_version }}.{% endtrans %}
     {%- endif %}
```

#### html2text {}

```diff
@@ -1,19 +1,17 @@
 {# basic/layout.html ~~~~~~~~~~~~~~~~~ Master layout template for Sphinx
-themes. :copyright: Copyright 2007-2021 by the Sphinx team, see AUTHORS. :
-license: BSD, see LICENSE for details. #} {%- block doctype -%}{%- if
-html5_doctype %}
-{%- else %}
-{%- endif %}{%- endblock %} {%- set reldelim1 = reldelim1 is not defined and '
-»' or reldelim1 %} {%- set reldelim2 = reldelim2 is not defined and ' |' or
-reldelim2 %} {%- set render_sidebar = (not embedded) and (not
-theme_nosidebar|tobool) and (sidebars != []) %} {# URL root should never be #,
-then all links are fragments #} {%- if not embedded and docstitle %} {%- set
-titlesuffix = " — "|safe + docstitle|e %} {%- else %} {%- set titlesuffix = ""
-%} {%- endif %} {%- macro relbar() %}
+themes. :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS. :
+license: BSD, see LICENSE for details. #} {%- block doctype -%}
+{%- endblock %} {%- set reldelim1 = reldelim1 is not defined and ' »' or
+reldelim1 %} {%- set reldelim2 = reldelim2 is not defined and ' |' or reldelim2
+%} {%- set render_sidebar = (not embedded) and (not theme_nosidebar|tobool) and
+(sidebars != []) %} {# URL root should never be #, then all links are fragments
+#} {%- if not embedded and docstitle %} {%- set titlesuffix = " — "|safe +
+docstitle|e %} {%- else %} {%- set titlesuffix = "" %} {%- endif %} {%- macro
+relbar() %}
 ******** {{{{ __((''NNaavviiggaattiioonn'')) }}}} ********
     * {%- for rellink in rellinks %}
     * % if loop.first %}style="margin-right: 10px"{% endif %}>
     * { accesskey(rellink[2]) }}>{{ rellink[3] }}
  {%- if not loop.first %}{{ reldelim2 }}{% endif %}
 {%- endfor %} {%- block rootrellink %}
 _{_{_ _s_h_o_r_t_t_i_t_l_e_|_e_ _}_}{{ reldelim1 }}
@@ -29,26 +27,23 @@
 {%- include sidebartemplate %} {%- endfor %} {%- else %} {#- old style
 sidebars: using blocks -- should be deprecated #} {%- block sidebartoc %} {%-
 include "localtoc.html" %} {%- endblock %} {%- block sidebarrel %} {%- include
 "relations.html" %} {%- endblock %} {%- block sidebarsourcelink %} {%- include
 "sourcelink.html" %} {%- endblock %} {%- if customsidebar %} {%- include
 customsidebar %} {%- endif %} {%- block sidebarsearch %} {%- include
 "searchbox.html" %} {%- endblock %} {%- endif %}
+{%- block sidebarextra %}{%- endblock %}
 {%- endif %} {%- endmacro %} {%- macro script() %} {%- for js in script_files
 %} {{ js_tag(js) }} {%- endfor %} {%- endmacro %} {%- macro css() %} {%- for
 css in css_files %} {%- if css|attr("filename") %} {{ css_tag(css) }} {%- else
 %}
 {%- endif %} {%- endfor %} {%- endmacro %} {%- if html_tag %} {{ html_tag }}
 {%- else %}
-% if not html5_doctype %} xmlns="http://www.w3.org/1999/xhtml"{% endif %}{% if
-language is not none %} lang="{{ language }}"{% endif %}> {%- endif %}
-{%- if not html5_doctype and not skip_ua_compatible %}
-{%- endif %} {%- if use_meta_charset or html5_doctype %}
-{%- else %}
-{%- endif %}
+% if language is not none %} lang="{{ language }}"{% endif %} data-
+content_root="{{ content_root }}"> {%- endif %}
 {{- metatags }} {%- block htmltitle %}
 {%- endblock %} {%- block css %} {{- css() }} {%- endblock %} {%- if not
 embedded %} {%- block scripts %} {{- script() }} {%- endblock %} {%- if pageurl
 %}
 {%- endif %} {%- if use_opensearch %}
 {%- endif %} {%- if favicon_url %}
 {%- endif %} {%- endif %} {%- block linktags %} {%- if hasdoc('about') %}
@@ -65,17 +60,24 @@
 {%- block document %}
 {%- if render_sidebar %}
 {%- endif %}
 {% block body %} {% endblock %}
 {%- if render_sidebar %}
 {%- endif %}
 {%- endblock %} {%- block sidebar2 %}{{ sidebar() }}{% endblock %}
-{%- endblock %} {%- block relbar2 %}{{ relbar() }}{% endblock %} {%- block
-footer %}
-{%- if show_copyright %} {%- if hasdoc('copyright') %} {% trans path=pathto
-('copyright'), copyright=copyright|e %}© _C_o_p_y_r_i_g_h_t {{ copyright }}.{% endtrans
-%} {%- else %} {% trans copyright=copyright|e %}© Copyright {{ copyright }}.{%
-endtrans %} {%- endif %} {%- endif %} {%- if last_updated %} {% trans
-last_updated=last_updated|e %}Last updated on {{ last_updated }}.{% endtrans %}
-{%- endif %} {%- if show_sphinx %} {% trans sphinx_version=sphinx_version|e
-%}Created using _S_p_h_i_n_x {{ sphinx_version }}.{% endtrans %} {%- endif %}
+{%- endblock %} {%- block relbar2 %}{{ relbar() }}{% endblock %} {%- macro
+copyright_block() %} {%- if hasdoc('copyright') %} {%- set copyright_prefix =
+'_'_ _+_ ___(_'_C_o_p_y_r_i_g_h_t_'_)_ _+_ _'' -%} {%- else %} {%- set copyright_prefix = _
+('Copyright') %} {%- endif %} {%- if copyright is iterable and copyright is not
+string %} {% for copyright_line in copyright %} {% trans trimmed
+copyright_prefix=copyright_prefix, copyright=copyright_line|e %} © {
+{ copyright_prefix }} {{ copyright }}. {% endtrans %} {%- if not loop.last %}
+{%- endif %} {% endfor %} {%- else %} {% trans trimmed
+copyright_prefix=copyright_prefix, copyright=copyright|e %} © {
+{ copyright_prefix }} {{ copyright }}. {% endtrans %} {%- endif %} {%- endmacro
+%} {%- block footer %}
+{%- if show_copyright %} {{- copyright_block() -}} {%- endif %} {%- if
+last_updated %} {% trans last_updated=last_updated|e %}Last updated on {
+{ last_updated }}.{% endtrans %} {%- endif %} {%- if show_sphinx %} {% trans
+sphinx_version=sphinx_version|e %}Created using _S_p_h_i_n_x {{ sphinx_version }}.{%
+endtrans %} {%- endif %}
 {%- endblock %}
```

### Comparing `lmfit-1.2.2/doc/sphinx/theme/sphinx13/layout.html` & `lmfit-1.3.0/doc/sphinx/theme/sphinx13/layout.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/lmfitheader.png` & `lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/lmfitheader.png`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/sphinx/theme/sphinx13/static/sphinx13.css` & `lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/sphinx13.css`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/support.rst` & `lmfit-1.3.0/doc/support.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/doc/whatsnew.rst` & `lmfit-1.3.0/doc/whatsnew.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,79 @@
 .. _lmfit GitHub repository: https://github.com/lmfit/lmfit-py
 
 This section discusses changes between versions, especially changes
 significant to the use and behavior of the library. This is not meant
 to be a comprehensive list of changes. For such a complete record,
 consult the `lmfit GitHub repository`_.
 
+.. _whatsnew_130_label:
+
+Version 1.3.0 Release Notes (April 4, 2024)
+===========================================
+
+New features:
+
+- add ``'min_rel_change'`` as optional variable in calculation of confidence intervals with
+   ``Model.conf_interval()``. (PR #937).
+
+- ``Model.eval_uncertainty`` now takes an optional ``dscale`` parameter (default value of 0.01) to
+   set the step size for calculating derivatives (PR #933).
+
+- add calculation of ``predicted_interval`` to ``Model.eval_uncertainty`` (PR #933).
+
+
+Bug fixes/enhancements:
+
+- restore best-fit parameter values for high accuracy values of constrained values (PR #907)
+
+- improvement to Model for the difference between Parameter, "independent variable", and
+  "option".  With this change, keyword arguments to model functions with non-numerice
+  default values such as ``do_thing=True``, or ``form='linear'`` has those arguments
+  become clearly identified as independent variables,and use the provided values as
+  default values. (PR #941)
+
+- better saving/loading saved states of Model now use dill, have several cleanups, and
+  are now versioned for future-proofing. Also, propagate funcdets for Parameters when
+  loading a Model. (PR #932, PR #934)
+
+- in the TNC method, ``maxfun`` is used instead of ``maxiter``.
+
+- fix bug calculating r-squared for fits with weights (PR #921, PR #923)
+
+- fix bug in ``modelresult.eval_uncertainty()`` after ``load_modelresult()`` (PR #909)
+
+- use StringIO for ``pandas.read_json``.
+
+- add test for MinimizerResult.uvars after successful fit (PR #913)
+
+- adding an example using basinhopping, can take other methods as command-line argument
+
+Maintenance/Deprecations:
+
+- drop support for Python 3.7 that reached EOL on 2023-06-27 (PR #927)
+
+- fix tests for Python 3.12 and Python 3.13-dev
+
+- increase minimum numpy verstio to 1.23 and scipy to 1.8.
+
+- updates for compatibility with numpy 2.0
+
+- the ``dill`` package is now required. (#940)
+
+- build switchded to use pyproject.toml (#928)
+
+- fix broken links in Examples gallery
+
+- fix intersphinx mapping to scipy docs.
+
+
 .. _whatsnew_122_label:
 
 Version 1.2.2 Release Notes (July 14, 2023)
-=================================================
+===========================================
 
 New features:
 
 - add ``ModelResult.uvars`` output to a ``ModelResult`` after a successful fit
   that contains ``ufloats`` from the ``uncertainties`` package which can be
   used for downstream calculations that propagate the uncertainties (and
   correlations) of the variable Parameters. (PR #888)
@@ -52,34 +113,31 @@
 - ``Model.eval`` now returns and array-like value. This adds to the coercion
   features above and fixes a bug for composite models that return lists (Issue #875; PR #901)
 
 - the HTML representation for a ``ModelResult`` or ``MinimizerResult`` are
   improved, and create fewer entries in the Table of Contents for Jupyter lab.
   (Issue #884; PR #883; PR #902)
 
-
-
-
 .. _whatsnew_121_label:
 
 Version 1.2.1 Release Notes (May 02, 2023)
-=================================================
+==========================================
 
 Bug fixes/enhancements:
 
 - fixed bug in ``Model.make_params()`` for initial parameter values that were
   not recognized as floats such as ``np.Int64``.  (Issue #871; PR #872)
 
 - explicitly set ``maxfun`` for ``l-bfgs-b`` method when setting
   ``maxiter``. (Issue #864; Discussion #865; PR #866)
 
 .. _whatsnew_120_label:
 
 Version 1.2.0 Release Notes (April 05, 2023)
-=================================================
+============================================
 
 New features:
 
 - add ``create_params`` function (PR #844)
 - add ``chi2_out`` and ``nsigma`` options to ``conf_interval2d()``
 - add ``ModelResult.summary()`` to return many resulting fit statistics and attributes into a JSON-able dict.
 - add ``correl_table()`` function to ``lmfit.printfuncs`` and ``correl_mode`` option to ``fit_report()`` and
@@ -106,15 +164,15 @@
   ``x`` (JeppeKlitgaard, Issue #840; PR #841)
 - update tests for latest versions of NumPy and SciPy.
 - many fixes of doc typos and updates of dependencies, pre-commit hooks, and CI.
 
 .. _whatsnew_110_label:
 
 Version 1.1.0 Release Notes (November 27, 2022)
-=================================================
+===============================================
 
 New features:
 
 - add ``Pearson4Model`` (@lellid; PR #800)
 - add ``SplineModel`` (PR #804)
 - add R^2 ``rsquared`` statistic to fit outputs and reports for Model fits (Issue #803; PR #810)
 - add calculation of ``dely`` for model components of composite models (Issue #761; PR #826)
```

### Comparing `lmfit-1.2.2/examples/NIST_Gauss2.dat` & `lmfit-1.3.0/examples/NIST_Gauss2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_builtinmodels_nistgauss.py` & `lmfit-1.3.0/examples/doc_builtinmodels_nistgauss.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_builtinmodels_nistgauss2.py` & `lmfit-1.3.0/examples/doc_builtinmodels_nistgauss2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_builtinmodels_peakmodels.py` & `lmfit-1.3.0/examples/doc_builtinmodels_peakmodels.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_builtinmodels_splinemodel.py` & `lmfit-1.3.0/examples/doc_builtinmodels_splinemodel.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_builtinmodels_stepmodel.py` & `lmfit-1.3.0/examples/doc_builtinmodels_stepmodel.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_confidence_advanced.py` & `lmfit-1.3.0/examples/doc_confidence_advanced.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_confidence_chi2_maps.py` & `lmfit-1.3.0/examples/doc_confidence_chi2_maps.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,28 +54,27 @@
 explicitly_calculate_sigma = True
 
 for pairs in (('sigma', 'amplitude'), ('intercept', 'amplitude'),
               ('slope', 'intercept'), ('slope', 'center'), ('sigma', 'center')):
 
     xpar, ypar = pairs
     if explicitly_calculate_sigma:
-        print("Generating chi-square map for ", pairs)
+        print(f"Generating chi-square map for {pairs}")
         c_x, c_y, chi2_mat = conf_interval2d(out, out, xpar, ypar,
                                              nsamples, nsamples, nsigma=3.5,
                                              chi2_out=True)
         # explicitly calculate sigma matrix: sigma increases chi_square
         # from  chi_square_best
         # to    chi_square + sigma**2 * reduced_chi_square
         # so:   sigma = sqrt((chi2-chi2_best)/ reduced_chi_square)
         chi2_min = chi2_mat.min()
         sigma_mat = np.sqrt((chi2_mat-chi2_min)/out.redchi)
     else:
-        print("Generating sigma map for ", pairs)
+        print(f"Generating sigma map for {pairs}")
         # or, you could just calculate the matrix of probabilities as:
-        # print("Generating chi-square map for ", pairs)
         c_x, c_y, sigma_mat = conf_interval2d(out, out, xpar, ypar,
                                               nsamples, nsamples, nsigma=3.5)
 
     aix += 1
     if aix == 2:
         aix = 0
         aiy += 1
```

### Comparing `lmfit-1.2.2/examples/doc_fitting_emcee.py` & `lmfit-1.3.0/examples/doc_fitting_emcee.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_fitting_withreport.py` & `lmfit-1.3.0/examples/doc_fitting_withreport.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_model_composite.py` & `lmfit-1.3.0/examples/doc_model_composite.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_model_gaussian.py` & `lmfit-1.3.0/examples/doc_model_gaussian.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_model_loadmodel.py` & `lmfit-1.3.0/examples/doc_model_loadmodel.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_model_loadmodelresult.py` & `lmfit-1.3.0/examples/doc_model_loadmodelresult.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_model_loadmodelresult2.py` & `lmfit-1.3.0/examples/doc_model_loadmodelresult2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_model_savemodelresult2.py` & `lmfit-1.3.0/examples/doc_model_savemodelresult2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_model_two_components.py` & `lmfit-1.3.0/examples/doc_model_two_components.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_model_uncertainty.py` & `lmfit-1.3.0/examples/doc_model_uncertainty.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_model_uncertainty2.py` & `lmfit-1.3.0/examples/doc_model_uncertainty2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_model_with_iter_callback.py` & `lmfit-1.3.0/examples/doc_model_with_iter_callback.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_model_with_nan_policy.py` & `lmfit-1.3.0/examples/doc_model_with_nan_policy.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_parameters_basic.py` & `lmfit-1.3.0/examples/doc_parameters_basic.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_parameters_valuesdict.py` & `lmfit-1.3.0/examples/doc_parameters_valuesdict.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/doc_uvars_params.py` & `lmfit-1.3.0/examples/doc_uvars_params.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_Model_interface.py` & `lmfit-1.3.0/examples/example_Model_interface.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_brute.py` & `lmfit-1.3.0/examples/example_brute.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_complex_resonator_model.py` & `lmfit-1.3.0/examples/example_complex_resonator_model.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_confidence_interval.py` & `lmfit-1.3.0/examples/example_confidence_interval.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_detect_outliers.py` & `lmfit-1.3.0/examples/example_detect_outliers.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_diffev.py` & `lmfit-1.3.0/examples/example_diffev.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_emcee_Model_interface.py` & `lmfit-1.3.0/examples/example_emcee_Model_interface.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_expression_model.py` & `lmfit-1.3.0/examples/example_expression_model.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_fit_multi_datasets.py` & `lmfit-1.3.0/examples/example_fit_multi_datasets.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_fit_with_algebraic_constraint.py` & `lmfit-1.3.0/examples/example_fit_with_algebraic_constraint.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_fit_with_bounds.py` & `lmfit-1.3.0/examples/example_fit_with_bounds.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_fit_with_derivfunc.py` & `lmfit-1.3.0/examples/example_fit_with_derivfunc.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_fit_with_inequality.py` & `lmfit-1.3.0/examples/example_fit_with_inequality.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_reduce_fcn.py` & `lmfit-1.3.0/examples/example_reduce_fcn.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_sympy.py` & `lmfit-1.3.0/examples/example_sympy.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 gauss_peak1 = sympy_parser.parse_expr('A1*exp(-(x-xc1)**2/(2*sigma1**2))')
 gauss_peak2 = sympy_parser.parse_expr('A2*exp(-(x-xc2)**2/(2*sigma2**2))')
 exp_back = sympy_parser.parse_expr('B*exp(-x/xw)')
 
 model_list = sympy.Array((gauss_peak1, gauss_peak2, exp_back))
 model = sum(model_list)
-print(model)
 
 ###############################################################################
 # We are using SymPy's lambdify function to make a function from the model
 # expressions. We then use these functions to generate some fake data.
 
 model_list_func = sympy.lambdify(list(model_list.free_symbols), model_list)
 model_func = sympy.lambdify(list(model.free_symbols), model)
@@ -46,28 +45,29 @@
 plt.plot(x, yn, 'o')
 plt.plot(x, y)
 for c in yi:
     plt.plot(x, c, color='0.7')
 
 ###############################################################################
 # Next, we will just create a lmfit model from the function and fit the data.
-lm_mod = lmfit.Model(model_func, independent_vars=('x'))
+lm_mod = lmfit.Model(model_func, independent_vars=('x',))
 res = lm_mod.fit(data=yn, **param_values)
 
 ###############################################################################
 res.plot_fit()
 plt.plot(x, y, label='true')
 plt.legend()
 
 ###############################################################################
 # The nice thing of using SymPy is that we can easily modify our fit function.
 # Let's assume we know that the width of both Gaussians are identical. Similarly,
 # we assume that the ratio between both Gaussians is fixed to 3:2 for some
 # reason. Both can be expressed by just substituting the variables.
 model2 = model.subs('sigma2', 'sigma1').subs('A2', '3/2*A1')
 model2_func = sympy.lambdify(list(model2.free_symbols), model2)
-lm_mod = lmfit.Model(model2_func, independent_vars=('x'))
+lm_mod = lmfit.Model(model2_func, independent_vars=('x',))
 param2_values = dict(x=x, A1=2, sigma1=1, xc1=2, xc2=5, xw=4, B=5)
 res2 = lm_mod.fit(data=yn, **param2_values)
 res2.plot_fit()
 plt.plot(x, y, label='true')
 plt.legend()
+plt.show()
```

### Comparing `lmfit-1.2.2/examples/example_two_dimensional_peak.py` & `lmfit-1.3.0/examples/example_two_dimensional_peak.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/example_use_pandas.py` & `lmfit-1.3.0/examples/example_use_pandas.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/lmfit_emcee_model_selection.py` & `lmfit-1.3.0/examples/lmfit_emcee_model_selection.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/model1d_gauss.dat` & `lmfit-1.3.0/examples/model1d_gauss.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/peak.csv` & `lmfit-1.3.0/examples/peak.csv`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/sinedata.dat` & `lmfit-1.3.0/examples/sinedata.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/test_peak.dat` & `lmfit-1.3.0/examples/test_peak.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/examples/test_splinepeak.dat` & `lmfit-1.3.0/examples/test_splinepeak.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/lmfit/__init__.py` & `lmfit-1.3.0/lmfit/__init__.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/lmfit/_ampgo.py` & `lmfit-1.3.0/lmfit/_ampgo.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/lmfit/conf_emcee.py` & `lmfit-1.3.0/lmfit/conf_emcee.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,15 @@
     bounds = np.array(bounds)
 
     self.nvarys = len(result.var_names)
 
     # set up multiprocessing options for the samplers
     auto_pool = None
     sampler_kwargs = {}
-    if isinstance(workers, int) and workers > 1 and HAS_DILL:
+    if isinstance(workers, int) and workers > 1:
         auto_pool = multiprocessing.Pool(workers)
         sampler_kwargs['pool'] = auto_pool
     elif hasattr(workers, 'map'):
         sampler_kwargs['pool'] = workers
 
     # function arguments for the log-probability functions
     # these values are sent to the log-probability functions by the sampler.
```

### Comparing `lmfit-1.2.2/lmfit/confidence.py` & `lmfit-1.3.0/lmfit/confidence.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,16 @@
 def restore_vals(tmp_params, params):
     """Restore values/stderrs of parameters from a temporary dictionary."""
     for para_key in params:
         params[para_key].value, params[para_key].stderr = tmp_params[para_key]
 
 
 def conf_interval(minimizer, result, p_names=None, sigmas=None, trace=False,
-                  maxiter=200, verbose=False, prob_func=None):
+                  maxiter=200, verbose=False, prob_func=None,
+                  min_rel_change=1e-5):
     """Calculate the confidence interval (CI) for parameters.
 
     The parameter for which the CI is calculated will be varied, while the
     remaining parameters are re-optimized to minimize the chi-square. The
     resulting chi-square is used to calculate the probability with a given
     statistic (e.g., F-test). This function uses a 1d-rootfinder from SciPy
     to find the values resulting in the searched confidence region.
@@ -83,14 +84,16 @@
         Maximum of iteration to find an upper limit (default is 200).
     verbose : bool, optional
         Print extra debugging information (default is False).
     prob_func : None or callable, optional
         Function to calculate the probability from the optimized chi-square.
         Default is None and uses the built-in function `f_compare`
         (i.e., F-test).
+    min_rel_change : float, optional
+        Minimum relative change in probability (default is 1e-5).
 
     Returns
     -------
     output : dict
         A dictionary containing a list of ``(sigma, vals)``-tuples for
         each parameter.
     trace_dict : dict, optional
@@ -135,15 +138,15 @@
     parameters.
 
     """
     if sigmas is None:
         sigmas = [1, 2, 3]
 
     ci = ConfidenceInterval(minimizer, result, p_names, prob_func, sigmas,
-                            trace, verbose, maxiter)
+                            trace, verbose, maxiter, min_rel_change)
     output = ci.calc_all_ci()
     if trace:
         return output, ci.trace_dict
     return output
 
 
 def map_trace_to_names(trace, params):
@@ -159,15 +162,51 @@
     return out
 
 
 class ConfidenceInterval:
     """Class used to calculate the confidence interval."""
 
     def __init__(self, minimizer, result, p_names=None, prob_func=None,
-                 sigmas=None, trace=False, verbose=False, maxiter=50):
+                 sigmas=None, trace=False, verbose=False, maxiter=50,
+                 min_rel_change=1e-5):
+        """Initialize the ConfidenceInterval class.
+
+        Parameters
+        ----------
+        minimizer : Minimizer
+            The minimizer to use, holding objective function.
+        result : MinimizerResult
+            The result of running minimize().
+        p_names : list, optional
+            Names of the parameters for which the CI is calculated. If None
+            (default), the CI is calculated for every parameter.
+        prob_func : None or callable, optional
+            Function to calculate the probability from the optimized chi-square.
+            Default is None and uses the built-in function `f_compare`
+            (i.e., F-test).
+        sigmas : list, optional
+            The sigma-levels to find (default is [1, 2, 3]).
+        trace : bool, optional
+            Defaults to False; if True, each result of a probability
+            calculation is saved along with the parameter. This can be used to
+            plot so-called "profile traces".
+        verbose : bool, optional
+            Print extra debugging information (default is False).
+        maxiter : int, optional
+            Maximum of iteration to find an upper limit (default is 50).
+        min_rel_change : float, optional
+            Minimum relative change in probability (default is 1e-5).
+
+        Raises
+        ------
+        MinimizerException
+            If there are less than two variables or if the stderrs are not
+            sensible.
+
+        """
         self.verbose = verbose
         self.minimizer = minimizer
         self.result = result
         self.params = result.params.copy()
         self.org = copy_vals(self.params)
         self.best_chi = result.chisqr
 
@@ -192,15 +231,15 @@
         else:
             self.prob_func = prob_func
         if trace:
             self.trace_dict = {i: [] for i in self.p_names}
 
         self.trace = trace
         self.maxiter = maxiter
-        self.min_rel_change = 1e-5
+        self.min_rel_change = min_rel_change
 
         if sigmas is None:
             sigmas = [1, 2, 3]
         self.sigmas = list(sigmas)
         self.sigmas.sort()
         self.probs = []
         for sigma in self.sigmas:
```

### Comparing `lmfit-1.2.2/lmfit/jsonutils.py` & `lmfit-1.3.0/lmfit/jsonutils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """JSON utilities."""
 
 from base64 import b64decode, b64encode
+from io import StringIO
 import sys
 import warnings
 
+import dill
 import numpy as np
 import uncertainties
 
-try:
-    import dill
-    HAS_DILL = True
-except ImportError:
-    HAS_DILL = False
+HAS_DILL = True
 
 try:
     from pandas import DataFrame, Series, read_json
 except ImportError:
     DataFrame = Series = type(NotImplemented)
     read_json = None
 
@@ -88,27 +86,29 @@
         return dict(__class__=ctype, value=val)
     if isinstance(obj, dict):
         out = dict(__class__='Dict')
         for key, val in obj.items():
             out[encode4js(key)] = encode4js(val)
         return out
     if callable(obj):
-        value = str(b64encode(dill.dumps(obj)), 'utf-8') if HAS_DILL else None
+        value = str(b64encode(dill.dumps(obj)), 'utf-8')
         return dict(__class__='Callable', __name__=obj.__name__,
                     pyversion=pyvers, value=value,
                     importer=find_importer(obj))
     return obj
 
 
 def decode4js(obj):
     """Return decoded Python object from encoded object."""
     if not isinstance(obj, dict):
         return obj
     out = obj
     classname = obj.pop('__class__', None)
+    if classname is None and isinstance(obj, dict):
+        classname = 'dict'
     if classname is None:
         return obj
     if classname == 'Complex':
         out = obj['value'][0] + 1j*obj['value'][1]
     elif classname in ('List', 'Tuple'):
         out = []
         for item in obj['value']:
@@ -123,32 +123,36 @@
         elif obj['__dtype__'].startswith('object'):
             val = [decode4js(v) for v in obj['value']]
             out = np.array(val, dtype=obj['__dtype__'])
         else:
             out = np.fromiter(obj['value'], dtype=obj['__dtype__'])
         out.shape = obj['__shape__']
     elif classname == 'PDataFrame' and read_json is not None:
-        out = read_json(obj['value'])
+        out = read_json(StringIO(obj['value']))
     elif classname == 'PSeries' and read_json is not None:
-        out = read_json(obj['value'], typ='series')
+        out = read_json(StringIO(obj['value']), typ='series')
     elif classname == 'UFloat':
         out = uncertainties.ufloat(obj['val'], obj['err'])
     elif classname == 'Callable':
         out = obj['__name__']
         try:
             out = import_from(obj['importer'], out)
             unpacked = True
         except (ImportError, AttributeError):
             unpacked = False
-        if not unpacked and HAS_DILL:
+        if not unpacked:
+            spyvers = obj.get('pyversion', '?')
+            if not pyvers == spyvers:
+                msg = f"Could not unpack dill-encoded callable '{out}', saved with Python version {spyvers}"
+                warnings.warn(msg)
+
             try:
                 out = dill.loads(b64decode(obj['value']))
             except RuntimeError:
-                msg = "Could not unpack dill-encoded callable `{0}`, saved with Python version {1}"
-                warnings.warn(msg.format(obj['__name__'],
-                                         obj['pyversion']))
+                msg = f"Could not unpack dill-encoded callable '{out}`, saved with Python version {spyvers}"
+                warnings.warn(msg)
 
     elif classname in ('Dict', 'dict'):
         out = {}
         for key, val in obj.items():
             out[key] = decode4js(val)
     return out
```

### Comparing `lmfit-1.2.2/lmfit/lineshapes.py` & `lmfit-1.3.0/lmfit/lineshapes.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/lmfit/minimizer.py` & `lmfit-1.3.0/lmfit/minimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,22 +61,14 @@
 # check for numdifftools
 try:
     import numdifftools as ndt
     HAS_NUMDIFFTOOLS = True
 except ImportError:
     HAS_NUMDIFFTOOLS = False
 
-# check for dill
-try:
-    import dill  # noqa: F401
-    HAS_DILL = True
-except ImportError:
-    HAS_DILL = False
-
-
 # define the namedtuple here so pickle will work with the MinimizerResult
 Candidate = namedtuple('Candidate', ['params', 'score'])
 
 maxeval_warning = "ignoring `{}` argument to `{}()`. Use `max_nfev` instead."
 
 
 def thisfuncname():
@@ -901,21 +893,27 @@
         params = result.params
 
         self.set_max_nfev(max_nfev, 2000*(result.nvarys+1))
 
         fmin_kws = dict(method=method, options={'maxiter': 2*self.max_nfev})
         if method == 'L-BFGS-B':
             fmin_kws['options']['maxfun'] = 2*self.max_nfev
+
         elif method == 'COBYLA':
             # for this method, we explicitly let the solver reach
-            # the users max nfev, and do not abort in _residual.
+            # the users max nfev, and do not abort in _residual
             fmin_kws['options']['maxiter'] = self.max_nfev
             self.max_nfev = 5*self.max_nfev
 
-        # fmin_kws = dict(method=method, options={'maxfun': 2*self.max_nfev})
+        # FIXME: update when SciPy requirement is >= 1.8
+        # ``maxiter`` deprecated in favor of ``maxfun``
+        elif method == "TNC" and int(scipy_version.split('.')[1]) >= 11:
+            fmin_kws['options']['maxfun'] = 2*self.max_nfev
+            fmin_kws['options'].pop('maxiter')
+
         fmin_kws.update(self.kws)
 
         if 'maxiter' in kws:
             warnings.warn(maxeval_warning.format('maxiter', thisfuncname()),
                           RuntimeWarning)
             kws.pop('maxiter')
         fmin_kws.update(kws)
@@ -1338,15 +1336,15 @@
         bounds = np.array(bounds)
 
         self.nvarys = len(result.var_names)
 
         # set up multiprocessing options for the samplers
         auto_pool = None
         sampler_kwargs = {}
-        if isinstance(workers, int) and workers > 1 and HAS_DILL:
+        if isinstance(workers, int) and workers > 1:
             auto_pool = multiprocessing.Pool(workers)
             sampler_kwargs['pool'] = auto_pool
         elif hasattr(workers, 'map'):
             sampler_kwargs['pool'] = workers
 
         # function arguments for the log-probability functions
         # these values are sent to the log-probability functions by the sampler.
@@ -1381,15 +1379,15 @@
                                                  self._lnprob, **sampler_kwargs)
 
         # user supplies an initialisation position for the chain
         # If you try to run the sampler with p0 of a wrong size then you'll get
         # a ValueError. Note, you can't initialise with a position if you are
         # reusing the sampler.
         if pos is not None and not reuse_sampler:
-            tpos = np.asfarray(pos)
+            tpos = np.asarray(pos, dtype=np.float64)
             if p0.shape == tpos.shape:
                 pass
             # trying to initialise with a previous chain
             elif tpos.shape[-1] == self.nvarys:
                 tpos = tpos[-1]
             else:
                 raise ValueError('pos should have shape (nwalkers, nvarys)')
@@ -1731,20 +1729,16 @@
         """
         result = self.prepare_fit(params=params)
         result.method = 'basinhopping'
         self.set_max_nfev(max_nfev, 200000*(result.nvarys+1))
         basinhopping_kws = dict(niter=100, T=1.0, stepsize=0.5,
                                 minimizer_kwargs=None, take_step=None,
                                 accept_test=None, callback=None, interval=50,
-                                disp=False, niter_success=None, seed=None)
-
-        # FIXME: update when SciPy requirement is >= 1.8
-        if int(scipy_version.split('.')[1]) >= 8:
-            basinhopping_kws.update({'target_accept_rate': 0.5,
-                                     'stepwise_factor': 0.9})
+                                disp=False, niter_success=None, seed=None,
+                                target_accept_rate=0.5, stepwise_factor=0.9)
 
         basinhopping_kws.update(self.kws)
         basinhopping_kws.update(kws)
 
         x0 = result._init_vals_internal
         result.call_kws = basinhopping_kws
         try:
@@ -2114,22 +2108,18 @@
 
         """
         result = self.prepare_fit(params=params)
         result.method = 'shgo'
 
         self.set_max_nfev(max_nfev, 200000*(result.nvarys+1))
 
-        shgo_kws = dict(constraints=None, n=100, iters=1, callback=None,
+        shgo_kws = dict(constraints=None, n=None, iters=1, callback=None,
                         minimizer_kwargs=None, options=None,
                         sampling_method='simplicial')
 
-        # FIXME: update when SciPy requirement is >= 1.7
-        if int(scipy_version.split('.')[1]) >= 7:
-            shgo_kws['n'] = None
-
         shgo_kws.update(self.kws)
         shgo_kws.update(kws)
 
         varying = np.asarray([par.vary for par in self.params.values()])
         bounds = np.asarray([(par.min, par.max) for par in
                              self.params.values()])[varying]
         result.call_kws = shgo_kws
@@ -2192,27 +2182,22 @@
         .. versionadded:: 0.9.14
 
         """
         result = self.prepare_fit(params=params)
         result.method = 'dual_annealing'
         self.set_max_nfev(max_nfev, 200000*(result.nvarys+1))
 
-        da_kws = dict(maxiter=1000, local_search_options={},
-                      initial_temp=5230.0, restart_temp_ratio=2e-05,
-                      visit=2.62, accept=-5.0, maxfun=2*self.max_nfev,
-                      seed=None, no_local_search=False, callback=None, x0=None)
+        da_kws = dict(maxiter=1000, minimizer_kwargs=None, initial_temp=5230.0,
+                      restart_temp_ratio=2e-05, visit=2.62, accept=-5.0,
+                      maxfun=2*self.max_nfev, seed=None, no_local_search=False,
+                      callback=None, x0=None)
 
         da_kws.update(self.kws)
         da_kws.update(kws)
 
-        # FIXME: update when SciPy requirement is >= 1.8
-        # ``local_search_options`` deprecated in favor of ``minimizer_kwargs``
-        if int(scipy_version.split('.')[1]) >= 8:
-            da_kws.update({'minimizer_kwargs': da_kws.pop('local_search_options')})
-
         varying = np.asarray([par.vary for par in self.params.values()])
         bounds = np.asarray([(par.min, par.max) for par in
                              self.params.values()])[varying]
 
         if not np.all(np.isfinite(bounds)):
             raise ValueError('dual_annealing requires finite bounds for all'
                              ' varying parameters')
@@ -2259,15 +2244,15 @@
             - `'least_squares'`: Least-Squares minimization, using Trust
               Region Reflective method
             - `'differential_evolution'`: differential evolution
             - `'brute'`: brute force method
             - `'basinhopping'`: basinhopping
             - `'ampgo'`: Adaptive Memory Programming for Global
               Optimization
-            - '`nelder`': Nelder-Mead
+            - `'nelder'`: Nelder-Mead
             - `'lbfgsb'`: L-BFGS-B
             - `'powell'`: Powell
             - `'cg'`: Conjugate-Gradient
             - `'newton'`: Newton-CG
             - `'cobyla'`: Cobyla
             - `'bfgs'`: BFGS
             - `'tnc'`: Truncated Newton
@@ -2391,24 +2376,24 @@
     -------
     array
         ndarray of type np.float64, possibly after applying the `nan_policy`,
         and usually raveling to 1-D array
 
     Notes
     -----
-    Parts of this function are based on scipy/stats/stats.py/_contains_nan
+    Parts of this fudtype=np.float64nction are based on scipy/stats/stats.py/_contains_nan
 
-    support for 'array-like` objects is from numpy `asfarray`, which includes
+    support for 'array-like` objects is from numpy `asarray`, which includes
     lists of numbers, pandas.Series, h5py.Datasets, and many other array-like
     Python objects
     """
     if np.iscomplexobj(arr):
-        arr = np.asfarray(arr, dtype=np.complex128).view(np.float64)
+        arr = np.asarray(arr, dtype=np.complex128).view(np.float64)
     else:
-        arr = np.asfarray(arr, dtype=np.float64)
+        arr = np.asarray(arr, dtype=np.float64)
 
     if ravel:
         arr = arr.ravel(order=ravel_order)
 
     if nan_policy not in ('propagate', 'omit', 'raise'):
         raise ValueError("nan_policy must be 'propagate', 'omit', or 'raise'.")
```

### Comparing `lmfit-1.2.2/lmfit/model.py` & `lmfit-1.3.0/lmfit/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from scipy.special import erf
 from scipy.stats import t
 
 import lmfit
 
 from . import Minimizer, Parameter, Parameters, lineshapes
 from .confidence import conf_interval
-from .jsonutils import HAS_DILL, decode4js, encode4js
+from .jsonutils import decode4js, encode4js
 from .minimizer import MinimizerResult
 from .printfuncs import ci_report, fit_report, fitreport_html_table
 
 tiny = 1.e-15
 
 # Use pandas.isnull for aligning missing data if pandas is available.
 # otherwise use numpy.isnan
@@ -141,15 +141,15 @@
     value of `z` the magnitude uncertainty is approximated by
     ``numpy.abs(dz)`` for that value.
 
     """
     if option not in ['real', 'imag', 'abs', 'angle']:
         raise ValueError(f"Invalid option ('{option}') for function 'propagate_err'.")
 
-    if z.shape != dz.shape:
+    if isinstance(dz, np.ndarray) and z.shape != dz.shape:
         raise ValueError(f"shape of z: {z.shape} != shape of dz: {dz.shape}")
 
     # Check the main vector for complex. Do nothing if real.
     if any(np.iscomplex(z)):
         # if uncertainties are real, apply them equally to
         # real and imaginary parts
         if all(np.isreal(dz)):
@@ -194,17 +194,17 @@
     """
     coerce lists, tuples, and pandas Series, hdf5 Groups, etc to an
     ndarray float64 or complex128, but leave other data structures
     and objects unchanged
     """
     if isinstance(x, (list, tuple, Series)) or hasattr(x, '__array__'):
         if np.isrealobj(x):
-            return np.asfarray(x)
+            return np.asarray(x, dtype=np.float64)
         if np.iscomplexobj(x):
-            return np.asfarray(x, dtype=np.complex128)
+            return np.asarray(x, dtype=np.complex128)
     return x
 
 
 class Model:
     """Create a model from a user-supplied model function."""
 
     _forbidden_args = ('data', 'weights', 'params')
@@ -240,21 +240,26 @@
             Name for the model. When None (default) the name is the same
             as the model function (`func`).
         **kws : dict, optional
             Additional keyword arguments to pass to model function.
 
         Notes
         -----
-        1. Parameter names are inferred from the function arguments, and a
-        residual function is automatically constructed.
-
-        2. The model function must return an array that will be the same
+        1. The model function must return an array that will be the same
         size as the data being modeled.
 
-        3. `nan_policy` sets what to do when a NaN or missing value is
+        2. Parameter names are inferred from the function arguments by default,
+        and a residual function is automatically constructed.
+
+        3. Specifying `independent_vars` here will explicitly name the
+        independent variables for the Model.  in contrast, `param_names` is
+        meant to help infer Parameter names for keyword arguments defined with
+        ``**kws`` in the Model function.
+
+        4. `nan_policy` sets what to do when a NaN or missing value is
         seen in the data. Should be one of:
 
            - `'raise'` : raise a `ValueError` (default)
            - `'propagate'` : do nothing
            - `'omit'` : drop missing data
 
         Examples
@@ -290,14 +295,15 @@
         self.independent_vars = independent_vars
         self._func_allargs = []
         self._func_haskeywords = False
         self.nan_policy = nan_policy
 
         self.opts = kws
         # the following has been changed from OrderedSet for the time being
+        self.independent_vars_defvals = {}
         self.param_hints = {}
         self._param_names = []
         self._parse_params()
         if self.independent_vars is None:
             self.independent_vars = []
         if name is None and hasattr(self.func, '__name__'):
             name = self.func.__name__
@@ -315,25 +321,44 @@
             out = f"{out}, {', '.join(opts)}"
         return f"Model({out})"
 
     def _get_state(self):
         """Save a Model for serialization.
 
         Note: like the standard-ish '__getstate__' method but not really
-        useful with Pickle.
+        useful with Pickle, and only useful with dill.
 
+        This, and the companion function _buildmodel to use this serialized model
+        now supports versions of 'state'.
+
+        State Version History:
+          original: up to and including version 1.2.2:
+             state is a tuple of length 9:
+                (self.func.__name__, funcdef, self._name, self._prefix,
+                self.independent_vars, self._param_root_names,
+                self.param_hints, self.nan_policy, self.opts)
+             with opts used in the version 1.2 sense
+          version 1.2.3 and beyond:
+             state is a dict with a 'version' keyword and all other
+             values from the original state in key/value pairs.
+             The initial value for 'version' is '2'.
         """
-        funcdef = None
-        if HAS_DILL:
-            funcdef = self.func
+        funcdef = self.func
         if self.func.__name__ == '_eval':
             funcdef = self.expr
-        state = (self.func.__name__, funcdef, self._name, self._prefix,
-                 self.independent_vars, self._param_root_names,
-                 self.param_hints, self.nan_policy, self.opts)
+        state = dict(version='2',
+                     funcname=self.func.__name__,
+                     funcdef=funcdef,
+                     name=self._name,
+                     prefix=self._prefix,
+                     independent_vars=self.independent_vars,
+                     param_root_names=self._param_root_names,
+                     param_hints=self.param_hints,
+                     nan_policy=self.nan_policy,
+                     opts=self.opts)
         return (state, None, None)
 
     def _set_state(self, state, funcdefs=None):
         """Restore Model from serialization.
 
         Note: like the standard-ish '__setstate__' method but not really
         useful with Pickle.
@@ -492,48 +517,70 @@
         if hasattr(self.func, 'argnames') and hasattr(self.func, 'kwargs'):
             pos_args = self.func.argnames[:]
             for name, defval in self.func.kwargs:
                 kw_args[name] = defval
         # 2. modern, best-practice approach: use inspect.signature
         else:
             pos_args = []
+            default_vals = {}
+            indep_vars = []
             sig = inspect.signature(self.func)
             for fnam, fpar in sig.parameters.items():
                 if fpar.kind == fpar.VAR_KEYWORD:
                     keywords_ = fnam
-                elif fpar.kind == fpar.POSITIONAL_OR_KEYWORD:
-                    if fpar.default == fpar.empty:
+                elif fpar.kind in (fpar.POSITIONAL_ONLY, fpar.POSITIONAL_OR_KEYWORD):
+                    default_vals[fnam] = fpar.default
+                    if (isinstance(fpar.default, (float, int, complex))
+                       and not isinstance(fpar.default, bool)):
+                        kw_args[fnam] = fpar.default
+                    elif fpar.default == fpar.empty:
                         pos_args.append(fnam)
                     else:
                         kw_args[fnam] = fpar.default
+                        indep_vars.append(fnam)
                 elif fpar.kind == fpar.VAR_POSITIONAL:
                     raise ValueError(f"varargs '*{fnam}' is not supported")
         # inspection done
 
         self._func_haskeywords = keywords_ is not None
-        self._func_allargs = pos_args + list(kw_args.keys())
-        allargs = self._func_allargs
+        self._func_allargs = list(default_vals.keys())
+        for key in kw_args:
+            if key not in self._func_allargs:
+                self._func_allargs.append(key)
 
-        if len(allargs) == 0 and keywords_ is not None:
+        if len(self._func_allargs) == 0 and keywords_ is not None:
             return
 
+        self.independent_vars_defvals = {}
         # default independent_var = 1st argument
         if self.independent_vars is None:
-            self.independent_vars = [pos_args[0]]
+            self.independent_vars = [pos_args.pop(0)]
+            # default values for independent variables
+            for vnam in indep_vars:
+                dval = default_vals[vnam]
+                if vnam in self.opts:
+                    dval = self.opts[vnam]
+                self.independent_vars_defvals[vnam] = dval
+                if vnam not in self.independent_vars:
+                    self.independent_vars.append(vnam)
 
         # default param names: all positional args
         # except independent variables
         self.def_vals = {}
         might_be_param = []
         if self._param_root_names is None:
-            self._param_root_names = pos_args[:]
+            self._param_root_names = []
+            for pname in pos_args:
+                if pname not in self.independent_vars:
+                    self._param_root_names.append(pname)
             for key, val in kw_args.items():
                 if (not isinstance(val, bool) and
                         isinstance(val, (float, int))):
-                    self._param_root_names.append(key)
+                    if key not in self._param_root_names:
+                        self._param_root_names.append(key)
                     self.def_vals[key] = val
                 elif val is None:
                     might_be_param.append(key)
             for p in self.independent_vars:
                 if p in self._param_root_names:
                     self._param_root_names.remove(p)
 
@@ -546,22 +593,23 @@
             elif opt in self._func_allargs:
                 new_opts[opt] = val
         self.opts = new_opts
 
         if self._prefix is None:
             self._prefix = ''
         names = [f"{self._prefix}{pname}" for pname in self._param_root_names]
+
         # check variables names for validity
         # The implicit magic in fit() requires us to disallow some
         fname = self.func.__name__
         for arg in self.independent_vars:
-            if arg not in allargs or arg in self._forbidden_args:
+            if arg not in self._func_allargs or arg in self._forbidden_args:
                 raise ValueError(self._invalid_ivar % (arg, fname))
         for arg in names:
-            if (self._strip_prefix(arg) not in allargs or
+            if (self._strip_prefix(arg) not in self._func_allargs or
                     arg in self._forbidden_args):
                 raise ValueError(self._invalid_par % (arg, fname))
         # the following as been changed from OrderedSet for the time being.
         self._param_names = names[:]
 
     def set_param_hint(self, name, **kwargs):
         """Set *hints* to use when creating parameters with `make_params()`.
@@ -678,14 +726,16 @@
         """
         params = Parameters()
 
         def setpar(par, val):
             # val is expected to be float-like or a dict: must have 'value' or 'expr' key
             if isinstance(val, dict):
                 dval = val
+            elif np.iscomplex(val) or isinstance(val, complex):
+                dval = {'value': val.real}
             else:
                 dval = {'value': float(val)}
             if len(dval) < 1 or not ('value' in dval or 'expr' in dval):
                 raise TypeError(f'Invalid parameter value for {par}: {val}')
 
             par.set(**dval)
 
@@ -737,14 +787,28 @@
                     setattr(par, item, hint[item])
             if basename in kwargs:
                 setpar(par, kwargs[basename])
             # Add the new parameter to self._param_names
             if name not in self._param_names:
                 self._param_names.append(name)
 
+        # check for parameters that were initially flagged as independent
+        # variables because the function signature used "key=None", "key=True",
+        # or "key=False": these could actually be variables
+        for key, val in kwargs.items():
+            if key in params:
+                continue
+            if key in self.independent_vars:
+                dxval = self.independent_vars_defvals.get(key, inspect._empty)
+                if dxval is None or isinstance(dxval, bool):
+                    name = f"{self._prefix}{key}"
+                    par = Parameter(name=name)
+                    setpar(par, val)
+                    params.add(par)
+
         for p in params.values():
             p._delay_asteval = False
         return params
 
     def guess(self, data, x, **kws):
         """Guess starting values for the parameters of a Model.
 
@@ -809,19 +873,19 @@
                    'aborted! Please check your model function and/or set '
                    'boundaries on parameters where applicable. In cases like '
                    'this, using "nan_policy=\'omit\'" will probably not work.')
             raise ValueError(msg)
 
         diff = model - data
 
-        if diff.dtype == complex:
+        if diff.dtype is complex:
             # data/model are complex
             diff = diff.ravel().view(float)
             if weights is not None:
-                if weights.dtype == complex:
+                if weights.dtype is complex:
                     # weights are complex
                     weights = weights.ravel().view(float)
                 else:
                     # real weights but complex data
                     weights = (weights + 1j * weights).ravel().view(float)
         if weights is not None:
             diff *= weights
@@ -836,16 +900,17 @@
     def make_funcargs(self, params=None, kwargs=None, strip=True):
         """Convert parameter values and keywords to function arguments."""
         if params is None:
             params = {}
         if kwargs is None:
             kwargs = {}
         out = {}
-        out.update(self.opts)
-
+        for key, val in self.independent_vars_defvals.items():
+            if val is not inspect._empty:
+                out[key] = val
         # 0: if a keyword argument is going to overwrite a parameter,
         #    save that value so it can be restored before returning
         saved_values = {}
         for name, val in kwargs.items():
             if name in params:
                 saved_values[name] = params[name].value
                 params[name].value = val
@@ -866,18 +931,20 @@
             for fullname in self._param_names:
                 if fullname in params:
                     name = self._strip_prefix(fullname)
                     if name in self._func_allargs or self._func_haskeywords:
                         out[name] = params[fullname].value
 
         # 3. kwargs might directly update function arguments
+        validnames = [ivar for ivar in self.independent_vars]
+        validnames.extend(self._func_allargs)
         for name, val in kwargs.items():
             if strip:
                 name = self._strip_prefix(name)
-            if name in self._func_allargs or self._func_haskeywords:
+            if name in validnames or self._func_haskeywords:
                 out[name] = val
 
         # 4. finally, reset any values that have overwritten parameter values
         for name, val in saved_values.items():
             params[name].value = val
         return out
 
@@ -1079,23 +1146,27 @@
                 data = data[mask]
             if weights is not None:
                 weights = _align(weights, mask, data)
 
         # If independent_vars and data are alignable (pandas), align them,
         # and apply the mask from above if there is one.
         for var in self.independent_vars:
-            if not np.isscalar(kwargs[var]):
-                kwargs[var] = _align(kwargs[var], mask, data)
+            if var not in params:
+                if var not in kwargs:
+                    raise ValueError(f"'Missing independent variable '{var}'")
+                if not np.isscalar(kwargs[var]):
+                    kwargs[var] = _align(kwargs[var], mask, data)
 
         if coerce_farray:
             # coerce data and independent variable(s) that are 'array-like' (list,
             # tuples, pandas Series) to float64/complex128.
             data = coerce_arraylike(data)
             for var in self.independent_vars:
-                kwargs[var] = coerce_arraylike(kwargs[var])
+                if var not in params and var in kwargs:
+                    kwargs[var] = coerce_arraylike(kwargs[var])
 
         if fit_kws is None:
             fit_kws = {}
 
         output = ModelResult(self, params, method=method, iter_cb=iter_cb,
                              scale_covar=scale_covar, fcn_kws=kwargs,
                              nan_policy=self.nan_policy, calc_covar=calc_covar,
@@ -1293,36 +1364,58 @@
     if len(state) != 3:
         raise ValueError("Cannot restore Model")
     known_funcs = {}
     for fname in lineshapes.functions:
         fcn = getattr(lineshapes, fname, None)
         if callable(fcn):
             known_funcs[fname] = fcn
-    if funcdefs is not None:
+    if funcdefs is None:
+        funcdefs = {}
+    else:
         known_funcs.update(funcdefs)
 
     left, right, op = state
     if op is None and right is None:
-        (fname, fcndef, name, prefix, ivars, pnames,
-         phints, nan_policy, opts) = left
-        if not callable(fcndef) and fname in known_funcs:
-            fcndef = known_funcs[fname]
+        if isinstance(left, tuple) and len(left) == 9:
+            (fname, func, name, prefix, ivars, pnames,
+             phints, nan_policy, opts) = left
+        elif isinstance(left, dict) and 'version' in left:
+            # for future-proofing, we could add "if left['version'] == '2':"
+            # here to cover cases when 'version' changes
+            fname = left.get('funcname', None)
+            func = left.get('funcdef', None)
+            name = left.get('name', None)
+            prefix = left.get('prefix', None)
+            ivars = left.get('indepedendent_vars', None)
+            pnames = left.get('param_root_names', None)
+            phints = left.get('param_hints', None)
+            nan_policy = left.get('nan_policy', None)
+            opts = left.get('opts', None)
+        else:
+            raise ValueError("Cannot restore Model: unrecognized state data")
+
+        # if the function definition was passed in, use that!
+        if fname in funcdefs and fname != '_eval':
+            func = funcdefs[fname]
 
-        if fcndef is None:
+        if not callable(func) and fname in known_funcs:
+            func = known_funcs[fname]
+
+        if func is None:
             raise ValueError("Cannot restore Model: model function not found")
 
-        if fname == '_eval' and isinstance(fcndef, str):
+        if fname == '_eval' and isinstance(func, str):
             from .models import ExpressionModel
-            model = ExpressionModel(fcndef, name=name,
+            model = ExpressionModel(func, name=name,
                                     independent_vars=ivars,
                                     param_names=pnames,
                                     nan_policy=nan_policy, **opts)
 
         else:
-            model = Model(fcndef, name=name, prefix=prefix,
+            model = Model(func, name=name, prefix=prefix,
                           independent_vars=ivars, param_names=pnames,
                           nan_policy=nan_policy, **opts)
 
         for name, hint in phints.items():
             model.set_param_hint(name, **hint)
         return model
     else:
@@ -1471,23 +1564,24 @@
         for attr in dir(_ret):
             if not attr.startswith('_'):
                 try:
                     setattr(self, attr, getattr(_ret, attr))
                 except AttributeError:
                     pass
 
-        if self.data is not None and len(self.data) > 1:
-            dat = coerce_arraylike(self.data)
-            sstot = ((dat - dat.mean())**2).sum()
-            if isinstance(self.residual, np.ndarray) and len(self.residual) > 1:
-                self.rsquared = 1.0 - (self.residual**2).sum()/max(tiny, sstot)
-
         self.init_values = self.model._make_all_args(self.init_params)
         self.best_values = self.model._make_all_args(_ret.params)
         self.best_fit = self.model.eval(params=_ret.params, **self.userkws)
+        if (self.data is not None and len(self.data) > 1
+           and isinstance(self.best_fit, np.ndarray)
+           and len(self.best_fit) > 1):
+            dat = coerce_arraylike(self.data)
+            resid = ((dat - self.best_fit)**2).sum()
+            sstot = ((dat - dat.mean())**2).sum()
+            self.rsquared = 1.0 - resid/max(tiny, sstot)
 
     def eval(self, params=None, **kwargs):
         """Evaluate model function.
 
         Parameters
         ----------
         params : Parameters, optional
@@ -1526,26 +1620,28 @@
         """
         userkws = self.userkws.copy()
         userkws.update(kwargs)
         if params is None:
             params = self.params
         return self.model.eval_components(params=params, **userkws)
 
-    def eval_uncertainty(self, params=None, sigma=1, **kwargs):
+    def eval_uncertainty(self, params=None, sigma=1, dscale=0.01, **kwargs):
         """Evaluate the uncertainty of the *model function*.
 
         This can be used to give confidence bands for the model from the
         uncertainties in the best-fit parameters.
 
         Parameters
         ----------
         params : Parameters, optional
             Parameters, defaults to ModelResult.params.
         sigma : float, optional
             Confidence level, i.e. how many sigma (default is 1).
+        dscale : float, optional
+            Scale for derivative steps (default is 0.01).
         **kwargs : optional
             Values of options, independent variables, etcetera.
 
         Returns
         -------
         numpy.ndarray
             Uncertainty at each value of the model.
@@ -1558,18 +1654,22 @@
            J. Wolberg, Data Analysis Using the Method of Least Squares, 2006, Springer
         2. The value of sigma is number of `sigma` values, and is converted
            to a probability. Values of 1, 2, or 3 give probabilities of
            0.6827, 0.9545, and 0.9973, respectively. If the sigma value is
            < 1, it is interpreted as the probability itself. That is,
            ``sigma=1`` and ``sigma=0.6827`` will give the same results,
            within precision errors.
-        3. Also sets attributes of `dely` for the uncertainty of the model
+        3. The derivatives are calculated by stepping each Parameter from its best value to
+           to +/- stderr*dscale, where `dscale` can be passed in and defaults to 0.01.
+        4. Sets attributes of `dely` for the uncertainty of the model
            (which will be the same as the array returned by this method) and
            `dely_comps`, a dictionary of `dely` for each component.
-
+        5. Sets the attribute of `dely_predicted` for the 'predicted interval', the sigma-scaled
+           quadrature sum of the uncertainty interval `dely` and reduced chi-square. This should
+           give an idea of the expected range in the data.
 
         Examples
         --------
 
         >>> out = model.fit(data, params, x=x)
         >>> dely = out.eval_uncertainty(x=x)
         >>> plt.plot(x, data)
@@ -1591,25 +1691,26 @@
         if any(p.stderr is None for p in params.values()):
             return np.zeros(ndata)
 
         # '0' would be an invalid prefix, here signifying 'Full'
         fjac = {'0': np.zeros((nvarys, ndata), dtype='float64')}
         df2 = {'0': np.zeros(ndata, dtype='float64')}
 
-        for comp in self.components:
+        for comp in self.model.components:
             label = comp.prefix if len(comp.prefix) > 1 else comp._name
             fjac[label] = np.zeros((nvarys, ndata), dtype='float64')
             df2[label] = np.zeros(ndata, dtype='float64')
 
         # find derivative by hand!
         pars = params.copy()
         for i in range(nvarys):
             pname = self.var_names[i]
-            val0 = pars[pname].value
-            dval = pars[pname].stderr/3.0
+            val0 = params[pname].value
+            dval = params[pname].stderr*dscale
+
             pars[pname].value = val0 + dval
             res1 = {'0': self.model.eval(pars, **userkws)}
             res1.update(self.model.eval_components(params=pars, **userkws))
 
             pars[pname].value = val0 - dval
             res2 = {'0': self.model.eval(pars, **userkws)}
             res2.update(self.model.eval_components(params=pars, **userkws))
@@ -1632,15 +1733,17 @@
         scale = t.ppf((prob+1)/2.0, self.ndata-nvarys)
 
         # for complex data, convert back to real/imag pairs
         if feval.dtype in ('complex64', 'complex128'):
             for key in fjac:
                 df2[key] = df2[key][0::2] + 1j * df2[key][1::2]
 
-        self.dely = scale * np.sqrt(df2.pop('0'))
+        df2_total = df2.pop('0')
+        self.dely = scale * np.sqrt(df2_total)
+        self.dely_predicted = scale * np.sqrt(df2_total + self.redchi)
 
         self.dely_comps = {}
         for key in df2:
             self.dely_comps[key] = scale * np.sqrt(df2[key])
         return self.dely
 
     def conf_interval(self, **kwargs):
@@ -1794,35 +1897,33 @@
             JSON string representation of ModelResult.
 
         See Also
         --------
         loads, json.dumps
 
         """
-        out = {'__class__': 'lmfit.ModelResult', '__version__': '1',
+        out = {'__class__': 'lmfit.ModelResult', '__version__': '2',
                'model': encode4js(self.model._get_state())}
-        pasteval = self.params._asteval
-        out['params'] = [p.__getstate__() for p in self.params.values()]
-        out['unique_symbols'] = {key: encode4js(pasteval.symtable[key])
-                                 for key in pasteval.user_defined_symbols()}
+
+        for attr in ('params', 'init_params'):
+            out[attr] = getattr(self, attr).dumps()
 
         for attr in ('aborted', 'aic', 'best_values', 'bic', 'chisqr',
                      'ci_out', 'col_deriv', 'covar', 'errorbars', 'flatchain',
                      'ier', 'init_values', 'lmdif_message', 'message',
                      'method', 'nan_policy', 'ndata', 'nfev', 'nfree',
                      'nvarys', 'redchi', 'residual', 'rsquared', 'scale_covar',
                      'calc_covar', 'success', 'userargs', 'userkws', 'values',
                      'var_names', 'weights', 'user_options'):
             try:
                 val = getattr(self, attr)
             except AttributeError:
                 continue
             if isinstance(val, np.bool_):
                 val = bool(val)
-
             out[attr] = encode4js(val)
 
         val = out.get('message', '')
         if isinstance(val, bytes):
             out['message'] = str(val, encoding='ASCII')
 
         return json.dumps(out, **kws)
@@ -1856,15 +1957,15 @@
         Parameters
         ----------
         s : str
             String representation of ModelResult, as from `dumps`.
         funcdefs : dict, optional
             Dictionary of custom function names and definitions.
         **kws : optional
-            Keyword arguments that are passed to `json.dumps`.
+            Keyword arguments that are passed to `json.loads`.
 
         Returns
         -------
         ModelResult
             ModelResult instance from JSON string representation.
 
         See Also
@@ -1879,24 +1980,39 @@
         modres = decode4js(modres)
         if 'model' not in modres or 'params' not in modres:
             raise AttributeError('ModelResult.loads() needs valid ModelResult')
 
         # model
         self.model = _buildmodel(decode4js(modres['model']), funcdefs=funcdefs)
 
-        # params
-        for target in ('params', 'init_params'):
-            state = {'unique_symbols': modres['unique_symbols'], 'params': []}
-            for parstate in modres['params']:
-                _par = Parameter(name='')
-                _par.__setstate__(parstate)
-                state['params'].append(_par)
-            _params = Parameters()
-            _params.__setstate__(state)
-            setattr(self, target, _params)
+        if funcdefs:
+            # Remove model function so as not pass it into the _asteval.symtable
+            funcdefs.pop(self.model.func.__name__, None)
+
+        # how params are saved was changed with version 2:
+        modres_vers = modres.get('__version__', '1')
+        if modres_vers == '1':
+            for target in ('params', 'init_params'):
+                state = {'unique_symbols': modres['unique_symbols'], 'params': []}
+                for parstate in modres['params']:
+                    _par = Parameter(name='')
+                    _par.__setstate__(parstate)
+                    state['params'].append(_par)
+                _params = Parameters(usersyms=funcdefs)
+                _params.__setstate__(state)
+                setattr(self, target, _params)
+
+        elif modres_vers == '2':
+            for target in ('params', 'init_params'):
+                _pars = Parameters()
+                _pars.loads(modres[target])
+                if funcdefs:
+                    for key, val in funcdefs.items():
+                        _pars._asteval.symtable[key] = val
+                setattr(self, target, _pars)
 
         for attr in ('aborted', 'aic', 'best_fit', 'best_values', 'bic',
                      'chisqr', 'ci_out', 'col_deriv', 'covar', 'data',
                      'errorbars', 'fjac', 'flatchain', 'ier', 'init_fit',
                      'init_values', 'kws', 'lmdif_message', 'message',
                      'method', 'nan_policy', 'ndata', 'nfev', 'nfree',
                      'nvarys', 'redchi', 'residual', 'rsquared', 'scale_covar',
@@ -1910,14 +2026,15 @@
             self.weights = self.userargs[1]
 
         for parname, val in self.init_values.items():
             par = self.init_params.get(parname, None)
             if par is not None:
                 par.correl = par.stderr = None
                 par.value = par.init_value = self.init_values[parname]
+
         self.init_fit = self.model.eval(self.init_params, **self.userkws)
         self.result = MinimizerResult()
         self.result.params = self.params
 
         if self.errorbars and self.covar is not None:
             self.uvars = self.result.params.create_uvars(covar=self.covar)
 
@@ -2065,15 +2182,14 @@
 
             ax.plot(
                 x_array_dense, reduce_complex(y_eval_init), initfmt,
                 label='initial fit', **init_kws)
 
         if yerr is None and self.weights is not None:
             yerr = 1.0/self.weights
-
         if yerr is not None:
             ax.errorbar(x_array, reduce_complex(self.data),
                         yerr=propagate_err(self.data, yerr, parse_complex),
                         fmt=datafmt, label='data', **data_kws)
         else:
             ax.plot(x_array, reduce_complex(self.data),
                     datafmt, label='data', **data_kws)
```

### Comparing `lmfit-1.2.2/lmfit/models.py` & `lmfit-1.3.0/lmfit/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Module containing built-in fitting models."""
-
-import time
+import inspect
 
 from asteval import Interpreter, get_ast_names
 import numpy as np
 from scipy.interpolate import splev, splrep
 
 from . import lineshapes
 from .lineshapes import (breit_wigner, damped_oscillator, dho, doniach,
@@ -1669,14 +1668,18 @@
            seen in the data. Should be one of:
 
             - `'raise'` : raise a `ValueError` (default)
             - `'propagate'` : do nothing
             - `'omit'` : drop missing data
 
         """
+        if 'prefix' in kws:
+            raise Warning(self.no_prefix)
+        kws["nan_policy"] = nan_policy
+
         # create ast evaluator, load custom functions
         self.asteval = Interpreter()
         for name in lineshapes.functions:
             self.asteval.symtable[name] = getattr(lineshapes, name, None)
         if init_script is not None:
             self.asteval.eval(init_script)
 
@@ -1707,46 +1710,48 @@
             lost = []
             for ix, found in enumerate(idvar_found):
                 if not found:
                     lost.append(independent_vars[ix])
             lost = ', '.join(lost)
             raise ValueError(self.idvar_notfound.format(lost, self.expr))
 
-        kws['independent_vars'] = independent_vars
-        if 'prefix' in kws:
-            raise Warning(self.no_prefix)
+        kws['independent_vars'] = self.independent_vars = independent_vars
 
         def _eval(**kwargs):
             for name, val in kwargs.items():
                 self.asteval.symtable[name] = val
-            self.asteval.start_time = time.time()
             return self.asteval.run(self.astcode)
 
         kws["nan_policy"] = nan_policy
 
         super().__init__(_eval, **kws)
 
         # set param names here, and other things normally
         # set in _parse_params(), which will be short-circuited.
-        self.independent_vars = independent_vars
         self._func_allargs = independent_vars + param_names
         self._param_names = param_names
         self._func_haskeywords = True
+        self.independent_var_defvals = {'x': inspect._empty}
         self.def_vals = {}
 
     def __repr__(self):
         """Return printable representation of ExpressionModel."""
         return f"<lmfit.ExpressionModel('{self.expr}')>"
 
+    def _reprstring(self, long=False):
+        """Return printable representation of ExpressionModel."""
+        return f"<lmfit.ExpressionModel('{self.expr}')>"
+
     def _parse_params(self):
         """Over-write ExpressionModel._parse_params with `pass`.
 
         This prevents normal parsing of function for parameter names.
 
         """
+        pass
 
 
 lmfit_models = {'Constant': ConstantModel,
                 'Complex Constant': ComplexConstantModel,
                 'Linear': LinearModel,
                 'Quadratic': QuadraticModel,
                 'Polynomial': PolynomialModel,
```

### Comparing `lmfit-1.2.2/lmfit/parameter.py` & `lmfit-1.3.0/lmfit/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,14 +505,15 @@
             will take the correlations into account when combining values.
         2.  See the uncertainties package documentation
             (https://pythonhosted.org/uncertainties) for more details.
         """
         uvars = {}
         has_expr = False
         vnames, vbest, vindex = [], [], -1
+        savevals = self.valuesdict()
         for par in self.values():
             has_expr = has_expr or par.expr is not None
             if par.vary:
                 vindex += 1
                 vnames.append(par.name)
                 vbest.append(par.value)
                 if getattr(par, 'sdterr', None) is None and covar is not None:
@@ -538,14 +539,17 @@
                     try:
                         uval = wrap_ueval(*corr_uvars, obj=par,
                                           pars=self, names=vnames)
                         par.stderr = uval.std_dev
                         uvars[par.name] = uval
                     except Exception:
                         par.stderr = 0
+        # restore all param values to saved best values
+        for parname, param in self.items():
+            param.value = savevals[parname]
         return uvars
 
     def dumps(self, **kws):
         """Represent Parameters as a JSON string.
 
         Parameters
         ----------
```

### Comparing `lmfit-1.2.2/lmfit/printfuncs.py` & `lmfit-1.3.0/lmfit/printfuncs.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/lmfit.egg-info/SOURCES.txt` & `lmfit-1.3.0/lmfit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .pre-commit-config.yaml
 AUTHORS.txt
 LICENSE
 README.rst
 azure-pipelines.yml
 publish_docs.sh
 pyproject.toml
-setup.cfg
 setup.py
 .github/CONTRIBUTING.md
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/dependabot.yml
 NIST_STRD/Bennett5.dat
 NIST_STRD/BoxBOD.dat
@@ -78,14 +77,15 @@
 doc/sphinx/theme/sphinx13/static/headerbg.png
 doc/sphinx/theme/sphinx13/static/listitem.png
 doc/sphinx/theme/sphinx13/static/lmfitheader.png
 doc/sphinx/theme/sphinx13/static/relbg.png
 doc/sphinx/theme/sphinx13/static/sphinx13.css
 examples/NIST_Gauss2.dat
 examples/README.txt
+examples/discuss_model_eval_uncertainty.ipynb
 examples/doc_builtinmodels_nistgauss.py
 examples/doc_builtinmodels_nistgauss2.py
 examples/doc_builtinmodels_peakmodels.py
 examples/doc_builtinmodels_splinemodel.py
 examples/doc_builtinmodels_stepmodel.py
 examples/doc_confidence_advanced.py
 examples/doc_confidence_basic.py
@@ -99,20 +99,22 @@
 examples/doc_model_loadmodelresult2.py
 examples/doc_model_savemodel.py
 examples/doc_model_savemodelresult.py
 examples/doc_model_savemodelresult2.py
 examples/doc_model_two_components.py
 examples/doc_model_uncertainty.py
 examples/doc_model_uncertainty2.py
+examples/doc_model_uncertainty_pred.py
 examples/doc_model_with_iter_callback.py
 examples/doc_model_with_nan_policy.py
 examples/doc_parameters_basic.py
 examples/doc_parameters_valuesdict.py
 examples/doc_uvars_params.py
 examples/example_Model_interface.py
+examples/example_basinhopping.py
 examples/example_brute.py
 examples/example_complex_resonator_model.py
 examples/example_confidence_interval.py
 examples/example_detect_outliers.py
 examples/example_diffev.py
 examples/example_emcee_Model_interface.py
 examples/example_expression_model.py
@@ -182,8 +184,11 @@
 tests/test_nose.py
 tests/test_pandas.py
 tests/test_parameter.py
 tests/test_parameters.py
 tests/test_params_uvars.py
 tests/test_printfuncs.py
 tests/test_shgo.py
-tests/test_stepmodel.py
+tests/test_stepmodel.py
+tests/saved_models/sinemodel_py310_lm122.sav
+tests/saved_models/sinemodel_py311_lm122.sav
+tests/saved_models/sinemodel_py312_lm122.sav
```

### Comparing `lmfit-1.2.2/publish_docs.sh` & `lmfit-1.3.0/publish_docs.sh`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/NISTModels.py` & `lmfit-1.3.0/tests/NISTModels.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/conftest.py` & `lmfit-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/gauss_modelresult_lmfit100.sav` & `lmfit-1.3.0/tests/gauss_modelresult_lmfit100.sav`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_1variable.py` & `lmfit-1.3.0/tests/test_1variable.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_NIST_Strd.py` & `lmfit-1.3.0/tests/test_NIST_Strd.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_algebraic_constraint.py` & `lmfit-1.3.0/tests/test_algebraic_constraint.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_ampgo.py` & `lmfit-1.3.0/tests/test_ampgo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Tests for the AMPGO global minimization algorithm."""
 
 import numpy as np
 from numpy.testing import assert_allclose
 import pytest
-from scipy import __version__ as scipy_version
 
 import lmfit
 from lmfit._ampgo import ampgo, tunnel
 
 # correct result for Alpine02 function
 global_optimum = [7.91705268, 4.81584232]
 fglob = -6.12950
@@ -56,23 +55,15 @@
     assert out.ampgo_msg == 'Maximum number of function evaluations exceeded'
 
 
 def test_ampgo_local_solver(minimizer_Alpine02):
     """Test AMPGO algorithm with local solver."""
     kws = {'local': 'Nelder-Mead'}
 
-    # bounds in Nelder-Mead are supported since SciPy v1.7.0
-    # FIXME: clean this up after we require SciPy >= 1.7.0
-    if int(scipy_version.split('.')[1]) < 7:
-        msg = r'Method Nelder-Mead cannot handle constraints nor bounds'
-        with pytest.warns(RuntimeWarning, match=msg):
-            out = minimizer_Alpine02.minimize(method='ampgo', **kws)
-    else:
-        out = minimizer_Alpine02.minimize(method='ampgo', **kws)
-
+    out = minimizer_Alpine02.minimize(method='ampgo', **kws)
     out_x = np.array([out.params['x0'].value, out.params['x1'].value])
 
     assert 'ampgo' and 'Nelder-Mead' in out.method
     assert_allclose(out.residual, fglob, rtol=1e-5)
     assert_allclose(min(out_x), min(global_optimum), rtol=1e-3)
     assert_allclose(max(out_x), max(global_optimum), rtol=1e-3)
     assert 'global' in out.ampgo_msg
```

### Comparing `lmfit-1.2.2/tests/test_basicfit.py` & `lmfit-1.3.0/tests/test_basicfit.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_basinhopping.py` & `lmfit-1.3.0/tests/test_basinhopping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Tests for the basinhopping minimization algorithm."""
 import numpy as np
 from numpy.testing import assert_allclose
 import pytest
-from scipy import __version__ as scipy_version
 from scipy.optimize import basinhopping
 
 import lmfit
 
 
 def test_basinhopping_lmfit_vs_scipy():
     """Test basinhopping in lmfit versus scipy."""
@@ -58,19 +57,14 @@
     kws = {'minimizer_kwargs': {'method': 'L-BFGS-B'}, 'seed': 7}
     out = mini.minimize(method='basinhopping', **kws)
 
     assert_allclose(out.residual, ret.fun)
     assert_allclose(out.params['x0'].value, ret.x[0], rtol=1e-5)
     assert_allclose(out.params['x1'].value, ret.x[1], rtol=1e-5)
 
-    # FIXME: update when SciPy requirement is >= 1.8
-    if int(scipy_version.split('.')[1]) >= 8:
-        assert 'target_accept_rate' in out.call_kws
-        assert 'stepwise_factor' in out.call_kws
-
 
 def test_basinhopping_Alpine02(minimizer_Alpine02):
     """Test basinhopping on Alpine02 function."""
     global_optimum = [7.91705268, 4.81584232]
     fglob = -6.12950
 
     kws = {'minimizer_kwargs': {'method': 'L-BFGS-B'}, 'seed': 7}
```

### Comparing `lmfit-1.2.2/tests/test_bounded_jacobian.py` & `lmfit-1.3.0/tests/test_bounded_jacobian.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_bounds.py` & `lmfit-1.3.0/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_brute.py` & `lmfit-1.3.0/tests/test_brute.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_builtin_models.py` & `lmfit-1.3.0/tests/test_builtin_models.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_confidence.py` & `lmfit-1.3.0/tests/test_confidence.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_covariance_matrix.py` & `lmfit-1.3.0/tests/test_covariance_matrix.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_custom_independentvar.py` & `lmfit-1.3.0/tests/test_custom_independentvar.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_default_kws.py` & `lmfit-1.3.0/tests/test_default_kws.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_dual_annealing.py` & `lmfit-1.3.0/tests/test_dual_annealing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Tests for the Dual Annealing algorithm."""
 
 import numpy as np
 from numpy.testing import assert_allclose
 import scipy
-from scipy import __version__ as scipy_version
 
 import lmfit
 
 
 def eggholder(x):
     return (-(x[1] + 47.0) * np.sin(np.sqrt(abs(x[0]/2.0 + (x[1] + 47.0))))
             - x[0] * np.sin(np.sqrt(abs(x[0] - (x[1] + 47.0)))))
@@ -50,21 +49,14 @@
     out_x = np.array([out.params['x0'].value, out.params['x1'].value])
 
     assert_allclose(out.residual, fglob, rtol=1e-5)
     assert_allclose(min(out_x), min(global_optimum), rtol=1e-3)
     assert_allclose(max(out_x), max(global_optimum), rtol=1e-3)
     assert out.method == 'dual_annealing'
 
-    # FIXME: update when SciPy requirement is >= 1.8
-    # ``local_search_options`` deprecated in favor of ``minimizer_kwargs``
-    if int(scipy_version.split('.')[1]) >= 8:
-        assert 'minimizer_kwargs' in out.call_kws
-    else:
-        assert 'local_search_options' in out.call_kws
-
 
 def test_da_bounds(minimizer_Alpine02):
     """Test dual_annealing algorithm with bounds."""
     pars_bounds = lmfit.Parameters()
     pars_bounds.add_many(('x0', 1., True, 5.0, 15.0),
                          ('x1', 1., True, 2.5, 7.5))
```

### Comparing `lmfit-1.2.2/tests/test_itercb.py` & `lmfit-1.3.0/tests/test_itercb.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_jsonutils.py` & `lmfit-1.3.0/tests/test_jsonutils.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_least_squares.py` & `lmfit-1.3.0/tests/test_least_squares.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_lineshapes.py` & `lmfit-1.3.0/tests/test_lineshapes.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_manypeaks_speed.py` & `lmfit-1.3.0/tests/test_manypeaks_speed.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_max_nfev.py` & `lmfit-1.3.0/tests/test_max_nfev.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_minimizer.py` & `lmfit-1.3.0/tests/test_minimizer.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_model.py` & `lmfit-1.3.0/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 from numpy.testing import assert_allclose, assert_almost_equal
 import pytest
 from scipy import __version__ as scipy_version
 
 import lmfit
 from lmfit import Model, Parameters, models
-from lmfit.lineshapes import gaussian, lorentzian
+from lmfit.lineshapes import gaussian, lorentzian, step, voigt
 from lmfit.model import get_reducer, propagate_err
 from lmfit.models import GaussianModel, PseudoVoigtModel
 
 
 @pytest.fixture()
 def gmodel():
     """Return a Gaussian model."""
@@ -198,19 +198,30 @@
 
 def test_Model_get_state(gmodel):
     """Test for Model class function _get_state."""
     out = gmodel._get_state()
 
     assert isinstance(out, tuple)
     assert out[1] == out[2] is None
-    assert (out[0][1] is not None) == lmfit.jsonutils.HAS_DILL
-
-    assert out[0][0] == 'gaussian'
-    assert out[0][2:] == ('gaussian', '', ['x'],
-                          ['amplitude', 'center', 'sigma'], {}, 'raise', {})
+    sstate = out[0]
+    if isinstance(sstate, tuple):  # state version 1
+        assert sstate[1] is not None
+        assert sstate[0] == 'gaussian'
+        assert sstate[2:] == ('gaussian', '', ['x'],
+                              ['amplitude', 'center', 'sigma'], {}, 'raise', {})
+    elif isinstance(sstate, dict) and 'version' in sstate:  # state version 2 or higher
+        if sstate['version'] == '2':
+            assert sstate['funcname'] == 'gaussian'
+            assert sstate['name'] == 'gaussian'
+            assert sstate['independent_vars'] == ['x']
+            assert sstate['param_root_names'] == ['amplitude', 'center', 'sigma']
+        else:
+            assert sstate['version'] == 'unknown version!'
+    else:
+        assert sstate == 'unknown model state'
 
 
 def test_Model_set_state(gmodel):
     """Test for Model class function _set_state.
 
     This function is just calling `_buildmodel`, which will be tested
     below together with the use of `funcdefs`.
@@ -860,15 +871,40 @@
             flexible_model.fit(self.data, pars, x=self.x, extra=5)
         self.assertTrue(len(w) == 1)
         self.assertTrue(issubclass(w[-1].category, UserWarning))
 
     def test_missing_independent_variable_raises_error(self):
         pars = self.model.make_params(**self.guess())
         f = lambda: self.model.fit(self.data, pars)
-        self.assertRaises(KeyError, f)
+        self.assertRaises(ValueError, f)
+
+    def test_independent_var_parsing(self):
+        """test the parsing of independent variables for model functions
+        with keyword arguments
+
+        step:  form='linear'
+        voigt: gamma=None,     can become a variable!!
+        """
+        stepmod = Model(step)
+        assert 'x' in stepmod.independent_vars
+        assert 'form' in stepmod.independent_vars
+        assert 'linear' == stepmod.independent_vars_defvals.get('form', None)
+
+        voigtmod = Model(voigt)
+        assert 'x' in voigtmod.independent_vars
+        assert 'gamma' in voigtmod.independent_vars
+        assert voigtmod.independent_vars_defvals['gamma'] is None
+
+        pars1 = voigtmod.make_params(amplitude=25, center=9.5, sigma=1)
+        assert 'sigma' in pars1
+        assert 'gamma' not in pars1
+
+        pars2 = voigtmod.make_params(amplitude=25, center=9.5, sigma=1, gamma=0.5)
+        assert 'sigma' in pars2
+        assert 'gamma' in pars2
 
     def test_bounding(self):
         true_values = self.true_values()
         true_values['center'] = 1.3  # as close as it's allowed to get
         pars = self.model.make_params(**self.guess())
         pars['center'].set(value=2, min=1.3)
         result = self.model.fit(self.data, pars, x=self.x)
@@ -1075,14 +1111,18 @@
             assert len(repr(par)) > 5
 
     @pytest.mark.skipif(not lmfit.model._HAS_MATPLOTLIB,
                         reason="requires matplotlib.pyplot")
     def test_composite_plotting(self):
         # test that a composite model has non-empty best_values
         import matplotlib
+        try:
+            matplotlib.pyplot.close('all')
+        except ValueError:
+            pass
         matplotlib.use('Agg')
 
         model1 = models.GaussianModel(prefix='g1_')
         model2 = models.GaussianModel(prefix='g2_')
 
         mod = model1 + model2
         pars = mod.make_params()
@@ -1531,7 +1571,24 @@
     Model2 = Model(lin2, independent_vars=["x"], prefix="m2_")
     ModelSum = Model1 + Model2
     pars = Parameters()
     pars.add('m1_k', value=0.5)
     pars.add('m2_k', value=0.5)
     result = ModelSum.fit(y, pars, x=x)
     assert len(result.best_fit) == len(x)
+
+
+def test_rsquared_with_weights():
+    """Github #921"""
+    def func(x, k=1, b=0):
+        return k*x+b
+
+    x = np.array([1, 2, 3, 4])
+    y = np.array([1.1, 1.9, 3.05, 3.95])
+    yerr = np.array([0.03, 0.04, 0.01, 0.02])
+
+    mod = Model(func)
+    params = mod.make_params()
+    result = mod.fit(y, params, x=x, weights=1.0/yerr)
+
+    assert result.rsquared < 1.00
+    assert result.rsquared > 0.95
```

### Comparing `lmfit-1.2.2/tests/test_model_saveload.py` & `lmfit-1.3.0/tests/test_model_saveload.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import time
 
 import numpy as np
 from numpy.testing import assert_allclose
 import pytest
 
 from lmfit import Parameters
-import lmfit.jsonutils
 from lmfit.lineshapes import gaussian, lorentzian
 from lmfit.model import (Model, ModelResult, load_model, load_modelresult,
                          save_model, save_modelresult)
 from lmfit.models import (ExponentialModel, ExpressionModel, GaussianModel,
                           VoigtModel)
 
 y, x = np.loadtxt(os.path.join(os.path.dirname(__file__), '..',
@@ -85,22 +84,16 @@
     assert_allclose(pars['g2_sigma'], 13.806948, rtol=1.0e-5)
     assert_allclose(pars['g2_center'], 153.270101, rtol=1.0e-5)
     assert_allclose(pars['g2_amplitude'], 2493.417703, rtol=1.0e-5)
     assert_allclose(pars['g2_fwhm'], 32.512878, rtol=1.0e-5)
     assert_allclose(pars['g2_height'], 72.045593, rtol=1.0e-5)
 
 
-@pytest.mark.parametrize("dill", [False, True])
-def test_save_load_model(dill):
-    """Save/load Model with/without dill."""
-    if dill:
-        pytest.importorskip("dill")
-    else:
-        lmfit.jsonutils.HAS_DILL = False
-
+def test_save_load_model():
+    """Save/load Model, now always asserting that dill is available."""
     # create/save Model and perform some tests
     model, _pars = create_model_params(x, y)
     save_model(model, SAVE_MODEL)
 
     file_exists = wait_for_file(SAVE_MODEL, timeout=10)
     assert file_exists
 
@@ -124,34 +117,28 @@
 
     result = saved_model.fit(y, params, x=x)
     check_fit_results(result)
 
     clear_savefile(SAVE_MODEL)
 
 
-@pytest.mark.parametrize("dill", [False, True])
-def test_save_load_modelresult(dill):
-    """Save/load ModelResult with/without dill."""
-    if dill:
-        pytest.importorskip("dill")
-    else:
-        lmfit.jsonutils.HAS_DILL = False
-
+def test_save_load_modelresult():
+    """Save/load ModelResult now always asserting that dill is available."""
     # create model, perform fit, save ModelResult and perform some tests
     model, params = create_model_params(x, y)
     result = model.fit(y, params, x=x)
     save_modelresult(result, SAVE_MODELRESULT)
 
     file_exists = wait_for_file(SAVE_MODELRESULT, timeout=10)
     assert file_exists
 
     text = ''
     with open(SAVE_MODELRESULT) as fh:
         text = fh.read()
-    assert 12000 < len(text) < 60000  # depending on whether dill is present
+    assert 12000 < len(text) < 60000
 
     # load the saved ModelResult from file and compare results
     result_saved = load_modelresult(SAVE_MODELRESULT)
     assert result_saved.residual is not None
     check_fit_results(result_saved)
 
     clear_savefile(SAVE_MODEL)
@@ -226,14 +213,70 @@
     assert result3 is not None
     assert_allclose(result2.params['a'], 0.5, rtol=1.0e-2)
     assert_allclose(result2.params['b'], 0.22, rtol=1.0e-2)
     assert_allclose(result3.params['a'], 0.50, rtol=1.0e-2)
     assert_allclose(result3.params['b'], 0.22, rtol=1.0e-2)
 
 
+def test_saveload_modelresult_roundtrip_user_expr_function():
+    """Test for modelresult.loads()/dumps() for a model with user defined expr function."""
+
+    def mfunc(x, a, b):
+        return a * (x-b)
+
+    def expr_func(x):
+        return 3 * x
+
+    model = Model(mfunc)
+    params = Parameters(usersyms={"expr_func": expr_func})
+    params.add("a", min=.01, max=1)
+    params.add("b", min=.01, max=3.1)
+    params.add("c", expr="expr_func(a)")
+
+    np.random.seed(2020)
+    xx = np.linspace(-5, 5, 201)
+    yy = 0.5 * (xx - 0.22) + np.random.normal(scale=0.01, size=xx.size)
+
+    result1 = model.fit(yy, params=params, x=xx)
+
+    result2 = ModelResult(model, Parameters())
+    result2.loads(result1.dumps(), funcdefs={'mfunc': mfunc, 'expr_func': expr_func})
+
+    assert result1.userfcn == result2.userfcn
+    assert result1.params == result2.params
+    assert result1.init_params == result2.init_params
+    assert set(result1.params._asteval.symtable) == set(result2.params._asteval.symtable)
+
+
+def test_saveload_modelresult_eval_uncertainty():
+    """Test for ModelResult.loads() and eval_uncertainty
+    GH Issue #909
+
+    """
+    savefile = 'modres_x.txt'
+    x = np.linspace(-10, 10, 201)
+    amp, cen, wid = 3.4, 1.8, 0.5
+
+    y = amp * np.exp(-(x-cen)**2 / (2*wid**2)) / (np.sqrt(2*np.pi)*wid)
+    y += np.random.normal(size=x.size, scale=0.01)
+
+    gmod = GaussianModel()
+    result = gmod.fit(y, x=x, amplitude=5, center=2, sigma=1)
+    save_modelresult(result, savefile)
+    time.sleep(0.25)
+
+    result2 = load_modelresult(savefile)
+
+    dymod = result2.eval_uncertainty()
+
+    assert len(dymod) == len(x)
+    assert dymod.sum() > 0.
+    os.unlink(savefile)
+
+
 def test_saveload_modelresult_expression_model():
     """Test for ModelResult.loads()/dumps() for ExpressionModel.
 
     * make sure that the loaded ModelResult has `init_params` and `init_fit`.
 
     """
     savefile = 'expr_modres.txt'
@@ -312,7 +355,31 @@
                  'nan_policy', 'scale_covar', 'calc_covar', 'ci_out',
                  'col_deriv', 'flatchain', 'call_kws', 'var_names',
                  'user_options', 'kws', 'init_values', 'best_values'):
         val = summary.get(attr, '__INVALID__')
         assert val != '__INVALID__'
 
     assert len(json.dumps(summary)) > 100
+
+
+def test_load_model_versions():
+    """test multiple loading saved models from different
+    python and lmfit versions:
+
+    note that providing the model function is important - these
+    cannot be transferred between Python versions
+    """
+    def local_sine(x, amp, freq, shift):
+        return amp * np.sin(x*freq + shift)
+
+    x = np.linspace(0, 10, 101)
+
+    for fname in ('sinemodel_py310_lm122.sav',
+                  'sinemodel_py311_lm122.sav',
+                  'sinemodel_py312_lm122.sav'):
+        fpath = os.path.join(os.path.dirname(__file__), 'saved_models', fname)
+
+        mod = load_model(fpath, funcdefs={'mysine': local_sine})
+        pars = mod.make_params(amp=2, freq=0.8, shift=0.200)
+        y = mod.eval(pars, x=x)
+        assert y.max() > 1.55
+        assert y.min() < -1.55
```

### Comparing `lmfit-1.2.2/tests/test_model_uncertainties.py` & `lmfit-1.3.0/tests/test_model_uncertainties.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_models.py` & `lmfit-1.3.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_multidatasets.py` & `lmfit-1.3.0/tests/test_multidatasets.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_nose.py` & `lmfit-1.3.0/tests/test_nose.py`

 * *Files 0% similar despite different names*

```diff
@@ -543,15 +543,15 @@
 
         self.mini.emcee(nwalkers=20, steps=25)
 
         # if you've run the sampler the Minimizer object should have a _lastpos
         # attribute
         assert hasattr(self.mini, '_lastpos')
 
-        # now try and re-use sampler
+        # now try and reuse sampler
         out2 = self.mini.emcee(steps=10, reuse_sampler=True)
         assert out2.chain.shape == (35, 20, 4)
 
         # you shouldn't be able to reuse the sampler if nvarys has changed.
         self.mini.params['amp'].vary = False
         pytest.raises(ValueError, self.mini.emcee, reuse_sampler=True)
```

### Comparing `lmfit-1.2.2/tests/test_pandas.py` & `lmfit-1.3.0/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_parameter.py` & `lmfit-1.3.0/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_parameters.py` & `lmfit-1.3.0/tests/test_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,17 +501,16 @@
     # to "<function test_dumps_loads_parameters_usersyms.<locals>.half at 0x?????????>
     # This result in the "importer" to be set to None and the final "decode4js"
     # does not do the correct thing.
     #
     # Of note, this is only an issue within the py.test framework and it DOES
     # work correctly in a normal Python interpreter. Also, it isn't an issue
     # when DILL is used, so in that case the two asserts below will pass.
-    if lmfit.jsonutils.HAS_DILL:
-        assert newpars == pars
-        assert_allclose(newpars['c'].value, 53.0)
+    assert newpars == pars
+    assert_allclose(newpars['c'].value, 53.0)
 
 
 def test_parameters_expr_and_constraints():
     """Regression tests for GitHub Issue #265. Test that parameters are re-
     evaluated if they have bounds and expr.
 
     """
```

### Comparing `lmfit-1.2.2/tests/test_printfuncs.py` & `lmfit-1.3.0/tests/test_printfuncs.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.2/tests/test_shgo.py` & `lmfit-1.3.0/tests/test_shgo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Tests for the SHGO global minimization algorithm."""
 
 import numpy as np
 from numpy.testing import assert_allclose
 import pytest
 import scipy
-from scipy import __version__ as scipy_version
 
 import lmfit
 
 
 def eggholder(x):
     return (-(x[1] + 47.0) * np.sin(np.sqrt(abs(x[0]/2.0 + (x[1] + 47.0))))
             - x[0] * np.sin(np.sqrt(abs(x[0] - (x[1] + 47.0)))))
@@ -78,20 +77,14 @@
     out = minimizer_Alpine02.minimize(method='shgo', sampling_method='sobol')
     out_x = np.array([out.params['x0'].value, out.params['x1'].value])
 
     assert_allclose(out.residual, fglob, rtol=1e-5)
     assert_allclose(min(out_x), min(global_optimum), rtol=1e-3)
     assert_allclose(max(out_x), max(global_optimum), rtol=1e-3)
 
-    # FIXME: update when SciPy requirement is >= 1.7
-    if int(scipy_version.split('.')[1]) >= 7:
-        assert out.call_kws['n'] is None
-    else:
-        assert out.call_kws['n'] == 100
-
 
 def test_shgo_bounds(minimizer_Alpine02):
     """Test SHGO algorithm with bounds."""
     pars_bounds = lmfit.Parameters()
     pars_bounds.add_many(('x0', 1., True, 5.0, 15.0),
                          ('x1', 1., True, 2.5, 7.5))
```

### Comparing `lmfit-1.2.2/tests/test_stepmodel.py` & `lmfit-1.3.0/tests/test_stepmodel.py`

 * *Files identical despite different names*

