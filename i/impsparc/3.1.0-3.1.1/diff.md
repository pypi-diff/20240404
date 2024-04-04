# Comparing `tmp/impsparc-3.1.0.tar.gz` & `tmp/impsparc-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impsparc-3.1.0.tar", last modified: Tue Apr  2 09:02:32 2024, max compression
+gzip compressed data, was "impsparc-3.1.1.tar", last modified: Thu Apr  4 10:32:59 2024, max compression
```

## Comparing `impsparc-3.1.0.tar` & `impsparc-3.1.1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.139594 impsparc-3.1.0/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1064 2023-11-16 11:18:05.000000 impsparc-3.1.0/LICENSE.md
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      244 2023-11-16 18:00:04.000000 impsparc-3.1.0/MANIFEST.in
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1230 2024-04-02 09:02:32.139278 impsparc-3.1.0/PKG-INFO
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      871 2023-11-16 11:18:05.000000 impsparc-3.1.0/README.md
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.027418 impsparc-3.1.0/cvsvc_apirisk/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 11:18:05.000000 impsparc-3.1.0/cvsvc_apirisk/__init__.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.033474 impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   363678 2023-11-16 11:18:05.000000 impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   262350 2023-11-16 11:18:05.000000 impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      615 2023-11-16 11:18:05.000000 impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      753 2023-11-16 11:18:05.000000 impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    23616 2023-11-16 11:18:05.000000 impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16394 2023-11-16 11:18:05.000000 impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16378 2023-11-16 11:18:05.000000 impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.034778 impsparc-3.1.0/cvsvc_apirisk/score/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 11:18:05.000000 impsparc-3.1.0/cvsvc_apirisk/score/__init__.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2891 2023-11-16 11:18:05.000000 impsparc-3.1.0/cvsvc_apirisk/score/base.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.062978 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/__init__.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)       80 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    18914 2024-04-02 08:59:19.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1503 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.071148 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2433 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2453 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2662 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2684 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2697 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2117 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2387 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2385 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2393 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2391 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2722 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2731 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.075878 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2346 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2474 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2477 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2459 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2462 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2760 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3371 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/json_line.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    26665 2024-03-11 08:57:07.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/rules_util.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     8837 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/s-origin.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.083635 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2084 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2418 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2339 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2867 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2292 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2163 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     5141 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2685 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2635 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2479 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2769 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     6786 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sp2_reporting.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.084379 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.023733 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.123973 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.126556 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    15291 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16918 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    15192 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    28781 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11370 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1363 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11350 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11421 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      966 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.134749 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      423 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16193 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      209 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3581 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3478 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3944 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      309 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      406 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     6482 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     9574 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1212 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    88994 2023-11-16 18:00:53.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.086066 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.021102 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.089182 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   207965 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      687 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      756 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2033 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.091624 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    59219 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   195090 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     4023 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    71478 2023-11-16 11:18:05.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/index_raw.html
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    56178 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.114179 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   100782 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   163872 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    80388 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11245 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      393 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11230 2023-11-16 11:18:05.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/reports.css
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.120691 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   181852 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   105536 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    60520 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    23940 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   388460 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   154228 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    10556 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     4960 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    32011 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc_html_generation.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    18967 2024-03-14 06:25:43.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/spec_parse.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     6207 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/spec_util.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     5478 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sps_common.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3194 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sps_main.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    26214 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sps_main_cr.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    12521 2023-11-16 17:30:59.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sps_spec_util.py
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1193 2023-12-05 04:59:05.000000 impsparc-3.1.0/cvsvc_apirisk/score/spec_security/yaml_line.py
-drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-02 09:02:32.138687 impsparc-3.1.0/impsparc.egg-info/
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1230 2024-04-02 09:02:31.000000 impsparc-3.1.0/impsparc.egg-info/PKG-INFO
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     7218 2024-04-02 09:02:31.000000 impsparc-3.1.0/impsparc.egg-info/SOURCES.txt
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        1 2024-04-02 09:02:31.000000 impsparc-3.1.0/impsparc.egg-info/dependency_links.txt
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      164 2024-04-02 09:02:31.000000 impsparc-3.1.0/impsparc.egg-info/entry_points.txt
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      178 2024-04-02 09:02:31.000000 impsparc-3.1.0/impsparc.egg-info/requires.txt
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)       14 2024-04-02 09:02:31.000000 impsparc-3.1.0/impsparc.egg-info/top_level.txt
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)       38 2024-04-02 09:02:32.139703 impsparc-3.1.0/setup.cfg
--rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1189 2024-04-02 08:59:54.000000 impsparc-3.1.0/setup.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.258764 impsparc-3.1.1/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1064 2023-11-16 11:18:05.000000 impsparc-3.1.1/LICENSE.md
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      244 2023-11-16 18:00:04.000000 impsparc-3.1.1/MANIFEST.in
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1230 2024-04-04 10:32:59.257716 impsparc-3.1.1/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      871 2023-11-16 11:18:05.000000 impsparc-3.1.1/README.md
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:58.989420 impsparc-3.1.1/cvsvc_apirisk/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 11:18:05.000000 impsparc-3.1.1/cvsvc_apirisk/__init__.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.001225 impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   363678 2023-11-16 11:18:05.000000 impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   262350 2023-11-16 11:18:05.000000 impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      615 2023-11-16 11:18:05.000000 impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      753 2023-11-16 11:18:05.000000 impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    23616 2023-11-16 11:18:05.000000 impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16394 2023-11-16 11:18:05.000000 impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16378 2023-11-16 11:18:05.000000 impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.009717 impsparc-3.1.1/cvsvc_apirisk/score/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 11:18:05.000000 impsparc-3.1.1/cvsvc_apirisk/score/__init__.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2891 2023-11-16 11:18:05.000000 impsparc-3.1.1/cvsvc_apirisk/score/base.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.030786 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/__init__.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)       80 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/apisparc_server.cfg
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    18889 2024-04-04 10:32:17.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1503 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.053427 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2433 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2453 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2662 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2684 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2697 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2117 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2387 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2385 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2393 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2391 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2722 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2731 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.068744 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2346 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2474 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2477 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2459 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2462 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2760 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3371 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/json_line.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    26665 2024-03-11 08:57:07.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/rules_util.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     8837 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/s-origin.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.111531 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        0 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/__init__.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2084 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2418 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2339 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2867 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2292 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2163 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     5141 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2685 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2635 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2479 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2769 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     6786 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sp2_reporting.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.115538 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:58.984633 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.212169 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.228989 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    15291 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16918 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    15192 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    28781 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11370 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1363 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11350 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11421 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      966 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.250867 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      423 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/_palette.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    16193 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      209 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/chart-styles.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3581 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3478 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3944 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      309 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-print.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      406 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     6482 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     9574 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1212 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    88994 2023-11-16 18:00:53.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.126780 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:58.981755 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.138318 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   207965 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      687 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      756 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     2033 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.146525 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    59219 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   195090 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     4023 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    71478 2023-11-16 11:18:05.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/index_raw.html
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    56178 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.161751 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   100782 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   163872 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    80388 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11245 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      393 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/print.css
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    11230 2023-11-16 11:18:05.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/reports.css
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.198217 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   181852 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   105536 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    60520 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    23940 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   388460 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)   154228 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    10556 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     4960 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    32011 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc_html_generation.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    18967 2024-03-14 06:25:43.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/spec_parse.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     5399 2024-04-04 10:31:47.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/spec_util.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     5478 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sps_common.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     3194 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sps_main.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    26214 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sps_main_cr.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)    12521 2023-11-16 17:30:59.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sps_spec_util.py
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1193 2023-12-05 04:59:05.000000 impsparc-3.1.1/cvsvc_apirisk/score/spec_security/yaml_line.py
+drwxr-xr-x   0 nainika.aggarwal   (503) staff       (20)        0 2024-04-04 10:32:59.256291 impsparc-3.1.1/impsparc.egg-info/
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1230 2024-04-04 10:32:58.000000 impsparc-3.1.1/impsparc.egg-info/PKG-INFO
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     7218 2024-04-04 10:32:58.000000 impsparc-3.1.1/impsparc.egg-info/SOURCES.txt
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)        1 2024-04-04 10:32:58.000000 impsparc-3.1.1/impsparc.egg-info/dependency_links.txt
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      164 2024-04-04 10:32:58.000000 impsparc-3.1.1/impsparc.egg-info/entry_points.txt
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)      178 2024-04-04 10:32:58.000000 impsparc-3.1.1/impsparc.egg-info/requires.txt
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)       14 2024-04-04 10:32:58.000000 impsparc-3.1.1/impsparc.egg-info/top_level.txt
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)       38 2024-04-04 10:32:59.258877 impsparc-3.1.1/setup.cfg
+-rw-r--r--   0 nainika.aggarwal   (503) staff       (20)     1189 2024-04-04 10:32:40.000000 impsparc-3.1.1/setup.py
```

### Comparing `impsparc-3.1.0/LICENSE.md` & `impsparc-3.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/PKG-INFO` & `impsparc-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 3.1.0
+Version: 3.1.1
 Summary: API Specification Analysis for Risks and Compliance
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `impsparc-3.1.0/README.md` & `impsparc-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf` & `impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/API_Risk_Assessment_OB.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf` & `impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/CloudVector-APIRiskTool-Documentation.pdf`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json` & `impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/cv_rules_sample.json`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt` & `impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/example_cmds.txt`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip` & `impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/orangebank.zip`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json` & `impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user.json`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json` & `impsparc-3.1.1/cvsvc_apirisk/cvapirisk_pkg/orangebank_user_orig.json`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/base.py` & `impsparc-3.1.1/cvsvc_apirisk/score/base.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/cv_apirisk_assessment.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,14 @@
         return indata
 
 
     def rules_matching(self, spectree, indata, inputfname):
         print("---- Starting match test against %i rules, global list:\n" % len(self.matchsets))
 
         request_ref_list = spectree.request_ref_list
-        #import pdb;pdb.set_trace()
         for m in self.matchsets:
             self.num_evaluations = self.num_evaluations + m.performGlobalMatches(spectree.nonapinodes, self.globalvs, indata, request_ref_list)
 
         apimatchsets = []
         for mset in self.matchsets :
             if not mset.allMatchGlobal :
                 apimatchsets.append(mset)
@@ -126,15 +125,15 @@
                 newmset.copyMatch(mset)
                 newmsets.append(newmset)
 
             #print("------ > Checking api=\'%s\', %s nodes ----> \n" % (apidef, len(apinodes)))
             perapiv = []
             for mset in newmsets :
                 self.num_evaluations = self.num_evaluations + mset.performPerAPIMatches(apidef, apinodes, perapiv, indata, request_ref_list)
-            self.perapivios[inputfname+":"+apidef]=perapiv
+            self.perapivios[inputfname.split('/')[-1]+":"+apidef]=perapiv
 
         refmatchsets = []
         for mset in self.matchsets :
             if not mset.allMatchGlobal :
                 refmatchsets.append(mset)
         print("---- Starting match test against %i rules against nodes referenced by APIs:\n" % len(apimatchsets))
 
@@ -145,40 +144,40 @@
                 newmset.copyMatch(mset)
                 newmsets.append(newmset)
 
             #print("------ > Checking $ref=\'%s\', %i nodes ----> \n" % (ref, len(refnodes)))
             perrefv = []
             for mset in newmsets :
                 self.num_evaluations = self.num_evaluations + mset.performRefMatches(ref, refnodes, perrefv, indata, request_ref_list)
-            self.refvios[inputfname+":"+ref]=perrefv
+            self.refvios[inputfname.split('/')[-1]+":"+ref]=perrefv
 
     def get_properties_voilations(self, report, abs_path, target_obj):
         spec_util_obj = SpecUtil()
         spec_util_obj.get_all_voilations(report, abs_path)
 
 
         report['files'][abs_path]['properties']['status'] = 'valid'
         report['files'][abs_path]['properties']['score'] = 9
         #report['files'][abs_path]['properties']['meta'] = spec_main.meta
         # report['files'][abs_path]['properties']['num_apis'] = \
         #     100
-        #import pdb;pdb.set_trace()
+
         report['files'][abs_path]['properties']['version'] = \
             target_obj['info']['version']
         report['files'][abs_path]['properties']['num_evaluations'] = \
             self.num_evaluations
 
 
 
     def get_voilations(self, outputjson, inputfname):
         apir = outputjson["files"][inputfname]["apis"]
         refr = outputjson["files"][inputfname]["$refs"]
         nvios = 0
         for v in self.globalvs:
-            apiname = inputfname+": All APIs (Global Definitions)"
+            apiname = inputfname.split('/')[-1] +": All APIs (Global Definitions)"
             apivs = []
             if not apiname in apir:
                 apir[apiname] = {"violations":apivs}
             else:
                 apivs = apir[apiname]["violations"]
             nvios += 1
             apivs.append(v.dictR)
```

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/cv_apirisk_server.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr07.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/data_attrs/sps_data_attr12.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/fmt_attrs/sps_fmt_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/json_line.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/json_line.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/rules_util.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/rules_util.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/s-origin.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/s-origin.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr01.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr02.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr03.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr04.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr05.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr06.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr07.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr08.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr09.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr10.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/security_attrs/sps_sec_attr11.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sp2_reporting.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sp2_reporting.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/api-method-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/design-issues-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/parameter-type-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/charts/response-code-distribution-donut.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/imperva_logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/info-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_cardinal.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/logo_navy.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/images/tile-bkgnd.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-classes.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/helper-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/report-styles-page1.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles-print.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/assets/styles/template-text-styles.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/bg.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/footer-logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/lmperva logo-white.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/chart.min.js`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/assets/scripts/index.js`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/index_raw.html` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/index_raw.html`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/risk-report-template-generic.html`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/all.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/html.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/reports.css` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/styles/reports.css`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc-templates-new/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sparc_html_generation.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sparc_html_generation.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/spec_parse.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/spec_parse.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/spec_util.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/spec_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -43,14 +43,23 @@
                                     response_node_names[responses] = response_node_names[responses] + 1
                                 else:
                                     response_node_names[responses] = 1
 
             return response_node_names
 
 
+    def get_data_type(selfs, parameter, data_types):
+        p_type = parameter['type']
+        if not isinstance(p_type, str):
+            p_type = parameter['type'][0]
+        if p_type in data_types:
+            data_types[p_type] = data_types[p_type] + 1
+        else:
+            data_types[p_type] = 1
+
     def get_param_objs(self, spec):
         #print(spec['openapi'])
         if 'openapi' in spec:
             self.openapi_ver = 'v3'
         else:
             self.openapi_ver = 'v2'
         if 'paths' not in spec:
@@ -71,65 +80,44 @@
                                 if self.openapi_ver == 'v3':
                                     if 'schema' in parameter:
                                         if '$ref' in parameter['schema']:
                                             if isinstance(parameter['schema']['$ref'], str):
                                                 ref_parameter.append(parameter['schema']['$ref'])
                                             else:
                                                 ref_parameter.append(parameter['schema']['$ref'][0])
-                                            #ref_parameter = ref_parameter.append(parameter['schema']['$ref'])
                                         if 'type' in parameter['schema']:
                                             num_params = num_params + 1
-                                            p_type = parameter['schema']['type'][0]
-                                            if p_type in data_types:
-                                                data_types[p_type] = data_types[p_type] + 1
-                                            else:
-                                                data_types[p_type] = 1
+                                            self.get_data_type(parameter['schema'], data_types)
 
                                 elif self.openapi_ver == 'v2':
                                     if 'schema' in parameter:
                                         parameter = parameter['schema']
                                     if '$ref' in parameter:
                                         if isinstance(parameter['$ref'], str):
                                             ref_parameter.append(parameter['$ref'])
                                         else:
                                             ref_parameter.append(parameter['$ref'][0])
 
                                     if 'type' in parameter:
                                         num_params = num_params + 1
-                                        p_type = parameter['type']
-                                        if not isinstance(p_type, str):
-                                            p_type = parameter['type'][0]
-                                        if p_type in data_types:
-                                            data_types[p_type] = data_types[p_type] + 1
-                                        else:
-                                            data_types[p_type] = 1
-
-
-            print(data_types)
+                                        self.get_data_type(parameter, data_types)
 
             for ref_data in ref_parameter:
                 spec_data = spec
                 for data in ref_data.split("/"):
                     if data == '#':
                         continue
                     else:
                         #print(data)
                         spec_data = spec_data.get(data, {})
 
                 if 'type' in spec_data:
                     num_params = num_params + 1
-                    p_type = spec_data['type']
-                    if not isinstance(p_type, str):
-                        p_type = spec_data['type'][0]
-                    if p_type in data_types:
-                        data_types[p_type] = data_types[p_type] + 1
-                    else:
-                        data_types[p_type] = 1
+                    self.get_data_type(parameter, data_types)
 
-            print(data_types)
             return num_params, data_types, num_apis
 
 
     def get_all_voilations(self, report, abs_path):
         all_voilations = []
         for data in ['apis', '$refs']:
             for api_path, voilation_key in report['files'][abs_path][data].items():
```

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sps_common.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sps_common.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sps_main.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sps_main.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sps_main_cr.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sps_main_cr.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/sps_spec_util.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/sps_spec_util.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/cvsvc_apirisk/score/spec_security/yaml_line.py` & `impsparc-3.1.1/cvsvc_apirisk/score/spec_security/yaml_line.py`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/impsparc.egg-info/PKG-INFO` & `impsparc-3.1.1/impsparc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impsparc
-Version: 3.1.0
+Version: 3.1.1
 Summary: API Specification Analysis for Risks and Compliance
 Author: Priyank Chheda
 Author-email: priyank.chheda@imperva.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `impsparc-3.1.0/impsparc.egg-info/SOURCES.txt` & `impsparc-3.1.1/impsparc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `impsparc-3.1.0/setup.py` & `impsparc-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="impsparc",
-    version=os.environ.get("VER", "3.1.0"),
+    version=os.environ.get("VER", "3.1.1"),
     author="Priyank Chheda",
     author_email="priyank.chheda@imperva.com",
     description="API Specification Analysis for Risks and Compliance",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

