# Comparing `tmp/rad-0.19.0.tar.gz` & `tmp/rad-0.19.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-0.19.0.tar", last modified: Fri Feb  9 17:31:51 2024, max compression
+gzip compressed data, was "rad-0.19.1.tar", last modified: Thu Apr  4 15:39:28 2024, max compression
```

## Comparing `rad-0.19.0.tar` & `rad-0.19.1.tar`

### file list

```diff
@@ -1,133 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.509467 rad-0.19.0/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-09 17:31:34.000000 rad-0.19.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.489467 rad-0.19.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-09 17:31:34.000000 rad-0.19.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-09 17:31:34.000000 rad-0.19.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.493467 rad-0.19.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-09 17:31:34.000000 rad-0.19.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-02-09 17:31:34.000000 rad-0.19.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-09 17:31:34.000000 rad-0.19.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-02-09 17:31:34.000000 rad-0.19.0/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-09 17:31:34.000000 rad-0.19.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-02-09 17:31:34.000000 rad-0.19.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-09 17:31:34.000000 rad-0.19.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-09 17:31:34.000000 rad-0.19.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-02-09 17:31:34.000000 rad-0.19.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-02-09 17:31:34.000000 rad-0.19.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-09 17:31:34.000000 rad-0.19.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-02-09 17:31:34.000000 rad-0.19.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:34.000000 rad-0.19.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-02-09 17:31:51.509467 rad-0.19.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-02-09 17:31:34.000000 rad-0.19.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.493467 rad-0.19.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-02-09 17:31:34.000000 rad-0.19.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.493467 rad-0.19.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-09 17:31:34.000000 rad-0.19.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    59966 2024-02-09 17:31:34.000000 rad-0.19.0/docs/_static/stsci_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.485468 rad-0.19.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.493467 rad-0.19.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-09 17:31:34.000000 rad-0.19.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-09 17:31:34.000000 rad-0.19.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-09 17:31:34.000000 rad-0.19.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-09 17:31:34.000000 rad-0.19.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-02-09 17:31:34.000000 rad-0.19.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-09 17:31:34.000000 rad-0.19.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-09 17:31:34.000000 rad-0.19.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-02-09 17:31:34.000000 rad-0.19.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-09 17:31:34.000000 rad-0.19.0/docs/manifests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-09 17:31:34.000000 rad-0.19.0/docs/reference_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-09 17:31:34.000000 rad-0.19.0/docs/schemas.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-02-09 17:31:34.000000 rad-0.19.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.493467 rad-0.19.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-02-09 17:31:34.000000 rad-0.19.0/scripts/insert_next_release.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      954 2024-02-09 17:31:34.000000 rad-0.19.0/scripts/set_release_date.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 17:31:51.509467 rad-0.19.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.485468 rad-0.19.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.493467 rad-0.19.0/src/rad/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-09 17:31:51.000000 rad-0.19.0/src/rad/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.497467 rad-0.19.0/src/rad/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.497467 rad-0.19.0/src/rad/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)    13031 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/manifests/datamodels-1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.501468 rad-0.19.0/src/rad/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/aperture-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/cal_logs-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/cal_step-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/coordinates-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14228 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/exposure-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/guidestar-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/mosaic_associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/msos_stack-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/observation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/photometry-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/pointing-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/program-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/ramp-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/ref_file-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.505468 rad-0.19.0/src/rad/resources/schemas/reference_files/
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/resample-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/source_detection-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.509467 rad-0.19.0/src/rad/resources/schemas/tagged_scalars/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/target-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/visit-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-02-09 17:31:34.000000 rad-0.19.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.509467 rad-0.19.0/src/rad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-02-09 17:31:51.000000 rad-0.19.0/src/rad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-02-09 17:31:51.000000 rad-0.19.0/src/rad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 17:31:51.000000 rad-0.19.0/src/rad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-09 17:31:51.000000 rad-0.19.0/src/rad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-09 17:31:51.000000 rad-0.19.0/src/rad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-09 17:31:51.000000 rad-0.19.0/src/rad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:51.509467 rad-0.19.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 17:31:34.000000 rad-0.19.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-09 17:31:34.000000 rad-0.19.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-02-09 17:31:34.000000 rad-0.19.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-02-09 17:31:34.000000 rad-0.19.0/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-02-09 17:31:34.000000 rad-0.19.0/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-02-09 17:31:34.000000 rad-0.19.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.827628 rad-0.19.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-04 15:39:19.000000 rad-0.19.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.803628 rad-0.19.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-04 15:39:19.000000 rad-0.19.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 15:39:19.000000 rad-0.19.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.803628 rad-0.19.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-04 15:39:19.000000 rad-0.19.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-04 15:39:19.000000 rad-0.19.1/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-04 15:39:19.000000 rad-0.19.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-04 15:39:19.000000 rad-0.19.1/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-04 15:39:19.000000 rad-0.19.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-04 15:39:19.000000 rad-0.19.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-04 15:39:19.000000 rad-0.19.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-04 15:39:19.000000 rad-0.19.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-04-04 15:39:19.000000 rad-0.19.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-04 15:39:19.000000 rad-0.19.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-04 15:39:19.000000 rad-0.19.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-04 15:39:19.000000 rad-0.19.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:19.000000 rad-0.19.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-04 15:39:28.827628 rad-0.19.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-04 15:39:19.000000 rad-0.19.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-04 15:39:19.000000 rad-0.19.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-04 15:39:19.000000 rad-0.19.1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    59966 2024-04-04 15:39:19.000000 rad-0.19.1/docs/_static/stsci_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.799628 rad-0.19.1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-04 15:39:19.000000 rad-0.19.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-04 15:39:19.000000 rad-0.19.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-04 15:39:19.000000 rad-0.19.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-04 15:39:19.000000 rad-0.19.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-04 15:39:19.000000 rad-0.19.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-04 15:39:19.000000 rad-0.19.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20610 2024-04-04 15:39:19.000000 rad-0.19.1/docs/creating.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-04 15:39:19.000000 rad-0.19.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-04 15:39:19.000000 rad-0.19.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-04 15:39:19.000000 rad-0.19.1/docs/manifests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-04 15:39:19.000000 rad-0.19.1/docs/reference_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-04 15:39:19.000000 rad-0.19.1/docs/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-04 15:39:19.000000 rad-0.19.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-04-04 15:39:19.000000 rad-0.19.1/scripts/insert_next_release.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      954 2024-04-04 15:39:19.000000 rad-0.19.1/scripts/set_release_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:39:28.827628 rad-0.19.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.799628 rad-0.19.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/src/rad/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/src/rad/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.807628 rad-0.19.1/src/rad/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/manifests/datamodels-1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.819628 rad-0.19.1/src/rad/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/aperture-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/base_exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/base_guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/cal_logs-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/coordinates-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/ephemeris-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/fps-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/ground_common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/groundtest-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/guidewindow-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/mosaic_associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/msos_stack-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/observation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/outlier_detection-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/photometry-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/pointing-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/program-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/rad_schema-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/ramp-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/ref_file-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.823628 rad-0.19.1/src/rad/resources/schemas/reference_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/resample-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/segmentation_map-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/source_catalog-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/source_detection-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.823628 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/target-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tvac-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11527 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/visit-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wfi_image-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-04 15:39:19.000000 rad-0.19.1/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.823628 rad-0.19.1/src/rad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-04 15:39:28.000000 rad-0.19.1/src/rad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:28.823628 rad-0.19.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:39:19.000000 rad-0.19.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 15:39:19.000000 rad-0.19.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-04 15:39:19.000000 rad-0.19.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-04 15:39:19.000000 rad-0.19.1/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-04 15:39:19.000000 rad-0.19.1/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-04 15:39:19.000000 rad-0.19.1/tox.ini
```

### Comparing `rad-0.19.0/.github/pull_request_template.md` & `rad-0.19.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/.github/workflows/changelog.yml` & `rad-0.19.1/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/.github/workflows/ci_cron.yml` & `rad-0.19.1/.github/workflows/ci_cron.yml`

 * *Files 3% similar despite different names*

```diff
@@ -16,10 +16,9 @@
 
 jobs:
   test:
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@v1
     if: (github.repository == 'spacetelescope/rad' && (github.event_name == 'schedule' || github.event_name == 'push' || github.event_name == 'workflow_dispatch' || contains(github.event.pull_request.labels.*.name, 'Weekly CI')))
     with:
       envs: |
-        - macos: py39-xdist
         - macos: py310-xdist
         - linux: py312-devdeps-xdist
```

### Comparing `rad-0.19.0/.github/workflows/release.yml` & `rad-0.19.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/.gitignore` & `rad-0.19.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/.pre-commit-config.yaml` & `rad-0.19.1/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -30,32 +30,32 @@
   hooks:
     - id: codespell
       args: ["--write-changes"]
       additional_dependencies:
         - tomli
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: 'v3.15.0'
+  rev: 'v3.15.1'
   hooks:
     - id: pyupgrade
       args: ["--py38-plus"]
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: 'v0.2.0'
+  rev: 'v0.2.2'
   hooks:
     - id: ruff
       args: ["--fix"]
 
 - repo: https://github.com/pycqa/isort
   rev: 5.13.2
   hooks:
     - id: isort
 
 - repo: https://github.com/psf/black
-  rev: 24.1.1
+  rev: 24.2.0
   hooks:
     - id: black
 
 - repo: https://github.com/PyCQA/bandit
   rev: 1.7.7
   hooks:
     - id: bandit
```

### Comparing `rad-0.19.0/CHANGES.rst` & `rad-0.19.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,46 @@
-0.19.1 (unreleased)
+0.20.0 (unreleased)
 -------------------
 
 -
 
-0.19.0 (2024-02-09)
+0.19.1 (2024-04-04)
+-------------------
+
+- Add new schemas to documentation. [#386]
+
+- Convert tag keywords to wildcards for external tags. [#370]
+
+- Added ``exact_datatype`` arguments to prevent ASDF from casting array
+  datatypes during save. [#369]
+
+- Add documentation on how to create a new schema. [#375]
+
+- Add ``FPS`` and ``TVAC`` schemas. [#364]
+
+- Update titles and descriptions to those provided by INS. [#361]
+
+- Updated product table names. [#382]
+
+- Changed image units from e/s to DN/s (and added support for MJy/sr). [#389]
+
+- Add attributes under the ``basic`` schema to ``WfiMosaic.meta``. [#390]
+
+- Split cal_step into L2 and L3 versions. [#397]
+
+- Add Members Keyword to Resample Schema. [#396]
+
+- Create the flux step schema. [#395]
+
+- Create ``outlier_detection`` schema and add bit mask field to both it and ``resample``. [#401]
+
+- Add source_catalog and segmentation_map schemas for Level 2 and Level 3 files. [#393]
+
+
+  0.19.0 (2024-02-09)
 -------------------
 
 - Added streamlined Level 3 Mosaic metadata schemas. [#334]
 
 - Remove the unused ``variance-1.0.0`` schema. [#344]
 
 - Add wcs tag to wfi_image and wfi_mosaic schemas. [#351]
@@ -33,15 +66,15 @@
 
 
 0.17.1 (2023-08-03)
 -------------------
 
 - Added "archive_catalog" field to ref_file. [#303]
 
-- Added a prefix "s_" to the archive destination in "cal_step". [#303]
+- Added a prefix ``s_`` to the archive destination in "cal_step". [#303]
 
 - Require all the new ``cal_step`` steps to be present in the ``cal_step`` schema. [#301]
 
 - Add missing unit enforcements to various schemas. [#300]
 
 0.17.0 (2023-07-27)
 -------------------
```

### Comparing `rad-0.19.0/CODE_OF_CONDUCT.md` & `rad-0.19.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/LICENSE` & `rad-0.19.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/PKG-INFO` & `rad-0.19.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.19.0
+Version: 0.19.1
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -34,32 +34,32 @@
         
 Project-URL: Bug Tracker, https://github.com/spacetelescope/rad/issues
 Project-URL: Source Code, https://github.com/spacetelescope/rad
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asdf>=2.14.2
 Requires-Dist: asdf-astropy>=0.5.0
 Provides-Extra: test
 Requires-Dist: pytest>=4.6.0; extra == "test"
 Requires-Dist: pytest-doctestplus>=0.11.1; extra == "test"
 Requires-Dist: crds>=11.16.16; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-asdf>=0.1.3; extra == "docs"
 Requires-Dist: sphinx-astropy; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: astropy>=5.0.4; extra == "docs"
 Requires-Dist: graphviz; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
 Requires-Dist: docutils; extra == "docs"
-Requires-Dist: stsci-rtd-theme; extra == "docs"
 Requires-Dist: tomli; python_version < "3.11" and extra == "docs"
 Requires-Dist: importlib-metadata; extra == "docs"
 
 # Roman Attribute Dictionary
 
 [![CI](https://github.com/spacetelescope/rad/actions/workflows/ci.yml/badge.svg)](https://github.com/spacetelescope/rad/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/rad/badge/?version=latest)](https://rad.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `rad-0.19.0/README.md` & `rad-0.19.1/README.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/docs/Makefile` & `rad-0.19.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/docs/_static/custom.css` & `rad-0.19.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/docs/_static/stsci_logo.png` & `rad-0.19.1/docs/_static/stsci_logo.png`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/docs/conf.py` & `rad-0.19.1/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 import datetime
 import os
 import sys
 from pathlib import Path
 
 # Ensure documentation examples are deterministically random.
 import numpy
-import stsci_rtd_theme
 
 if sys.version_info < (3, 11):
     import tomli as tomllib
 else:
     import tomllib
 
 from importlib_metadata import distribution
@@ -61,14 +60,15 @@
 # needs_sphinx = '1.2'
 
 intersphinx_mapping["pypa-packaging"] = ("https://packaging.python.org/en/latest/", None)  # noqa: E501, F405
 intersphinx_mapping["asdf"] = ("https://asdf.readthedocs.io/en/latest/", None)  # noqa: E501, F405
 intersphinx_mapping["asdf-standard"] = ("https://asdf-standard.readthedocs.io/en/latest/", None)  # noqa: E501, F405
 intersphinx_mapping["asdf-astropy"] = ("https://asdf-astropy.readthedocs.io/en/latest/", None)  # noqa: E501, F405
 intersphinx_mapping["pytest"] = ("https://docs.pytest.org/en/latest/", None)  # noqa: E501, F405
+intersphinx_mapping["roman_datamodels"] = ("https://roman-datamodels.readthedocs.io/en/latest/", None)  # noqa: E501, F405
 
 # To perform a Sphinx version check that needs to be more specific than
 # major.minor, call `check_sphinx_version("x.y.z")` here.
 # check_sphinx_version("1.2.1")
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
@@ -101,16 +101,15 @@
 # Add any paths that contain custom themes here, relative to this directory.
 # To use a different custom theme, add the directory containing the theme.
 # html_theme_path = []
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes. To override the custom theme, set this to the
 # name of a builtin theme or the name of a custom theme in html_theme_path.
-html_theme = "stsci_rtd_theme"
-html_theme_path = [stsci_rtd_theme.get_html_theme_path()]
+html_theme = "sphinx_rtd_theme"
 
 html_static_path = ["_static"]
 
 # Custom sidebar templates, maps document names to template names.
 # html_sidebars = {}
 
 # The name of an image file (within the static path) to use as favicon of the
@@ -156,7 +155,10 @@
 
 # -- sphinx_asdf configuration ---------------------------------------------
 
 # Top-level directory containing ASDF schemas (relative to current directory)
 asdf_schema_path = "../src/rad/resources"
 # This is the prefix common to all schema IDs in this repository
 asdf_schema_standard_prefix = "schemas"
+asdf_schema_reference_mappings = [
+    ("asdf://stsci.edu/datamodels/roman/tags/", "https://rad.readthedocs.io/en/latest/generated/schemas/"),
+]
```

### Comparing `rad-0.19.0/docs/index.rst` & `rad-0.19.1/docs/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 .. _rad:
 
 **************************
 Roman Attribute Dictionary
 **************************
 
-The Roman Attribute Dictionary (RAD) is package which defines schemas for the Nancy Grace
-Roman Space Telescope shared attributes for processing and archive.
+The Roman Attribute Dictionary (RAD) is a package which defines schemas for the Nancy Grace
+Roman Space Telescope files. Metadata attributes are used by both Science Data Processing and
+the Archive Keyword Dictionary.
 
 .. note::
-  These schemas are schemas for the :ref:`ASDF file <asdf-standard:asdf-standard>` file format, which
-  are used by ASDF to serialize and deserialize data for the Nancy Grace Roman Space Telescope.
+  These are schemas for the :ref:`ASDF file <asdf-standard:asdf-standard>` file format,
+  used by ASDF to serialize and deserialize data for the Nancy Grace Roman Space Telescope.
 
 Included Resources
 ==================
 
 The following are listings of all the schemas provided by this package for ASDF.
 
 .. note::
@@ -28,14 +29,15 @@
 
 Developer Resources
 ===================
 
 .. toctree::
   :maxdepth: 1
 
+  creating.rst
   contributing.rst
   changes.rst
 
 Index
 =====
 
 * :ref:`genindex`
```

### Comparing `rad-0.19.0/docs/make.bat` & `rad-0.19.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/scripts/insert_next_release.py` & `rad-0.19.1/scripts/insert_next_release.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/scripts/set_release_date.py` & `rad-0.19.1/scripts/set_release_date.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/src/rad/integration.py` & `rad-0.19.1/src/rad/integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/src/rad/resources/manifests/datamodels-1.0.yaml` & `rad-0.19.1/src/rad/resources/manifests/datamodels-1.0.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -111,19 +111,29 @@
   description: |-
     Wcsinfo information
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/guidestar-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/guidestar-1.0.0
   title: Guidestar information
   description: |-
     Guidestar information
-- tag_uri: asdf://stsci.edu/datamodels/roman/tags/cal_step-1.0.0
-  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/cal_step-1.0.0
-  title: Calibration Step status information
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/l2_cal_step-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/l2_cal_step-1.0.0
+  title: Level 2 Calibration Step status information
+  description: |-
+    Level 2 Calibration Step status information
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/l3_cal_step-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/l3_cal_step-1.0.0
+  title: Level 3 Calibration Step status information
+  description: |-
+    Level 3 Calibration Step status information
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/outlier_detection-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/outlier_detection-1.0.0
+  title: Outlier Detection information
   description: |-
-    Calibration Step status information
+    Outlier Detection information
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/resample-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/resample-1.0.0
   title: Resample information
   description: |-
     Resample information
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/individual_image_meta-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/individual_image_meta-1.0.0
@@ -141,14 +151,45 @@
   description: |-
     Mosaic associations metadata keywords
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/mosaic_wcsinfo-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/mosaic_wcsinfo-1.0.0
   title: Mosaic WCS parameters
   description: |-
     Mosaic WCS parameters
+# Ground Modules
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/base_exposure-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/base_exposure-1.0.0
+  title: Exposure information
+  description: |-
+    Ground test exposure information
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/base_guidestar-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/base_guidestar-1.0.0
+  title: Guidestar information
+  description: |-
+    Guidestar information
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/groundtest-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/groundtest-1.0.0
+  title: Ground Test Information
+  description: |-
+    Ground test description.
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac_groundtest-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac_groundtest-1.0.0
+  title: TVAC Ground Test Information
+  description: |-
+    TVAC ground test description.
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/fps-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/fps-1.0.0
+  title: FPS schema
+  description: |-
+    FPS test data
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/tvac-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tvac-1.0.0
+  title: TVAC schema
+  description: |-
+    TVAC test data
 # Reference Modules
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/dark-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/reference_files/dark-1.0.0
   title: Dark reference schema
   description: |-
     Dark reference schema
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/distortion-1.0.0
@@ -228,14 +269,34 @@
   description: |-
     Calibration log message
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/ref_file-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/ref_file-1.0.0
   title: Calibration reference file names.
   description: |-
     Calibration reference file names.
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/source_catalog-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/source_catalog-1.0.0
+  title: Source catalog
+  description: |-
+    Photometry and astrometry computed by the Source Catalog Step
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/segmentation_map-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/segmentation_map-1.0.0
+  title: Segmentation map
+  description: |-
+    Segmentation map computed by the Source Catalog Step
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/mosaic_source_catalog-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/mosaic_source_catalog-1.0.0
+  title: Mosaic source catalog
+  description: |-
+    Photometry and astrometry computed by the Source Catalog Step
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/mosaic_segmentation_map-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/mosaic_segmentation_map-1.0.0
+  title: Mosaic segmentation map
+  description: |-
+    Segmentation map computed by the Source Catalog Step
 # Tagged Scalars
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/calibration_software_version-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tagged_scalars/calibration_software_version-1.0.0
   title: Calibration software version
   description: |-
     Calibration software version number
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/filename-1.0.0
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/aperture-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/aperture-1.0.0.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/aperture-1.0.0
 
-title: Aperture information
+title: Aperture Information
 type: object
 properties:
   name:
-    title: PRD science aperture used
+    title: PRD Science Aperture Used
+    description: |
+      Science aperture used as defined in the Project
+      Reference Database (PRD).
     type: string
     enum: ['WFI_01_FULL', 'WFI_02_FULL', 'WFI_03_FULL', 'WFI_04_FULL',
            'WFI_05_FULL', 'WFI_06_FULL', 'WFI_07_FULL', 'WFI_08_FULL',
            'WFI_09_FULL', 'WFI_10_FULL', 'WFI_11_FULL', 'WFI_12_FULL',
            'WFI_13_FULL', 'WFI_14_FULL', 'WFI_15_FULL', 'WFI_16_FULL',
            'WFI_17_FULL', 'WFI_18_FULL',
            'BORESIGHT',
            'CGI_CEN', 'WFI_CEN']
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:aperture.AperName
     archive_catalog:
       datatype: nvarchar(40)
-      destination: [ScienceCommon.aperture_name, GuideWindow.aperture_name]
+      destination: [WFIExposure.aperture_name, GuideWindow.aperture_name]
   position_angle:
-    title: "[deg] Position angle of aperture used"
+    title: "Position Angle of Aperture Used (deg)"
+    description: |
+      Position angle of the science aperture as measured in degrees.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD #v3_position_angle in baseline_prime_visits or spacecraft_parameters
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.position_angle, GuideWindow.position_angle]
+      destination: [WFIExposure.position_angle, GuideWindow.position_angle]
 propertyOrder: [name, position_angle]
 flowStyle: block
 required: [name, position_angle]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/common-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/source_catalog-1.0.0.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/common-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/source_catalog-1.0.0
 
-title: Common metadata properties
+title: Source catalog generated from a Level 2 file by the Source Catalog Step.
 
-allOf:
-# Meta Variables
-- $ref: asdf://stsci.edu/datamodels/roman/schemas/basic-1.0.0
-- type: object
-  properties:
-    # Meta Objects
-    aperture:
-      tag: asdf://stsci.edu/datamodels/roman/tags/aperture-1.0.0
-    cal_step:
-      tag: asdf://stsci.edu/datamodels/roman/tags/cal_step-1.0.0
-    coordinates:
-      tag: asdf://stsci.edu/datamodels/roman/tags/coordinates-1.0.0
-    ephemeris:
-      tag: asdf://stsci.edu/datamodels/roman/tags/ephemeris-1.0.0
-    exposure:
-      tag: asdf://stsci.edu/datamodels/roman/tags/exposure-1.0.0
-    guidestar:
-      tag: asdf://stsci.edu/datamodels/roman/tags/guidestar-1.0.0
-    instrument:
-      tag: asdf://stsci.edu/datamodels/roman/tags/wfi_mode-1.0.0
-    observation:
-      tag: asdf://stsci.edu/datamodels/roman/tags/observation-1.0.0
-    pointing:
-      tag: asdf://stsci.edu/datamodels/roman/tags/pointing-1.0.0
-    program:
-      tag: asdf://stsci.edu/datamodels/roman/tags/program-1.0.0
-    ref_file:
-      tag: asdf://stsci.edu/datamodels/roman/tags/ref_file-1.0.0
-    target:
-      tag: asdf://stsci.edu/datamodels/roman/tags/target-1.0.0
-    velocity_aberration:
-      tag: asdf://stsci.edu/datamodels/roman/tags/velocity_aberration-1.0.0
-    visit:
-      tag: asdf://stsci.edu/datamodels/roman/tags/visit-1.0.0
-    wcsinfo:
-      tag: asdf://stsci.edu/datamodels/roman/tags/wcsinfo-1.0.0
-  required: [aperture, cal_step, coordinates, ephemeris, exposure, guidestar,
-             instrument, observation, pointing, program, ref_file,
-             target, velocity_aberration, visit, wcsinfo]
+datamodel_name: SourceCatalogModel
+
+archive_meta: None
+type: object
+properties:
+  meta:
+    allOf:
+      - $ref: basic-1.0.0
+      - type: object
+        properties:
+          optical_element:
+            title: WFI Optical Element
+            description: |
+              WFI optical element used to take the data.
+            $ref: wfi_optical_element-1.0.0
+          exposure:
+            title: Exposure Information
+            tag: asdf://stsci.edu/datamodels/roman/tags/exposure-1.0.0
+          photometry:
+            title: Photometry Information
+            tag: asdf://stsci.edu/datamodels/roman/tags/photometry-1.0.0
+          program:
+            title: Program Information
+            tag: asdf://stsci.edu/datamodels/roman/tags/program-1.0.0
+          visit:
+            title: Visit Information
+            tag: asdf://stsci.edu/datamodels/roman/tags/visit-1.0.0
+        required: [optical_element, exposure, photometry, program, visit]
+  source_catalog:
+    title: Source Catalog
+    description: |
+       Photometry and astrometry computed in the Source Catalog Step.
+    tag: tag:astropy.org:astropy/table/table-1.*
+
+required: [meta, source_catalog]
+flowStyle: block
+propertyOrder: [meta, source_catalog]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/coordinates-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/coordinates-1.0.0.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/coordinates-1.0.0
 
-title: Information about the coordinates in the file
+title: Name Of The Coordinate Reference Frame
 type: object
 properties:
   reference_frame:
-    title: Name of the coordinate reference frame
+    title: Name of the Coordinate Reference Frame
+    description: |
+      Name of the coordinate reference frame.
     type: string
     default: ICRS
     enum: [ICRS]
     archive_catalog:
       datatype: nvarchar(10)
-      destination: [ScienceCommon.reference_frame, GuideWindow.reference_frame]
+      destination: [WFIExposure.reference_frame, WFIMosaic.reference_frame, GuideWindow.reference_frame]
 flowStyle: block
 required: [reference_frame]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/exposure-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/guidewindow-1.0.0.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,423 +1,289 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/exposure-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/guidewindow-1.0.0
 
+title: Guide Star Window Information
 
-title: |
-  Exposure information
+datamodel_name: GuidewindowModel
+
+archive_meta: None
 
 type: object
 properties:
-  id:
-    title: Exposure id number within visit
-    description: The exposure number for a given visit id
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: int
-      destination: [ScienceCommon.exposure_id, GuideWindow.exposure_id]
-
-  type:
-    $ref: exposure_type-1.0.0
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: nvarchar(25)
-      destination: [ScienceCommon.exposure_type, GuideWindow.exposure_type]
-
-  start_time:
-    title: UTC exposure start time
-    description: |
-        This is a python date-time object that records the
-        time at the start of the exposure in UTC.
-    tag: tag:stsci.edu:asdf/time/time-1.1.0
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: datetime2
-      destination: [ScienceCommon.exposure_start_time, GuideWindow.exposure_start_time]
-  mid_time:
-    title: UTC exposure mid time
-    description: |
-        This is a python date-time object that records the
-        time at the middle of the exposure in UTC.
-    tag: tag:stsci.edu:asdf/time/time-1.1.0
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: datetime2
-      destination: [ScienceCommon.exposure_mid_time, GuideWindow.exposure_mid_time]
-  end_time:
-    title: UTC exposure end time
-    description: |
-        This is a python date-time object that records the
-        time at the end of the exposure in UTC.
-    tag: tag:stsci.edu:asdf/time/time-1.1.0
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: datetime2
-      destination: [ScienceCommon.exposure_end_time, GuideWindow.exposure_end_time]
-  start_time_mjd:
-    title: "[d] exposure start time in MJD"
-    description: |
-         This records the time at the start of the exposure using the
-         Modified Julian Date (MJD). This is used in the archive catalog for
-         multi-mission matching.
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.exposure_start_time_mjd, GuideWindow.exposure_start_time_mjd]
-  mid_time_mjd:
-    title: "[d] exposure mid time in MJD"
-    description: |
-        This records the time at the midpoint of the exposure using the
-        Modified Julian Date  (MJD). This is used in the archive catalog for
-        multi-mission matching.
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.exposure_mid_time_mjd, GuideWindow.exposure_mid_time_mjd]
-  end_time_mjd:
-    title: "[d] exposure end time in MJD"
-    description: |
-        This records the time at the end of the exposure using the
-        Modified Julian Date  (MJD). This is used in the archive catalog for
-        multi-mission matching.
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.exposure_end_time_mjd, GuideWindow.exposure_end_time_mjd]
-  start_time_tdb:
-    title: "[d] TDB time of exposure start in MJD"
-    description: |
-        This records the time at the start of the exposure using
-        the Modified Julian Date for the Barycentric Dynamical Time system
-        (TDB, Temps Dynamique Barycentrique), a relativistic coordinate
-        time scale.
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.exposure_start_time_tdb, GuideWindow.exposure_start_time_tdb]
-  mid_time_tdb:
-    title: "[d] TDB time of exposure mid in MJD"
-    description: |
-        This records the time at the midpoint of the exposure using
-        the Modified Julian Date for the Barycentric Dynamical Time system
-        (TDB, Temps Dynamique Barycentrique), a relativistic coordinate
-        time scale.
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.exposure_mid_time_tdb, GuideWindow.exposure_mid_time_tdb]
-  end_time_tdb:
-    title: "[d] TDB time of exposure end in MJD"
-    description: |
-        This records the time at the end of the exposure using
-        the Modified Julian Date for the Barycentric Dynamical Time system
-        (TDB, Temps Dynamique Barycentrique), a relativistic coordinate
-        time scale.
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.exposure_end_time_tdb, GuideWindow.exposure_end_time_tdb]
-  ngroups:
-    title: Number of groups in integration
-    description: |
-        This is the number of resultant frames in the exposure
-        that are transmitted to the ground. The WFI data always has the
-        number of integrations=1.
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: int
-      destination: [ScienceCommon.exposure_ngroups, GuideWindow.exposure_ngroups]
-  nframes:
-    title: Number of frames per group
-    description: |
-        This is the number of science frames that are combined to
-        produce a resultant frame.
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: int
-      destination: [ScienceCommon.exposure_nframes, GuideWindow.exposure_nframes]
-  data_problem:
-    title: Science telemetry indicated a problem
-    description: |
-        This is a flag to indicate that the science telemetry
-        experienced a problem.
-    type: boolean
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: nchar(1)
-      destination: [ScienceCommon.exposure_data_problem, GuideWindow.exposure_data_problem]
-  sca_number:
-    title: Sensor Chip Assembly number
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: int
-      destination: [ScienceCommon.exposure_sca_number, GuideWindow.exposure_sca_number]
-  gain_factor:
-    title: Gain scale factor
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.exposure_gain_factor, GuideWindow.exposure_gain_factor]
-  integration_time:
-    title: "[s] Effective integration time"
-    description: The effective time that the sensor has been exposed to the sky.
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.exposure_integration_time, GuideWindow.exposure_integration_time]
-  elapsed_exposure_time:
-    title: "[s] Total elapsed exposure time"
-    description: |
-        The time between the start of the first Reset/Read Science Frame of an Exposure
-        and the completion of the final Read Only Science Frame of that Exposure.
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.elapsed_exposure_time, GuideWindow.elapsed_exposure_time]
-  frame_divisor:
-    title: Divisor applied to frame-averaged groups
-    description: |
-        This is the number of reads per resultant. Its use depends upon the definition
-        in the MA table.
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: int
-      destination: [ScienceCommon.exposure_frame_divisor, GuideWindow.exposure_frame_divisor]
-  groupgap:
-    title: Number of frames dropped between groups
-    description: This is the number of reads that are "dropped" and not used in the resultant.
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: int
-      destination: [ScienceCommon.exposure_groupgap, GuideWindow.exposure_groupgap]
-  frame_time:
-    title: "[s] Time between frames"
-    description: |
-        The time between the end of one read and the start of the next read. This
-        depends on the MA table being used.
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.exposure_frame_time, GuideWindow.exposure_frame_time]
-  group_time:
-    title: "[s] Time between groups"
-    description: |
-        The time that is the sum of the reads that are used to construct a resultant.
-        This will depend on the MA table being used.
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.exposure_group_time, GuideWindow.exposure_group_time]
-  exposure_time:
-    title: "[s] exposure time"
-    description: |
-        The time between the start of the first Reset/Read Science Frame of an Exposure
-        and the completion of the final Read Only Science Frame of that Exposure.
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.exposure_time, GuideWindow.exposure_time]
-  effective_exposure_time:
-    title: "[s] Effective exposure time"
-    description: The time that the detector is collecting photons that are used in the resultants.
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.effective_exposure_time, GuideWindow.effective_exposure_time]
-  duration:
-    title: "[s] Total duration of exposure"
-    description: |
-        The time that the detector is dedicated to an exposure. This includes any overhead
-        and times for dropped frames etc.
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.exposure_duration, GuideWindow.exposure_duration]
-  ma_table_name:
-    title: Identifier for the multi-accumulation table used
-    description: |
-        The name of the MA table used for the exposure as defined by the
-        PRD (Project Reference Database)
-    type: string
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: nvarchar(50)
-      destination: [ScienceCommon.ma_table_name, GuideWindow.ma_table_name]
-  ma_table_number:
-    title: Numerical identifier for the multi-accumulation table used
-    description: |
-        The number of the MA table used for the exposure as defined by the
-        PRD (Project Reference Database). This is used for matching the exposure
-        to the appropriate calibration data.
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: smallint
-      destination: [ScienceCommon.ma_table_number, GuideWindow.ma_table_number]
-  level0_compressed:
-    title: Level 0 data was compressed
-    description: |
-        A flag to indicate that the exposure has data that needed to be decompressed by
-        the ground system.
-    type: boolean
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: nchar(1)
-      destination: [ScienceCommon.exposure_level0_compressed, GuideWindow.exposure_level0_compressed]
-  read_pattern:
-    title: Pattern of reads
-    description: |
-      Enumeration of detector reads to resultants making up the L1 data downlinked
-      from the observatory
-    type: array
-    items:
-      type: array
-      items:
-        type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: nvarchar(3500)
-      destination: [ScienceCommon.read_pattern, GuideWindow.read_pattern]
-  truncated:
-    title: MA Tables were truncated
-    description: |
-        This is a flag to indicate that the the MA table was truncated.
-    type: boolean
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: nchar(1)
-      destination: [ScienceCommon.exposure_truncated]
-propertyOrder: [id, type,
-           start_time, mid_time, end_time,
-           start_time_mjd, mid_time_mjd, end_time_mjd,
-           start_time_tdb, mid_time_tdb, end_time_tdb,
-           ngroups, nframes, data_problem, sca_number,
-           gain_factor, integration_time, elapsed_exposure_time,
-           frame_divisor, groupgap,
-           frame_time, group_time, exposure_time,
-           effective_exposure_time, duration,
-           ma_table_name, ma_table_number, level0_compressed,
-           read_pattern, truncated]
+  meta:
+    allOf:
+      - $ref: common-1.0.0
+      - type: object
+        properties:
+          gw_start_time:
+            title: Start Time of Guide Window Exposure (UTC)
+            description: |
+              Time in UTC at the start of the guide window exposure.
+            tag: tag:stsci.edu:asdf/time/time-1.*
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: datetime2
+              destination: [GuideWindow.gw_start_time]
+          gw_end_time:
+            title: End Time of Guide Window Exposure (UTC)
+            description: |
+              Time in UTC at the end of the guide window exposure.
+            tag: tag:stsci.edu:asdf/time/time-1.*
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: datetime2
+              destination: [GuideWindow.gw_end_time]
+          gw_frame_readout_time:
+            title: Guide Window Read Time (Seconds)
+            description: |
+              Time to read out the guide window frame in units of seconds.
+            type: number
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: float
+              destination: [GuideWindow.gw_frame_readout_time]
+          gw_function_start_time:
+            title: Guide Window Function Start Time (UTC)
+            description: |
+              Time in UTC at the start of the guider function.
+            tag: tag:stsci.edu:asdf/time/time-1.*
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: datetime2
+              destination: [GuideWindow.gw_function_start_time]
+          gw_function_end_time:
+            title: Guide Window Function End Time (UTC)
+            description: |
+              Time in UTC at the end of the guider function.
+            tag: tag:stsci.edu:asdf/time/time-1.*
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: datetime2
+              destination: [GuideWindow.gw_function_end_time]
+          gw_acq_exec_stat:
+            title: Guide Star Acquisition Status
+            description: |
+              Status of the guide star acquisition.
+            type: string
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: nvarchar(15)
+              destination: [GuideWindow.gw_acq_exec_stat]
+          pedestal_resultant_exp_time:
+            title: Guide Window Pedestal Exposure Time (Seconds)
+            description: |
+              Cumulative exposure time for all of the guide window pedestal
+              resultants in units of seconds.
+            type: number
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: float
+              destination: [GuideWindow.gw_pedestal_resultant_exp_time]
+          signal_resultant_exp_time:
+            title: Guide Window Signal Exposure Time (Seconds)
+            description: |
+              Cumulative exposure time for all of the guide window signal
+              resultants in units of seconds
+            type: number
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: float
+              destination: [GuideWindow.gw_signal_resultant_exp_time]
+          gw_acq_number:
+            title: Guide Star Acquisition Identifier
+            description: |
+              Identifier representing the guide star acquisition number within
+              the visit.
+            type: integer
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: int
+              destination: [GuideWindow.gw_acq_number]
+          gw_science_file_source:
+            title: Science File Name
+            description: |
+                Name of the file containing the WFI science exposure
+                corresponding to the guide window data contained within this
+                file.
+            type: string
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: nvarchar(120)
+              destination: [GuideWindow.gw_science_file_source]
+          gw_mode:
+            $ref: guidewindow_modes-1.0.0
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: nvarchar(18)
+              destination: [GuideWindow.gw_mode]
+          gw_window_xstart:
+            title: Guide Window X Start Position (pixels)
+            description: |
+              Minimum X position in the science coordinate frame of all tracking
+              guide windows in this exposure measured in pixels.
+            type: integer
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: int
+              destination: [GuideWindow.gw_window_xstart]
+          gw_window_ystart:
+            title: Guide Window Y Start Position (pixels)
+            description: |
+              Minimum Y position in the science coordinate frame of all tracking
+              guide windows in this exposure measured in pixels.
+            type: integer
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: int
+              destination: [GuideWindow.gw_window_ystart]
+          gw_window_xstop:
+            title: Guide Window X Stop Position (pixels)
+            description: |
+              Maximum X position in the science coordinate frame of all tracking
+              guide windows in this exposure measured in pixels.
+            type: integer
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: int
+              destination: [GuideWindow.gw_window_xstop]
+          gw_window_ystop:
+            title: Guide Window Y Stop Position (pixels)
+            description: |
+              Maximum Y position in the science coordinate frame of all tracking
+              guide windows in this exposure measured in pixels.
+            type: integer
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: int
+              destination: [GuideWindow.gw_window_ystop]
+          gw_window_xsize:
+            title: Guide window size in the x direction in detector coordinates
+            type: integer
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: int
+              destination: [GuideWindow.gw_window_xsize]
+          gw_window_ysize:
+            title: Guide window size in the y direction in detector coordinates
+            type: integer
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: int
+              destination: [GuideWindow.gw_window_ysize]
+        required: [gw_start_time, gw_end_time, gw_frame_readout_time,
+                   gw_function_start_time, gw_function_end_time,
+                   gw_acq_exec_stat, pedestal_resultant_exp_time,
+                   signal_resultant_exp_time, gw_acq_number,
+                   gw_mode, gw_window_xstart, gw_window_ystart,
+                   gw_window_xstop, gw_window_ystop,
+                   gw_window_xsize, gw_window_ysize, gw_science_file_source]
+  pedestal_frames:
+    title: Guide Window Pedestal Resultant Array (DN)
+    description: |
+      Array containing the guide window pedestal resultants in units of DN. The
+      array has dimensions of (J, H, K, X, Y) where J is the number of science
+      resultants, H is the number of reads of the detector in a given science
+      resultant, K is the number of guide window reads in a science read, and X
+      and Y are the pixel locations.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: uint16
+        exact_datatype: true
+        ndim: 5
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.*
+        enum: ["DN"]
+  signal_frames:
+    title: Guide Window Signal Resultant Array (DN)
+    description: |
+      Array containing the guide window signal resultants in units of DN. The
+      array has dimensions of (J, H, K, X, Y) where J is the number of science
+      resultants, H is the number of reads of the detector in a given science
+      resultant, K is the number of guide window reads in a science read, and X
+      and Y are the pixel locations.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: uint16
+        exact_datatype: true
+        ndim: 5
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.*
+        enum: ["DN"]
+  amp33:
+    title: Guide Window Amplifier 33 Reference Pixel Resultant Array (DN)
+    description: |
+      Array containing the amplifier 33 reference pixel resultants in units of
+      DN. The array has dimensions of (J, H, K, X, Y) where J is the number of
+      science resultants, H is the number of reads of the detector in a given
+      science resultant, K is the number of guide window reads in a science
+      read, and X and Y are the pixel locations.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: uint16
+        exact_datatype: true
+        ndim: 5
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.*
+        enum: ["DN"]
+propertyOrder: [meta, pedestal_frames, signal_frames, amp33]
 flowStyle: block
-required: [id, type,
-           start_time, mid_time, end_time,
-           start_time_mjd, mid_time_mjd, end_time_mjd,
-           start_time_tdb, mid_time_tdb, end_time_tdb,
-           ngroups, nframes, data_problem, sca_number,
-           gain_factor, integration_time, elapsed_exposure_time,
-           frame_divisor, groupgap,
-           frame_time, group_time, exposure_time,
-           effective_exposure_time, duration,
-           ma_table_name, ma_table_number, level0_compressed,
-           read_pattern]
+required: [meta, pedestal_frames, signal_frames, amp33]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/guidestar-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/guidestar-1.0.0.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,297 +1,241 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/guidestar-1.0.0
 
-title: Guide star window information
-type: object
-properties:
-  gw_id:
-    title: guide star window identifier
-    type: string
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: nvarchar(20)
-      destination: [ScienceCommon.gw_id, GuideWindow.gw_id]
-  gw_fgs_mode:
-    $ref: guidewindow_modes-1.0.0
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: nvarchar(18)
-      destination: [ScienceCommon.gw_fgs_mode, GuideWindow.gw_fgs_mode]
-  gs_id:
-    title: guide star identifier from the GSC2 catalog
-    description: guide star catalog id from the GSC2, field gsc2ID
-    type: string
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: nvarchar(20)
-      destination: [ScienceCommon.gs_id, GuideWindow.gs_id]
-  gs_catalog_version:
-    title: The version of the Guide Star Catalog
-    description: The version of the catalog that the guide stars are selected, currently  "GSC 2.4.2", SDF should populate
-        this from the return value of CAT e.g. CAT=GSC242
-    type: string
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: nvarchar(20)
-      destination: [ScienceCommon.gs_catalog_version]
-  gs_ra:
-    title: "[deg] guide star right ascension"
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_ra, GuideWindow.gs_ra]
-  gs_dec:
-    title: "[deg] guide star declination"
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_dec, GuideWindow.gs_dec]
-  gs_ura:
-    title: "[deg] guide star right ascension uncertainty"
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_ura, GuideWindow.gs_ura]
-  gs_udec:
-    title: "[deg] guide star declination uncertainty"
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_udec, GuideWindow.gs_udec]
-  gs_mag:
-    title: guide star magnitude in detector
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_mag, GuideWindow.gs_mag]
-  gs_umag:
-    title: guide star magnitude uncertainty
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_umag, GuideWindow.gs_umag]
-  data_start:
-    title: MJD start time of guider data within this file
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.data_start, GuideWindow.data_start]
-  data_end:
-    title: MJD end time of guider data within this file
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.data_end, GuideWindow.data_end]
-  gs_ctd_x:
-    title: "[arcsec] guide star centroid x position in guider ideal frame"
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_ctd_x, GuideWindow.gs_ctd_x]
-  gs_ctd_y:
-    title: "[arcsec] guide star centroid y position in guider ideal frame"
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_ctd_y, GuideWindow.gs_ctd_y]
-  gs_ctd_ux:
-    title: uncertainty in the x position of the centroid
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_ctd_ux, GuideWindow.gs_ctd_ux]
-  gs_ctd_uy:
-    title: uncertainty in the y position of the centroid
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_ctd_uy, GuideWindow.gs_ctd_uy]
-  gs_epoch:
-    title: Epoch of guide star coordinates
-    type: string
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: nvarchar(10)
-      destination: [ScienceCommon.gs_epoch, GuideWindow.gs_epoch]
-  gs_mura:
-    title: "[mas/yr] Guide star ICRS right ascension proper motion"
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_mura, GuideWindow.gs_mura]
-  gs_mudec:
-    title: "[mas/yr] Guide star ICRS declination proper motion"
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_mudec, GuideWindow.gs_mudec]
-  gs_para:
-    title: Guide star annual parallax
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_para, GuideWindow.gs_para]
-  gs_pattern_error:
-    title: RMS of guide star position
-    description: RMS of guide star position in guide window from pattern matching (error on
-      centroid not explicitly calculated, the FACE information takes all the centroids and
-      calculates the error across the guiding pattern)
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_pattern_error, GuideWindow.gs_pattern_error]
-  gw_window_xstart:
-    title: Guide window x start position on the detector
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: Science Data Formatting
-    archive_catalog:
-      datatype: int
-      destination: [ScienceCommon.gw_window_xstart]
-  gw_window_ystart:
-    title: Guide window y start position on the detector
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: Science Data Formatting
-    archive_catalog:
-      datatype: int
-      destination: [ScienceCommon.gw_window_ystart]
-  gw_window_xstop:
-    title: Guide window x stop position on the detector
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: Science Data Formatting
-    archive_catalog:
-      datatype: int
-      destination: [ScienceCommon.gw_window_xstop]
-  gw_window_ystop:
-    title: Guide window y stop position on the detector
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: Science Data Formatting
-    archive_catalog:
-      datatype: int
-      destination: [ScienceCommon.gw_window_ystop]
-  gw_window_xsize:
-    title: Guide window size in the x direction in detector coordinates
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: Science Data Formatting
-    archive_catalog:
-      datatype: int
-      destination: [ScienceCommon.gw_window_xsize]
-  gw_window_ysize:
-    title: Guide window size in the y direction in detector coordinates
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: Science Data Formatting
-    archive_catalog:
-      datatype: int
-      destination: [  ScienceCommon.gw_window_ysize]
-propertyOrder: [gw_id, gs_id, gs_catalog_version, gs_ra, gs_dec,
-               gs_ura, gs_udec, gs_mag, gs_umag, gw_fgs_mode,
-               data_start, data_end, gs_ctd_x, gs_ctd_y, gs_ctd_ux, gs_ctd_uy,
-               gs_epoch, gs_mura, gs_mudec, gs_para, gs_pattern_error, gw_window_xstart,
-               gw_window_ystart, gw_window_xstop, gw_window_ystop, gw_window_xsize,
-               gw_window_ysize]
+title: Guide Star Window Information
+
+allOf:
+  - $ref: asdf://stsci.edu/datamodels/roman/schemas/base_guidestar-1.0.0
+  - type: object
+    properties:
+      gs_id:
+        title: Guide Star Identifier from Guide Star Catalog
+        description: |
+          Identification of the guide star from the guide star catalog.
+        type: string
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: nvarchar(20)
+          destination: [WFIExposure.gs_id, GuideWindow.gs_id]
+      gs_catalog_version:
+        title: Version of the Guide Star Catalog
+        description: |
+          Version identifier of the guide star catalog used for the observation.
+        type: string
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: nvarchar(20)
+          destination: [WFIExposure.gs_catalog_version]
+      gs_ra:
+        title: Guide Star Right Ascension (deg)
+        description: |
+          Right ascension of the guide star from the guide star catalog in units of
+          degrees.
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_ra, GuideWindow.gs_ra]
+      gs_dec:
+        title: Guide Star Declination (deg)
+        description: |
+          Declination of the guide star from the guide star catalog in units of
+          degrees.
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_dec, GuideWindow.gs_dec]
+      gs_ura:
+        title: Guide Star Right Ascension Uncertainty (deg)
+        description: |
+          Uncertainty in the guide star right ascension from the guide star catalog
+          in units of degrees.
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_ura, GuideWindow.gs_ura]
+      gs_udec:
+        title: Guide Star Declination Uncertainty (deg)
+        description: |
+          Uncertainty in the guide star declination from the guide star catalog in
+          units of degrees.
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_udec, GuideWindow.gs_udec]
+      gs_mag:
+        title: Guide Star Instrumental Magnitude
+        description: |
+          Predicted instrumental magnitude of the guide star from the guide star
+          catalog.
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_mag, GuideWindow.gs_mag]
+      gs_umag:
+        title: Guide Star Instrumental Magnitude Uncertainty
+        description: |
+          Uncertainty in the predicted instrumental magnitude of the guide star from
+          the guide star catalog.
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_umag, GuideWindow.gs_umag]
+      gs_ctd_x:
+        title: Guide Star Centroid X Position (arcsec)
+        description: |
+          Centroid of the guide star position longa the X axis of the guider ideal
+          frame measured in units of arcseconds.
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_ctd_x, GuideWindow.gs_ctd_x]
+      gs_ctd_y:
+        title: Guide Star Centroid Y Position (arcsec)
+        description: |
+          Centroid of the guide star position along the Y axis of the guider ideal
+          frame measured in units of arcseconds.
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_ctd_y, GuideWindow.gs_ctd_y]
+      gs_ctd_ux:
+        title: Guide Star Centroid X Position Uncertainty (arcsec)
+        description: |
+          Uncertainty in the centroid of the guide star position along the X axis of
+          the guider ideal frame measured in units of arcseconds
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_ctd_ux, GuideWindow.gs_ctd_ux]
+      gs_ctd_uy:
+        title: Guide Star Centroid Y Position Uncertainty (arcsec)
+        description: |
+          Uncertainty in the centroid of the guide star position along the Y axis of
+          the guider ideal frame measured in units of arcseconds.
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_ctd_uy, GuideWindow.gs_ctd_uy]
+      gs_epoch:
+        title: Guide Star Coordinates Epoch
+        description: |
+          Epoch of the celestial coordinates of the guide star.
+        type: string
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: nvarchar(10)
+          destination: [WFIExposure.gs_epoch, GuideWindow.gs_epoch]
+      gs_mura:
+        title: Proper Motion of the Guide Star Right Ascension (mas / yr)
+        description: |
+          Proper motion of the guide star in right ascension from the guide star
+          catalog measured in units of milli-arcseconds per year.
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_mura, GuideWindow.gs_mura]
+      gs_mudec:
+        title: Proper Motion of the Guide Star Declination (mas / yr)
+        description: |
+          Proper motion of the guide star in declination from the guide star catalog
+          measured in units of milli-arcseconds per year.
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_mudec, GuideWindow.gs_mudec]
+      gs_para:
+        title: Guide Star Annual Parallax
+        description: |
+          Annual parallax of the guide star from the guide star catalog.
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_para, GuideWindow.gs_para]
+      gs_pattern_error:
+        title: Guide Star Centroid RMS
+        description: |
+          RMS of the guide star position in the tracking guide windows from the Fine
+          Attitude Correction Estimate (FACE) information. The FACE information
+          determines the error across the guiding pattern using all centroid
+          measurements.
+        type: number
+        sdf:
+          special_processing: VALUE_REQUIRED
+          source:
+            origin: TBD
+        archive_catalog:
+          datatype: float
+          destination: [WFIExposure.gs_pattern_error, GuideWindow.gs_pattern_error]
+    propertyOrder: [gs_id, gs_catalog_version, gs_ra, gs_dec,
+                  gs_ura, gs_udec, gs_mag, gs_umag,
+                  gs_ctd_x, gs_ctd_y, gs_ctd_ux, gs_ctd_uy,
+                  gs_epoch, gs_mura, gs_mudec, gs_para, gs_pattern_error]
+    required: [gs_id, gs_catalog_version, gs_ra, gs_dec,
+              gs_ura, gs_udec, gs_mag, gs_umag,
+              gs_ctd_x, gs_ctd_y, gs_ctd_ux, gs_ctd_uy,
+              gs_epoch, gs_mura, gs_mudec, gs_para, gs_pattern_error]
+
 flowStyle: block
-required: [gw_id, gs_id, gs_catalog_version, gs_ra, gs_dec,
-           gs_ura, gs_udec, gs_mag, gs_umag, gw_fgs_mode,
-           data_start, data_end, gs_ctd_x, gs_ctd_y, gs_ctd_ux, gs_ctd_uy,
-           gs_epoch, gs_mura, gs_mudec, gs_para, gs_pattern_error, gw_window_xstart,
-           gw_window_ystart, gw_window_xstop, gw_window_ystop, gw_window_xsize,
-           gw_window_ysize]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -6,78 +6,78 @@
 title: Combined level 2 metadata
 
 type: object
 properties:
   basic:
     description: |
       Table of basic level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   aperture:
     description: |
       Table of aperture level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   cal_step:
     description: |
       Table of cal_step level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   coordinates:
     description: |
       Table of coordinates level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   ephemeris:
     description: |
       Table of ephemeris level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   exposure:
     description: |
       Table of exposure level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   guidestar:
     description: |
       Table of guidestar level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   instrument:
     description: |
       Table of instrument level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   observation:
     description: |
       Table of observation level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   photometry:
     description: |
       Table of photometry level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   pointing:
     description: |
       Table of pointing level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   program:
     description: |
       Table of program level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   ref_file:
     description: |
       Table of ref_file level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   target:
     description: |
       Table of target level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   velocity_aberration:
     description: |
       Table of velocity_aberration level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   visit:
     description: |
       Table of visit level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
   wcsinfo:
     description: |
       Table of wcsinfo level 2 metadata.
-    tag: tag:astropy.org:astropy/table/table-1.1.0
+    tag: tag:astropy.org:astropy/table/table-1.*
 flowStyle: block
 propertyOrder: [basic, aperture, cal_step, coordinates, ephemeris,
 exposure, guidestar, instrument, observation, photometry,
 pointing, program, ref_file, target, velocity_aberration,
 visit, wcsinfo]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/ephemeris-1.0.0.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,173 +1,161 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/mosaic_basic-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/ephemeris-1.0.0
 
-title: Basic mosaic metadata keywords
+title: Ephemeris Data Information
 type: object
-
 properties:
-  time_first_mjd:
-    title: Earliest component image start time in the mosaic in MJD
+  earth_angle:
+    title: Earth Angle (radians)
+    description: |
+      Earth angle in radians.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.time_first_mjd]
-  time_last_mjd:
-    title: Latest component image end time in the mosaic in MJD
+      destination: [WFIExposure.earth_angle, GuideWindow.earth_angle]
+  moon_angle:
+    title: Moon Angle (radians)
+    description: |
+      Moon angle in radians.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.time_last_mjd]
-  time_mean_mjd:
-    title: Mean of mid-times of component images in MJD
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.time_mean_mjd]
-  max_exposure_time:
-    title: Maximum component image exposure time in MJD
-    type: number
+      destination: [WFIExposure.moon_angle, GuideWindow.moon_angle]
+  ephemeris_reference_frame:
+    title: Ephemeris Reference Frame
+    description: |
+      Ephemeris reference frame.
+    type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.max_exposure_time]
-  mean_exposure_time:
-    title: Mean of component image exposure times in MJD
+      datatype: nvarchar(10)
+      destination: [WFIExposure.ephemeris_reference_frame, GuideWindow.ephemeris_reference_frame]
+  sun_angle:
+    title: Sun Angle (radians)
+    description: |
+      Sun angle in radians.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.mean_exposure_time]
-  model_type:
-    title: Type of data model
+      destination: [WFIExposure.sun_angle, GuideWindow.sun_angle]
+  type:
+    title: Type of Ephemeris
+    description: |
+      Type of ephemeris.
     type: string
+    enum: [DEFINITIVE, PREDICTED]
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: nvarchar(50)
-      destination: [ScienceCommon.model_type, GuideWindow.model_type]
-  visit:
-    title: Visit number within the observation, defined range of
-           values is 1..999; included in obs_id and visit_id as 'VVV'.
-    type: integer
+      datatype: nvarchar(10)
+      destination: [WFIExposure.ephemeris_type, GuideWindow.ephemeris_type]
+  time:
+    title: UTC Time of Position and Velocity Vectors in Ephemeris (MJD)
+    description: |
+      UTC time of position and velocity vectors in ephemeris in MJD.
+    type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
-        origin: TBD
+        origin: Roman Science Data Processing (RSDP)
     archive_catalog:
-      datatype: smallint
-      destination: [ScienceCommon.visit]
-  segment:
-    title: Segment Number within pass, defined range is 1..999;
-           included in obs_id and visit_id as 'SSS'.
-    type: integer
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: smallint
-      destination: [ScienceCommon.segment]
-  pass:
-    title: Pass number within execution plan, defined range is 1..999;
-           included in obs_id and visit_id as 'AA'.
-    type: integer
+      datatype: float
+      destination: [WFIExposure.ephemeris_time, GuideWindow.ephemeris_time]
+  spatial_x:
+    title: X Spatial Coordinate of Roman (km)
+    description: |
+      X spatial coordinate of Roman in km.
+    type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
-        origin: TBD
+        origin: Roman Science Data Processing (RSDP)
     archive_catalog:
-      datatype: smallint
-      destination: [ScienceCommon.pass]
-  program:
-    title: Program number, defined range is 1..18445;
-           included in obs_id and visit_id as 'PPPPP'.
-    type: string
+      datatype: float
+      destination: [WFIExposure.spatial_x, GuideWindow.spatial_x]
+  spatial_y:
+    title: Y Spatial Coordinate of Roman (km)
+    description: |
+      Y spatial coordinate of Roman in km.
+    type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
-        origin: TBD
+        origin: Roman Science Data Processing (RSDP)
     archive_catalog:
-      datatype: int
-      destination: [ScienceCommon.program]
-  survey:
-    title: Observation Survey
-    type: string
-    archive_catalog:
-      datatype: nvarchar(15)
-      destination: [ScienceCommon.survey]
-  optical_element:
-    $ref: wfi_optical_element-1.0.0
+      datatype: float
+      destination: [WFIExposure.spatial_y, GuideWindow.spatial_y]
+  spatial_z:
+    title: Z Spatial Coordinate of Roman (km)
+    description: |
+      Z spatial coordinate of Roman in km.
+    type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
-        origin: TBD
+        origin: Roman Science Data Processing (RSDP)
     archive_catalog:
-      datatype: nvarchar(20)
-      destination: [ScienceCommon.optical_element]
-  instrument:
-    title: Instrument used to acquire the data
-    type: string
-    enum: [WFI]
+      datatype: float
+      destination: [WFIExposure.spatial_z, GuideWindow.spatial_z]
+  velocity_x:
+    title: X Component of Roman Velocity (km / s)
+    description: |
+      X component of Roman velocity in km / s.
+    type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
-        origin: TBD
+        origin: Roman Science Data Processing (RSDP)
     archive_catalog:
-      datatype: nvarchar(5)
-      destination: [ScienceCommon.instrument_name]
-  telescope:
-    tag: asdf://stsci.edu/datamodels/roman/tags/telescope-1.0.0
-  location_name:
-    title: Name of the skycell containing the mosaic
-    type: string
+      datatype: float
+      destination: [WFIExposure.velocity_x, GuideWindow.velocity_x]
+  velocity_y:
+    title: Y Component of Roman Velocity (km / s)
+    description: |
+      Y component of Roman velocity in km / s.
+    type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
-        origin: TBD
+        origin: Roman Science Data Processing (RSDP)
     archive_catalog:
-      datatype: nvarchar(25)
-      destination: [ScienceCommon.location_name]
-  product_type:
-    title: Association product type
-    type: string
+      datatype: float
+      destination: [WFIExposure.velocity_y, GuideWindow.velocity_y]
+  velocity_z:
+    title: Z Component of Roman Velocity (km / s)
+    description: |
+      Z component of Roman velocity in km / s.
+    type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
-        origin: TBD
+        origin: Roman Science Data Processing (RSDP)
     archive_catalog:
-      datatype: nvarchar(25)
-      destination: [ScienceCommon.product_type]
-  filename:
-    tag: asdf://stsci.edu/datamodels/roman/tags/filename-1.0.0
-propertyOrder: [ time_first_mjd, time_last_mjd, time_mean_mjd, max_exposure_time,
-                 mean_exposure_time, model_type, visit, segment, pass, program,
-                 survey, optical_element, instrument, telescope, location_name, product_type,
-                 filename ]
+      datatype: float
+      destination: [WFIExposure.velocity_z, GuideWindow.velocity_z]
+propertyOrder: [earth_angle, moon_angle, sun_angle, type, time,
+                ephemeris_reference_frame, spatial_x, spatial_y,
+                spatial_z, velocity_x, velocity_y, velocity_z]
 flowStyle: block
-required: [ time_first_mjd, time_last_mjd, time_mean_mjd, max_exposure_time,
-            mean_exposure_time, model_type, visit, segment, pass, program,
-            survey, optical_element, instrument, telescope, location_name, product_type,
-            filename ]
+required: [earth_angle, moon_angle, sun_angle, type, time,
+           ephemeris_reference_frame, spatial_x, spatial_y,
+           spatial_z, velocity_x, velocity_y, velocity_z]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -12,234 +12,234 @@
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.ra_ref]
+      destination: [WFIMosaic.ra_ref]
   dec_ref:
     title: "[deg] Projection center Dec"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.dec_ref]
+      destination: [WFIMosaic.dec_ref]
   x_ref:
     title: Pixel number in mosaic corresponding to projection center ra/dec
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.x_ref]
+      destination: [WFIMosaic.x_ref]
   y_ref:
     title: Pixel number in mosaic corresponding to projection center ra/dec
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.y_ref]
+      destination: [WFIMosaic.y_ref]
   rotation_matrix:
     title: 2x2 rotation matrix
     type: array
     items:
       type: array
       items:
         type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(3500)
-      destination: [ScienceCommon.rotation_matrix]
+      destination: [WFIMosaic.rotation_matrix]
   pixel_scale:
     title: Pixel scale at projection center
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.pixel_scale]
+      destination: [WFIMosaic.pixel_scale]
   pixel_scale_local:
     title: Pixel scale at image center
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.pixel_scale_local]
+      destination: [WFIMosaic.pixel_scale_local]
   projection:
     title: Projection type and order
     type: string
     enum: ["TAN"]
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(50)
-      destination: [ScienceCommon.projection]
+      destination: [WFIMosaic.projection]
   s_region:
     title: spatial extent of the observation
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(max)
-      destination: [ScienceCommon.s_region]
+      destination: [WFIMosaic.s_region]
   pixel_shape:
     title: Shape of image (nx, ny)
     type: array
     items:
       type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(50)
-      destination: [ScienceCommon.pixel_shape]
+      destination: [WFIMosaic.pixel_shape]
   ra_center:
     title: "[deg] Mosaic center RA"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.ra_center]
+      destination: [WFIMosaic.ra_center]
   dec_center:
     title: "[deg] Mosaic center Dec"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.dec_center]
+      destination: [WFIMosaic.dec_center]
   ra_corn1:
     title: "[deg] Mosaic corner 1 RA"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.ra_corn1]
+      destination: [WFIMosaic.ra_corn1]
   dec_corn1:
     title: "[deg] Mosaic corner 1 Dec"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.dec_corn1]
+      destination: [WFIMosaic.dec_corn1]
   ra_corn2:
     title: "[deg] Mosaic corner 2 RA"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.ra_corn2]
+      destination: [WFIMosaic.ra_corn2]
   dec_corn2:
     title: "[deg] Mosaic corner 2 Dec"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.dec_corn2]
+      destination: [WFIMosaic.dec_corn2]
   ra_corn3:
     title: "[deg] Mosaic corner 3 RA"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.ra_corn3]
+      destination: [WFIMosaic.ra_corn3]
   dec_corn3:
     title: "[deg] Mosaic corner 3 Dec"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.dec_corn3]
+      destination: [WFIMosaic.dec_corn3]
   ra_corn4:
     title: "[deg] Mosaic corner 4 RA"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.ra_corn4]
+      destination: [WFIMosaic.ra_corn4]
   dec_corn4:
     title: "[deg] Mosaic corner 4 Dec"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.dec_corn4]
+      destination: [WFIMosaic.dec_corn4]
   orientat_local:
     title: Angle between north and the y axis of the projection at the mosaic
       center, turning positive in the direction of increasing right ascenscion.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.orientat_local]
+      destination: [WFIMosaic.orientat_local]
   orientat:
     title: Angle between north and the y axis of the projection at the projection
       center, turning positive in the direction of increasing right ascenscion.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.orientat]
+      destination: [WFIMosaic.orientat]
 propertyOrder: [ ra_ref, dec_ref, x_ref, y_ref, rotation_matrix, pixel_scale,
                  pixel_scale_local, projection, s_region, pixel_shape, ra_center,
                  dec_center, ra_corn1, dec_corn1, ra_corn2, dec_corn2, ra_corn3,
                  dec_corn3, ra_corn4, dec_corn4, orientat_local, orientat ]
 flowStyle: block
 required: [ ra_ref, dec_ref, x_ref, y_ref, rotation_matrix, pixel_scale,
             pixel_scale_local, projection, s_region, pixel_shape, ra_center,
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/msos_stack-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/msos_stack-1.0.0.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -12,34 +12,46 @@
 properties:
   meta:
     allOf:
       - $ref: common-1.0.0
       - image_list:
           type: string
   data:
-    title: Flux data
+    title: Flux Data
+    description: |
+      Flux array of stacked image data.
     value:
-      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+      tag: tag:stsci.edu:asdf/core/ndarray-1.*
       datatype: float64
+      exact_datatype: true
       ndim: 2
   uncertainty:
-    title: uncertainty data
+    title: Uncertainty Data
+    description: |
+      Uncertainty array of stacked image data.
     value:
-      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+      tag: tag:stsci.edu:asdf/core/ndarray-1.*
       datatype: float64
+      exact_datatype: true
       ndim: 2
   mask:
-    title: mask data
+    title: Mask Data
+    description: |
+      Mask array of stacked image data.
     value:
-      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+      tag: tag:stsci.edu:asdf/core/ndarray-1.*
       datatype: uint8
+      exact_datatype: true
       ndim: 2
   coverage:
-    title: coverage data
+    title: Coverage Data
+    description: |
+      Coverage array of stacked image data.
     value:
-      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+      tag: tag:stsci.edu:asdf/core/ndarray-1.*
       datatype: uint8
+      exact_datatype: true
       ndim: 2
 propertyOrder: [meta, data, uncertainty, mask, coverage]
 flowStyle: block
 required: [meta, data, uncertainty, mask, coverage]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/observation-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/observation-1.0.0.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,179 +1,215 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/observation-1.0.0
 
-title: Observation identifiers
+title: Observation Identifiers
 type: object
 properties:
   obs_id:
-    title: Programmatic observation identifier. The format is 'PPPPPCCAAASSSOOOVVVggsaaeeee' where
-           'PPPPP' is the Program, 'CC' is the execution plan, 'AAA' is the pass, 'SSS' is the
-           segment, 'OOO' is the Observation, 'VVV' is the Visit, 'gg' is the visit file group,
-           's' is the visit file sequence, 'aa' is the visit file activity, and 'eeee' is the
-           exposure ID. The observation ID is the complete concatenation of visit_id +
-           visit_file_statement (visit_file_group + visit_file_sequence + visit_file_activity) +
-           exposure.
+    title: Programmatic Observation Identifier
+    description: |
+      The format of the programmatic observation identifier is
+      'PPPPPCCAAASSSOOOVVVggsaaeeee' where 'PPPPP' is the program, 'CC' is the
+      execution plan, 'AAA' is the pass, 'SSS' is the segment number, 'OOO' is
+      the observation, 'VVV' is the visit, 'gg' is the visit file group, 's' is
+      the visit file sequence, 'aa' is the visit file activity, and 'eeee' is
+      the exposure ID. The observation ID is the complete concatenation of
+      visit_id + visit_file_statement (visit_file_group + visit_file_sequence +
+      visit_file_activity) + exposure.
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(28)
-      destination: [ScienceCommon.obs_id, GuideWindow.obs_id]
+      destination: [WFIExposure.obs_id, GuideWindow.obs_id]
   visit_id:
-    title: A unique identifier for a visit. The format is 'PPPPPCCAAASSSOOOVVV' where 'PPPPP' is the
-           Program, 'CC' is the execution plan, 'AAA' is the pass, 'SSS' is the segment number,
-           'OOO' is the Observation and 'VVV' is the Visit.
+    title: Visit Identifier
+    description: |
+      A unique identifier for a visit. The format is 'PPPPPCCAAASSSOOOVVV' where
+      'PPPPP' is the program, 'CC' is the execution plan, 'AAA' is the pass,
+      'SSS' is the segment number, 'OOO' is the observation and 'VVV' is the
+      visit.
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(19)
-      destination: [ScienceCommon.visit_id, GuideWindow.visit_id]
+      destination: [WFIExposure.visit_id, GuideWindow.visit_id]
   program:
-    title: Program number, defined range is 1..18445; included in obs_id and visit_id as 'PPPPP'.
+    title: Program Number
+    description: |
+      The defined range of the program number is 00001 to 18445; included in
+      obs_id and visit_id as 'PPPPP'.
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [ScienceCommon.program, GuideWindow.program]
+      destination: [WFIExposure.program, GuideWindow.program]
   execution_plan:
-    title: Execution plan within the program, defined range is 1..99; included in obs_id and
-           visit_id as 'CC'.
+    title: Execution Plan
+    description: |
+      The defined range of the execution plan within the program is 01 to 99;
+      included in obs_id and visit_id as 'CC'.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: smallint
-      destination: [ScienceCommon.execution_plan, GuideWindow.execution_plan]
+      destination: [WFIExposure.execution_plan, GuideWindow.execution_plan]
   pass:
-    title: Pass number within execution plan, defined range is 1..999; included in obs_id and
-           visit_id as 'AA'.
+    title: Pass Number
+    description: |
+      The defined range of the pass number within the execution plan is 001 to
+      999; included in obs_id and visit_id as 'AAA'.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: smallint
-      destination: [ScienceCommon.pass, GuideWindow.pass]
+      destination: [WFIExposure.pass, GuideWindow.pass]
   segment:
-    title: Segment Number within pass, defined range is 1..999; included in obs_id and visit_id as
-           'SSS'.
+    title: Segment Number
+    description: |
+      The defined range of the segment number within the pass is 001 to 999;
+      included in obs_id and visit_id as 'SSS'.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: smallint
-      destination: [ScienceCommon.segment, GuideWindow.segment]
+      destination: [WFIExposure.segment, GuideWindow.segment]
   observation:
-    title: Observation number within the segment, defined range is 1..999; included in obs_id and
-           visit_id as 'OOO'.
+    title: Observation Number
+    description: |
+      The defined range of the observation number within the segment is 001 to
+      999; included in obs_id and visit_id as 'OOO'.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: smallint
-      destination: [ScienceCommon.observation, GuideWindow.observation]
+      destination: [WFIExposure.observation, GuideWindow.observation]
   visit:
-    title: Visit number within the observation, defined range of values is 1..999; included in
-           obs_id and visit_id as 'VVV'.
+    title: Visit Number
+    description: |
+      The defined range of the visit number within the observation is 001 to
+      999; included in obs_id and visit_id as 'VVV'.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: smallint
-      destination: [ScienceCommon.visit, GuideWindow.visit]
+      destination: [WFIExposure.visit, GuideWindow.visit]
   visit_file_group:
-    title: Sequence group within the visit file, defined range of values is 1..99; included in
-           obs_id as 'gg'.
+    title: Visit File Group
+    description: |
+      The visit file group describes the sequence group within the visit file
+      and has a defined range of 01 to 99; included in obs_id as 'gg'.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: smallint
-      destination: [ScienceCommon.visit_file_group, GuideWindow.visit_file_group]
+      destination: [WFIExposure.visit_file_group, GuideWindow.visit_file_group]
   visit_file_sequence:
-    title: Visit file sequence within the group, defined range of values is 1..5; included in
-           obs_id as 's'.
+    title: Visit File Sequence
+    description: |
+      The defined range of the visit file sequence within the group 1 to 5;
+      included in obs_id as 's'.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: tinyint
-      destination: [ScienceCommon.visit_file_sequence, GuideWindow.visit_file_sequence]
+      destination: [WFIExposure.visit_file_sequence, GuideWindow.visit_file_sequence]
   visit_file_activity:
-    title: Visit file activity within the sequence, defined range of values is 1..ZZ; included in
-           obs_id as 'aa'.
+    title: Visit File Activity
+    description: |
+      The defined range of the visit file activity within the sequence is 01 to
+      ZZ; included in obs_id as 'aa'.
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(2)
-      destination: [ScienceCommon.visit_file_activity, GuideWindow.visit_file_activity]
+      destination: [WFIExposure.visit_file_activity, GuideWindow.visit_file_activity]
   exposure:
-    title: Exposure within the visit, defined range of values is 1..9999; included in obs_id as
-           'eeee'.
+    title: Exposure Number
+    description: |
+      The defined range of the assigned exposure number within the visit is 0001
+      to 9999; included in obs_id as 'eeee'.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [ScienceCommon.observation_exposure, GuideWindow.observation_exposure]
+      destination: [WFIExposure.observation_exposure, GuideWindow.observation_exposure]
   template:
-    title: Observation template used
+    title: Observation Template
+    description: |
+      The template used to design this observation.
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_visit.template
     archive_catalog:
       datatype: nvarchar(50)
-      destination: [ScienceCommon.template, GuideWindow.template]
+      destination: [WFIExposure.template, GuideWindow.template]
   observation_label:
-    title: Proposer label for the observation
+    title: Observation Label
+    description: |
+      The label given by the proposer to describe the observation.
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(max)
-      destination: [ScienceCommon.observation_label, GuideWindow.observation_label]
+      destination: [WFIExposure.observation_label, GuideWindow.observation_label]
   survey:
     title: Observation Survey
+    description: |
+      The available survey options for observations are: HLS = High Latitude
+      Wide Area Survey, EMS = Galactic Bulge Time Domain Survey, SN = High
+      Latitude Time Domain Survey, N/A = General Astrophysics Surveys or other
+      survey not otherwise defined here.
     type: string
     enum: [HLS, EMS, SN, N/A]
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceCommon.survey, GuideWindow.survey]
+      destination: [WFIExposure.survey, GuideWindow.survey]
 propertyOrder: [obs_id, visit_id, program,
            execution_plan, pass, observation, segment,
            visit, visit_file_group, visit_file_sequence,
            visit_file_activity, exposure, template,
            observation_label, survey]
 flowStyle: block
 required: [obs_id, visit_id, program,
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/photometry-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/photometry-1.0.0.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,119 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/photometry-1.0.0
 
-title: Photometry information
+title: Photometry Information
 type: object
 properties:
   conversion_megajanskys:
-    title: Flux density (MJy/steradian) producing 1 cps
+    title: Flux Density Producing 1 count per second (MJy / steradian)
+    description: |
+      The conversion from DN / s to MJy / steradian.
     anyOf:
-      - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+      - tag: tag:stsci.edu:asdf/unit/quantity-1.*
         properties:
           datatype:
             enum: ["float64"]
           unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+            tag: tag:stsci.edu:asdf/unit/unit-1.*
             enum: ["MJy.sr**-1"]
       - type: "null"
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.conversion_megajanskys]
+      destination: [WFIExposure.conversion_megajanskys, WFIMosaic.conversion_megajanskys,
+                    SourceCatalog.conversion_megajanskys]
   conversion_microjanskys:
-    title: Flux density (uJy/arcsec2) producing 1 cps
+    title: Flux Density Producing 1 count per second (uJy / arcsec2)
+    description: |
+      The conversion from DN / s to uJy / steradian.
     anyOf:
-      - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+      - tag: tag:stsci.edu:asdf/unit/quantity-1.*
         properties:
           datatype:
             enum: ["float64"]
           unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+            tag: tag:stsci.edu:asdf/unit/unit-1.*
             enum: ["uJy.arcsec**-2"]
       - type: "null"
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.conversion_microjanskys]
+      destination: [WFIExposure.conversion_microjanskys, WFIMosaic.conversion_microjanskys,
+                    SourceCatalog.conversion_microjanskys]
   pixelarea_steradians:
-    title: Nominal pixel area in steradians
+    title: Nominal Pixel Area (steradians)
+    description: |
+      The average pixel area in units of steradians.
     anyOf:
-      - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+      - tag: tag:stsci.edu:asdf/unit/quantity-1.*
         properties:
           datatype:
             enum: ["float64"]
           unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+            tag: tag:stsci.edu:asdf/unit/unit-1.*
             enum: ["sr"]
       - type: "null"
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.pixelarea_steradians]
+      destination: [WFIExposure.pixelarea_steradians, WFIMosaic.pixelarea_steradians,
+                    SourceCatalog.pixelarea_steradians]
   pixelarea_arcsecsq:
-    title: Nominal pixel area in arcsec^2
+    title: Nominal Pixel Area (arcsec^2)
+    description: |
+      The average pixel area in units of square arcseconds.
     anyOf:
-      - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+      - tag: tag:stsci.edu:asdf/unit/quantity-1.*
         properties:
           datatype:
             enum: ["float64"]
           unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+            tag: tag:stsci.edu:asdf/unit/unit-1.*
             enum: ["arcsec**2"]
       - type: "null"
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.pixelarea_arcsecsq]
+      destination: [WFIExposure.pixelarea_arcsecsq, WFIMosaic.pixelarea_arcsecsq,
+                    SourceCatalog.pixelarea_arcsecsq]
   conversion_megajanskys_uncertainty:
-    title: Uncertainty in flux density conversion to MJy/steradians
+    title: Uncertainty in Flux Density Conversion (from DN / s to MJy / steradians)
+    description: |
+      The uncertainty in the flux density conversion from DN to MJy /steradians
+      in units of MJy / steradians.
     anyOf:
-      - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+      - tag: tag:stsci.edu:asdf/unit/quantity-1.*
         properties:
           datatype:
             enum: ["float64"]
           unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+            tag: tag:stsci.edu:asdf/unit/unit-1.*
             enum: ["MJy.sr**-1"]
       - type: "null"
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.conversion_megajanskys_uncertainty]
+      destination: [WFIExposure.conversion_megajanskys_uncertainty, WFIMosaic.conversion_megajanskys_uncertainty,
+                    SourceCatalog.conversion_megajanskys_uncertainty]
   conversion_microjanskys_uncertainty:
-    title: Uncertainty in flux density conversion to uJy/arcsec2
+    title: Uncertainty in Flux Density Conversion (from DN / s to uJy / arcsec^2)
+    description: |
+      The uncertainty in the flux density conversion from DN / s to
+      uJy /arcsec^2.
     anyOf:
-      - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+      - tag: tag:stsci.edu:asdf/unit/quantity-1.*
         properties:
           datatype:
             enum: ["float64"]
           unit:
-            tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+            tag: tag:stsci.edu:asdf/unit/unit-1.*
             enum: ["uJy.arcsec**-2"]
       - type: "null"
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.conversion_microjanskys_uncertainty]
+      destination: [WFIExposure.conversion_microjanskys_uncertainty, WFIMosaic.conversion_microjanskys_uncertainty,
+                    SourceCatalog.conversion_microjanskys_uncertainty]
 propertyOrder: [conversion_microjanskys, conversion_megajanskys,
                 pixelarea_steradians, pixelarea_arcsecsq,
                 conversion_megajanskys_uncertainty, conversion_microjanskys_uncertainty]
 flowStyle: block
 required: [conversion_microjanskys, conversion_megajanskys,
            pixelarea_steradians, pixelarea_arcsecsq,
            conversion_megajanskys_uncertainty, conversion_microjanskys_uncertainty]
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/rad_schema-1.0.0.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,75 +1,80 @@
 %YAML 1.1
 ---
 $schema: http://stsci.edu/schemas/yaml-schema/draft-01
 id: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 
-title: Roman Attribute Dictionary metaschema
-description: |-
-  A metaschema extending the ASDF metaschema to add support for
-  sdf and archive_catalog properties.
+title: RAD Metaschema
+description: |
+  A metaschema that extends the ASDF metaschema to add support for Science
+  Data Formatting and archive catalog-related properties.
 
 allOf:
   - $ref: http://stsci.edu/schemas/asdf/asdf-schema-1.0.0
   - type: object
     properties:
       datamodel_name:
+        title: Datamodel Name
         description: |-
-          The name of the datamodel that this schema describes.
+          Name of the datamodel described by this schema
         type: string
-
       archive_meta:
+        title: Archive Metadata
         description: |-
-          Metadata to aide the archive in determining how to handle
-          a given file.
+          Metadata that aids the archive in identifying ASDF files.
         type: string
-
       sdf:
+        title: Scientific Data Format
         description: |-
-          Documents source of this attribute's value when level 1
-          files are created.
+          Information on this attribute's value upon creation of Level 1 files.
         type: object
         properties:
           special_processing:
+            title: Special Processing
             description: |-
-              Indicates whether attribute is required to be present
-              in the ASDF file or optional.
+              A flag indicating whether this attribute must be present in the
+              SDF file.
             type: string
             enum: [VALUE_REQUIRED, OPTIONAL]
           source:
             type: object
             properties:
               origin:
+                title: Origin
                 description: |-
                   Source of the attribute value.
                 type: string
               function:
+                title: Function
                 description: |-
                   Optional function that transforms the source value.
                 type: string
             required: [origin]
         required: [special_processing, source]
 
       archive_catalog:
+        title: Archive Catalog
         description: |-
-          Documents destination table/column and datatype of this attribute
-          in the archive catalog.
+          Information on this attribute's data type and destination table and
+          column in the archive catalog.
         type: object
         properties:
           datatype:
+            title: Archive Catalog Database Column Type
             description: |-
-              Archive catalog database column type.
+              Column type in the archive catalog database.
             anyOf:
               - type: string
                 enum: [datetime2, float, int, nchar(1), nvarchar(max), bigint, smallint, tinyint]
               - type: string
                 pattern: "^nvarchar\\([0-9]+\\)$"
           destination:
+            title: Destination
             description: |-
-              Archive catalog database table and column.
+              Table and column in the archive catalog database
             type: array
             items:
               type: string
               pattern: "^[A-Za-z0-9]+\\.[a-z0-9_]+$"
             minItems: 1
             uniqueItems: true
         required: [datatype, destination]
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/ramp-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/tvac-1.0.0.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,130 +1,119 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/ramp-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/tvac-1.0.0
 
-title: Ramp schema
+title: |
+  Schema for the TVAC Test Data
 
-datamodel_name: RampModel
+datamodel_name: TvacModel
+
+archive_meta: None
 
 type: object
 properties:
   meta:
-    $ref: common-1.0.0
+    allOf:
+      - $ref: asdf://stsci.edu/datamodels/roman/schemas/ground_common-1.0.0
+      - type: object
+        properties:
+          groundtest:
+            tag: asdf://stsci.edu/datamodels/roman/tags/tvac_groundtest-1.0.0
+        required: [groundtest]
+
   data:
     title: Science data, including the border reference pixels.
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: uint16
+        exact_datatype: true
         ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["DN", "electron"]
-  pixeldq:
-    title: 2-D data quality array for all planes
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    ndim: 2
-    datatype: uint32
-  groupdq:
-    title: 3-D data quality array (plane dq for each group)
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    ndim: 3
-    datatype: uint8
-  err:
-    title: Error array containing the square root of the exposure-level combined variance
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+        tag: tag:astropy.org:astropy/units/unit-1.*
+        enum: ["DN"]
+
+  amp33:
+    title: Amp 33 reference pixel data.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: uint16
+        exact_datatype: true
         ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["DN", "electron"]
-  amp33:
-    title: Amp 33 reference pixel data
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+        tag: tag:astropy.org:astropy/units/unit-1.*
+        enum: ["DN"]
+
+  amp33_reset_reads:
+    title: Amp 33 reset reads performed before integration data.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: uint16
+        exact_datatype: true
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.*
+        enum: ["DN"]
+
+  amp33_reference_read:
+    title: Amp 33 reference reads that can be subtracted from the amp33 ramp data, if present.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: uint16
+        exact_datatype: true
         ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.*
         enum: ["DN"]
-  border_ref_pix_left:
-    title: Original border reference pixels, on left (from viewers perspective).
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    value:
-      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-      datatype: float32
-      ndim: 3
-    unit:
-      tag: tag:astropy.org:astropy/units/unit-1.0.0
-      enum: ["DN"]
-  border_ref_pix_right:
-    title: Original border reference pixels, on right (from viewers perspective).
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+
+  guidewindow:
+    title: Guide window data.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: uint16
+        exact_datatype: true
         ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.*
         enum: ["DN"]
-  border_ref_pix_top:
-    title: Original border reference pixels, on top.
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+
+  reference_read:
+    title: Reference read that can be subtracted from ramp, if present.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: uint16
+        exact_datatype: true
         ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.*
         enum: ["DN"]
-  border_ref_pix_bottom:
-    title: Original border reference pixels, on bottom.
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+
+  reset_reads:
+    title: Reset reads performed before the ramp integration, if present.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: uint16
+        exact_datatype: true
         ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.*
         enum: ["DN"]
-  dq_border_ref_pix_left:
-    title: DQ for border reference pixels, on left (from viewers perspective).
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: uint32
-    ndim: 2
-  dq_border_ref_pix_right:
-    title: DQ for border reference pixels, on right (from viewers perspective).
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: uint32
-    ndim: 2
-  dq_border_ref_pix_top:
-    title: DQ for border reference pixels, on top.
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: uint32
-    ndim: 2
-  dq_border_ref_pix_bottom:
-    title: DQ for border reference pixels, on bottom.
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: uint32
-    ndim: 2
-propertyOrder: [meta, data, pixeldq, groupdq, err, amp33, border_ref_pix_left,
-                border_ref_pix_right, border_ref_pix_top,
-                border_ref_pix_bottom, dq_border_ref_pix_left,
-                dq_border_ref_pix_right, dq_border_ref_pix_top,
-                dq_border_ref_pix_bottom]
+
+propertyOrder: [meta, data, amp33, amp33_reset_reads, amp33_reference_read,
+                guidewindow, reference_read, reset_reads]
 flowStyle: block
-required: [meta, data, pixeldq, groupdq, err, amp33, border_ref_pix_left,
-           border_ref_pix_right, border_ref_pix_top, border_ref_pix_bottom,
-           dq_border_ref_pix_left, dq_border_ref_pix_right,
-           dq_border_ref_pix_top, dq_border_ref_pix_bottom]
+required: [meta, data, amp33, guidewindow]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,112 +1,112 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/ramp_fit_output-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/dark-1.0.0
 
-title: Ramp fit output schema
+title: Dark Reference File Schema
 
-datamodel_name: RampFitOutputModel
+datamodel_name: DarkRefModel
 
 type: object
 properties:
   meta:
-    $ref: common-1.0.0
-  slope:
-    title: Segment-specific slope
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    allOf:
+      - $ref: ref_common-1.0.0
+      - type: object
+        properties:
+          reftype:
+            type: string
+            enum: [DARK]
+          exposure:
+            type: object
+            properties:
+              ngroups:
+                title: Number of Resultants
+                description: |
+                  The number of resultants averaged according to
+                  Multi-Accumulation (MA) Table read pattern.
+                type: integer
+              nframes:
+                title: Number of frames per resultant # should be removed
+                type: integer
+              groupgap:
+                title: Number of Skips Between Resultants
+                description: |
+                  The number of frames skipped between resultants according to
+                  MA Table read pattern.
+                type: integer
+              ma_table_name:
+                title: Multi-Accumulation Table Name
+                description: |
+                  The name of the MA Table used. Not a unique identifier; see
+                  ma_table_number.
+                type: string
+              ma_table_number:
+                title: Multi-Accumulation Table Number
+                description: |
+                  The unique number of the MA Table used. A modification to a MA
+                  Table that keeps the same name will have a new
+                  ma_table_number.
+                type: integer
+            required: [ngroups, nframes, groupgap, ma_table_name, ma_table_number]
+        required: [exposure]
+      - $ref: ref_exposure_type-1.0.0
+      - $ref: ref_optical_element-1.0.0
+  data:
+    title: Dark Current Array
+    description: |
+      The dark current array represents the integrated number of counts due to
+      the accumulation of dark current electrons in the pixels.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: float32
+        exact_datatype: true
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.*
+        enum: ["DN"]
+  dq:
+    title: 2-D Data Quality Array
+    description: |
+      The 2-D data quality array for the Dark Current Array.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
+    datatype: uint32
+    exact_datatype: true
+    ndim: 2
+  dark_slope:
+    title: Dark Current Rate Array
+    description: |
+      The dark current rate array represents the slope of the integrated number
+      of counts due to the accumulation of dark current electrons in the pixels
+      calculated from slope fitting the Dark Current Array.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
-        ndim: 3
-      unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron / s"]
-  sigslope:
-    title: Sigma for segment-specific slope
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
-        ndim: 3
-      unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron / s"]
-  yint:
-    title: Segment-specific y-intercept
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
-        ndim: 3
-      unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron"]
-  sigyint:
-    title: Sigma for segment-specific y-intercept
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
-        ndim: 3
-      unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron"]
-  pedestal:
-    title: Pedestal array
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: float32
+        exact_datatype: true
         ndim: 2
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron"]
-  weights:
-    title: Weights for segment-specific fits
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    ndim: 3
-    datatype: float32
-  crmag:
-    title: Approximate CR magnitudes
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
-        ndim: 3
-      unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron"]
-  var_poisson:
-    title: Variance due to poisson noise for segment-specific slope
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
-        ndim: 3
-      unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron2 / s2"]
-  var_rnoise:
-    title: Variance due to read noise for segment-specific slope
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+        tag: tag:astropy.org:astropy/units/unit-1.*
+        enum: ["DN / s"]
+  dark_slope_error:
+    title: Dark Current Rate Uncertainty Array
+    description: |
+      The uncertainty calculated from the slope fitting of the Dark Current
+      Array.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: float32
-        ndim: 3
+        exact_datatype: true
+        ndim: 2
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron2 / s2"]
-required: [meta, slope, sigslope, yint, sigyint, pedestal, weights, crmag, var_poisson,
-           var_rnoise]
-propertyOrder: [meta, slope, sigslope, yint, sigyint, pedestal, weights, crmag, var_poisson,
-                var_rnoise]
+        tag: tag:astropy.org:astropy/units/unit-1.*
+        enum: ["DN / s"]
+required: [meta, data, dq, dark_slope, dark_slope_error]
 flowStyle: block
+propertyOrder: [meta, data, dq, dark_slope, dark_slope_error]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,56 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/dark-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/wfi_science_raw-1.0.0
 
-title: Dark reference schema
+title: Level 1 WFI Imaging and Spectrographic Science Data
 
-datamodel_name: DarkRefModel
+datamodel_name: ScienceRawModel
+
+archive_meta: None
 
 type: object
 properties:
   meta:
-    allOf:
-      - $ref: ref_common-1.0.0
-      - type: object
-        properties:
-          reftype:
-            type: string
-            enum: [DARK]
-          exposure:
-            type: object
-            properties:
-              ngroups:
-                title: Number of groups in integration
-                type: integer
-              nframes:
-                title: Number of frames per group
-                type: integer
-              groupgap:
-                title: Number of frames dropped between groups
-                type: integer
-              ma_table_name:
-                title: Identifier for the multi-accumulation table used
-                type: string
-              ma_table_number:
-                title: Number of the multi-accumulation table used
-                type: integer
-            required: [ngroups, nframes, groupgap, ma_table_name, ma_table_number]
-        required: [exposure]
-      - $ref: ref_exposure_type-1.0.0
-      - $ref: ref_optical_element-1.0.0
+    $ref: common-1.0.0
   data:
-    title: Dark current array
+    title: Science Data (DN)
     description: |
-       The dark current array represents the integrated number of counts
-       due to the accumulation of dark current electrons in the pixels.
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+      Science data, including reference pixels in units of DN
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: uint16
+        exact_datatype: true
         ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.*
         enum: ["DN"]
-  dq:
-    title: 2-D data quality array for all planes
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: uint32
-    ndim: 2
-  dark_slope:
-    title: Dark current slope array
+  amp33:
+    title: Amplifier 33 Reference Pixel Data (DN)
     description: |
-       The dark current slope array represents the slope of the
-       integrated number of counts due to the accumulation of dark
-       current electrons in the pixels for slope fitting purposes.
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
-        ndim: 2
-      unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["DN / s"]
-  dark_slope_error:
-    title: Uncertainty in dark current slope array
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+      Reference pixel data from amplifier 33 in units of DN.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
-        ndim: 2
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: uint16
+        exact_datatype: true
+        ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["DN / s"]
-required: [meta, data, dq, dark_slope, dark_slope_error]
+        tag: tag:astropy.org:astropy/units/unit-1.*
+        enum: ["DN"]
+
+  resultantdq:
+    title: Resultant Data Quality Array
+    description: |
+      An optional, 3-D data quality array, with plane DQ for each resultant.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
+    ndim: 3
+    datatype: uint8
+    exact_datatype: true
+propertyOrder: [meta, data, amp33, resultantdq]
 flowStyle: block
-propertyOrder: [meta, data, dq, dark_slope, dark_slope_error]
+required: [meta, data, amp33]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/distortion-1.0.0
 
-title: Distortion reference schema
+title: Distortion Reference Schema
 
 datamodel_name: DistortionRefModel
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
             enum: [DISTORTION]
           input_units:
-            title: Units of the detector coordinate inputs to this model.
-            tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+            title: Input Model Units
+            description: |
+              The pixel input units of the detector coordinate model.
+            tag: tag:stsci.edu:asdf/unit/unit-1.*
             enum: ["pixel"]
           output_units:
-            title: Output units of V2/V3 coordinates after the model is applied.
-            tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+            title: Output Model Units
+            description: |
+              The V2/V3 coordinates output units after the model is applied.
+            tag: tag:stsci.edu:asdf/unit/unit-1.*
             enum: ["arcsec"]
         required: [output_units, input_units]
       - $ref: ref_optical_element-1.0.0
   coordinate_distortion_transform:
-    title: Distortion transform as an instance of astropy.modeling.Model.
+    title: Distortion Transform Model
+    description: |
+      The astropy.modeling.Model instance of of the distortion transform model.
     type: object
 required: [meta, coordinate_distortion_transform]
 flowStyle: block
 propertyOrder: [meta, coordinate_distortion_transform]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/segmentation_map-1.0.0.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/flat-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/segmentation_map-1.0.0
 
-title: Flat reference schema
+title: Segmentation map generated from a Level 2 file by the Source Catalog Step.
 
-datamodel_name: FlatRefModel
+datamodel_name: SegmentationMapModel
 
+archive_meta: None
 type: object
 properties:
   meta:
     allOf:
-      - $ref: ref_common-1.0.0
+      - $ref: basic-1.0.0
       - type: object
         properties:
-          reftype:
-            type: string
-            enum: [FLAT]
-      - $ref: ref_optical_element-1.0.0
+          optical_element:
+            title: WFI Optical Element
+            description: |
+              WFI optical element used to take the data.
+            $ref: wfi_optical_element-1.0.0
+          program:
+            title: Program Information
+            tag: asdf://stsci.edu/datamodels/roman/tags/program-1.0.0
+          visit:
+            title: Visit Information
+            tag: asdf://stsci.edu/datamodels/roman/tags/visit-1.0.0
+        required: [optical_element, program, visit]
   data:
-    title: Flat data array
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: float32
+    title: Segmentation map
+    description: |
+       Segmentation map of an image model, zeros correspond to background.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     ndim: 2
-  dq:
-    title: Data quality array
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
     datatype: uint32
-    ndim: 2
-  err:
-    title: Error array
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: float32
-    ndim: 2
-required: [meta, data, dq, err]
+    exact_datatype: true
+
+required: [meta, data]
 flowStyle: block
-propertyOrder: [meta, data, dq, err]
+propertyOrder: [meta, data]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/inverselinearity-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/refpix-1.0.0
 
-title: Inverse linearity correction reference schema
+title: Reference Pixel Correction Reference Schema
 
-datamodel_name: InverselinearityRefModel
+# NOTE: this needs titles and descriptions added.
+
+datamodel_name: RefpixRefModel
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
-            enum: [INVERSELINEARITY]
+            enum: [REFPIX]
           input_units:
-            title: Units of the input to the inverse linearity polynomial.
-            tag: tag:astropy.org:astropy/units/unit-1.0.0
+            title: Units of the input to the linearity polynomial.
+            tag: tag:astropy.org:astropy/units/unit-1.*
             enum: ["DN"]
           output_units:
-            title: Units of the output of the inverse linearity polynomial.
-            tag: tag:astropy.org:astropy/units/unit-1.0.0
+            title: Units of the output of the linearity polynomial.
+            tag: tag:astropy.org:astropy/units/unit-1.*
             enum: ["DN"]
         required: [output_units, input_units]
-  coeffs:
-    title: Inverse linearity coefficients
-    description: |
-      Contains the coefficients of a polynomial to add classic non-linearity
-      to pixels. Both the input to and output from the polynomial are in units
-      of DN. The coefficients have units that contain various powers of DN.
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: float32
-    # Dimensions: numcoeffs, ysize, xsize
-    ndim: 3
-  dq:
-    title: 2-D data quality array for all planes
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: uint32
+
+  gamma:
+    title: Left column correction coefficients
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
+    datatype: complex128
+    exact_datatype: true
+    ndim: 2
+
+  zeta:
+    title: Right column correction coefficients
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
+    datatype: complex128
+    exact_datatype: true
     ndim: 2
-required: [meta, coeffs, dq]
+
+  alpha:
+    title: Reference output correction coefficients
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
+    datatype: complex128
+    exact_datatype: true
+    ndim: 2
+
+required: [meta, gamma, zeta, alpha]
 flowStyle: block
-propertyOrder: [meta, coeffs, dq]
+propertyOrder: [meta, gamma, zeta, alpha]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/ipc-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/readnoise-1.0.0
 
-title: IPC kernel reference schema
+title: Read Noise Reference File Schema
 
-datamodel_name: IpcRefModel
+datamodel_name: ReadnoiseRefModel
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
-      - $ref: ref_optical_element-1.0.0
       - type: object
         properties:
           reftype:
-            type: string
-            enum: [IPC]
+            enum: [READNOISE]
+      - $ref: ref_exposure_type-1.0.0
   data:
-    title: Interpixel capacitance correction kernel array
+    title: Read Noise Data Array
     description: |
-      Reference kernel used for convolving with data in order to correct
-      for interpixel capacitance
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: float32
-    ndim: 2
+      The pixel-by-pixel map read noise data array is used in estimating the
+      expected noise in each pixel.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
+        datatype: float32
+        exact_datatype: true
+        ndim: 2
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.*
+        enum: ["DN"]
 required: [meta, data]
 flowStyle: block
 propertyOrder: [meta, data]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/linearity-1.0.0
 
-title: Linearity correction  reference schema
+title: Linearity Correction Reference Schema
 
 datamodel_name: LinearityRefModel
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
             enum: [LINEARITY]
           input_units:
-            title: Units of the input to the linearity polynomial.
-            tag: tag:astropy.org:astropy/units/unit-1.0.0
+            title: Units of the Input to the Linearity Polynomial
+            description: |
+              Units of the input to the linearity polynomial.
+            tag: tag:astropy.org:astropy/units/unit-1.*
             enum: ["DN"]
           output_units:
-            title: Units of the output of the linearity polynomial.
-            tag: tag:astropy.org:astropy/units/unit-1.0.0
+            title: Units of the Output of the Linearity Polynomial
+            description: |
+              Units of the output to the linearity polynomial.
+            tag: tag:astropy.org:astropy/units/unit-1.*
             enum: ["DN"]
         required: [output_units, input_units]
   coeffs:
-    title: Linearity coefficients
+    title: Linearity Coefficients
     description: |
-      Contains the coefficients of a polynomial to correct pixel
-      values for classic non-linearity. Both the input to and
-      output from the polynomial are in units of DN. The coefficients
-      have units that contain various powers of DN.
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+      Contains the coefficients of a polynomial to correct the non-linear
+      response of each pixel to a linear signal. Both the input to and output
+      from the polynomial are in units of DN. The coefficients have units that
+      contain various powers of DN.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: float32
+    exact_datatype: true
     # Dimensions: numcoeffs, ysize, xsize
     ndim: 3
   dq:
-    title: 2-D data quality array for all planes
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    title: Two Dimensional Data Quality Array for All Resultants
+    description: |
+      Two Dimensional data Quality Array for all Resultants
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: uint32
+    exact_datatype: true
     ndim: 2
 required: [meta, coeffs, dq]
 flowStyle: block
 propertyOrder: [meta, coeffs, dq]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/mask-1.0.0
 
-title: DQ Mask reference schema
+title: Mask Reference File Schema
 
 datamodel_name: MaskRefModel
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
             enum: [MASK]
   dq:
-    title: Data quality mask array
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    title: Mask Data Quality Array
+    description: |
+      The Mask Data Quality Array is the pixel value of the sum of bit integer
+      dq flags.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: uint32
+    exact_datatype: true
     ndim: 2
 required: [meta, dq]
 flowStyle: block
 propertyOrder: [meta, dq]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/pixelarea-1.0.0
 
-title: Pixel area reference schema
+title: Pixel Area Reference Schema
 
 datamodel_name: PixelareaRefModel
 
 type: object
 properties:
   meta:
     allOf:
@@ -17,40 +17,47 @@
           reftype:
             type: string
             enum: [AREA]
           photometry:
             type: object
             properties:
               pixelarea_steradians:
-                title: Nominal pixel area in steradians
+                title: Pixel Area (steradians)
+                description: |
+                  The nominal pixel area in steradians.
                 anyOf:
-                  - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+                  - tag: tag:stsci.edu:asdf/unit/quantity-1.*
                     properties:
                       datatype:
                         enum: ["float64"]
                       unit:
-                        tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+                        tag: tag:stsci.edu:asdf/unit/unit-1.*
                         enum: ["sr"]
                   - type: "null"
               pixelarea_arcsecsq:
-                title: Nominal pixel area in arcsec^2
+                title: Pixel Area (arcsec^2)
+                description:
+                  The nominal pixel area in arcec^2.
                 anyOf:
-                  - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+                  - tag: tag:stsci.edu:asdf/unit/quantity-1.*
                     properties:
                       datatype:
                         enum: ["float64"]
                       unit:
-                        tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+                        tag: tag:stsci.edu:asdf/unit/unit-1.*
                         enum: ["arcsec**2"]
                   - type: "null"
             required: [pixelarea_steradians, pixelarea_arcsecsq]
         required: [photometry]
       - $ref: ref_optical_element-1.0.0
   data:
-    title: Pixel area array
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    title: Pixel Area Array
+    description: |
+      Pixel area in units of of either arcseconds or steradians.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: float32
+    exact_datatype: true
     ndim: 2
 required: [meta, data]
 flowStyle: block
 propertyOrder: [meta, data]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/ref_exposure_type-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/ipc-1.0.0
 
-title: Type of data in the reference file exposure (viewing mode)
+title: Interpixel Capacitance Reference File Schema
+
+datamodel_name: IpcRefModel
 
 type: object
 properties:
-  exposure:
-    type: object
-    properties:
-      type:
-          $ref: ../exposure_type-1.0.0
-      p_exptype:
-        title: Applicable exposure type.
-        type: string
-        pattern: "^((WFI_IMAGE|WFI_GRISM|WFI_PRISM|WFI_DARK|WFI_FLAT|WFI_WFSC)\\s*\\|\\s*)+$"
-    required: [type,p_exptype]
-required: [exposure]
+  meta:
+    allOf:
+      - $ref: ref_common-1.0.0
+      - $ref: ref_optical_element-1.0.0
+      - type: object
+        properties:
+          reftype:
+            type: string
+            enum: [IPC]
+  data:
+    title: Interpixel Capacitance Kernel Array
+    description: |
+      The kernel array used for convolving data to correct for interpixel
+      capacitance of neighboring pixels.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
+    datatype: float32
+    exact_datatype: true
+    ndim: 2
+required: [meta, data]
+flowStyle: block
+propertyOrder: [meta, data]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/saturation-1.0.0
 
-title: Saturation reference schema
+title: Saturation Reference File Schema
 
 datamodel_name: SaturationRefModel
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
             enum: [SATURATION]
   data:
-    title: Saturation threshold
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    title: Saturation Threshold Array
+    description: |
+      The pixel level threshold for determining saturation before non-linearity
+      corrections are applied.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: float32
+        exact_datatype: true
         ndim: 2
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.*
         enum: ["DN"]
   dq:
-    title: 2-D data quality array for all planes
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    title: 2-D Data Quality Array
+    description: |
+      The 2-D data quality array for the Saturation Threshold Array.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: uint32
+    exact_datatype: true
     ndim: 2
 required: [meta, data, dq]
 flowStyle: block
 propertyOrder: [meta, data, dq]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/superbias-1.0.0
 
-title: Super-bias reference schema
+title: Super-Bias Reference Schema
 
 datamodel_name: SuperbiasRefModel
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
             enum: [BIAS]
   data:
-    title: 2-D super-bias array
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    title: Two Dimensional Bias Array
+    description: |
+      Two Dimensional Bias Array.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: float32
+    exact_datatype: true
     ndim: 2
   dq:
+    title: Two Dimensional Quality Array for all Resultants
+    description: |
+      Two Dimensional Quality Array for all Resultants.
     title: 2-D data quality array for all planes
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: uint32
+    exact_datatype: true
     ndim: 2
   err:
-    title: 2-D Error array
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    title: Two Dimensional Error Array
+    description: |
+      Two Dimensional Error Array.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: float32
+    exact_datatype: true
     ndim: 2
 required: [meta, data, dq, err]
 flowStyle: block
 propertyOrder: [meta, data, dq, err]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,73 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/wfi_img_photom-1.0.0
 
-title: WFI imaging photometric flux conversion data model
+title: WFI Imaging Photometric Flux Conversion Data Model
 
 datamodel_name: WfiImgPhotomRefModel
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
             enum: [PHOTOM]
   phot_table:
-    title: Photometric flux conversion factors table
+    title: Photometric Flux Conversion Factors Table
+    description: |
+      Table containing photometric flux conversion factors to physical units of
+      MJy / steradian.
     type: object
     patternProperties:
       "^(F062|F087|F106|F129|F146|F158|F184|F213|GRISM|PRISM|DARK)$":
         type: object
         properties:
           photmjsr:
-            title: Surface brightness, in MJy/steradian
+            title: Surface Brightness
+            description: |
+              Surface brightness, in MJy / steradian.
             anyOf:
-              - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+              - tag: tag:stsci.edu:asdf/unit/quantity-1.*
                 properties:
                   value:
                     type: number
                   unit:
-                    tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+                    tag: tag:stsci.edu:asdf/unit/unit-1.*
                     enum: [MJy.sr**-1]
               - type: "null"
           uncertainty:
-            title: Uncertainty of surface brightness, in MJy/steradian
+            title: Surface Brightness Uncertainty
+            description: |
+              Uncertainty of surface brightness, in MJy / steradian.
             anyOf:
-              - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+              - tag: tag:stsci.edu:asdf/unit/quantity-1.*
                 properties:
                   value:
                     type: number
                   unit:
-                    tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+                    tag: tag:stsci.edu:asdf/unit/unit-1.*
                     enum: [MJy.sr**-1]
               - type: "null"
           pixelareasr:
-            title: Nominal pixel area, in steradian
+            title: Pixel Area
+            description: |
+              The nominal pixel area, in steradian.
             anyOf:
-              - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+              - tag: tag:stsci.edu:asdf/unit/quantity-1.*
                 properties:
                   value:
                     type: number
                   unit:
-                    tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+                    tag: tag:stsci.edu:asdf/unit/unit-1.*
                     enum: [sr]
               - type: "null"
         required: [photmjsr, uncertainty, pixelareasr]
     additionalProperties: false
 required: [meta, phot_table]
 flowStyle: block
 propertyOrder: [meta, phot_table]
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/velocity_aberration-1.0.0
 
-title: Velocity aberration correction information
+title: Velocity Aberration Correction Information
 type: object
 properties:
   ra_offset:
-    title: Velocity aberration right ascension offset
+    title: Velocity Aberration RA Offset (degree)
+    description: |
+      Right ascension offset for velocity aberration in degrees.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.ra_offset, GuideWindow.ra_offset]
+      destination: [WFIExposure.ra_offset, GuideWindow.ra_offset]
   dec_offset:
-    title: Velocity aberration declination offset
+    title: Velocity Aberration Dec Offset (degree)
+    description: |
+      Declination offset for velocity aberration in degrees.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.dec_offset, GuideWindow.dec_offset]
+      destination: [WFIExposure.dec_offset, GuideWindow.dec_offset]
   scale_factor:
-    title: Velocity aberration scale factor
+    title: Velocity Aberration Scale Factor
+    description: |
+      Velocity aberration scale factor.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.scale_factor, GuideWindow.scale_factor]
+      destination: [WFIExposure.scale_factor, GuideWindow.scale_factor]
 flowStyle: block
 propertyOrder: [ra_offset, dec_offset, scale_factor]
 required: [ra_offset, dec_offset, scale_factor]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/visit-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/wcsinfo-1.0.0.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,106 +1,116 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/visit-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/wcsinfo-1.0.0
 
-title: Visit information
+title: World Coordinate System (WCS) Parameters
 type: object
 properties:
-  engineering_quality:
-    title: Engineering data quality indicator from EngDB
-    type: string
-    enum: [OK, SUSPECT]
+  v2_ref:
+    title: Reference Position V2 Coordinate (arcsec)
+    description: |
+      Coordinate of the reference position along the telescope V2 axis in units
+      of arcseconds.
+    type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: nvarchar(10)
-      destination: [ScienceCommon.engineering_quality, GuideWindow.engineering_quality]
-  pointing_engdb_quality:
-    title: Quality of pointing information from EngDB
-    type: string
-    enum: [CALCULATED, PLANNED]
+      datatype: float
+      destination: [WFIExposure.v2_ref, GuideWindow.v2_ref]
+  v3_ref:
+    title: Reference Position V3 Coordinate (arcsec)
+    description: |
+      Coordinate of the reference position along the telescope V3 axis in units
+      of arcseconds.
+    type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: nvarchar(10)
-      destination: [ScienceCommon.pointing_engdb_quality, GuideWindow.pointing_engdb_quality]
-  type:
-    title: Visit type
-    type: string
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: PSS:dms_visit.visit_type
-    archive_catalog:
-      datatype: nvarchar(30)
-      destination: [ScienceCommon.visit_type, GuideWindow.visit_type]
-  start_time:
-    title: UTC visit start time
-    tag: tag:stsci.edu:asdf/time/time-1.1.0
+      datatype: float
+      destination: [WFIExposure.v3_ref, GuideWindow.v3_ref]
+  vparity:
+    title: Relative Rotation Between Ideal and Telescope Axes
+    description: |
+      Relative sense of rotation between the ideal and telescope coordinate
+      systems. The value may be either 1 or -1. See documents STScI-JWST-001550
+      and STScI-Roman-000143 for more information.
+    type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: datetime2
-      destination: [ScienceCommon.visit_start_time, GuideWindow.visit_start_time]
-  end_time:
-    title: UTC visit end time
-    tag: tag:stsci.edu:asdf/time/time-1.1.0
+      datatype: int
+      destination: [WFIExposure.vparity, GuideWindow.vparity]
+  v3yangle:
+    title: Angle Between the V3 and Ideal Y Axes (deg)
+    description: |
+      Angle between the telescope V3 axis and the ideal coordinate frame y-axis
+      in units of degrees.
+    type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: datetime2
-      destination: [ScienceCommon.visit_end_time, GuideWindow.visit_end_time]
-  status:
-    title: Status of a visit
-    type: string
+      datatype: float
+      destination: [WFIExposure.v3yangle, GuideWindow.v3yangle]
+  ra_ref:
+    title: Right Ascension of the Reference Position (deg)
+    description: |
+      Right ascension of the reference position on the sky in units of degrees.
+    type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: nvarchar(15)
-      destination: [ScienceCommon.visit_status, GuideWindow.visit_status]
-  total_exposures:
-    title: Total number of planned exposures in visit
-    type: integer
+      datatype: float
+      destination: [WFIExposure.ra_ref, GuideWindow.ra_ref]
+  dec_ref:
+    title: Declination of the Reference Position (deg)
+    description: |
+      Declination of the reference position on the sky in units of degrees.
+    type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: int
-      destination: [ScienceCommon.visit_total_exposures, GuideWindow.visit_total_exposures]
-  internal_target:
-    title: At least one exposure in visit is internal
-    type: boolean
+      datatype: float
+      destination: [WFIExposure.dec_ref, GuideWindow.dec_ref]
+  roll_ref:
+    title: V3 Position Angle at the Reference Position
+    description: |
+      Position angle of the V3 axis at the reference position measured from
+      North to East.
+    type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: nchar(1)
-      destination: [ScienceCommon.visit_internal_target, GuideWindow.visit_internal_target]
-  target_of_opportunity:
-    title: Visit scheduled as target of opportunity
-    type: boolean
+      datatype: float
+      destination: [WFIExposure.roll_ref, GuideWindow.roll_ref]
+  s_region:
+    title: Spatial Extent of the Observation
+    description: |
+      The region of the sky enclosed by the observation footprint. This is given
+      as a polygon stored as a string with the vertices defined by a list of
+      right ascension and declination pairs in units of degrees.
+    type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: nchar(1)
-      destination: [ScienceCommon.target_of_opportunity, GuideWindow.target_of_opportunity]
-propertyOrder: [engineering_quality, pointing_engdb_quality, type,
-           start_time, end_time, status, total_exposures, internal_target, target_of_opportunity]
+      datatype: nvarchar(max)
+      destination: [WFIExposure.s_region, GuideWindow.s_region]
+propertyOrder: [v2_ref, v3_ref, vparity, v3yangle, ra_ref, dec_ref, roll_ref, s_region]
 flowStyle: block
-required: [engineering_quality, pointing_engdb_quality, type,
-           start_time, end_time, status, total_exposures, internal_target, target_of_opportunity]
+required: [v2_ref, v3_ref, vparity, v3yangle, ra_ref, dec_ref, roll_ref, s_region]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/ramp-1.0.0.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,172 +1,174 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/wfi_image-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/ramp-1.0.0
 
-title: |
-  The schema for WFI Level 2 images.
+title: Ramp Schema
 
-datamodel_name: ImageModel
-archive_meta: None
+datamodel_name: RampModel
 
 type: object
 properties:
   meta:
-    allOf:
-      - $ref: common-1.0.0
-      - type: object
-        properties:
-          wcs:
-            title: WCS object
-            anyOf:
-              - tag: tag:stsci.edu:gwcs/wcs-*
-              - type: "null"
-          photometry:
-            tag: asdf://stsci.edu/datamodels/roman/tags/photometry-1.0.0
-          source_detection:
-            tag: asdf://stsci.edu/datamodels/roman/tags/source_detection-1.0.0
-        required: [photometry, wcs]
+    $ref: common-1.0.0
   data:
-    title: Science data, excluding border reference pixels.
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    title: Science Data Including Border Reference Pixels (DN, electrons)
+    description: |
+      Science Data Including Border Reference Pixels in units of DN or
+      electrons.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: float32
-        ndim: 2
+        exact_datatype: true
+        ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron / s"]
-  dq:
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: uint32
+        tag: tag:astropy.org:astropy/units/unit-1.*
+        enum: ["DN", "electron"]
+  pixeldq:
+    title: Two Dimensional Data Quality Flags Array for Each Pixel
+    description: |
+      Two dimensional data quality flags array applying to all resultants in a
+      given pixel.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     ndim: 2
+    datatype: uint32
+    exact_datatype: true
+  groupdq:
+    title: Three-dimensional Data Quality Array For Each Resultant in Each Pixel
+    description: |
+      Three-dimensional data quality array indicating quality of each individual
+      resultant for each pixel.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
+    ndim: 3
+    datatype: uint8
+    exact_datatype: true
   err:
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
-        ndim: 2
-      unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron / s"]
-  var_poisson:
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
-        ndim: 2
-      unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron2 / s2"]
-  var_rnoise:
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    title: Error Array Containing the Square Root of the Exposure-level Combined Variance (DN, electrons)
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: float32
-        ndim: 2
-      unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron2 / s2"]
-  var_flat:
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
-        ndim: 2
+        exact_datatype: true
+        ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron2 / s2"]
+        tag: tag:astropy.org:astropy/units/unit-1.*
+        enum: ["DN", "electron"]
   amp33:
-    title: Amp 33 reference pixel data
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    title: Amp 33 Reference Pixel Data (DN)
+    description: |
+      Amplifier 33 Reference Pixel Data in units of DN.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: uint16
+        exact_datatype: true
         ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.*
         enum: ["DN"]
   border_ref_pix_left:
-    title: Original border reference pixels, on left (from viewers perspective).
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
-        ndim: 3
-      unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["DN"]
+    title: Border Reference Pixels on the Left of the Detector, from the Instrument's Perspective (DN)
+    description: |
+      Border Reference Pixels on the Left of the Detector, from the instrument's
+      perspective in units of DN.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
+    value:
+      tag: tag:stsci.edu:asdf/core/ndarray-1.*
+      datatype: float32
+      exact_datatype: true
+      ndim: 3
+    unit:
+      tag: tag:astropy.org:astropy/units/unit-1.*
+      enum: ["DN"]
   border_ref_pix_right:
-    title: Original border reference pixels, on right (from viewers perspective).
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    title: Border Reference Pixels on the Right of the Detector, from the Instrument's Perspective (DN)
+    description: |
+      Border Reference Pixels on the Right of the Detector, from the
+      instrument's perspective in units of DN.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: float32
+        exact_datatype: true
         ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.*
         enum: ["DN"]
   border_ref_pix_top:
-    title: Original border reference pixels, on top.
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    title: Border Reference Pixels on the Top of the Detector (DN)
+    description: |
+      Border Reference Pixels on the Top of the Detector in units of DN.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: float32
+        exact_datatype: true
         ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.*
         enum: ["DN"]
   border_ref_pix_bottom:
-    title: Original border reference pixels, on bottom.
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    title: Border Reference Pixels on the Bottom of the Detector (DN)
+    description: |
+      Border Reference Pixels on the Bottom of the Detector in units of DN.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: float32
+        exact_datatype: true
         ndim: 3
       unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.*
         enum: ["DN"]
   dq_border_ref_pix_left:
-    title: DQ for border reference pixels, on left (from viewers perspective).
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    title: Data Quality Flag for Border Reference Pixels, on the Left Edge of the Detector from the Instrument Perspective
+    description: |
+      Data Quality Flag for Border Reference Pixels, on the Left Edge of the
+      Detector from the Instrument Perspective.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: uint32
+    exact_datatype: true
     ndim: 2
   dq_border_ref_pix_right:
-    title: DQ for border reference pixels, on right (from viewers perspective).
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    title: Data Quality Flag for Border Reference Pixels, on the Right Edge of the Detector from the Instrument Perspective
+    description: |
+      Data Quality Flag for Border Reference Pixels, on the Right Edge of the
+      Detector from the Instrument Perspective.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: uint32
+    exact_datatype: true
     ndim: 2
   dq_border_ref_pix_top:
-    title: DQ for border reference pixels, on top.
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    title: Data Quality Flag for Border Reference Pixels, on Top.
+    description: |
+      Data Quality Flag for Border Reference Pixels, on Top.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: uint32
+    exact_datatype: true
     ndim: 2
   dq_border_ref_pix_bottom:
-    title: DQ for border reference pixels, on bottom.
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    title: Data Quality Flag for Border Reference Pixels, on Bottom.
+    description: |
+      Data Quality Flag for Border Reference Pixels, on Bottom.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: uint32
+    exact_datatype: true
     ndim: 2
-  cal_logs:
-    tag: asdf://stsci.edu/datamodels/roman/tags/cal_logs-1.0.0
-propertyOrder: [meta, data, dq, err, var_poisson, var_rnoise, var_flat,
-                amp33, border_ref_pix_left, border_ref_pix_right,
-                border_ref_pix_top, border_ref_pix_bottom,
-                dq_border_ref_pix_left, dq_border_ref_pix_right,
-                dq_border_ref_pix_top, dq_border_ref_pix_bottom, cal_logs]
+propertyOrder: [meta, data, pixeldq, groupdq, err, amp33, border_ref_pix_left,
+                border_ref_pix_right, border_ref_pix_top,
+                border_ref_pix_bottom, dq_border_ref_pix_left,
+                dq_border_ref_pix_right, dq_border_ref_pix_top,
+                dq_border_ref_pix_bottom]
 flowStyle: block
-required: [meta, data, dq, err, var_poisson, var_rnoise, amp33,
-           border_ref_pix_left, border_ref_pix_right, border_ref_pix_top,
-           border_ref_pix_bottom, dq_border_ref_pix_left,
-           dq_border_ref_pix_right, dq_border_ref_pix_top,
-           dq_border_ref_pix_bottom, cal_logs]
+required: [meta, data, pixeldq, groupdq, err, amp33, border_ref_pix_left,
+           border_ref_pix_right, border_ref_pix_top, border_ref_pix_bottom,
+           dq_border_ref_pix_left, dq_border_ref_pix_right,
+           dq_border_ref_pix_top, dq_border_ref_pix_bottom]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/wfi_mode-1.0.0.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/wfi_mode-1.0.0
 
 
-title: |
-  WFI observing configuration
+title: WFI Observing Configuration
 type: object
 properties:
   name:
-    title: Instrument used to acquire the data
+    title: Instrument Used to Acquire the Data
+    description: |
+      Instrument used to acquire the data.
     type: string
     enum: [WFI]
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(5)
-      destination: [ScienceCommon.instrument_name, GuideWindow.instrument_name]
+      destination: [WFIExposure.instrument_name, GuideWindow.instrument_name, WFICommon.instrument_name]
   detector:
+    title: WFI Detector
+    description: |
+      WFI detector used to take the data.
     $ref: wfi_detector-1.0.0
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(10)
-      destination: [ScienceCommon.detector, GuideWindow.detector]
+      destination: [WFIExposure.detector, GuideWindow.detector, WFICommon.detector]
   optical_element:
+    title: WFI Optical Element
+    description: |
+      WFI optical element used to take the data.
     $ref: wfi_optical_element-1.0.0
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(20)
-      destination: [ScienceCommon.optical_element, GuideWindow.optical_element]
+      destination: [WFIExposure.optical_element, GuideWindow.optical_element, WFICommon.optical_element]
 propertyOrder: [detector, optical_element, name]
 flowStyle: block
 required: [detector, optical_element, name]
 ...
```

### Comparing `rad-0.19.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml` & `rad-0.19.1/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 datamodel_name: MosaicModel
 archive_meta: None
 
 type: object
 properties:
   meta:
     allOf:
+      - $ref: basic-1.0.0
       - type: object
         properties:
           # Placeholder for 'dither' schema tag
           asn:
             tag: asdf://stsci.edu/datamodels/roman/tags/mosaic_associations-1.0.0
           basic:
             tag: asdf://stsci.edu/datamodels/roman/tags/mosaic_basic-1.0.0
           cal_step:
-            tag: asdf://stsci.edu/datamodels/roman/tags/cal_step-1.0.0
+            tag: asdf://stsci.edu/datamodels/roman/tags/l3_cal_step-1.0.0
           coordinates:
             tag: asdf://stsci.edu/datamodels/roman/tags/coordinates-1.0.0
           individual_image_meta:
             tag: asdf://stsci.edu/datamodels/roman/tags/individual_image_meta-1.0.0
           photometry:
             tag: asdf://stsci.edu/datamodels/roman/tags/photometry-1.0.0
           program:
@@ -39,71 +40,87 @@
             anyOf:
               - tag: tag:stsci.edu:gwcs/wcs-*
               - type: "null"
           wcsinfo:
             tag: asdf://stsci.edu/datamodels/roman/tags/mosaic_wcsinfo-1.0.0
         required: [asn, basic, cal_step, photometry, program, resample, wcs, wcsinfo]
   data:
-    title: Science data, excluding border reference pixels.
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    title: Science Data (MJy / steradian)
+    description: |
+      The science data array, excluding the border reference pixels in units of
+      MJy / steradian.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: float32
+        exact_datatype: true
         ndim: 2
       unit:
-        tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
         enum: ["MJy.sr**-1"]
   err:
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    title: Error Data (MJy / steradian)
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: float32
+        exact_datatype: true
         ndim: 2
       unit:
-        tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
         enum: ["MJy.sr**-1"]
   context:
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    title: Context Data
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: uint32
+    exact_datatype: true
     ndim: 3
   weight:
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    title: Weight Data
+    tag: tag:stsci.edu:asdf/core/ndarray-1.*
     datatype: float32
+    exact_datatype: true
     ndim: 2
   var_poisson:
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    title: Poisson Variability (MJy^2 / steradian^2)
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: float32
+        exact_datatype: true
         ndim: 2
       unit:
-        tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
         enum: ["MJy**2.sr**-2"]
   var_rnoise:
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    title: Read Noise Variance (MJy^2 / steradian^2
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: float32
+        exact_datatype: true
         ndim: 2
       unit:
-        tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
         enum: ["MJy**2.sr**-2"]
   var_flat:
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    title: Flat Field Variance (MJy^2 / steradian^2)
+    tag: tag:stsci.edu:asdf/unit/quantity-1.*
     properties:
       value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        tag: tag:stsci.edu:asdf/core/ndarray-1.*
         datatype: float32
+        exact_datatype: true
         ndim: 2
       unit:
-        tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+        tag: tag:stsci.edu:asdf/unit/unit-1.*
         enum: ["MJy**2.sr**-2"]
   cal_logs:
     tag: asdf://stsci.edu/datamodels/roman/tags/cal_logs-1.0.0
 propertyOrder: [meta, data, context, err, weight, var_poisson, var_rnoise, var_flat,
                 cal_logs]
 flowStyle: block
 required: [meta, data, context, err, weight, var_poisson, var_rnoise, var_flat,
```

### Comparing `rad-0.19.0/src/rad.egg-info/PKG-INFO` & `rad-0.19.1/src/rad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.19.0
+Version: 0.19.1
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -34,32 +34,32 @@
         
 Project-URL: Bug Tracker, https://github.com/spacetelescope/rad/issues
 Project-URL: Source Code, https://github.com/spacetelescope/rad
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asdf>=2.14.2
 Requires-Dist: asdf-astropy>=0.5.0
 Provides-Extra: test
 Requires-Dist: pytest>=4.6.0; extra == "test"
 Requires-Dist: pytest-doctestplus>=0.11.1; extra == "test"
 Requires-Dist: crds>=11.16.16; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-asdf>=0.1.3; extra == "docs"
 Requires-Dist: sphinx-astropy; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: astropy>=5.0.4; extra == "docs"
 Requires-Dist: graphviz; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
 Requires-Dist: docutils; extra == "docs"
-Requires-Dist: stsci-rtd-theme; extra == "docs"
 Requires-Dist: tomli; python_version < "3.11" and extra == "docs"
 Requires-Dist: importlib-metadata; extra == "docs"
 
 # Roman Attribute Dictionary
 
 [![CI](https://github.com/spacetelescope/rad/actions/workflows/ci.yml/badge.svg)](https://github.com/spacetelescope/rad/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/rad/badge/?version=latest)](https://rad.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `rad-0.19.0/src/rad.egg-info/SOURCES.txt` & `rad-0.19.1/src/rad.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 .github/workflows/ci.yml
 .github/workflows/ci_cron.yml
 .github/workflows/release.yml
 docs/Makefile
 docs/changes.rst
 docs/conf.py
 docs/contributing.rst
+docs/creating.rst
 docs/index.rst
 docs/make.bat
 docs/manifests.rst
 docs/reference_files.rst
 docs/schemas.rst
 docs/_static/custom.css
 docs/_static/stsci_logo.png
@@ -42,41 +43,54 @@
 src/rad.egg-info/entry_points.txt
 src/rad.egg-info/requires.txt
 src/rad.egg-info/top_level.txt
 src/rad/resources/__init__.py
 src/rad/resources/manifests/datamodels-1.0.yaml
 src/rad/resources/schemas/aperture-1.0.0.yaml
 src/rad/resources/schemas/associations-1.0.0.yaml
+src/rad/resources/schemas/base_exposure-1.0.0.yaml
+src/rad/resources/schemas/base_guidestar-1.0.0.yaml
 src/rad/resources/schemas/basic-1.0.0.yaml
 src/rad/resources/schemas/cal_logs-1.0.0.yaml
-src/rad/resources/schemas/cal_step-1.0.0.yaml
 src/rad/resources/schemas/common-1.0.0.yaml
 src/rad/resources/schemas/coordinates-1.0.0.yaml
 src/rad/resources/schemas/ephemeris-1.0.0.yaml
 src/rad/resources/schemas/exposure-1.0.0.yaml
 src/rad/resources/schemas/exposure_type-1.0.0.yaml
+src/rad/resources/schemas/fps-1.0.0.yaml
+src/rad/resources/schemas/ground_common-1.0.0.yaml
+src/rad/resources/schemas/groundtest-1.0.0.yaml
 src/rad/resources/schemas/guidestar-1.0.0.yaml
 src/rad/resources/schemas/guidewindow-1.0.0.yaml
 src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
 src/rad/resources/schemas/individual_image_meta-1.0.0.yaml
+src/rad/resources/schemas/l2_cal_step-1.0.0.yaml
+src/rad/resources/schemas/l3_cal_step-1.0.0.yaml
 src/rad/resources/schemas/mosaic_associations-1.0.0.yaml
 src/rad/resources/schemas/mosaic_basic-1.0.0.yaml
+src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml
+src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml
 src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml
 src/rad/resources/schemas/msos_stack-1.0.0.yaml
 src/rad/resources/schemas/observation-1.0.0.yaml
+src/rad/resources/schemas/outlier_detection-1.0.0.yaml
 src/rad/resources/schemas/photometry-1.0.0.yaml
 src/rad/resources/schemas/pointing-1.0.0.yaml
 src/rad/resources/schemas/program-1.0.0.yaml
 src/rad/resources/schemas/rad_schema-1.0.0.yaml
 src/rad/resources/schemas/ramp-1.0.0.yaml
 src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
 src/rad/resources/schemas/ref_file-1.0.0.yaml
 src/rad/resources/schemas/resample-1.0.0.yaml
+src/rad/resources/schemas/segmentation_map-1.0.0.yaml
+src/rad/resources/schemas/source_catalog-1.0.0.yaml
 src/rad/resources/schemas/source_detection-1.0.0.yaml
 src/rad/resources/schemas/target-1.0.0.yaml
+src/rad/resources/schemas/tvac-1.0.0.yaml
+src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml
 src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
 src/rad/resources/schemas/visit-1.0.0.yaml
 src/rad/resources/schemas/wcsinfo-1.0.0.yaml
 src/rad/resources/schemas/wfi_detector-1.0.0.yaml
 src/rad/resources/schemas/wfi_image-1.0.0.yaml
 src/rad/resources/schemas/wfi_mode-1.0.0.yaml
 src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
```

### Comparing `rad-0.19.0/tests/test_integration.py` & `rad-0.19.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/tests/test_manifest.py` & `rad-0.19.1/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.0/tests/test_schemas.py` & `rad-0.19.1/tests/test_schemas.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,23 +43,20 @@
 
 
 @pytest.fixture(scope="session")
 def valid_tag_uris(manifest):
     uris = {t["tag_uri"] for t in manifest["tags"]}
     uris.update(
         [
-            "tag:stsci.edu:asdf/time/time-1.1.0",
-            "tag:stsci.edu:asdf/core/ndarray-1.0.0",
-            "tag:stsci.edu:asdf/unit/quantity-1.1.0",
-            "tag:stsci.edu:asdf/unit/unit-1.0.0",
-            "tag:astropy.org:astropy/units/unit-1.0.0",
-            "tag:astropy.org:astropy/table/table-1.1.0",
-            "tag:stsci.edu:gwcs/wcs-1.0.0",
-            "tag:stsci.edu:gwcs/wcs-1.1.0",
-            "tag:stsci.edu:gwcs/wcs-1.2.0",
+            "tag:stsci.edu:asdf/time/time-1.*",
+            "tag:stsci.edu:asdf/core/ndarray-1.*",
+            "tag:stsci.edu:asdf/unit/quantity-1.*",
+            "tag:stsci.edu:asdf/unit/unit-1.*",
+            "tag:astropy.org:astropy/units/unit-1.*",
+            "tag:astropy.org:astropy/table/table-1.*",
             "tag:stsci.edu:gwcs/wcs-*",
         ]
     )
     return uris
 
 
 def test_required_properties(schema):
@@ -175,24 +172,67 @@
         ]["patternProperties"]
     )
     r = re.compile(phot_table_keys[0])
     for element_str in WFI_OPTICAL_ELEMENTS:
         assert r.search(element_str)
 
 
-# Confirm that the p_keyword version of exposure type match the enum version
 def test_matched_p_exptype_entries():
+    """Confirm that the p_keyword version of exposure type match the enum version."""
     p_exptype = asdf.schema.load_schema("asdf://stsci.edu/datamodels/roman/schemas/reference_files/ref_exposure_type-1.0.0")[
         "properties"
     ]["exposure"]["properties"]["p_exptype"]["pattern"]
     r = re.compile(p_exptype)
     for element_str in EXPOSURE_TYPE_ELEMENTS:
         assert r.search(element_str + "|")
 
 
+def _find_ndarrays(key, schema):
+    """
+    Find all the ndarray entries in the schema
+    """
+    entries = []
+    if isinstance(schema, dict):
+        for new_key, value in schema.items():
+            if isinstance(value, str) and value.startswith("tag:stsci.edu:asdf/core/ndarray-"):
+                entries.append((key,))
+            else:
+                entries.extend((key, *key_) for key_ in _find_ndarrays(new_key, value))
+    elif isinstance(schema, list):
+        for index, value in enumerate(schema):
+            entries.extend((key, *key_) for key_ in _find_ndarrays(index, value))
+
+    return entries
+
+
+def _get_ndarray_entry(schema, entry):
+    """
+    Get the ndarray portion of the schema for the entry
+    """
+    current = schema
+
+    for key in entry[1:]:
+        current = current[key]
+
+    return current
+
+
+def test_exact_datatype(schema):
+    """Confirm that `exact_datatype` is defined for all arrays"""
+    entries = _find_ndarrays("", schema)
+
+    if entries:
+        for entry in entries:
+            if "datatype" in (ndarray_entry := _get_ndarray_entry(schema, entry)):
+                assert "exact_datatype" in ndarray_entry, f"extact_datatype needed for {'.'.join(entry[1:])}"
+                assert ndarray_entry["exact_datatype"] is True
+            else:
+                raise ValueError(f"datatype not found for {'.'.join(entry[1:])}")
+
+
 def _get_reftype(schema):
     """
     Extract the reftype from the schema
     """
     all_of = schema["properties"]["meta"]["allOf"]
 
     for sub_schema in all_of:
```

### Comparing `rad-0.19.0/tox.ini` & `rad-0.19.1/tox.ini`

 * *Files identical despite different names*

