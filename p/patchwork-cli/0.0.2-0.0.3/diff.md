# Comparing `tmp/patchwork_cli-0.0.2.tar.gz` & `tmp/patchwork_cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchwork_cli-0.0.2.tar", max compression
+gzip compressed data, was "patchwork_cli-0.0.3.tar", max compression
```

## Comparing `patchwork_cli-0.0.2.tar` & `patchwork_cli-0.0.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0    34522 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     5125 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/__main__.py
--rw-r--r--   0        0        0     2857 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/app.py
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/common/client/__init__.py
--rw-r--r--   0        0        0    12412 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/common/client/scm.py
--rw-r--r--   0        0        0      816 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/common/utils.py
--rw-r--r--   0        0        0     1550 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/logger.py
--rw-r--r--   0        0        0      168 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/managed_files.py
--rw-r--r--   0        0        0     2783 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/AutoFix/AutoFix.py
--rw-r--r--   0        0        0     2182 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/AutoFix/default_prompt.json
--rw-r--r--   0        0        0      809 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/AutoFix/defaults.yml
--rw-r--r--   0        0        0     5442 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/DependencyUpgrade/DependencyUpgrade.py
--rw-r--r--   0        0        0      704 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/DependencyUpgrade/defaults.yml
--rw-r--r--   0        0        0     2409 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
--rw-r--r--   0        0        0     2218 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/GenerateREADME/GenerateREADME.py
--rw-r--r--   0        0        0      612 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/GenerateREADME/defaults.yml
--rw-r--r--   0        0        0      484 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/GenerateREADME/generate_readme_prompt.json
--rw-r--r--   0        0        0     3559 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/PRReview/PRReview.py
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/PRReview/__init__.py
--rw-r--r--   0        0        0      608 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/PRReview/defaults.yml
--rw-r--r--   0        0        0      557 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/PRReview/pr_review_prompt.json
--rw-r--r--   0        0        0     2169 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/README.md
--rw-r--r--   0        0        0      276 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/patchflows/__init__.py
--rw-r--r--   0        0        0      499 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/step.py
--rw-r--r--   0        0        0     5978 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/AnalyzeImpact/AnalyzeImpact.py
--rw-r--r--   0        0        0     1205 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/AnalyzeImpact/README.md
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/AnalyzeImpact/__init__.py
--rw-r--r--   0        0        0     2445 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CallCode2Prompt/CallCode2Prompt.py
--rw-r--r--   0        0        0      967 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CallCode2Prompt/README.md
--rw-r--r--   0        0        0      579 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CallCode2Prompt/TestCallCode2Prompt.py
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CallCode2Prompt/__init__.py
--rw-r--r--   0        0        0     2830 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CallOpenAI/CallOpenAI.py
--rw-r--r--   0        0        0      503 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CallOpenAI/README.md
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CallOpenAI/__init__.py
--rw-r--r--   0        0        0     5263 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CommitChanges/CommitChanges.py
--rw-r--r--   0        0        0     1106 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CommitChanges/README.md
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CommitChanges/__init__.py
--rw-r--r--   0        0        0     3919 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CreatePR/CreatePR.py
--rw-r--r--   0        0        0     1279 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CreatePR/README.md
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CreatePR/__init__.py
--rw-r--r--   0        0        0     1370 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CreatePRComment/CreatePRComment.py
--rw-r--r--   0        0        0      621 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CreatePRComment/README.md
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/CreatePRComment/__init__.py
--rw-r--r--   0        0        0     8858 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/ExtractCode.py
--rw-r--r--   0        0        0      755 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/README.md
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/context_strategy/__init__.py
--rw-r--r--   0        0        0     2585 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/context_strategy/context_strategies.py
--rw-r--r--   0        0        0      593 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/context_strategy/generic.py
--rw-r--r--   0        0        0     1491 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/context_strategy/java.py
--rw-r--r--   0        0        0     2442 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/context_strategy/javascript.py
--rw-r--r--   0        0        0      281 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/context_strategy/protocol.py
--rw-r--r--   0        0        0     2885 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/context_strategy/python.py
--rw-r--r--   0        0        0     8888 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractDiff/ExtractDiff.py
--rw-r--r--   0        0        0      833 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractDiff/README.md
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractDiff/__init__.py
--rw-r--r--   0        0        0     1655 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractModelResponse/ExtractModelResponse.py
--rw-r--r--   0        0        0     1318 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractModelResponse/README.md
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractModelResponse/__init__.py
--rw-r--r--   0        0        0    12064 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
--rw-r--r--   0        0        0     1765 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractPackageManagerFile/README.md
--rw-r--r--   0        0        0     6177 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ExtractPackageManagerFile/__init__.py
--rw-r--r--   0        0        0     3263 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ModifyCode/ModifyCode.py
--rw-r--r--   0        0        0     1045 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ModifyCode/README.md
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ModifyCode/__init__.py
--rw-r--r--   0        0        0     3130 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/PreparePR/PreparePR.py
--rw-r--r--   0        0        0      743 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/PreparePR/README.md
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/PreparePR/__init__.py
--rw-r--r--   0        0        0     3190 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/PreparePrompt/PreparePrompt.py
--rw-r--r--   0        0        0     1274 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/PreparePrompt/README.md
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/PreparePrompt/__init__.py
--rw-r--r--   0        0        0     1655 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/README.md
--rw-r--r--   0        0        0      903 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ReadPRDiffs/README.md
--rw-r--r--   0        0        0     1399 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ReadPRDiffs/ReadPRDiffs.py
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.946744 patchwork_cli-0.0.2/patchwork_cli/steps/ReadPRDiffs/__init__.py
--rw-r--r--   0        0        0     1588 2024-04-03 02:05:09.950744 patchwork_cli-0.0.2/patchwork_cli/steps/ScanDepscan/README.md
--rw-r--r--   0        0        0     4752 2024-04-03 02:05:09.950744 patchwork_cli-0.0.2/patchwork_cli/steps/ScanDepscan/ScanDepscan.py
--rw-r--r--   0        0        0     2030 2024-04-03 02:05:09.950744 patchwork_cli-0.0.2/patchwork_cli/steps/ScanDepscan/TestScanDepscan.py
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.950744 patchwork_cli-0.0.2/patchwork_cli/steps/ScanDepscan/__init__.py
--rw-r--r--   0        0        0      677 2024-04-03 02:05:09.950744 patchwork_cli-0.0.2/patchwork_cli/steps/ScanSemgrep/README.md
--rw-r--r--   0        0        0     1063 2024-04-03 02:05:09.950744 patchwork_cli-0.0.2/patchwork_cli/steps/ScanSemgrep/ScanSemgrep.py
--rw-r--r--   0        0        0        0 2024-04-03 02:05:09.950744 patchwork_cli-0.0.2/patchwork_cli/steps/ScanSemgrep/__init__.py
--rw-r--r--   0        0        0     1545 2024-04-03 02:05:09.950744 patchwork_cli-0.0.2/patchwork_cli/steps/__init__.py
--rw-r--r--   0        0        0     1597 2024-04-03 02:05:09.950744 patchwork_cli-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6274 1970-01-01 00:00:00.000000 patchwork_cli-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34522 2024-04-02 03:23:14.301159 patchwork_cli-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     5115 2024-04-04 04:10:24.325019 patchwork_cli-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.325070 patchwork_cli-0.0.3/patchwork/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.325169 patchwork_cli-0.0.3/patchwork/__main__.py
+-rw-r--r--   0        0        0     2849 2024-04-04 04:10:24.326540 patchwork_cli-0.0.3/patchwork/app.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.326608 patchwork_cli-0.0.3/patchwork/common/client/__init__.py
+-rw-r--r--   0        0        0    12408 2024-04-04 04:10:24.326830 patchwork_cli-0.0.3/patchwork/common/client/scm.py
+-rw-r--r--   0        0        0      816 2024-04-04 04:10:24.326964 patchwork_cli-0.0.3/patchwork/common/utils.py
+-rw-r--r--   0        0        0     1546 2024-04-04 04:10:24.327093 patchwork_cli-0.0.3/patchwork/logger.py
+-rw-r--r--   0        0        0      168 2024-04-04 04:10:24.327205 patchwork_cli-0.0.3/patchwork/managed_files.py
+-rw-r--r--   0        0        0     2775 2024-04-04 04:10:24.327337 patchwork_cli-0.0.3/patchwork/patchflows/AutoFix/AutoFix.py
+-rw-r--r--   0        0        0     2182 2024-04-04 04:10:24.327457 patchwork_cli-0.0.3/patchwork/patchflows/AutoFix/default_prompt.json
+-rw-r--r--   0        0        0      809 2024-04-04 04:10:24.327567 patchwork_cli-0.0.3/patchwork/patchflows/AutoFix/defaults.yml
+-rw-r--r--   0        0        0     5434 2024-04-04 04:10:24.327717 patchwork_cli-0.0.3/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py
+-rw-r--r--   0        0        0      704 2024-04-04 04:10:24.327912 patchwork_cli-0.0.3/patchwork/patchflows/DependencyUpgrade/defaults.yml
+-rw-r--r--   0        0        0     2409 2024-04-04 04:10:24.328054 patchwork_cli-0.0.3/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
+-rw-r--r--   0        0        0     2210 2024-04-04 04:10:24.328186 patchwork_cli-0.0.3/patchwork/patchflows/GenerateREADME/GenerateREADME.py
+-rw-r--r--   0        0        0      612 2024-04-04 04:10:24.328301 patchwork_cli-0.0.3/patchwork/patchflows/GenerateREADME/defaults.yml
+-rw-r--r--   0        0        0      484 2024-04-04 04:10:24.328415 patchwork_cli-0.0.3/patchwork/patchflows/GenerateREADME/generate_readme_prompt.json
+-rw-r--r--   0        0        0     3551 2024-04-04 04:10:24.328546 patchwork_cli-0.0.3/patchwork/patchflows/PRReview/PRReview.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.328578 patchwork_cli-0.0.3/patchwork/patchflows/PRReview/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-04 04:10:24.328738 patchwork_cli-0.0.3/patchwork/patchflows/PRReview/defaults.yml
+-rw-r--r--   0        0        0      557 2024-04-04 04:10:24.328850 patchwork_cli-0.0.3/patchwork/patchflows/PRReview/pr_review_prompt.json
+-rw-r--r--   0        0        0     2163 2024-04-04 04:10:24.328995 patchwork_cli-0.0.3/patchwork/patchflows/README.md
+-rw-r--r--   0        0        0      276 2024-04-04 04:10:24.329097 patchwork_cli-0.0.3/patchwork/patchflows/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-04 04:10:24.329202 patchwork_cli-0.0.3/patchwork/step.py
+-rw-r--r--   0        0        0     5970 2024-04-04 04:10:24.329355 patchwork_cli-0.0.3/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py
+-rw-r--r--   0        0        0     1205 2024-04-04 04:10:24.329481 patchwork_cli-0.0.3/patchwork/steps/AnalyzeImpact/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.329529 patchwork_cli-0.0.3/patchwork/steps/AnalyzeImpact/__init__.py
+-rw-r--r--   0        0        0     2437 2024-04-04 04:10:24.329709 patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py
+-rw-r--r--   0        0        0      967 2024-04-04 04:10:24.329832 patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/README.md
+-rw-r--r--   0        0        0      575 2024-04-04 04:10:24.329947 patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.329981 patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/__init__.py
+-rw-r--r--   0        0        0     2822 2024-04-04 04:10:24.330160 patchwork_cli-0.0.3/patchwork/steps/CallOpenAI/CallOpenAI.py
+-rw-r--r--   0        0        0      503 2024-04-04 04:10:24.330285 patchwork_cli-0.0.3/patchwork/steps/CallOpenAI/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.330316 patchwork_cli-0.0.3/patchwork/steps/CallOpenAI/__init__.py
+-rw-r--r--   0        0        0     5255 2024-04-04 04:10:24.330494 patchwork_cli-0.0.3/patchwork/steps/CommitChanges/CommitChanges.py
+-rw-r--r--   0        0        0     1106 2024-04-04 04:10:24.330605 patchwork_cli-0.0.3/patchwork/steps/CommitChanges/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.330636 patchwork_cli-0.0.3/patchwork/steps/CommitChanges/__init__.py
+-rw-r--r--   0        0        0     3907 2024-04-04 04:10:24.330809 patchwork_cli-0.0.3/patchwork/steps/CreatePR/CreatePR.py
+-rw-r--r--   0        0        0     1279 2024-04-04 04:10:24.330922 patchwork_cli-0.0.3/patchwork/steps/CreatePR/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.330952 patchwork_cli-0.0.3/patchwork/steps/CreatePR/__init__.py
+-rw-r--r--   0        0        0     1358 2024-04-04 04:10:24.331210 patchwork_cli-0.0.3/patchwork/steps/CreatePRComment/CreatePRComment.py
+-rw-r--r--   0        0        0      621 2024-04-04 04:10:24.331316 patchwork_cli-0.0.3/patchwork/steps/CreatePRComment/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.331443 patchwork_cli-0.0.3/patchwork/steps/CreatePRComment/__init__.py
+-rw-r--r--   0        0        0     8850 2024-04-04 04:10:24.331758 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/ExtractCode.py
+-rw-r--r--   0        0        0      755 2024-04-04 04:10:24.331913 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.331952 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.332032 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/__init__.py
+-rw-r--r--   0        0        0     2585 2024-04-04 04:10:24.332199 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/context_strategies.py
+-rw-r--r--   0        0        0      593 2024-04-04 04:10:24.332325 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/generic.py
+-rw-r--r--   0        0        0     1491 2024-04-04 04:10:24.332433 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/java.py
+-rw-r--r--   0        0        0     2442 2024-04-04 04:10:24.332544 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/javascript.py
+-rw-r--r--   0        0        0      281 2024-04-04 04:10:24.332732 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/protocol.py
+-rw-r--r--   0        0        0     2885 2024-04-04 04:10:24.332877 patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/python.py
+-rw-r--r--   0        0        0     8880 2024-04-04 04:10:24.333049 patchwork_cli-0.0.3/patchwork/steps/ExtractDiff/ExtractDiff.py
+-rw-r--r--   0        0        0      833 2024-04-04 04:10:24.333176 patchwork_cli-0.0.3/patchwork/steps/ExtractDiff/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.333207 patchwork_cli-0.0.3/patchwork/steps/ExtractDiff/__init__.py
+-rw-r--r--   0        0        0     1647 2024-04-04 04:10:24.333385 patchwork_cli-0.0.3/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py
+-rw-r--r--   0        0        0     1318 2024-04-04 04:10:24.333529 patchwork_cli-0.0.3/patchwork/steps/ExtractModelResponse/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.333560 patchwork_cli-0.0.3/patchwork/steps/ExtractModelResponse/__init__.py
+-rw-r--r--   0        0        0    12367 2024-04-04 04:10:24.333765 patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
+-rw-r--r--   0        0        0     1765 2024-04-04 04:10:24.333884 patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/README.md
+-rw-r--r--   0        0        0     6173 2024-04-04 04:10:24.334021 patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.334052 patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/__init__.py
+-rw-r--r--   0        0        0     3255 2024-04-04 04:10:24.334221 patchwork_cli-0.0.3/patchwork/steps/ModifyCode/ModifyCode.py
+-rw-r--r--   0        0        0     1045 2024-04-04 04:10:24.334344 patchwork_cli-0.0.3/patchwork/steps/ModifyCode/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.334374 patchwork_cli-0.0.3/patchwork/steps/ModifyCode/__init__.py
+-rw-r--r--   0        0        0     3122 2024-04-04 04:10:24.334523 patchwork_cli-0.0.3/patchwork/steps/PreparePR/PreparePR.py
+-rw-r--r--   0        0        0      743 2024-04-04 04:10:24.334875 patchwork_cli-0.0.3/patchwork/steps/PreparePR/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.334943 patchwork_cli-0.0.3/patchwork/steps/PreparePR/__init__.py
+-rw-r--r--   0        0        0     3182 2024-04-04 04:10:24.335255 patchwork_cli-0.0.3/patchwork/steps/PreparePrompt/PreparePrompt.py
+-rw-r--r--   0        0        0     1274 2024-04-04 04:10:24.335372 patchwork_cli-0.0.3/patchwork/steps/PreparePrompt/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.335405 patchwork_cli-0.0.3/patchwork/steps/PreparePrompt/__init__.py
+-rw-r--r--   0        0        0     1652 2024-04-04 04:10:24.335557 patchwork_cli-0.0.3/patchwork/steps/README.md
+-rw-r--r--   0        0        0      903 2024-04-04 04:10:24.335681 patchwork_cli-0.0.3/patchwork/steps/ReadPRDiffs/README.md
+-rw-r--r--   0        0        0     1387 2024-04-04 04:10:24.335793 patchwork_cli-0.0.3/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.335826 patchwork_cli-0.0.3/patchwork/steps/ReadPRDiffs/__init__.py
+-rw-r--r--   0        0        0     1588 2024-04-04 04:10:24.335982 patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/README.md
+-rw-r--r--   0        0        0     4744 2024-04-04 04:10:24.336123 patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/ScanDepscan.py
+-rw-r--r--   0        0        0     2026 2024-04-04 04:10:24.336229 patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/TestScanDepscan.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.336258 patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/__init__.py
+-rw-r--r--   0        0        0      677 2024-04-04 04:10:24.336398 patchwork_cli-0.0.3/patchwork/steps/ScanSemgrep/README.md
+-rw-r--r--   0        0        0     1055 2024-04-04 04:10:24.336499 patchwork_cli-0.0.3/patchwork/steps/ScanSemgrep/ScanSemgrep.py
+-rw-r--r--   0        0        0        0 2024-04-04 04:10:24.336528 patchwork_cli-0.0.3/patchwork/steps/ScanSemgrep/__init__.py
+-rw-r--r--   0        0        0     1481 2024-04-04 04:10:24.336660 patchwork_cli-0.0.3/patchwork/steps/__init__.py
+-rw-r--r--   0        0        0     1555 2024-04-04 04:10:24.337840 patchwork_cli-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6258 1970-01-01 00:00:00.000000 patchwork_cli-0.0.3/PKG-INFO
```

### Comparing `patchwork_cli-0.0.2/LICENSE.txt` & `patchwork_cli-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/README.md` & `patchwork_cli-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 ```bash
 patchwork AutoFix openai_api_key=<YOUR_OPENAI_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
 The above command will default to patching code in the current directory, by running Semgrep to identify the vulnerabilities.
 
-You can take a look at the `default.yml` [file](patchwork_cli/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. 
+You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. 
 
 ## PatchWork in CI
 
 You can also run PatchWork in a CI environment with ease:
 
 ### Jenkins CI
 
@@ -98,15 +98,15 @@
   pull_request: {}
   # Patch on-demand through GitHub Actions interface:
   workflow_dispatch: {}
 
 jobs:
   patchwork:
     # User definable name of this GitHub Actions job.
-    name: semgrep/ci
+    name: patchwork/ci
     runs-on: ubuntu-latest
 
     container:
       # A Docker image with patchwork installed. Do not change this.
       image: patched-codes/patchwork
 
     steps:
@@ -165,10 +165,10 @@
 }
 ```
 
 Each patchflow comes with an optimized default prompt template. But you can specify your own using the `prompt_template_file=/path/to/prompt/template/file` option. 
 
 ## Contributing
 
-To create a new patchflow, follow [these instructions](patchwork_cli/patchflows/README.md).
+To create a new patchflow, follow [these instructions](patchwork/patchflows/README.md).
 
-To create a new step, follow [these instructions](patchwork_cli/steps/README.md).
+To create a new step, follow [these instructions](patchwork/steps/README.md).
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/app.py` & `patchwork_cli-0.0.3/patchwork/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import importlib
 import json
 from pathlib import Path
 
 import click
 import yaml
 
-from patchwork_cli.logger import init_cli_logger, logger
+from patchwork.logger import init_cli_logger, logger
 
 
 @click.command(
     context_settings=dict(
         ignore_unknown_options=True,
     )
 )
@@ -37,15 +37,15 @@
 @click.argument("patchflow", nargs=1, required=True)
 @click.argument("opts", nargs=-1, type=click.UNPROCESSED, required=False)
 @click.option("--config", type=click.Path(exists=True, dir_okay=True, resolve_path=True, file_okay=True))
 @click.option("--output", type=click.Path(exists=False, resolve_path=True, writable=True), help="Output data file")
 @click.option("data_format", "--format", type=click.Choice(["yaml", "json"]), default="json", help="Output data format")
 def cli(log: str, patchflow: str, opts: list[str], config: str | None, output: str | None, data_format: str):
     try:
-        module = importlib.import_module(f".patchflows", "patchwork_cli")
+        module = importlib.import_module(f".patchflows", "patchwork")
     except ModuleNotFoundError:
         logger.debug(f"Patchflow {patchflow} not found")
         exit(1)
 
     try:
         patchflow_class = getattr(module, patchflow)
     except AttributeError:
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/common/client/scm.py` & `patchwork_cli-0.0.3/patchwork/common/client/scm.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Protocol
 
 import gitlab.const
 from github import Auth, Consts, Github, GithubException, PullRequest
 from gitlab import Gitlab, GitlabAuthenticationError, GitlabError
 from gitlab.v4.objects import ProjectMergeRequest
 
-from patchwork_cli.logger import logger
+from patchwork.logger import logger
 
 
 @dataclass(slots=True)
 class Comment:
     path: str
     body: str
     start_line: int | None
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/common/utils.py` & `patchwork_cli-0.0.3/patchwork/common/utils.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/logger.py` & `patchwork_cli-0.0.3/patchwork/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Callable
 
 import click
 
-from patchwork_cli.managed_files import LOG_FILE
+from patchwork.managed_files import LOG_FILE
 
 # default noop logger
 logger = logging.getLogger("patched")
 _noop = logging.NullHandler()
 logger.addHandler(_noop)
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/patchflows/AutoFix/AutoFix.py` & `patchwork_cli-0.0.3/patchwork/patchflows/AutoFix/AutoFix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from pathlib import Path
 
 import yaml
 
-from patchwork_cli.step import Step
-from patchwork_cli.steps import (
+from patchwork.step import Step
+from patchwork.steps import (
     CallOpenAI,
     CommitChanges,
     CreatePR,
     ExtractCode,
     ExtractModelResponse,
     ModifyCode,
     PreparePR,
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/patchflows/AutoFix/default_prompt.json` & `patchwork_cli-0.0.3/patchwork/patchflows/AutoFix/default_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/patchflows/AutoFix/defaults.yml` & `patchwork_cli-0.0.3/patchwork/patchflows/AutoFix/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/patchflows/DependencyUpgrade/DependencyUpgrade.py` & `patchwork_cli-0.0.3/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import json
 from pathlib import Path
 
 import yaml
 
-from patchwork_cli.step import Step
-from patchwork_cli.steps import (
+from patchwork.step import Step
+from patchwork.steps import (
     AnalyzeImpact,
     CallOpenAI,
     CommitChanges,
     CreatePR,
     ExtractDiff,
     ExtractModelResponse,
     ExtractPackageManagerFile,
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/patchflows/DependencyUpgrade/defaults.yml` & `patchwork_cli-0.0.3/patchwork/patchflows/DependencyUpgrade/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json` & `patchwork_cli-0.0.3/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/patchflows/GenerateREADME/GenerateREADME.py` & `patchwork_cli-0.0.3/patchwork/patchflows/GenerateREADME/GenerateREADME.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 import yaml
 
-from patchwork_cli.step import Step
-from patchwork_cli.steps import (
+from patchwork.step import Step
+from patchwork.steps import (
     CallCode2Prompt,
     CallOpenAI,
     CommitChanges,
     CreatePR,
     ExtractModelResponse,
     ModifyCode,
     PreparePR,
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/patchflows/GenerateREADME/defaults.yml` & `patchwork_cli-0.0.3/patchwork/patchflows/GenerateREADME/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/patchflows/PRReview/PRReview.py` & `patchwork_cli-0.0.3/patchwork/patchflows/PRReview/PRReview.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 import yaml
 
-from patchwork_cli.step import Step
-from patchwork_cli.steps import (
+from patchwork.step import Step
+from patchwork.steps import (
     CallOpenAI,
     CreatePRComment,
     ExtractModelResponse,
     PreparePR,
     PreparePrompt,
     ReadPRDiffs,
 )
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/patchflows/PRReview/defaults.yml` & `patchwork_cli-0.0.3/patchwork/patchflows/PRReview/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/patchflows/PRReview/pr_review_prompt.json` & `patchwork_cli-0.0.3/patchwork/patchflows/PRReview/pr_review_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/patchflows/README.md` & `patchwork_cli-0.0.3/patchwork/patchflows/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,21 +14,24 @@
 3. Update `patchwork/patchflows/__init__.py` to include the new patchflow by importing the class `MyPatchflow` and adding it to `__all__`.
 
 ## Example
 
 ### Path: `patchwork/patchflows/MyPatchflow/MyPatchflow.py`
 
 ```python
-from patchwork_cli.step import Step
-from patchwork_cli.steps import {
+from patchwork.step import Step
+from patchwork.steps import
+
+{
     Step1,
     Step2,
     Step3
 }
 
+
 class MyPatchflow(Step):
     def __init__(self, inputs):
         super().__init__(inputs)
 
         if 'input1' not in inputs:
             raise ValueError("Missing required input: input1")
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/AnalyzeImpact/AnalyzeImpact.py` & `patchwork_cli-0.0.3/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import tempfile
 from pathlib import Path
 
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 _PURL_TO_LANGUAGE_ = {
     "pypi": "python",
     "npm": "javascript",
     "maven": "java",
     "golang": "go",
     "gem": "ruby",
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/AnalyzeImpact/README.md` & `patchwork_cli-0.0.3/patchwork/steps/AnalyzeImpact/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/CallCode2Prompt/CallCode2Prompt.py` & `patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 import subprocess
 import tempfile
 from pathlib import Path
 
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 FOLDER_PATH = "folder_path"
 
 
 class CallCode2Prompt(Step):
     required_keys = {FOLDER_PATH}
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/CallCode2Prompt/README.md` & `patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/CallCode2Prompt/TestCallCode2Prompt.py` & `patchwork_cli-0.0.3/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from pathlib import Path
 
-from patchwork_cli.steps import CallCode2Prompt
+from patchwork.steps import CallCode2Prompt
 
 
 class TestCallCode2Prompt(unittest.TestCase):
     def test_run(self):
         inputs = {}
         folder_path = Path.cwd()
         inputs["folder_path"] = folder_path
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/CallOpenAI/CallOpenAI.py` & `patchwork_cli-0.0.3/patchwork/steps/CallOpenAI/CallOpenAI.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import tempfile
 from pathlib import Path
 from pprint import pformat
 from textwrap import indent
 
 from openai import OpenAI
 
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 
 class CallOpenAI(Step):
     required_keys = {"openai_api_key", "prompt_file"}
 
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/CommitChanges/CommitChanges.py` & `patchwork_cli-0.0.3/patchwork/steps/CommitChanges/CommitChanges.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import contextlib
 from pathlib import Path
 from typing import Generator
 
 import git
 from git import Head, Repo
 
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 
 def get_slug_from_remote_url(remote_url: str) -> str:
     # TODO: consider using https://github.com/nephila/giturlparse instead
     if remote_url.startswith("git@"):
         # ssh
         _, _, potential_slug = remote_url.partition(":")
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/CommitChanges/README.md` & `patchwork_cli-0.0.3/patchwork/steps/CommitChanges/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/CreatePR/CreatePR.py` & `patchwork_cli-0.0.3/patchwork/steps/CreatePR/CreatePR.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pathlib import Path
 
 import git
 
-from patchwork_cli.common.client.scm import (
+from patchwork.common.client.scm import (
     GithubClient,
     GitlabClient,
     ScmPlatformClientProtocol,
 )
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 
 def get_slug_from_remote_url(remote_url: str) -> str:
     # TODO: consider using https://github.com/nephila/giturlparse instead
     if remote_url.startswith("git@"):
         # ssh
         _, _, potential_slug = remote_url.partition(":")
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/CreatePR/README.md` & `patchwork_cli-0.0.3/patchwork/steps/CreatePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/CreatePRComment/CreatePRComment.py` & `patchwork_cli-0.0.3/patchwork/steps/CreatePRComment/CreatePRComment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from patchwork_cli.common.client.scm import GithubClient, GitlabClient
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.common.client.scm import GithubClient, GitlabClient
+from patchwork.logger import logger
+from patchwork.step import Step
 
 
 class CreatePRComment(Step):
     required_keys = {"pr_url", "pr_comments"}
 
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/CreatePRComment/README.md` & `patchwork_cli-0.0.3/patchwork/steps/CreatePRComment/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/ExtractCode.py` & `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/ExtractCode.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import tempfile
 from collections import defaultdict
 from pathlib import Path
 from urllib.parse import urlparse
 
 import tiktoken
 
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 from ...common.utils import open_with_chardet
 from .context_strategy.context_strategies import ContextStrategies
 
 _ENCODING = tiktoken.get_encoding("cl100k_base")
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/README.md` & `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/context_strategy/context_strategies.py` & `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/context_strategies.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/context_strategy/generic.py` & `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/generic.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/context_strategy/java.py` & `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/java.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/context_strategy/javascript.py` & `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/javascript.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractCode/context_strategy/python.py` & `patchwork_cli-0.0.3/patchwork/steps/ExtractCode/context_strategy/python.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractDiff/ExtractDiff.py` & `patchwork_cli-0.0.3/patchwork/steps/ExtractDiff/ExtractDiff.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import tempfile
 from pathlib import Path
 from typing import Dict, List
 
 import requests
 from packageurl import PackageURL
 
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 _PURL_TO_LANGUAGE_ = {
     "pypi": "python",
     "npm": "javascript",
     "maven": "java",
     "golang": "go",
     "gem": "ruby",
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractDiff/README.md` & `patchwork_cli-0.0.3/patchwork/steps/ExtractDiff/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractModelResponse/ExtractModelResponse.py` & `patchwork_cli-0.0.3/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import defaultdict
 
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 
 class ExtractModelResponse(Step):
     required_keys = {"openai_responses"}
 
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractModelResponse/README.md` & `patchwork_cli-0.0.3/patchwork/steps/ExtractModelResponse/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py` & `patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import tempfile
 from collections import defaultdict
 from pathlib import Path
 
 import semver
 from packageurl import PackageURL
 
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 # Define a mapping from CVSS severity level strings to numbers
 SEVERITY_LEVELS = {"none": 0, "low": 1, "medium": 2, "high": 3, "critical": 4}
 
 
 def to_semver(version_string):
     """
@@ -170,14 +170,20 @@
                 src_file = self.package_manager_file
             else:
                 found_src_files = find_package_manager_files(Path.cwd(), purl)
                 if len(found_src_files) > 1:
                     logger.info(
                         f"{len(found_src_files)} package manager files found in the current working directory. Use the package_manager_file argument to specify the one to update."
                     )
+                    continue
+                elif len(found_src_files) == 0:
+                    logger.info(
+                        "No package manager files found in the current working directory. Use the package_manager_file argument to specify the file."
+                    )
+                    continue
                 else:
                     src_file = found_src_files[0]
 
             # Add the mapping to the dictionary if both purl and src_file are found
             if purl and src_file:
                 purl_to_srcfile[purl] = src_file
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractPackageManagerFile/README.md` & `patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py` & `patchwork_cli-0.0.3/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import tempfile
 import unittest
 from pathlib import Path
 
-from patchwork_cli.steps import ExtractPackageManagerFile
+from patchwork.steps import ExtractPackageManagerFile
 
 
 class TestExtractPackageManagerFile(unittest.TestCase):
     def test_run(self):
         # Content of a SBOM VDR file
         sbom_vdr_file_content = """{
         "components": [
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ModifyCode/ModifyCode.py` & `patchwork_cli-0.0.3/patchwork/steps/ModifyCode/ModifyCode.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from pathlib import Path
 
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 CODE_SNIPPETS_KEY = "code_file"
 UPDATED_SNIPPETS_KEY = "extracted_responses"
 
 
 def load_json_file(file_path):
     """Utility function to load a json file."""
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ModifyCode/README.md` & `patchwork_cli-0.0.3/patchwork/steps/ModifyCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/PreparePR/PreparePR.py` & `patchwork_cli-0.0.3/patchwork/steps/PreparePR/PreparePR.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import defaultdict
 from textwrap import indent
 
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 
 class PreparePR(Step):
     required_keys = {"modified_code_files"}
 
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/PreparePR/README.md` & `patchwork_cli-0.0.3/patchwork/steps/PreparePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/PreparePrompt/PreparePrompt.py` & `patchwork_cli-0.0.3/patchwork/steps/PreparePrompt/PreparePrompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import tempfile
 from pathlib import Path
 
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 
 class PreparePrompt(Step):
     required_keys = {"prompt_template_file", "prompt_id"}
 
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/PreparePrompt/README.md` & `patchwork_cli-0.0.3/patchwork/steps/PreparePrompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/README.md` & `patchwork_cli-0.0.3/patchwork/steps/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 3. Update `patchwork/steps/__init__.py` to include the new step in the list of available steps.
 
 ## Example
 
 ### Path: `patchwork/steps/RunExample/RunExample.py`
 
 ```python
-from patchwork_cli.step import Step
+from patchwork.step import Step
+
 
 class RunExample(Step):
     required_keys = ['input1', 'input2']
 
     def __init__(self, inputs):
         super().__init__(inputs)
         for key in self.required_keys:
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ReadPRDiffs/README.md` & `patchwork_cli-0.0.3/patchwork/steps/ReadPRDiffs/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ReadPRDiffs/ReadPRDiffs.py` & `patchwork_cli-0.0.3/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import tempfile
 
-from patchwork_cli.common.client.scm import GithubClient, GitlabClient
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.common.client.scm import GithubClient, GitlabClient
+from patchwork.logger import logger
+from patchwork.step import Step
 
 
 class ReadPRDiffs(Step):
     required_keys = {"pr_url"}
 
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ScanDepscan/README.md` & `patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ScanDepscan/ScanDepscan.py` & `patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/ScanDepscan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import subprocess
 import tempfile
 
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 
 def is_cdxgen_installed():
     """Check if cdxgen is installed."""
     try:
         # Attempt to run cdxgen --version to check if it's installed
         subprocess.run(["cdxgen", "--version"], capture_output=True, check=True)
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ScanDepscan/TestScanDepscan.py` & `patchwork_cli-0.0.3/patchwork/steps/ScanDepscan/TestScanDepscan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import tempfile
 import unittest
 from pathlib import Path
 
-from patchwork_cli.steps import ScanDepscan
+from patchwork.steps import ScanDepscan
 
 
 class TestScanDepscan(unittest.TestCase):
     def test_run(self):
         inputs = {}
         # String content to be written to the package.lock file
         package_lock_content = """{
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ScanSemgrep/README.md` & `patchwork_cli-0.0.3/patchwork/steps/ScanSemgrep/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/ScanSemgrep/ScanSemgrep.py` & `patchwork_cli-0.0.3/patchwork/steps/ScanSemgrep/ScanSemgrep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import subprocess
 import tempfile
 from pathlib import Path
 
-from patchwork_cli.logger import logger
-from patchwork_cli.step import Step
+from patchwork.logger import logger
+from patchwork.step import Step
 
 
 class ScanSemgrep(Step):
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
         self.enabled = "sarif_file_path" not in inputs.keys()
```

### Comparing `patchwork_cli-0.0.2/patchwork_cli/steps/__init__.py` & `patchwork_cli-0.0.3/patchwork/steps/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from patchwork_cli.steps.AnalyzeImpact.AnalyzeImpact import AnalyzeImpact
-from patchwork_cli.steps.CallCode2Prompt.CallCode2Prompt import CallCode2Prompt
-from patchwork_cli.steps.CallOpenAI.CallOpenAI import CallOpenAI
-from patchwork_cli.steps.CommitChanges.CommitChanges import CommitChanges
-from patchwork_cli.steps.CreatePR.CreatePR import CreatePR
-from patchwork_cli.steps.CreatePRComment.CreatePRComment import CreatePRComment
-from patchwork_cli.steps.ExtractCode.ExtractCode import ExtractCode
-from patchwork_cli.steps.ExtractDiff.ExtractDiff import ExtractDiff
-from patchwork_cli.steps.ExtractModelResponse.ExtractModelResponse import (
+from patchwork.steps.AnalyzeImpact.AnalyzeImpact import AnalyzeImpact
+from patchwork.steps.CallCode2Prompt.CallCode2Prompt import CallCode2Prompt
+from patchwork.steps.CallOpenAI.CallOpenAI import CallOpenAI
+from patchwork.steps.CommitChanges.CommitChanges import CommitChanges
+from patchwork.steps.CreatePR.CreatePR import CreatePR
+from patchwork.steps.CreatePRComment.CreatePRComment import CreatePRComment
+from patchwork.steps.ExtractCode.ExtractCode import ExtractCode
+from patchwork.steps.ExtractDiff.ExtractDiff import ExtractDiff
+from patchwork.steps.ExtractModelResponse.ExtractModelResponse import (
     ExtractModelResponse,
 )
-from patchwork_cli.steps.ExtractPackageManagerFile.ExtractPackageManagerFile import (
+from patchwork.steps.ExtractPackageManagerFile.ExtractPackageManagerFile import (
     ExtractPackageManagerFile,
 )
-from patchwork_cli.steps.ModifyCode.ModifyCode import ModifyCode
-from patchwork_cli.steps.PreparePR.PreparePR import PreparePR
-from patchwork_cli.steps.PreparePrompt.PreparePrompt import PreparePrompt
-from patchwork_cli.steps.ReadPRDiffs.ReadPRDiffs import ReadPRDiffs
-from patchwork_cli.steps.ScanDepscan.ScanDepscan import ScanDepscan
-from patchwork_cli.steps.ScanSemgrep.ScanSemgrep import ScanSemgrep
+from patchwork.steps.ModifyCode.ModifyCode import ModifyCode
+from patchwork.steps.PreparePR.PreparePR import PreparePR
+from patchwork.steps.PreparePrompt.PreparePrompt import PreparePrompt
+from patchwork.steps.ReadPRDiffs.ReadPRDiffs import ReadPRDiffs
+from patchwork.steps.ScanDepscan.ScanDepscan import ScanDepscan
+from patchwork.steps.ScanSemgrep.ScanSemgrep import ScanSemgrep
 
 __all__ = [
     "AnalyzeImpact",
     "CallCode2Prompt",
     "CallOpenAI",
     "CommitChanges",
     "CreatePR",
```

### Comparing `patchwork_cli-0.0.2/pyproject.toml` & `patchwork_cli-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 [tool.poetry]
 name = "patchwork-cli"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["patched.code"]
 license = "AGPL"
 readme = "README.md"
+packages = [
+    { include = "patchwork", from = "." }
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "~8.1.0"
 pygithub = "~2.1.1"
 gitpython = "~3.1.40"
 semgrep = "^1.51.0"
 pydantic = "^2.6.4"
 openai = "^1.13.3"
 tree-sitter-languages = "^1.10.2"
 tiktoken = "^0.6.0"
-libcst = "^1.2.0"
+libcst = "~1.2.0"
 python-gitlab = "^4.4.0"
 owasp-depscan = "^5.2.12"
-# pypi don't allow for git direct dependencies
-#code2prompt = {git = "https://github.com/raphaelmansuy/code2prompt.git"}
+patched-code2prompt = "0.2.0"
 pyyaml = "^6.0.1"
 packageurl-python = "~0.15.0"
 semver = "~3.0.2"
 requests = "~2.31.0"
+chardet = "^5.2.0"
 # pinning transitive dependencies
 orjson = "~3.9.15"
-chardet = "^5.2.0"
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "*"
 poethepoet = { version = "^0.24.2", extras = ["poetry-plugin"] }
 mypy = "^1.7.1"
 types-requests = "~2.31.0"
 black = "^23.12.0"
@@ -40,22 +42,22 @@
 pytest = "^8.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-patchwork = 'patchwork_cli.app:cli'
+patchwork = 'patchwork.app:cli'
 
 [tool.poe.poetry_hooks]
 #pre_build = "mypy"
 post_update = "lint"
 
 [tool.poe.env]
-PROJ_PATH.default = "patchwork_cli"
+PROJ_PATH.default = "patchwork"
 
 [tool.poe.tasks]
 #mypy = "mypy ${PROJ_PATH}"
 lint = [
     {cmd = "autoflake --recursive ${PROJ_PATH}"},
     {cmd = "isort ${PROJ_PATH}"},
     {cmd = "black ${PROJ_PATH}"}
```

### Comparing `patchwork_cli-0.0.2/PKG-INFO` & `patchwork_cli-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: patchwork-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 License: AGPL
 Author: patched.code
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: click (>=8.1.0,<8.2.0)
 Requires-Dist: gitpython (>=3.1.40,<3.2.0)
-Requires-Dist: libcst (>=1.2.0,<2.0.0)
+Requires-Dist: libcst (>=1.2.0,<1.3.0)
 Requires-Dist: openai (>=1.13.3,<2.0.0)
 Requires-Dist: orjson (>=3.9.15,<3.10.0)
 Requires-Dist: owasp-depscan (>=5.2.12,<6.0.0)
 Requires-Dist: packageurl-python (>=0.15.0,<0.16.0)
+Requires-Dist: patched-code2prompt (==0.2.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pygithub (>=2.1.1,<2.2.0)
 Requires-Dist: python-gitlab (>=4.4.0,<5.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<2.32.0)
 Requires-Dist: semgrep (>=1.51.0,<2.0.0)
 Requires-Dist: semver (>=3.0.2,<3.1.0)
@@ -92,15 +92,15 @@
 
 ```bash
 patchwork AutoFix openai_api_key=<YOUR_OPENAI_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
 The above command will default to patching code in the current directory, by running Semgrep to identify the vulnerabilities.
 
-You can take a look at the `default.yml` [file](patchwork_cli/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. 
+You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. 
 
 ## PatchWork in CI
 
 You can also run PatchWork in a CI environment with ease:
 
 ### Jenkins CI
 
@@ -129,15 +129,15 @@
   pull_request: {}
   # Patch on-demand through GitHub Actions interface:
   workflow_dispatch: {}
 
 jobs:
   patchwork:
     # User definable name of this GitHub Actions job.
-    name: semgrep/ci
+    name: patchwork/ci
     runs-on: ubuntu-latest
 
     container:
       # A Docker image with patchwork installed. Do not change this.
       image: patched-codes/patchwork
 
     steps:
@@ -196,11 +196,11 @@
 }
 ```
 
 Each patchflow comes with an optimized default prompt template. But you can specify your own using the `prompt_template_file=/path/to/prompt/template/file` option. 
 
 ## Contributing
 
-To create a new patchflow, follow [these instructions](patchwork_cli/patchflows/README.md).
+To create a new patchflow, follow [these instructions](patchwork/patchflows/README.md).
 
-To create a new step, follow [these instructions](patchwork_cli/steps/README.md).
+To create a new step, follow [these instructions](patchwork/steps/README.md).
```

