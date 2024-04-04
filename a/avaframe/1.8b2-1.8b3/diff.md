# Comparing `tmp/avaframe-1.8b2.tar.gz` & `tmp/avaframe-1.8b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avaframe-1.8b2.tar", last modified: Thu Nov 16 12:20:40 2023, max compression
+gzip compressed data, was "avaframe-1.8b3.tar", last modified: Thu Nov 16 21:07:26 2023, max compression
```

## Comparing `avaframe-1.8b2.tar` & `avaframe-1.8b3.tar`

### file list

```diff
@@ -1,226 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.417134 avaframe-1.8b2/
--rw-r--r--   0 runner    (1001) docker     (127)    13827 2023-11-16 12:18:38.000000 avaframe-1.8b2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-11-16 12:18:38.000000 avaframe-1.8b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-11-16 12:20:40.417134 avaframe-1.8b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-11-16 12:18:38.000000 avaframe-1.8b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.381134 avaframe-1.8b2/avaframe/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-16 12:18:49.000000 avaframe-1.8b2/avaframe/RELEASE-VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.385134 avaframe-1.8b2/avaframe/ana1Tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana1Tests/FPtest.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana1Tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana1Tests/analysisTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14865 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana1Tests/damBreak.py
--rw-r--r--   0 runner    (1001) docker     (127)    17687 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana1Tests/energyLineTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana1Tests/energyLineTestCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)    11058 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana1Tests/rotationTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana1Tests/rotationTestCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)    30699 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana1Tests/simiSolTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana1Tests/testUtilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.385134 avaframe-1.8b2/avaframe/ana3AIMEC/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana3AIMEC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54214 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana3AIMEC/aimecTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    24620 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana3AIMEC/ana3AIMEC.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana3AIMEC/ana3AIMECCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)    11038 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana3AIMEC/dfa2Aimec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.385134 avaframe-1.8b2/avaframe/ana4Stats/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana4Stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana4Stats/getStats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana4Stats/getStatsCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)    37524 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana4Stats/probAna.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana4Stats/probAnaCfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.389134 avaframe-1.8b2/avaframe/ana5Utils/
--rw-r--r--   0 runner    (1001) docker     (127)    25307 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana5Utils/DFAPathGeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana5Utils/DFAPathGenerationCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana5Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33851 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana5Utils/distanceTimeAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/ana5Utils/distanceTimeAnalysisCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)      863 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/avaframeCfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.397134 avaframe-1.8b2/avaframe/com1DFA/
--rw-r--r--   0 runner    (1001) docker     (127)  1563948 2023-11-16 12:18:47.000000 avaframe-1.8b2/avaframe/com1DFA/DFAToolsCython.c
--rw-r--r--   0 runner    (1001) docker     (127)  2627557 2023-11-16 12:18:48.000000 avaframe-1.8b2/avaframe/com1DFA/DFAfunctionsCython.c
--rw-r--r--   0 runner    (1001) docker     (127)    16203 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFA/DFAtools.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFA/checkCfg.py
--rw-r--r--   0 runner    (1001) docker     (127)   109895 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFA/com1DFA.py
--rw-r--r--   0 runner    (1001) docker     (127)    19292 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFA/com1DFACfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)    10041 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFA/com1DFATools.py
--rw-r--r--   0 runner    (1001) docker     (127)  1393703 2023-11-16 12:18:49.000000 avaframe-1.8b2/avaframe/com1DFA/damCom1DFA.c
--rw-r--r--   0 runner    (1001) docker     (127)    33907 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFA/deriveParameterSet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10275 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFA/particleInitialisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    34251 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFA/particleTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFA/testSPH.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFA/timeDiscretizations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.397134 avaframe-1.8b2/avaframe/com1DFAOrig/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFAOrig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21819 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFAOrig/com1DFAOrig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFAOrig/com1DFAOrigCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com1DFAOrig/runCom1DFAOrig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.397134 avaframe-1.8b2/avaframe/com2AB/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com2AB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15310 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com2AB/com2AB.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com2AB/com2ABCfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.397134 avaframe-1.8b2/avaframe/com3Hybrid/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com3Hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com3Hybrid/com3Hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com3Hybrid/com3HybridCfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.397134 avaframe-1.8b2/avaframe/com4FlowPy/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com4FlowPy/com4FlowPyCfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.397134 avaframe-1.8b2/avaframe/com5SnowSlide/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com5SnowSlide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com5SnowSlide/com5SnowSlide.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com5SnowSlide/com5SnowSlideCfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.397134 avaframe-1.8b2/avaframe/com6RockAvalanche/
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/com6RockAvalanche/com6RockAvalancheCfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.377134 avaframe-1.8b2/avaframe/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.377134 avaframe-1.8b2/avaframe/data/avaDamBreak/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.397134 avaframe-1.8b2/avaframe/data/avaDamBreak/Inputs/
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/data/avaDamBreak/Inputs/damBreak_com1DFACfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.377134 avaframe-1.8b2/avaframe/data/avaFPtest/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.397134 avaframe-1.8b2/avaframe/data/avaFPtest/Inputs/
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/data/avaFPtest/Inputs/FlatPlane_com1DFACfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.377134 avaframe-1.8b2/avaframe/data/avaSimilaritySol/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.397134 avaframe-1.8b2/avaframe/data/avaSimilaritySol/Inputs/
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/data/avaSimilaritySol/Inputs/simiSol_com1DFACfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.401134 avaframe-1.8b2/avaframe/in1Data/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in1Data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in1Data/computeFromDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in1Data/computeFromDistributionCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)    28406 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in1Data/getInput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.401134 avaframe-1.8b2/avaframe/in2Trans/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in2Trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in2Trans/ascUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14707 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in2Trans/shpConversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.401134 avaframe-1.8b2/avaframe/in3Utils/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in3Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18428 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in3Utils/cfgHandling.py
--rw-r--r--   0 runner    (1001) docker     (127)    23775 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in3Utils/cfgUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26084 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in3Utils/fileHandlerUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23266 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in3Utils/generateTopo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in3Utils/generateTopoCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)    49581 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in3Utils/geoTrans.py
--rw-r--r--   0 runner    (1001) docker     (127)     6902 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in3Utils/getReleaseArea.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in3Utils/getReleaseAreaCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in3Utils/initialiseDirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in3Utils/initializeProject.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in3Utils/logUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/in3Utils/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.401134 avaframe-1.8b2/avaframe/log2Report/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/log2Report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/log2Report/generateCompareReport.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/log2Report/generateCompareReportCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/log2Report/generateReport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.401134 avaframe-1.8b2/avaframe/out1Peak/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out1Peak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out1Peak/outPlotAllPeak.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.405134 avaframe-1.8b2/avaframe/out3Plot/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9767 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/amaPlots.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/in1DataPlots.py
--rw-r--r--   0 runner    (1001) docker     (127)    11489 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/outAB.py
--rw-r--r--   0 runner    (1001) docker     (127)    61732 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/outAIMEC.py
--rw-r--r--   0 runner    (1001) docker     (127)    48487 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/outAna1Plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    17379 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/outCom1DFA.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/outCom3Plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/outContours.py
--rw-r--r--   0 runner    (1001) docker     (127)    15820 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/outDebugPlots.py
--rw-r--r--   0 runner    (1001) docker     (127)    34799 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/outDistanceTimeAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    27924 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/outParticlesAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/outParticlesAnalysisCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)    21018 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/outQuickPlot.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/outQuickPlotCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/outTopo.py
--rw-r--r--   0 runner    (1001) docker     (127)    28184 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/plotUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/plotUtilsCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)    24656 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/out3Plot/statsPlots.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/runAna4ProbAna.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/runCom1DFA.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/runCom2AB.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/runCom4FlowPy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/runCom5SnowSlide.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/runCom6RockAvalanche.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/runIn1RelInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/runOperational.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/runPlotCom1DFA.py
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/runStandardTestsCom1DFA.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/runTmp1Ex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/runUpdateBenchmarkTestsCom1DFA.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.413134 avaframe-1.8b2/avaframe/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.413134 avaframe-1.8b2/avaframe/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.413134 avaframe-1.8b2/avaframe/tests/data/com1DFAConfigs/
--rw-r--r--   0 runner    (1001) docker     (127)    17135 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/data/com1DFAConfigs/0_com1DFACfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)    17127 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/data/com1DFAConfigs/1_com1DFACfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)    17130 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/data/com1DFAConfigs/2_com1DFACfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/data/com1DFAConfigs/3_com1DFACfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/data/test2Cfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.413134 avaframe-1.8b2/avaframe/tests/data/testCom1DFA/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/data/testCom1DFA/getIniP_com1DFACfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/data/testCom1DFA/test_com1DFACfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.413134 avaframe-1.8b2/avaframe/tests/data/testDamBreak/
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/data/testDamBreak/damBreak_com1DFACfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.413134 avaframe-1.8b2/avaframe/tests/data/testEnergyLine/
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/data/testEnergyLine/energyLineTestCfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.413134 avaframe-1.8b2/avaframe/tests/data/testSimiSol/
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/data/testSimiSol/simiSol_com1DFACfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)    10008 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_DFAPathGeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11200 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_DFAToolsCython.py
--rw-r--r--   0 runner    (1001) docker     (127)    24118 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_DFAfunctionsCython.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_DFAtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_aimecTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_ana1Tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    17738 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_ana3AIMEC.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_ascUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8988 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_cfgHandling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_cfgUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_checkCfg.py
--rw-r--r--   0 runner    (1001) docker     (127)    78486 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_com1DFA.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_com1DFATools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_com2AB.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_computeFromDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_damBreak.py
--rw-r--r--   0 runner    (1001) docker     (127)    20338 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_damCom1DFA.py
--rw-r--r--   0 runner    (1001) docker     (127)    17655 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_deriveParameterSet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9346 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_dfa2Aimec.py
--rw-r--r--   0 runner    (1001) docker     (127)    14946 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_distanceTimeAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14236 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_fileHandlerUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_generateCompareReport.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_generateReport.py
--rw-r--r--   0 runner    (1001) docker     (127)     8641 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_generateTopo.py
--rw-r--r--   0 runner    (1001) docker     (127)    37262 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_geoTrans.py
--rw-r--r--   0 runner    (1001) docker     (127)    21818 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_getInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_getReleaseArea.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_getStats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_initializeDirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_initializeProject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_logUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_logUtilsCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_out1Peak.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_outDistanceTimeAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_outParticlesAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_outQuickPlot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_particleInitialisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13385 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_particleTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8200 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_plotUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    38768 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_probAna.py
--rw-r--r--   0 runner    (1001) docker     (127)     9369 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_shpConversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_simiSol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_snowSlide.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_testUtilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_timeDiscretization.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tests/test_tmp1Ex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.417134 avaframe-1.8b2/avaframe/tmp1Ex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tmp1Ex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tmp1Ex/tmp1Ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/tmp1Ex/tmp1ExCfg.ini
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2023-11-16 12:18:38.000000 avaframe-1.8b2/avaframe/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:20:40.385134 avaframe-1.8b2/avaframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-11-16 12:20:40.000000 avaframe-1.8b2/avaframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6611 2023-11-16 12:20:40.000000 avaframe-1.8b2/avaframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 12:20:40.000000 avaframe-1.8b2/avaframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 12:19:40.000000 avaframe-1.8b2/avaframe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-11-16 12:20:40.000000 avaframe-1.8b2/avaframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-16 12:20:40.000000 avaframe-1.8b2/avaframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-11-16 12:18:39.000000 avaframe-1.8b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 12:20:40.417134 avaframe-1.8b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2023-11-16 12:18:39.000000 avaframe-1.8b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.286921 avaframe-1.8b3/
+-rw-r--r--   0 runner    (1001) docker     (127)    13827 2023-11-16 21:05:25.000000 avaframe-1.8b3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-11-16 21:05:25.000000 avaframe-1.8b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-11-16 21:07:26.286921 avaframe-1.8b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2023-11-16 21:05:25.000000 avaframe-1.8b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.250920 avaframe-1.8b3/avaframe/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-16 21:05:36.000000 avaframe-1.8b3/avaframe/RELEASE-VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.254920 avaframe-1.8b3/avaframe/ana1Tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana1Tests/FPtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana1Tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana1Tests/analysisTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14865 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana1Tests/damBreak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17687 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana1Tests/energyLineTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana1Tests/energyLineTestCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    11058 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana1Tests/rotationTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana1Tests/rotationTestCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    30699 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana1Tests/simiSolTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana1Tests/testUtilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.254920 avaframe-1.8b3/avaframe/ana3AIMEC/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana3AIMEC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54214 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana3AIMEC/aimecTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24620 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana3AIMEC/ana3AIMEC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana3AIMEC/ana3AIMECCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    11038 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana3AIMEC/dfa2Aimec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.254920 avaframe-1.8b3/avaframe/ana4Stats/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana4Stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana4Stats/getStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana4Stats/getStatsCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    37524 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana4Stats/probAna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana4Stats/probAnaCfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.258920 avaframe-1.8b3/avaframe/ana5Utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    25307 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana5Utils/DFAPathGeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana5Utils/DFAPathGenerationCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana5Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33851 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana5Utils/distanceTimeAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/ana5Utils/distanceTimeAnalysisCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/avaframeCfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.266920 avaframe-1.8b3/avaframe/com1DFA/
+-rw-r--r--   0 runner    (1001) docker     (127)  1563948 2023-11-16 21:05:34.000000 avaframe-1.8b3/avaframe/com1DFA/DFAToolsCython.c
+-rw-r--r--   0 runner    (1001) docker     (127)  2627557 2023-11-16 21:05:35.000000 avaframe-1.8b3/avaframe/com1DFA/DFAfunctionsCython.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16203 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFA/DFAtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFA/checkCfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109895 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFA/com1DFA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19292 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFA/com1DFACfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    10041 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFA/com1DFATools.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1393703 2023-11-16 21:05:36.000000 avaframe-1.8b3/avaframe/com1DFA/damCom1DFA.c
+-rw-r--r--   0 runner    (1001) docker     (127)    33907 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFA/deriveParameterSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10275 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFA/particleInitialisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34251 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFA/particleTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFA/testSPH.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFA/timeDiscretizations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.266920 avaframe-1.8b3/avaframe/com1DFAOrig/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFAOrig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21819 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFAOrig/com1DFAOrig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFAOrig/com1DFAOrigCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com1DFAOrig/runCom1DFAOrig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.266920 avaframe-1.8b3/avaframe/com2AB/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com2AB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15310 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com2AB/com2AB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com2AB/com2ABCfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.266920 avaframe-1.8b3/avaframe/com3Hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com3Hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com3Hybrid/com3Hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com3Hybrid/com3HybridCfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.266920 avaframe-1.8b3/avaframe/com4FlowPy/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com4FlowPy/com4FlowPyCfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.266920 avaframe-1.8b3/avaframe/com5SnowSlide/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com5SnowSlide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com5SnowSlide/com5SnowSlide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com5SnowSlide/com5SnowSlideCfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.266920 avaframe-1.8b3/avaframe/com6RockAvalanche/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com6RockAvalanche/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com6RockAvalanche/com6RockAvalanche.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/com6RockAvalanche/com6RockAvalancheCfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.246920 avaframe-1.8b3/avaframe/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.246920 avaframe-1.8b3/avaframe/data/avaDamBreak/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.266920 avaframe-1.8b3/avaframe/data/avaDamBreak/Inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2023-11-16 21:05:25.000000 avaframe-1.8b3/avaframe/data/avaDamBreak/Inputs/damBreak_com1DFACfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.246920 avaframe-1.8b3/avaframe/data/avaFPtest/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.266920 avaframe-1.8b3/avaframe/data/avaFPtest/Inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/data/avaFPtest/Inputs/FlatPlane_com1DFACfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.246920 avaframe-1.8b3/avaframe/data/avaSimilaritySol/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.266920 avaframe-1.8b3/avaframe/data/avaSimilaritySol/Inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/data/avaSimilaritySol/Inputs/simiSol_com1DFACfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.270920 avaframe-1.8b3/avaframe/in1Data/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in1Data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in1Data/computeFromDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in1Data/computeFromDistributionCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    28406 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in1Data/getInput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.270920 avaframe-1.8b3/avaframe/in2Trans/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in2Trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in2Trans/ascUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14707 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in2Trans/shpConversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.270920 avaframe-1.8b3/avaframe/in3Utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in3Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18428 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in3Utils/cfgHandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23775 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in3Utils/cfgUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26084 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in3Utils/fileHandlerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23266 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in3Utils/generateTopo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in3Utils/generateTopoCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    49581 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in3Utils/geoTrans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6902 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in3Utils/getReleaseArea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in3Utils/getReleaseAreaCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in3Utils/initialiseDirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in3Utils/initializeProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in3Utils/logUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/in3Utils/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.270920 avaframe-1.8b3/avaframe/log2Report/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/log2Report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/log2Report/generateCompareReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/log2Report/generateCompareReportCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/log2Report/generateReport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.270920 avaframe-1.8b3/avaframe/out1Peak/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out1Peak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out1Peak/outPlotAllPeak.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.274920 avaframe-1.8b3/avaframe/out3Plot/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9767 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/amaPlots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/in1DataPlots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/outAB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61732 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/outAIMEC.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48487 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/outAna1Plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17379 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/outCom1DFA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11577 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/outCom3Plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/outContours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15820 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/outDebugPlots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34799 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/outDistanceTimeAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27924 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/outParticlesAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/outParticlesAnalysisCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    21018 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/outQuickPlot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/outQuickPlotCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/outTopo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28184 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/plotUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/plotUtilsCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    24656 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/out3Plot/statsPlots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/runAna4ProbAna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/runCom1DFA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/runCom2AB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/runCom4FlowPy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/runCom5SnowSlide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/runCom6RockAvalanche.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/runIn1RelInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/runOperational.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/runPlotCom1DFA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/runStandardTestsCom1DFA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/runTmp1Ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/runUpdateBenchmarkTestsCom1DFA.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.282920 avaframe-1.8b3/avaframe/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.282920 avaframe-1.8b3/avaframe/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.282920 avaframe-1.8b3/avaframe/tests/data/com1DFAConfigs/
+-rw-r--r--   0 runner    (1001) docker     (127)    17135 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/data/com1DFAConfigs/0_com1DFACfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    17127 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/data/com1DFAConfigs/1_com1DFACfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    17130 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/data/com1DFAConfigs/2_com1DFACfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/data/com1DFAConfigs/3_com1DFACfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/data/test2Cfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.286921 avaframe-1.8b3/avaframe/tests/data/testCom1DFA/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/data/testCom1DFA/getIniP_com1DFACfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/data/testCom1DFA/test_com1DFACfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.286921 avaframe-1.8b3/avaframe/tests/data/testDamBreak/
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/data/testDamBreak/damBreak_com1DFACfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.286921 avaframe-1.8b3/avaframe/tests/data/testEnergyLine/
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/data/testEnergyLine/energyLineTestCfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.286921 avaframe-1.8b3/avaframe/tests/data/testSimiSol/
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/data/testSimiSol/simiSol_com1DFACfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    10008 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_DFAPathGeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11200 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_DFAToolsCython.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24118 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_DFAfunctionsCython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_DFAtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_aimecTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_ana1Tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17738 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_ana3AIMEC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_ascUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_cfgHandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_cfgUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_checkCfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78486 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_com1DFA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_com1DFATools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_com2AB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_computeFromDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_damBreak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20338 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_damCom1DFA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17655 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_deriveParameterSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_dfa2Aimec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14946 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_distanceTimeAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14236 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_fileHandlerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_generateCompareReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_generateReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8641 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_generateTopo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37262 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_geoTrans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21818 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_getInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_getReleaseArea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_getStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_initializeDirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_initializeProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_logUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_logUtilsCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_out1Peak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_outDistanceTimeAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_outParticlesAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_outQuickPlot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_particleInitialisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_particleTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_plotUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38768 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_probAna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_shpConversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_simiSol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_snowSlide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_testUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_timeDiscretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tests/test_tmp1Ex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.286921 avaframe-1.8b3/avaframe/tmp1Ex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tmp1Ex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tmp1Ex/tmp1Ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/tmp1Ex/tmp1ExCfg.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2023-11-16 21:05:26.000000 avaframe-1.8b3/avaframe/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 21:07:26.254920 avaframe-1.8b3/avaframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-11-16 21:07:26.000000 avaframe-1.8b3/avaframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2023-11-16 21:07:26.000000 avaframe-1.8b3/avaframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 21:07:26.000000 avaframe-1.8b3/avaframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 21:06:26.000000 avaframe-1.8b3/avaframe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-11-16 21:07:26.000000 avaframe-1.8b3/avaframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-16 21:07:26.000000 avaframe-1.8b3/avaframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2023-11-16 21:05:27.000000 avaframe-1.8b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 21:07:26.286921 avaframe-1.8b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2023-11-16 21:05:27.000000 avaframe-1.8b3/setup.py
```

### Comparing `avaframe-1.8b2/LICENSE.txt` & `avaframe-1.8b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/PKG-INFO` & `avaframe-1.8b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avaframe
-Version: 1.8b2
+Version: 1.8b3
 Summary: The Open Avalanche Framework
 Home-page: http://avaframe.org
 Author: AvaFrame Contributors
 Author-email: felix@avaframe.org
 License: EUPL
 Description: **The AvaFrame documentation is hosted on ReadTheDocs: http://docs.avaframe.org**
```

### Comparing `avaframe-1.8b2/README.md` & `avaframe-1.8b3/README.md`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana1Tests/FPtest.py` & `avaframe-1.8b3/avaframe/ana1Tests/FPtest.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana1Tests/analysisTools.py` & `avaframe-1.8b3/avaframe/ana1Tests/analysisTools.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana1Tests/damBreak.py` & `avaframe-1.8b3/avaframe/ana1Tests/damBreak.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana1Tests/energyLineTest.py` & `avaframe-1.8b3/avaframe/ana1Tests/energyLineTest.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana1Tests/energyLineTestCfg.ini` & `avaframe-1.8b3/avaframe/ana1Tests/energyLineTestCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana1Tests/rotationTest.py` & `avaframe-1.8b3/avaframe/ana1Tests/rotationTest.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana1Tests/rotationTestCfg.ini` & `avaframe-1.8b3/avaframe/ana1Tests/rotationTestCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana1Tests/simiSolTest.py` & `avaframe-1.8b3/avaframe/ana1Tests/simiSolTest.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana1Tests/testUtilities.py` & `avaframe-1.8b3/avaframe/ana1Tests/testUtilities.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana3AIMEC/aimecTools.py` & `avaframe-1.8b3/avaframe/ana3AIMEC/aimecTools.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana3AIMEC/ana3AIMEC.py` & `avaframe-1.8b3/avaframe/ana3AIMEC/ana3AIMEC.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana3AIMEC/ana3AIMECCfg.ini` & `avaframe-1.8b3/avaframe/ana3AIMEC/ana3AIMECCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana3AIMEC/dfa2Aimec.py` & `avaframe-1.8b3/avaframe/ana3AIMEC/dfa2Aimec.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana4Stats/getStats.py` & `avaframe-1.8b3/avaframe/ana4Stats/getStats.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana4Stats/getStatsCfg.ini` & `avaframe-1.8b3/avaframe/ana4Stats/getStatsCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana4Stats/probAna.py` & `avaframe-1.8b3/avaframe/ana4Stats/probAna.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana4Stats/probAnaCfg.ini` & `avaframe-1.8b3/avaframe/ana4Stats/probAnaCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana5Utils/DFAPathGeneration.py` & `avaframe-1.8b3/avaframe/ana5Utils/DFAPathGeneration.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana5Utils/DFAPathGenerationCfg.ini` & `avaframe-1.8b3/avaframe/ana5Utils/DFAPathGenerationCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana5Utils/distanceTimeAnalysis.py` & `avaframe-1.8b3/avaframe/ana5Utils/distanceTimeAnalysis.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/ana5Utils/distanceTimeAnalysisCfg.ini` & `avaframe-1.8b3/avaframe/ana5Utils/distanceTimeAnalysisCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/avaframeCfg.ini` & `avaframe-1.8b3/avaframe/avaframeCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFA/DFAToolsCython.c` & `avaframe-1.8b3/avaframe/com1DFA/DFAToolsCython.c`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFA/DFAfunctionsCython.c` & `avaframe-1.8b3/avaframe/com1DFA/DFAfunctionsCython.c`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFA/DFAtools.py` & `avaframe-1.8b3/avaframe/com1DFA/DFAtools.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFA/checkCfg.py` & `avaframe-1.8b3/avaframe/com1DFA/checkCfg.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFA/com1DFA.py` & `avaframe-1.8b3/avaframe/com1DFA/com1DFA.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFA/com1DFACfg.ini` & `avaframe-1.8b3/avaframe/com1DFA/com1DFACfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFA/com1DFATools.py` & `avaframe-1.8b3/avaframe/com1DFA/com1DFATools.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFA/damCom1DFA.c` & `avaframe-1.8b3/avaframe/com1DFA/damCom1DFA.c`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFA/deriveParameterSet.py` & `avaframe-1.8b3/avaframe/com1DFA/deriveParameterSet.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFA/particleInitialisation.py` & `avaframe-1.8b3/avaframe/com1DFA/particleInitialisation.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFA/particleTools.py` & `avaframe-1.8b3/avaframe/com1DFA/particleTools.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFA/testSPH.py` & `avaframe-1.8b3/avaframe/com1DFA/testSPH.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFA/timeDiscretizations.py` & `avaframe-1.8b3/avaframe/com1DFA/timeDiscretizations.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFAOrig/com1DFAOrig.py` & `avaframe-1.8b3/avaframe/com1DFAOrig/com1DFAOrig.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFAOrig/com1DFAOrigCfg.ini` & `avaframe-1.8b3/avaframe/com1DFAOrig/com1DFAOrigCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com1DFAOrig/runCom1DFAOrig.py` & `avaframe-1.8b3/avaframe/com1DFAOrig/runCom1DFAOrig.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com2AB/com2AB.py` & `avaframe-1.8b3/avaframe/com2AB/com2AB.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com2AB/com2ABCfg.ini` & `avaframe-1.8b3/avaframe/com2AB/com2ABCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com3Hybrid/com3Hybrid.py` & `avaframe-1.8b3/avaframe/com3Hybrid/com3Hybrid.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com3Hybrid/com3HybridCfg.ini` & `avaframe-1.8b3/avaframe/com3Hybrid/com3HybridCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com4FlowPy/com4FlowPyCfg.ini` & `avaframe-1.8b3/avaframe/com4FlowPy/com4FlowPyCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com5SnowSlide/com5SnowSlide.py` & `avaframe-1.8b3/avaframe/com5SnowSlide/com5SnowSlide.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com5SnowSlide/com5SnowSlideCfg.ini` & `avaframe-1.8b3/avaframe/com5SnowSlide/com5SnowSlideCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/com6RockAvalanche/com6RockAvalancheCfg.ini` & `avaframe-1.8b3/avaframe/com6RockAvalanche/com6RockAvalancheCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/data/avaDamBreak/Inputs/damBreak_com1DFACfg.ini` & `avaframe-1.8b3/avaframe/data/avaDamBreak/Inputs/damBreak_com1DFACfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/data/avaFPtest/Inputs/FlatPlane_com1DFACfg.ini` & `avaframe-1.8b3/avaframe/data/avaFPtest/Inputs/FlatPlane_com1DFACfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/data/avaSimilaritySol/Inputs/simiSol_com1DFACfg.ini` & `avaframe-1.8b3/avaframe/data/avaSimilaritySol/Inputs/simiSol_com1DFACfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in1Data/computeFromDistribution.py` & `avaframe-1.8b3/avaframe/in1Data/computeFromDistribution.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in1Data/computeFromDistributionCfg.ini` & `avaframe-1.8b3/avaframe/in1Data/computeFromDistributionCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in1Data/getInput.py` & `avaframe-1.8b3/avaframe/in1Data/getInput.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in2Trans/ascUtils.py` & `avaframe-1.8b3/avaframe/in2Trans/ascUtils.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in2Trans/shpConversion.py` & `avaframe-1.8b3/avaframe/in2Trans/shpConversion.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in3Utils/cfgHandling.py` & `avaframe-1.8b3/avaframe/in3Utils/cfgHandling.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in3Utils/cfgUtils.py` & `avaframe-1.8b3/avaframe/in3Utils/cfgUtils.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in3Utils/fileHandlerUtils.py` & `avaframe-1.8b3/avaframe/in3Utils/fileHandlerUtils.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in3Utils/generateTopo.py` & `avaframe-1.8b3/avaframe/in3Utils/generateTopo.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in3Utils/generateTopoCfg.ini` & `avaframe-1.8b3/avaframe/in3Utils/generateTopoCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in3Utils/geoTrans.py` & `avaframe-1.8b3/avaframe/in3Utils/geoTrans.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in3Utils/getReleaseArea.py` & `avaframe-1.8b3/avaframe/in3Utils/getReleaseArea.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in3Utils/getReleaseAreaCfg.ini` & `avaframe-1.8b3/avaframe/in3Utils/getReleaseAreaCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in3Utils/initialiseDirs.py` & `avaframe-1.8b3/avaframe/in3Utils/initialiseDirs.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in3Utils/initializeProject.py` & `avaframe-1.8b3/avaframe/in3Utils/initializeProject.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in3Utils/logUtils.py` & `avaframe-1.8b3/avaframe/in3Utils/logUtils.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/in3Utils/logging.conf` & `avaframe-1.8b3/avaframe/in3Utils/logging.conf`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/log2Report/generateCompareReport.py` & `avaframe-1.8b3/avaframe/log2Report/generateCompareReport.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/log2Report/generateCompareReportCfg.ini` & `avaframe-1.8b3/avaframe/log2Report/generateCompareReportCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/log2Report/generateReport.py` & `avaframe-1.8b3/avaframe/log2Report/generateReport.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out1Peak/outPlotAllPeak.py` & `avaframe-1.8b3/avaframe/out1Peak/outPlotAllPeak.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/amaPlots.py` & `avaframe-1.8b3/avaframe/out3Plot/amaPlots.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/in1DataPlots.py` & `avaframe-1.8b3/avaframe/out3Plot/in1DataPlots.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/outAB.py` & `avaframe-1.8b3/avaframe/out3Plot/outAB.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/outAIMEC.py` & `avaframe-1.8b3/avaframe/out3Plot/outAIMEC.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/outAna1Plots.py` & `avaframe-1.8b3/avaframe/out3Plot/outAna1Plots.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/outCom1DFA.py` & `avaframe-1.8b3/avaframe/out3Plot/outCom1DFA.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/outCom3Plots.py` & `avaframe-1.8b3/avaframe/out3Plot/outCom3Plots.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/outContours.py` & `avaframe-1.8b3/avaframe/out3Plot/outContours.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/outDebugPlots.py` & `avaframe-1.8b3/avaframe/out3Plot/outDebugPlots.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/outDistanceTimeAnalysis.py` & `avaframe-1.8b3/avaframe/out3Plot/outDistanceTimeAnalysis.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/outParticlesAnalysis.py` & `avaframe-1.8b3/avaframe/out3Plot/outParticlesAnalysis.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/outParticlesAnalysisCfg.ini` & `avaframe-1.8b3/avaframe/out3Plot/outParticlesAnalysisCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/outQuickPlot.py` & `avaframe-1.8b3/avaframe/out3Plot/outQuickPlot.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/outTopo.py` & `avaframe-1.8b3/avaframe/out3Plot/outTopo.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/plotUtils.py` & `avaframe-1.8b3/avaframe/out3Plot/plotUtils.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/plotUtilsCfg.ini` & `avaframe-1.8b3/avaframe/out3Plot/plotUtilsCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/out3Plot/statsPlots.py` & `avaframe-1.8b3/avaframe/out3Plot/statsPlots.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/runAna4ProbAna.py` & `avaframe-1.8b3/avaframe/runAna4ProbAna.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/runCom1DFA.py` & `avaframe-1.8b3/avaframe/runCom1DFA.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/runCom2AB.py` & `avaframe-1.8b3/avaframe/runCom2AB.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/runCom4FlowPy.py` & `avaframe-1.8b3/avaframe/runCom4FlowPy.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/runCom5SnowSlide.py` & `avaframe-1.8b3/avaframe/runCom5SnowSlide.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/runCom6RockAvalanche.py` & `avaframe-1.8b3/avaframe/runCom6RockAvalanche.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/runIn1RelInfo.py` & `avaframe-1.8b3/avaframe/runIn1RelInfo.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/runOperational.py` & `avaframe-1.8b3/avaframe/runOperational.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/runPlotCom1DFA.py` & `avaframe-1.8b3/avaframe/runPlotCom1DFA.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/runStandardTestsCom1DFA.py` & `avaframe-1.8b3/avaframe/runStandardTestsCom1DFA.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/runTmp1Ex.py` & `avaframe-1.8b3/avaframe/runTmp1Ex.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/runUpdateBenchmarkTestsCom1DFA.py` & `avaframe-1.8b3/avaframe/runUpdateBenchmarkTestsCom1DFA.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/data/com1DFAConfigs/0_com1DFACfg.ini` & `avaframe-1.8b3/avaframe/tests/data/com1DFAConfigs/0_com1DFACfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/data/com1DFAConfigs/1_com1DFACfg.ini` & `avaframe-1.8b3/avaframe/tests/data/com1DFAConfigs/1_com1DFACfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/data/com1DFAConfigs/2_com1DFACfg.ini` & `avaframe-1.8b3/avaframe/tests/data/com1DFAConfigs/2_com1DFACfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/data/com1DFAConfigs/3_com1DFACfg.ini` & `avaframe-1.8b3/avaframe/tests/data/com1DFAConfigs/3_com1DFACfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/data/test2Cfg.ini` & `avaframe-1.8b3/avaframe/tests/data/test2Cfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/data/testCom1DFA/getIniP_com1DFACfg.ini` & `avaframe-1.8b3/avaframe/tests/data/testCom1DFA/getIniP_com1DFACfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/data/testCom1DFA/test_com1DFACfg.ini` & `avaframe-1.8b3/avaframe/tests/data/testCom1DFA/test_com1DFACfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/data/testDamBreak/damBreak_com1DFACfg.ini` & `avaframe-1.8b3/avaframe/tests/data/testDamBreak/damBreak_com1DFACfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/data/testEnergyLine/energyLineTestCfg.ini` & `avaframe-1.8b3/avaframe/tests/data/testEnergyLine/energyLineTestCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/data/testSimiSol/simiSol_com1DFACfg.ini` & `avaframe-1.8b3/avaframe/tests/data/testSimiSol/simiSol_com1DFACfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_DFAPathGeneration.py` & `avaframe-1.8b3/avaframe/tests/test_DFAPathGeneration.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_DFAToolsCython.py` & `avaframe-1.8b3/avaframe/tests/test_DFAToolsCython.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_DFAfunctionsCython.py` & `avaframe-1.8b3/avaframe/tests/test_DFAfunctionsCython.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_DFAtools.py` & `avaframe-1.8b3/avaframe/tests/test_DFAtools.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_aimecTools.py` & `avaframe-1.8b3/avaframe/tests/test_aimecTools.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_ana1Tests.py` & `avaframe-1.8b3/avaframe/tests/test_ana1Tests.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_ana3AIMEC.py` & `avaframe-1.8b3/avaframe/tests/test_ana3AIMEC.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_ascUtils.py` & `avaframe-1.8b3/avaframe/tests/test_ascUtils.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_cfgHandling.py` & `avaframe-1.8b3/avaframe/tests/test_cfgHandling.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_cfgUtils.py` & `avaframe-1.8b3/avaframe/tests/test_cfgUtils.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_checkCfg.py` & `avaframe-1.8b3/avaframe/tests/test_checkCfg.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_com1DFA.py` & `avaframe-1.8b3/avaframe/tests/test_com1DFA.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_com1DFATools.py` & `avaframe-1.8b3/avaframe/tests/test_com1DFATools.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_com2AB.py` & `avaframe-1.8b3/avaframe/tests/test_com2AB.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_computeFromDistribution.py` & `avaframe-1.8b3/avaframe/tests/test_computeFromDistribution.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_damBreak.py` & `avaframe-1.8b3/avaframe/tests/test_damBreak.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_damCom1DFA.py` & `avaframe-1.8b3/avaframe/tests/test_damCom1DFA.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_deriveParameterSet.py` & `avaframe-1.8b3/avaframe/tests/test_deriveParameterSet.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_dfa2Aimec.py` & `avaframe-1.8b3/avaframe/tests/test_dfa2Aimec.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_distanceTimeAnalysis.py` & `avaframe-1.8b3/avaframe/tests/test_distanceTimeAnalysis.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_fileHandlerUtils.py` & `avaframe-1.8b3/avaframe/tests/test_fileHandlerUtils.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_generateCompareReport.py` & `avaframe-1.8b3/avaframe/tests/test_generateCompareReport.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_generateReport.py` & `avaframe-1.8b3/avaframe/tests/test_generateReport.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_generateTopo.py` & `avaframe-1.8b3/avaframe/tests/test_generateTopo.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_geoTrans.py` & `avaframe-1.8b3/avaframe/tests/test_geoTrans.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_getInput.py` & `avaframe-1.8b3/avaframe/tests/test_getInput.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_getReleaseArea.py` & `avaframe-1.8b3/avaframe/tests/test_getReleaseArea.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_getStats.py` & `avaframe-1.8b3/avaframe/tests/test_getStats.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_initializeDirs.py` & `avaframe-1.8b3/avaframe/tests/test_initializeDirs.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_initializeProject.py` & `avaframe-1.8b3/avaframe/tests/test_initializeProject.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_logUtils.py` & `avaframe-1.8b3/avaframe/tests/test_logUtils.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_logUtilsCfg.ini` & `avaframe-1.8b3/avaframe/tests/test_logUtilsCfg.ini`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_out1Peak.py` & `avaframe-1.8b3/avaframe/tests/test_out1Peak.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_outDistanceTimeAnalysis.py` & `avaframe-1.8b3/avaframe/tests/test_outDistanceTimeAnalysis.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_outParticlesAnalysis.py` & `avaframe-1.8b3/avaframe/tests/test_outParticlesAnalysis.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_outQuickPlot.py` & `avaframe-1.8b3/avaframe/tests/test_outQuickPlot.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_particleInitialisation.py` & `avaframe-1.8b3/avaframe/tests/test_particleInitialisation.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_particleTools.py` & `avaframe-1.8b3/avaframe/tests/test_particleTools.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_plotUtils.py` & `avaframe-1.8b3/avaframe/tests/test_plotUtils.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_probAna.py` & `avaframe-1.8b3/avaframe/tests/test_probAna.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_shpConversion.py` & `avaframe-1.8b3/avaframe/tests/test_shpConversion.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_simiSol.py` & `avaframe-1.8b3/avaframe/tests/test_simiSol.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_snowSlide.py` & `avaframe-1.8b3/avaframe/tests/test_snowSlide.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_testUtilities.py` & `avaframe-1.8b3/avaframe/tests/test_testUtilities.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tests/test_timeDiscretization.py` & `avaframe-1.8b3/avaframe/tests/test_timeDiscretization.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/tmp1Ex/tmp1Ex.py` & `avaframe-1.8b3/avaframe/tmp1Ex/tmp1Ex.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe/version.py` & `avaframe-1.8b3/avaframe/version.py`

 * *Files identical despite different names*

### Comparing `avaframe-1.8b2/avaframe.egg-info/PKG-INFO` & `avaframe-1.8b3/avaframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avaframe
-Version: 1.8b2
+Version: 1.8b3
 Summary: The Open Avalanche Framework
 Home-page: http://avaframe.org
 Author: AvaFrame Contributors
 Author-email: felix@avaframe.org
 License: EUPL
 Description: **The AvaFrame documentation is hosted on ReadTheDocs: http://docs.avaframe.org**
```

### Comparing `avaframe-1.8b2/avaframe.egg-info/SOURCES.txt` & `avaframe-1.8b3/avaframe.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,16 @@
 avaframe/com3Hybrid/__init__.py
 avaframe/com3Hybrid/com3Hybrid.py
 avaframe/com3Hybrid/com3HybridCfg.ini
 avaframe/com4FlowPy/com4FlowPyCfg.ini
 avaframe/com5SnowSlide/__init__.py
 avaframe/com5SnowSlide/com5SnowSlide.py
 avaframe/com5SnowSlide/com5SnowSlideCfg.ini
+avaframe/com6RockAvalanche/__init__.py
+avaframe/com6RockAvalanche/com6RockAvalanche.py
 avaframe/com6RockAvalanche/com6RockAvalancheCfg.ini
 avaframe/data/avaDamBreak/Inputs/damBreak_com1DFACfg.ini
 avaframe/data/avaFPtest/Inputs/FlatPlane_com1DFACfg.ini
 avaframe/data/avaSimilaritySol/Inputs/simiSol_com1DFACfg.ini
 avaframe/in1Data/__init__.py
 avaframe/in1Data/computeFromDistribution.py
 avaframe/in1Data/computeFromDistributionCfg.ini
```

### Comparing `avaframe-1.8b2/setup.py` & `avaframe-1.8b3/setup.py`

 * *Files identical despite different names*

