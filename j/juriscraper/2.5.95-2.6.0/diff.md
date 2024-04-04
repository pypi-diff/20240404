# Comparing `tmp/juriscraper-2.5.95.tar.gz` & `tmp/juriscraper-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juriscraper-2.5.95.tar", last modified: Wed Feb 14 19:04:25 2024, max compression
+gzip compressed data, was "juriscraper-2.6.0.tar", last modified: Thu Apr  4 01:09:20 2024, max compression
```

## Comparing `juriscraper-2.5.95.tar` & `juriscraper-2.6.0.tar`

### file list

```diff
@@ -1,445 +1,447 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.700572 juriscraper-2.5.95/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-14 19:04:13.000000 juriscraper-2.5.95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-14 19:04:13.000000 juriscraper-2.5.95/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-14 19:04:13.000000 juriscraper-2.5.95/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    16435 2024-02-14 19:04:25.700572 juriscraper-2.5.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14792 2024-02-14 19:04:13.000000 juriscraper-2.5.95/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.632572 juriscraper-2.5.95/juriscraper/
--rw-r--r--   0 runner    (1001) docker     (127)    17349 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/AbstractSite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/DeferringList.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/OpinionSite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/OpinionSiteLinear.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/OpinionSiteLinearWebDriven.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/OpinionSiteWebDriven.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/OralArgumentSite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/OralArgumentSiteLinear.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/OralArgumentSiteLinearWebDriven.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/WebDriven.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.632572 juriscraper-2.5.95/juriscraper/fdsys/
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/fdsys/FDSysSite.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/fdsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-02-14 19:04:13.000000 juriscraper-2.5.95/juriscraper/fdsys/scrape_court_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.632572 juriscraper-2.5.95/juriscraper/fdsys/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/fdsys/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/fdsys/utils/get_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/fdsys/utils/get_xpath_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.632572 juriscraper-2.5.95/juriscraper/lasc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lasc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lasc/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lasc/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.636572 juriscraper-2.5.95/juriscraper/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/cookie_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/diff_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/html_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/judge_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/log_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26813 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.636572 juriscraper-2.5.95/juriscraper/opinions/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/opinion_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.636572 juriscraper-2.5.95/juriscraper/opinions/united_states/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.640572 juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/asbca.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/bia.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/bva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/mspb_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/mspb_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/olc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.644572 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca11_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca11_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca2_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca2_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca3_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca3_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca7.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca8.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca9_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca9_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/cadc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/cadc_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/cafc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/scotus_relating.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.644572 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_bankruptcy/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_bankruptcy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_bankruptcy/bap1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.644572 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_district/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_district/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_district/dcd.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_district/ed_louisiana.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.644572 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/acca_memorandum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/acca_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/acca_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/afcca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/ag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/armfor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/cavc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/cit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/nmcca.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/tax.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/uscfc.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/uscfc_u.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/uscgcoca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.680572 juriscraper-2.5.95/juriscraper/opinions/united_states/state/
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ala.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/alacivapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/alacrimapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/alaska.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/alaskactapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ariz.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/arizctapp_div_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/arizctapp_div_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ark.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/arkctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/cal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/calag.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/calctapp_1st.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/calctapp_2nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/calctapp_3rd.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/calctapp_4th_div1.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/calctapp_4th_div2.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/calctapp_4th_div3.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/calctapp_5th.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/calctapp_6th.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/calctapp_app_div.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/calctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/colo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/coloctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/conn.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/connappct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/dc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/delaware.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/delch.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/delctcompl.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/delsuperct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/fla.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/fladistctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/fladistctapp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/fladistctapp_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/fladistctapp_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/fladistctapp_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/fladistctapp_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/fladistctapp_6.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/gactapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/haw.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/haw_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/hawapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/idaho_civil.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/idaho_criminal.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/idahoctapp_civil.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/idahoctapp_criminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/idahoctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ill.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/illappct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ind.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/indctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/indtc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/iowa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/iowactapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/kan_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/kan_u.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/kanctapp_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/kanctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ky.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/kyctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/la.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/lactapp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/massappct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/massappct_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/masslandct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/md.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/mdag.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/mdctspecapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/me.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/mesuperct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/mich.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/michctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/minn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/minnag.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/minnctapp_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/minnctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/miss.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/miss_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/missctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/mo.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/moctapp_eastern.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/moctapp_southern.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/moctapp_western.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/mont.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nc.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ncctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/neb.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nebctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nev.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nevapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nj.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/njsuperctappdiv_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/njsuperctappdiv_u.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/njtaxct_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/njtaxct_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nm.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nmctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ny.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nyag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nyappdiv_1st.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nyappdiv_2nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nyappdiv_3rd.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nyappdiv_4th.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nyappterm_1st.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nyappterm_2nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nycityct.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nycivct.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nyclaimsct.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nycountyct.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nycrimct.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nydistct.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nyfamct.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nyjustct.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nysupct.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nysupct_commercial.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nysurct.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/nytrial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohio.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctapp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctapp_10.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctapp_11.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctapp_12.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctapp_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctapp_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctapp_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctapp_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctapp_6.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctapp_7.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctapp_8.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctapp_9.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctcl.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/okla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/oklaag.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/oklacivapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/oklacrimapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/or.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/orctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/pa.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/pacommwct.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/pasuperct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ri_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/ri_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/sc.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/scctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/sd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/tenn.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/tenncrimapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/tennctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/tex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texag.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_10.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_11.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_12.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_13.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_14.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_6.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_7.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_8.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texapp_9.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/texcrimapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/utah.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/utahctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/va.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/vactapp_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/vactapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/vt.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/vt_criminal.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/vtsuperct_civil.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/vtsuperct_environmental.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/vtsuperct_family.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/vtsuperct_probate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/wash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/washctapp_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/washctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/wis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/wva.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/wvactapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/state/wyo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.680572 juriscraper-2.5.95/juriscraper/opinions/united_states/territories/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/territories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/territories/as.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/territories/guam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/territories/nmariana.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/territories/prapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/territories/prsupreme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/territories/virginislands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/territories/visuper_p.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states/territories/visuper_u.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.680572 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.684572 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/administrative_agency/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/administrative_agency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.684572 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_appellate/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_appellate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.684572 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_district/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_district/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.688572 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2011.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.692572 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/cal_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_criminal.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/ill.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/illappct_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/illappct_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/illappct_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/illappct_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/illappct_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/ind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/indctapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/indtc.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/me.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/me_2013.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/ny.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_1st.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_2nd.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_3rd.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_4th.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/sd.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.692572 juriscraper-2.5.95/juriscraper/oral_args/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/oral_argument_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.692572 juriscraper-2.5.95/juriscraper/oral_args/united_states/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.696572 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca11.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca7.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca8.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca9.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/cadc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/cafc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/scotus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.696572 juriscraper-2.5.95/juriscraper/oral_args/united_states/state/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/state/ill.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/state/illappct_1st_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/state/illappct_2nd_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/state/illappct_3rd_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/state/illappct_4th_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/state/illappct_5th_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/state/illappct_workers_comp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/oral_args/united_states/state/md.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.700572 juriscraper-2.5.95/juriscraper/pacer/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/acms_docket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/appellate_attachment_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    30499 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/appellate_docket.py
--rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/attachment_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/case_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/case_query_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/claims_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/claims_register.py
--rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/docket_history_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    63192 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/docket_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/docket_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/download_confirmation_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    34933 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/email.py
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/free_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/hidden_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15932 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/internet_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/list_of_creditors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/mobile_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    15850 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    16181 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/rss_feeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacer/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/pacerdocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.700572 juriscraper-2.5.95/juriscraper/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.700572 juriscraper-2.5.95/juriscraper/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:14.000000 juriscraper-2.5.95/juriscraper/video/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:04:25.700572 juriscraper-2.5.95/juriscraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16435 2024-02-14 19:04:25.000000 juriscraper-2.5.95/juriscraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22269 2024-02-14 19:04:25.000000 juriscraper-2.5.95/juriscraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 19:04:25.000000 juriscraper-2.5.95/juriscraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-14 19:04:25.000000 juriscraper-2.5.95/juriscraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-14 19:04:25.000000 juriscraper-2.5.95/juriscraper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-14 19:04:14.000000 juriscraper-2.5.95/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-14 19:04:14.000000 juriscraper-2.5.95/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-14 19:04:25.700572 juriscraper-2.5.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-02-14 19:04:14.000000 juriscraper-2.5.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.011596 juriscraper-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-04 01:09:07.000000 juriscraper-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 01:09:07.000000 juriscraper-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 01:09:07.000000 juriscraper-2.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-04 01:09:20.011596 juriscraper-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14792 2024-04-04 01:09:07.000000 juriscraper-2.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.943596 juriscraper-2.6.0/juriscraper/
+-rw-r--r--   0 runner    (1001) docker     (127)    17359 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/AbstractSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/DeferringList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OpinionSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OpinionSiteLinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OpinionSiteLinearWebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OpinionSiteWebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OralArgumentSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OralArgumentSiteLinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/OralArgumentSiteLinearWebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/WebDriven.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.947597 juriscraper-2.6.0/juriscraper/fdsys/
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/fdsys/FDSysSite.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/fdsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-04 01:09:07.000000 juriscraper-2.6.0/juriscraper/fdsys/scrape_court_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.947597 juriscraper-2.6.0/juriscraper/fdsys/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/fdsys/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/fdsys/utils/get_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/fdsys/utils/get_xpath_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.947597 juriscraper-2.6.0/juriscraper/lasc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lasc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lasc/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lasc/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.947597 juriscraper-2.6.0/juriscraper/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/cookie_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/diff_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/html_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/judge_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/log_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26813 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.951597 juriscraper-2.6.0/juriscraper/opinions/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/opinion_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.951597 juriscraper-2.6.0/juriscraper/opinions/united_states/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.951597 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/asbca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/bia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/bva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/mspb_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/mspb_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/olc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.955597 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca11_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca11_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca2_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca2_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca3_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca3_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca9_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca9_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cadc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cadc_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cafc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/scotus_relating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.955597 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/bap1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.955597 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_district/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_district/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_district/dcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_district/ed_louisiana.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.959596 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/acca_memorandum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/acca_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/acca_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/afcca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/ag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/armfor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/cavc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/cit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/fisc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/fiscr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/nmcca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscgcoca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.991596 juriscraper-2.6.0/juriscraper/opinions/united_states/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ala.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/alacivapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/alacrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/alaska.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/alaskactapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ariz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/arizctapp_div_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/arizctapp_div_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/arkctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/cal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_1st.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_3rd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_4th_div1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_4th_div2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_4th_div3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_5th.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_6th.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_app_div.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/colo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/coloctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/conn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/connappct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/dc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/delaware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/delch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/delctcompl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/delsuperct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/gactapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/haw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/haw_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/hawapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/idaho_civil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/idaho_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/idahoctapp_civil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/idahoctapp_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/idahoctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/illappct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/indctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/indtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/iowa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/iowactapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/kan_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/kan_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/kanctapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/kanctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ky.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/kyctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/la.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/lactapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/massappct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/massappct_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/masslandct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mdag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mdctspecapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/me.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mesuperct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/michctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/minn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/minnag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/minnctapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/minnctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/miss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/miss_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/missctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/moctapp_eastern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/moctapp_southern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/moctapp_western.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/mont.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ncctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/neb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nebctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nevapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nj.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/njsuperctappdiv_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/njsuperctappdiv_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/njtaxct_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/njtaxct_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nmctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappdiv_1st.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappdiv_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappdiv_3rd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappdiv_4th.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappterm_1st.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappterm_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nycityct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nycivct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyclaimsct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nycountyct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nycrimct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nydistct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyfamct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyjustct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nysupct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nysupct_commercial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nysurct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/nytrial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctapp_9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/okla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/oklaag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/oklacivapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/oklacrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/or.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/orctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/pa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/pacommwct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/pasuperct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ri_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/ri_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/sc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/scctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/sd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/tenn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/tenncrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/tennctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/tex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_13.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_14.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texapp_9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/texcrimapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/utah.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/utahctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/va.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vactapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vactapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vt_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vtsuperct_civil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vtsuperct_environmental.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vtsuperct_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/vtsuperct_probate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/wash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/washctapp_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/washctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/wis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/wva.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/wvactapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/state/wyo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.991596 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/as.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/guam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/nmariana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/prapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/prsupreme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/virginislands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/visuper_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states/territories/visuper_u.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.991596 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.991596 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/administrative_agency/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/administrative_agency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.995596 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.995596 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.999596 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2011.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:19.999596 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/cal_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_criminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/illappct_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/illappct_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/illappct_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/illappct_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/illappct_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/indctapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/indtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/me.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/me_2013.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_1st.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_2nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_3rd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/nyappdiv_4th.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/sd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.003596 juriscraper-2.6.0/juriscraper/oral_args/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/oral_argument_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.003596 juriscraper-2.6.0/juriscraper/oral_args/united_states/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.003596 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca9.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/cadc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/cafc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/scotus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.003596 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/ill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_1st_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_2nd_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_3rd_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_4th_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_5th_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_workers_comp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/oral_args/united_states/state/md.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.007596 juriscraper-2.6.0/juriscraper/pacer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/acms_docket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/appellate_attachment_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30499 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/appellate_docket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/attachment_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/case_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/case_query_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/claims_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/claims_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/docket_history_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63103 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/docket_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/docket_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/download_confirmation_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34933 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15137 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/free_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/hidden_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15932 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/internet_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/list_of_creditors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/mobile_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15850 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16181 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/rss_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacer/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      582 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/pacerdocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.007596 juriscraper-2.6.0/juriscraper/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.007596 juriscraper-2.6.0/juriscraper/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:08.000000 juriscraper-2.6.0/juriscraper/video/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:09:20.007596 juriscraper-2.6.0/juriscraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-04 01:09:19.000000 juriscraper-2.6.0/juriscraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22388 2024-04-04 01:09:19.000000 juriscraper-2.6.0/juriscraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:09:19.000000 juriscraper-2.6.0/juriscraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-04 01:09:19.000000 juriscraper-2.6.0/juriscraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 01:09:19.000000 juriscraper-2.6.0/juriscraper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-04 01:09:08.000000 juriscraper-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-04 01:09:08.000000 juriscraper-2.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-04 01:09:20.011596 juriscraper-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-04 01:09:08.000000 juriscraper-2.6.0/setup.py
```

### Comparing `juriscraper-2.5.95/LICENSE` & `juriscraper-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/PKG-INFO` & `juriscraper-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juriscraper
-Version: 2.5.95
+Version: 2.6.0
 Summary: An API to scrape American court websites for metadata.
 Home-page: https://github.com/freelawproject/juriscraper
 Author: Free Law Project
 Author-email: info@free.law
 Maintainer: Free Law Project
 Maintainer-email: info@free.law
 License: BSD
@@ -31,15 +31,15 @@
 Requires-Dist: certifi>=2017.4.17
 Requires-Dist: chardet>=3.0.2
 Requires-Dist: cssselect
 Requires-Dist: dateparser>=1.2.0
 Requires-Dist: feedparser>=6.0.11
 Requires-Dist: geonamescache>=2.0.0
 Requires-Dist: html5lib
-Requires-Dist: lxml>=4.9
+Requires-Dist: lxml>=5.2
 Requires-Dist: nh3
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: requests>=2.20.0
 Requires-Dist: selenium>=4.9.1
 Requires-Dist: tldextract
 
 +---------------+---------------------+-------------------+
```

### Comparing `juriscraper-2.5.95/README.rst` & `juriscraper-2.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/AbstractSite.py` & `juriscraper-2.6.0/juriscraper/AbstractSite.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 class AbstractSite:
     """Contains generic methods for scraping data. Should be extended by all
     scrapers.
 
     Should not contain lists that can't be sorted by the _date_sort function.
     """
 
-    def __init__(self, cnt=None):
+    def __init__(self, cnt=None, **kwargs):
         super().__init__()
 
         # Computed metadata
         self.hash = None
         self.html = None
         self.method = "GET"
         self.back_scrape_iterable = None
```

### Comparing `juriscraper-2.5.95/juriscraper/DeferringList.py` & `juriscraper-2.6.0/juriscraper/DeferringList.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/OpinionSite.py` & `juriscraper-2.6.0/juriscraper/OpinionSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/OpinionSiteLinear.py` & `juriscraper-2.6.0/juriscraper/OpinionSiteLinear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/OralArgumentSite.py` & `juriscraper-2.6.0/juriscraper/OralArgumentSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/OralArgumentSiteLinear.py` & `juriscraper-2.6.0/juriscraper/OralArgumentSiteLinear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/WebDriven.py` & `juriscraper-2.6.0/juriscraper/WebDriven.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/fdsys/FDSysSite.py` & `juriscraper-2.6.0/juriscraper/fdsys/FDSysSite.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/fdsys/scrape_court_names.py` & `juriscraper-2.6.0/juriscraper/fdsys/scrape_court_names.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/fdsys/utils/get_metadata.py` & `juriscraper-2.6.0/juriscraper/fdsys/utils/get_metadata.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/fdsys/utils/get_xpath_results.py` & `juriscraper-2.6.0/juriscraper/fdsys/utils/get_xpath_results.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/lasc/fetch.py` & `juriscraper-2.6.0/juriscraper/lasc/fetch.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/lasc/http.py` & `juriscraper-2.6.0/juriscraper/lasc/http.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/lib/cookie_utils.py` & `juriscraper-2.6.0/juriscraper/lib/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/lib/date_utils.py` & `juriscraper-2.6.0/juriscraper/lib/date_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/lib/diff_tools.py` & `juriscraper-2.6.0/juriscraper/lib/diff_tools.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/lib/exceptions.py` & `juriscraper-2.6.0/juriscraper/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/lib/html_utils.py` & `juriscraper-2.6.0/juriscraper/lib/html_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 import re
 import sys
 from copy import deepcopy
 from urllib.parse import urlsplit, urlunsplit
 
 import nh3
 from lxml import etree, html
-from lxml.etree import XMLSyntaxError
 from lxml.html import HtmlElement, fromstring, tostring
-from lxml.html.clean import Cleaner
 from requests import Response
 
 try:
     # Use charset-normalizer for performance to detect the character encoding.
     import charset_normalizer as chardet
 except ImportError:
     import chardet
@@ -118,28 +116,14 @@
     :param row: HtmlElement
     :param cell_num: int
     :return: string
     """
     return row.xpath(".//td[%d]//a/@href" % cell_num)[0]
 
 
-def get_clean_body_content(content, remove_extra_tags=[]):
-    """Parse out the body from an html string, clean it up, and send it along."""
-    remove_tags = ["a", "body", "font", "noscript"]
-    remove_tags.extend(remove_extra_tags)
-    cleaner = Cleaner(style=True, remove_tags=remove_tags)
-    try:
-        return cleaner.clean_html(content)
-    except XMLSyntaxError:
-        return (
-            "Unable to extract the content from this file. Please try "
-            "reading the original."
-        )
-
-
 def strip_bad_html_tags_insecure(
     text: str, remove_scripts=True
 ) -> HtmlElement:
     """Remove bad HTML that isn't used by our parsers.
 
     This is insecure in the sense that it does not strip all JavaScript. lxml
     provides a `javascript` parameter that can be passed to the Cleaner object,
```

### Comparing `juriscraper-2.5.95/juriscraper/lib/importer.py` & `juriscraper-2.6.0/juriscraper/lib/importer.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/lib/judge_parsers.py` & `juriscraper-2.6.0/juriscraper/lib/judge_parsers.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/lib/log_tools.py` & `juriscraper-2.6.0/juriscraper/lib/log_tools.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/lib/network_utils.py` & `juriscraper-2.6.0/juriscraper/lib/network_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/lib/string_utils.py` & `juriscraper-2.6.0/juriscraper/lib/string_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/lib/test_utils.py` & `juriscraper-2.6.0/juriscraper/lib/test_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/lib/utils.py` & `juriscraper-2.6.0/juriscraper/lib/utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/opinion_template.py` & `juriscraper-2.6.0/juriscraper/opinions/opinion_template.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/asbca.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/asbca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/bia.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/bia.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/bva.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/bva.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/mspb_p.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/mspb_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/mspb_u.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/mspb_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/administrative_agency/olc.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/administrative_agency/olc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca1.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca10.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca11_p.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca11_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca11_u.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca11_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca2_p.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca2_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca2_u.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca2_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca3_p.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca3_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca4.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca4.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca5.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca6.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca6.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca7.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca7.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca8.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca8.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca9_p.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca9_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/ca9_u.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/ca9_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/cadc.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cadc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cadc_pi.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/cadc_u.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cadc_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/cafc.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/cafc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/scotus_chambers.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_appellate/scotus_slip.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_bankruptcy/bap1.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/bap1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/bap10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_bankruptcy/bap9.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_district/dcd.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_district/dcd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/acca_p.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/acca_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/afcca.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/afcca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/ag.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/ag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/armfor.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/armfor.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/cavc.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/cavc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/cit.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/cit.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/nmcca.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/nmcca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/tax.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/tax.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/uscfc.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/uscfc_u.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/federal_special/uscgcoca.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/federal_special/uscgcoca.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/__init__.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/__init__.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/ala.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ala.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/alaska.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/alaska.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/ariz.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ariz.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/arizctapp_div_2.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/arizctapp_div_2.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/ark.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ark.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/cal.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/cal.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/calag.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/calag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/calctapp_1st.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/calctapp_1st.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/colo.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/colo.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/coloctapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/coloctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/conn.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/conn.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/connappct.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/connappct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/dc.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/dc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/delaware.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/delaware.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/fla.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/fla.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/fladistctapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/fladistctapp_5.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/fladistctapp_5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/ga.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ga.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/gactapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/gactapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/haw.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/haw.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/haw_beginningofyear.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/haw_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/hawapp_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/idaho_civil.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/idaho_civil.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/idahoctapp_u.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/idahoctapp_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/ill.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ill.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/illappct.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/illappct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/ind.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ind.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/iowa.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/iowa.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/iowactapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/iowactapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/kan_p.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/kan_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/ky.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ky.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/kyctapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/kyctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/la.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/la.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/lactapp_1.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/lactapp_1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/mass.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mass.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/massappct_u.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/massappct_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/masslandct.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/masslandct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/md.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/md.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/mdag.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mdag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/mdctspecapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mdctspecapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/me.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/me.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/mesuperct.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mesuperct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/mich.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mich.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/michctapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/michctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/minn.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/minn.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/minnag.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/minnag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/minnctapp_u.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/minnctapp_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/miss.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/miss.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/miss_beginningofyear.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/miss_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/missctapp_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/mo.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mo.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/moctapp_southern.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/moctapp_southern.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/mont.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/mont.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/nc.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/ncctapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ncctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/nd.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/neb.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/neb.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/nev.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nev.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/nevapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nevapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/nh.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nh.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/nj.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nj.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/nm.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nm.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/ny.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ny.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/nyag.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/nyappdiv_1st.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappdiv_1st.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/nyappterm_1st.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nyappterm_1st.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/nytrial.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/nytrial.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohio.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohio.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ohioctcl_beginningofyear.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/okla.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/okla.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/oklaag.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/oklaag.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/oklacivapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/oklacivapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/oklacrimapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/oklacrimapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/orctapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/orctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/pa.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/pa.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/pacommwct.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/pacommwct.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/ri_p.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ri_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/ri_u.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/ri_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/sc.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/sc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/scctapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/scctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/sd.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/sd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/tenn.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/tenn.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/tex.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/tex.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/texag.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/texag.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 
 class Site(OpinionSiteLinear):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.court_id = self.__module__
         self.url = "https://texasattorneygeneral.gov/opinions"
-        self.expected_content_types = ["text/html"]
+        self.expected_content_types = ["application/pdf"]
 
     def _process_html(self):
         cases = self.html.xpath("//div[@class='sidebar-ag-opinion-content']")
         for case in cases:
             docket = case.xpath(".//h4")[0].text_content().strip()
             summary = case.xpath(".//p")[0].text_content().strip()
-            url = case.xpath(".//h4/a/@href")[0]
+            url = case.xpath(".//a[contains(@href, '.pdf')]/@href")[0]
             name = f"Untitled Texas Attorney General Opinion: {docket}"
             date = case.xpath(
                 ".//div[@class='sidebar-ag-opinion-casedate']/text()"
             )[0].strip()
             self.cases.append(
                 {
                     "name": name,
```

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/utah.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/utah.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/utahctapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/utahctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/va.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/va.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/vactapp_p.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/vactapp_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/vactapp_u.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/vactapp_u.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/vt.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/vt.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/wash.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/wash.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/washctapp_p.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/washctapp_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/wis.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/wis.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/wva.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/wva.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/state/wyo.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/state/wyo.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/territories/guam.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/territories/guam.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/territories/nmariana.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/territories/nmariana.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/territories/prapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/territories/prapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/territories/prsupreme.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/territories/prsupreme.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/territories/virginislands.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/territories/virginislands.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states/territories/visuper_p.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states/territories/visuper_p.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/administrative_agency/bia.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/administrative_agency/olc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca3.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/ca5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_appellate/cadc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2009.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2010.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2011.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2012.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_district/dcd_2013.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2004.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/armfor_2005.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_1999.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2000.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2001.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2002.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2003.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2004.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2005.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2006.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2007.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2008.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2009.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2010.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/federal_special/cit_2012.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/idahoctapp_civil.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/ill.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ill.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/ind.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ind.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ind_2005.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/indctapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/indctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/me.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/me.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/me_2013.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/me_2013.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/nd.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/nd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/ny.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/ny.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/sd.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/sd.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py` & `juriscraper-2.6.0/juriscraper/opinions/united_states_backscrapers/state/utahctapp.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/oral_argument_template.py` & `juriscraper-2.6.0/juriscraper/oral_args/oral_argument_template.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca1.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca1.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca10.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca10.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca11.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca11.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca2.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca2.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca3.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca3.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca4.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca4.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca5.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca5.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca6.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca6.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca7.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca7.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca8.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca8.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/ca9.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/ca9.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/cadc.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/cadc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/cafc.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/cafc.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/federal_appellate/scotus.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/federal_appellate/scotus.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/state/ill.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/state/ill.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/state/illappct_1st_dist.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/state/illappct_1st_dist.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/oral_args/united_states/state/md.py` & `juriscraper-2.6.0/juriscraper/oral_args/united_states/state/md.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/__init__.py` & `juriscraper-2.6.0/juriscraper/pacer/__init__.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/acms_docket.py` & `juriscraper-2.6.0/juriscraper/pacer/acms_docket.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/appellate_attachment_page.py` & `juriscraper-2.6.0/juriscraper/pacer/appellate_attachment_page.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/appellate_docket.py` & `juriscraper-2.6.0/juriscraper/pacer/appellate_docket.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/attachment_page.py` & `juriscraper-2.6.0/juriscraper/pacer/attachment_page.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/case_query.py` & `juriscraper-2.6.0/juriscraper/pacer/case_query.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/case_query_advanced.py` & `juriscraper-2.6.0/juriscraper/pacer/case_query_advanced.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/claims_activity.py` & `juriscraper-2.6.0/juriscraper/pacer/claims_activity.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/claims_register.py` & `juriscraper-2.6.0/juriscraper/pacer/claims_register.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/docket_history_report.py` & `juriscraper-2.6.0/juriscraper/pacer/docket_history_report.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/docket_report.py` & `juriscraper-2.6.0/juriscraper/pacer/docket_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -929,18 +929,15 @@
                 "name": " ".join(name_parts),
                 "roles": [],
                 "contact": "",
             }
             path = "./following-sibling::* | ./following-sibling::text()"
             for prev, node, nxt in previous_and_next(atty_node.xpath(path)):
                 # noinspection PyProtectedMember
-                if isinstance(
-                    node,
-                    (etree._ElementStringResult, etree._ElementUnicodeResult),
-                ):
+                if isinstance(node, etree._ElementUnicodeResult):
                     clean_atty = "%s\n" % " ".join(
                         n.strip() for n in node.split()
                     )
                     if clean_atty.strip():
                         attorney["contact"] += clean_atty
                 else:
                     if node.tag == "i":
```

### Comparing `juriscraper-2.5.95/juriscraper/pacer/docket_utils.py` & `juriscraper-2.6.0/juriscraper/pacer/docket_utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/download_confirmation_page.py` & `juriscraper-2.6.0/juriscraper/pacer/download_confirmation_page.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/email.py` & `juriscraper-2.6.0/juriscraper/pacer/email.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/free_documents.py` & `juriscraper-2.6.0/juriscraper/pacer/free_documents.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 """Classes for querying PACER's Written Opinion Report (WrtOpRpt.pl),
 which is free.
 """
+import pprint
+import sys
 
 from ..lib.date_utils import make_date_range_tuples
 from ..lib.html_utils import (
     clean_html,
     fix_links_in_lxml_tree,
     get_html_parsed_text,
     set_response_encoding,
 )
 from ..lib.log_tools import make_default_logger
-from ..lib.string_utils import convert_date_string
+from ..lib.string_utils import clean_string, convert_date_string, harmonize
 from ..pacer.utils import (
     get_nonce_from_form,
     get_pacer_case_id_from_nonce_url,
     get_pacer_doc_id_from_doc1_url,
     reverse_goDLS_function,
 )
+from .docket_report import BaseDocketReport
 from .reports import BaseReport
 
 logger = make_default_logger()
 
 
 class FreeOpinionReport(BaseReport):
     """An object for querying and parsing the free opinion report."""
 
     EXCLUDED_COURT_IDS = ["casb", "innb", "miwb", "ohsb"]
     VALID_SORT_PARAMS = ("date_filed", "case_number")
 
-    def __init__(self, court_id, pacer_session):
+    def __init__(self, court_id, pacer_session=None):
         self.responses = []
         self.trees = []
         super().__init__(court_id, pacer_session)
 
     @property
     def url(self):
         if self.court_id == "ohnd":
@@ -104,14 +107,34 @@
             response.raise_for_status()
             set_response_encoding(response)
             text = clean_html(response.text)
             tree = get_html_parsed_text(text)
             tree.rewrite_links(fix_links_in_lxml_tree, base_href=response.url)
             self.trees.append(tree)
 
+    def _parse_text(self, text):
+        """Parse the HTML as unicode text and set self.tree
+
+        This is a particularly critical method when running tests, which pull
+        from local disk instead of from a query response. This is also used
+        when data comes from a source other than self.query() (such as a user
+        upload). This method should probably be made public as .parse_text().
+
+        :param text: A unicode object
+        :return: None
+        """
+        assert isinstance(
+            text, str
+        ), f"Input must be unicode, not {type(text)}"
+        text = clean_html(text)
+        self.tree = get_html_parsed_text(text)
+        self._strip_bad_html_tags_insecure(text)
+        self.tree.rewrite_links(fix_links_in_lxml_tree, base_href=self.url)
+        self.trees.append(self.tree)
+
     @property
     def data(self):
         results = []
         for tree in self.trees:
             opinion_count = int(
                 tree.xpath(
                     '//b[contains(text(), "Total number of '
@@ -124,15 +147,15 @@
             for row in rows:
                 if results:
                     # If we have results already, pass the previous result to
                     # the FreeOpinionRow object.
                     row = FreeOpinionRow(row, results[-1], self.court_id)
                 else:
                     row = FreeOpinionRow(row, {}, self.court_id)
-                results.append(row)
+                results.append(row.data)
         logger.info(
             "Parsed %s results from written opinions report at %s",
             len(results),
             self.court_id,
         )
         return results
 
@@ -144,15 +167,15 @@
         else:
             raise ValueError(
                 "Invalid sort parameter. Value must be one of: %s"
                 % ", ".join(self.VALID_SORT_PARAMS)
             )
 
 
-class FreeOpinionRow:
+class FreeOpinionRow(BaseDocketReport):
     """A row in the Free Opinions report.
 
     For the most part this is fairly straightforward, however eight courts have
     a different type of report that only has four columns instead of the usual
     five (hib, deb, njb, ndb, ohnb, txsb, txwb, vaeb), and a couple courts
     (areb & arwb) have five columns, but are designed more like the four column
     variants.
@@ -177,45 +200,56 @@
         Joe v. Volcano | 12/31/2008 | 128 | The first doc from case | More here
                        | 12/31/2008 | 129 | The 2nd doc from case   | More here
 
         By having the values from the previous row, we can be sure to be able
         to complete the empty cells.
 
         """
-        super().__init__()
+        super().__init__(court_id)
+        self._metadata = None
         self.element = element
         self.last_good_row = last_good_row
         self.court_id = court_id
         self._column_count = self._get_column_count()
         self._sort_order = self._detect_sort_order()
+        self.docket_number = self._parse_docket_number_strs(
+            [self.get_docket_number()]
+        )
+
+    def __str__(self):
+        return f"<FreeOpinionRow in {self.court_id}>\n{self.data}"
+
+    @property
+    def metadata(self):
+        if self._metadata is not None:
+            return self._metadata
 
-        # Parsed data
         results = self.get_pacer_case_id_and_pacer_seq_no()
-        self.pacer_case_id, self.pacer_seq_no = results[0], results[1]
-        self.docket_number = self.get_docket_number()
-        self.case_name = self.get_case_name()
-        self.date_filed = self.get_date_filed()
-        self.pacer_doc_id = self.get_pacer_doc_id()
-        self.document_number = self.get_document_number()
-        self.description = self.get_description()
-        self.nature_of_suit = self.get_nos()
-        self.cause = self.get_cause()
+        data = {
+            "court_id": self.court_id,
+            "pacer_case_id": results[0],
+            "pacer_seq_no": results[1],
+            "docket_number": self.docket_number,
+            "case_name": self.get_case_name(),
+            "date_filed": self.get_date_filed(),
+            "pacer_doc_id": self.get_pacer_doc_id(),
+            "document_number": self.get_document_number(),
+            "description": self.get_description(),
+            "nature_of_suit": self.get_nos(),
+            "cause": self.get_cause(),
+        }
 
-    def __str__(self):
-        return "<FreeOpinionRow in {}>\n{}".format(
-            self.court_id,
-            {
-                "pacer_case_id": self.pacer_case_id,
-                "docket_number": self.docket_number,
-                "case_name": self.case_name,
-                "date_filed": self.date_filed,
-                "pacer_doc_id": self.pacer_doc_id,
-                "document_number": self.document_number,
-            },
-        )
+        self._metadata = data
+        return data
+
+    @property
+    def data(self):
+        """Get all the data back from this endpoint."""
+        data = self.metadata.copy()
+        return data
 
     def _get_column_count(self):
         return len(self.element.xpath("./td"))
 
     def _detect_sort_order(self):
         """Detect whether the report is ordered by case number or by date filed.
 
@@ -266,28 +300,28 @@
             except IndexError:
                 logger.info(
                     "No content provided in first cell of row. Using "
                     "last good row for pacer_case_id, docket_number, "
                     "and case_name."
                 )
                 last_row = self.last_good_row
-                return last_row.pacer_case_id, last_row.pacer_seq_no
+                return last_row["pacer_case_id"], last_row["pacer_seq_no"]
         elif self._sort_order == "date_filed":
             href = self.element.xpath("./td[2]//@href")[0]
         return get_pacer_case_id_from_nonce_url(href), None
 
     def get_docket_number(self):
         try:
             if self._sort_order == "case_number":
                 cell = self.element.xpath("./td[1]//a")[0]
             else:
                 cell = self.element.xpath("./td[2]//a")[0]
         except IndexError:
             # No content in the cell.
-            return self.last_good_row.docket_number
+            return self.last_good_row["docket_number"]
         else:
             s = cell.text_content().strip()
 
         if self._column_count == 4 or self.court_id in ["areb", "arwb"]:
             # In this case s will be something like:
             #   14-90018 Stewart v. Kauanui
             # Split on the first space, left is docket number, right
@@ -299,26 +333,28 @@
     def get_case_name(self):
         if self._sort_order == "case_number":
             cell = self.element.xpath("./td[1]")[0]
         else:
             cell = self.element.xpath("./td[2]")[0]
         s = cell.text_content().strip()
         if not s:
-            return self.last_good_row.case_name
+            return clean_string(harmonize(self.last_good_row["case_name"]))
 
         if self._column_count == 4 or self.court_id in ["areb", "arwb"]:
             # See note in docket number
             try:
-                return s.split(" ", 1)[1]
+                return clean_string(harmonize(s.split(" ", 1)[1]))
             except IndexError:
                 # No case name, but a docket number is provided.
                 return "Case name unknown"
         else:
             try:
-                return cell.xpath(".//b")[0].text_content()
+                return clean_string(
+                    harmonize(cell.xpath(".//b")[0].text_content())
+                )
             except IndexError:
                 logger.warning(
                     "Unable to get case name for %s in %s.",
                     self.docket_number,
                     self.court_id,
                 )
                 return "Case name unknown"
@@ -327,15 +363,15 @@
         if self._sort_order == "case_number":
             path = "./td[2]//text()"
         elif self._sort_order == "date_filed":
             path = "./td[1]//text()"
         s = self.element.xpath(path)[0]
         if not s.strip() and self._sort_order == "date_filed":
             # Empty cell, return the previous value.
-            return self.last_good_row.date_filed
+            return self.last_good_row["date_filed"]
         else:
             return convert_date_string(s)
 
     def get_pacer_doc_id(self):
         doc1_url = self.element.xpath("./td[3]//@href")[0]
         return get_pacer_doc_id_from_doc1_url(doc1_url)
 
@@ -360,7 +396,27 @@
             return ""
         try:
             return self.element.xpath(
                 "./td[5]/i[contains(./text(), " '"Cause")]'
             )[0].tail.strip()
         except IndexError:
             return ""
+
+
+def _main():
+    if len(sys.argv) != 2:
+        print("Usage: python -m juriscraper.pacer.docket_report filepath")
+        print("Please provide a path to an HTML file to parse.")
+        sys.exit(1)
+    report = FreeOpinionReport(
+        "cand", None
+    )  # Court ID is only needed for querying.
+    filepath = sys.argv[1]
+    print(f"Parsing HTML file at {filepath}")
+    with open(filepath) as f:
+        text = f.read()
+    report._parse_text(text)
+    pprint.pprint(report.data, indent=2)
+
+
+if __name__ == "__main__":
+    _main()
```

### Comparing `juriscraper-2.5.95/juriscraper/pacer/hidden_api.py` & `juriscraper-2.6.0/juriscraper/pacer/hidden_api.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/http.py` & `juriscraper-2.6.0/juriscraper/pacer/http.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/internet_archive.py` & `juriscraper-2.6.0/juriscraper/pacer/internet_archive.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/list_of_creditors.py` & `juriscraper-2.6.0/juriscraper/pacer/list_of_creditors.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/mobile_query.py` & `juriscraper-2.6.0/juriscraper/pacer/mobile_query.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/reports.py` & `juriscraper-2.6.0/juriscraper/pacer/reports.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/rss_feeds.py` & `juriscraper-2.6.0/juriscraper/pacer/rss_feeds.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacer/utils.py` & `juriscraper-2.6.0/juriscraper/pacer/utils.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/pacerdocket.py` & `juriscraper-2.6.0/juriscraper/pacerdocket.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper/report.py` & `juriscraper-2.6.0/juriscraper/report.py`

 * *Files identical despite different names*

### Comparing `juriscraper-2.5.95/juriscraper.egg-info/PKG-INFO` & `juriscraper-2.6.0/juriscraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juriscraper
-Version: 2.5.95
+Version: 2.6.0
 Summary: An API to scrape American court websites for metadata.
 Home-page: https://github.com/freelawproject/juriscraper
 Author: Free Law Project
 Author-email: info@free.law
 Maintainer: Free Law Project
 Maintainer-email: info@free.law
 License: BSD
@@ -31,15 +31,15 @@
 Requires-Dist: certifi>=2017.4.17
 Requires-Dist: chardet>=3.0.2
 Requires-Dist: cssselect
 Requires-Dist: dateparser>=1.2.0
 Requires-Dist: feedparser>=6.0.11
 Requires-Dist: geonamescache>=2.0.0
 Requires-Dist: html5lib
-Requires-Dist: lxml>=4.9
+Requires-Dist: lxml>=5.2
 Requires-Dist: nh3
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: requests>=2.20.0
 Requires-Dist: selenium>=4.9.1
 Requires-Dist: tldextract
 
 +---------------+---------------------+-------------------+
```

### Comparing `juriscraper-2.5.95/juriscraper.egg-info/SOURCES.txt` & `juriscraper-2.6.0/juriscraper.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,16 @@
 juriscraper/opinions/united_states/federal_special/acca_p.py
 juriscraper/opinions/united_states/federal_special/acca_summary.py
 juriscraper/opinions/united_states/federal_special/afcca.py
 juriscraper/opinions/united_states/federal_special/ag.py
 juriscraper/opinions/united_states/federal_special/armfor.py
 juriscraper/opinions/united_states/federal_special/cavc.py
 juriscraper/opinions/united_states/federal_special/cit.py
+juriscraper/opinions/united_states/federal_special/fisc.py
+juriscraper/opinions/united_states/federal_special/fiscr.py
 juriscraper/opinions/united_states/federal_special/nmcca.py
 juriscraper/opinions/united_states/federal_special/tax.py
 juriscraper/opinions/united_states/federal_special/uscfc.py
 juriscraper/opinions/united_states/federal_special/uscfc_u.py
 juriscraper/opinions/united_states/federal_special/uscfc_vaccine.py
 juriscraper/opinions/united_states/federal_special/uscfc_vaccine_u.py
 juriscraper/opinions/united_states/federal_special/uscgcoca.py
```

### Comparing `juriscraper-2.5.95/setup.py` & `juriscraper-2.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import codecs
 import os
 import unittest
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
-VERSION = "2.5.95"
+VERSION = "2.6.0"
 AUTHOR = "Free Law Project"
 EMAIL = "info@free.law"
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 
 reqs_path = f"{HERE}/requirements.txt"
 with open(reqs_path) as reqs_file:
```

