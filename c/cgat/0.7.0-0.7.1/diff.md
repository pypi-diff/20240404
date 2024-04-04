# Comparing `tmp/cgat-0.7.0.tar.gz` & `tmp/cgat-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgat-0.7.0.tar", last modified: Mon Apr  1 21:18:17 2024, max compression
+gzip compressed data, was "cgat-0.7.1.tar", last modified: Thu Apr  4 14:46:03 2024, max compression
```

## Comparing `cgat-0.7.0.tar` & `cgat-0.7.1.tar`

### file list

```diff
@@ -1,174 +1,168 @@
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.087669 cgat-0.7.0/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1273 2024-04-01 08:10:13.000000 cgat-0.7.0/COPYING
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1188 2024-04-01 08:10:13.000000 cgat-0.7.0/LICENSE
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      680 2024-04-01 08:10:13.000000 cgat-0.7.0/MANIFEST.in
--rw-r--r--   0 caeruleus  (1000) caeruleus  (1000)      783 2024-04-01 21:18:17.087669 cgat-0.7.0/PKG-INFO
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2721 2024-04-01 08:10:13.000000 cgat-0.7.0/README.md
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      734 2024-04-01 08:10:13.000000 cgat-0.7.0/THANKS.txt
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.075668 cgat-0.7.0/cgat/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2378 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/AGP.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2016 2024-04-01 20:22:36.000000 cgat-0.7.0/cgat/AString.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.079668 cgat-0.7.0/cgat/BamTools/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    84091 2024-04-01 19:44:25.000000 cgat-0.7.0/cgat/BamTools/bamtools.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    73647 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/BamTools/geneprofile.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    13457 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/BamTools/peakshape.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    17233 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    28840 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Blat.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    39690 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/CBioPortal.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.079668 cgat-0.7.0/cgat/Components/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4766 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Components/Components.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3847 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Components/connected_components.cpp
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1734 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Components/connected_components.h
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3878 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/FastaIterator.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12895 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Fastq.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.079668 cgat-0.7.0/cgat/FastqTools/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3528 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/FastqTools/fastqtools.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3108 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/GFF3.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    31953 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/GTF.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)   185318 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/GeneModelAnalysis.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    49913 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/Genomics.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1053 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Glam2.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1492 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Glam2Scan.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19547 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Histogram.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1395 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Histogram2D.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4581 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/IGV.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    41375 2024-04-01 20:17:59.000000 cgat-0.7.0/cgat/IndexedFasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4570 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/IndexedGenome.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11505 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Intervals.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1756 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Iterators.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5499 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/MEME.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7369 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Masker.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12153 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/MatrixTools.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2312 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Motifs.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.079668 cgat-0.7.0/cgat/NCL/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5656 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/NCL/__init__.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4148 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/NCL/_cnestedlist.pxd
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19606 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/NCL/cnestedlist.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3933 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/NCL/default.h
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    32028 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/NCL/intervaldb.c
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4921 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/NCL/intervaldb.h
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1563 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/RLE.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5705 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/RateEstimation.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    36488 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/SVGdraw.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    40103 2024-04-01 15:50:46.000000 cgat-0.7.0/cgat/SequenceProperties.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6141 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/SetTools.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7596 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Sra.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    34513 2024-04-01 18:24:35.000000 cgat-0.7.0/cgat/Stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    20140 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Tree.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    44920 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/TreeTools.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3137 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/VCF.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.079668 cgat-0.7.0/cgat/VCFTools/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    25310 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/VCFTools/vcftools.pyx
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19027 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Variants.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/__init__.py
--rwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)     3480 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/cgat.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    28781 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/dictzip.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7542 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/makeGeneset.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.087669 cgat-0.7.0/cgat/tools/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/__init__.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    25343 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2bam.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1895 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2bam_split_reads.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6227 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3410 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2depth.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    16746 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4895 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2fastq.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    38204 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2geneprofile.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    37840 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    16966 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2wiggle.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2502 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2window_stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9672 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam_compare_alignments.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9070 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam_pileup2tsv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3866 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam_vs_bam.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8170 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam_vs_bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9174 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam_vs_gtf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8328 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bams2bam.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3208 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bcl2fastq.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    22414 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed2bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5688 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4029 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed2gff.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2181 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed2graph.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5363 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed2stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    24191 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4857 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed_vs_bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10208 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/beds2beds.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4295 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/beds2counts.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10672 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/cgat2dot.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5393 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/cgat_get_options.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2586 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/cgat_rebuild_extensions.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1033 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/cgat_script_template.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1470 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/csv2csv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10096 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/csvs2csv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9275 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/data2histogram.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7781 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/diff_bam.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11704 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/tools/diff_bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    15078 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/diff_chains.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9500 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/diff_fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14426 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/tools/diff_gtf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6238 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/extract_stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10207 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    21393 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/tools/fasta2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14562 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2fastq.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5500 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2kmercontent.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2682 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12477 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3771 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2variants.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2536 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2vcf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2281 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastas2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1884 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastq2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    17342 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastq2fastq.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5343 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastq2summary.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6364 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastq2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12133 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastq2tpm.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1337 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastq2tsv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5041 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastqs2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3534 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastqs2fastq.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9491 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastqs2fastqs.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2597 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/genome_bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5443 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11034 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2coverage.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14023 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    30534 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2gff.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9967 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2histogram.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4265 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2psl.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7200 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14982 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12848 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff32gtf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    18122 2024-04-01 20:23:32.000000 cgat-0.7.0/cgat/tools/gtf2fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    40355 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gtf2gff.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    52205 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gtf2gtf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    39563 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gtf2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11698 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gtf2tsv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11190 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gtfs2tsv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4123 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/index2bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12771 2024-04-01 13:26:07.000000 cgat-0.7.0/cgat/tools/index_fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6509 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/split_fasta.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7956 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/split_file.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4570 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/split_gff.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3071 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/table2stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2346 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/table2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9522 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/tables2table.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11183 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/vcf2tsv.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14736 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/vcf2vcf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8970 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/vcf_compare_phase.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6901 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/vcf_stats.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3447 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/vcf_vs_vcf.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6581 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/vcfstats2db.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6204 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/wig2bed.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       22 2024-04-01 20:35:56.000000 cgat-0.7.0/cgat/version.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.087669 cgat-0.7.0/cgat.egg-info/
--rw-r--r--   0 caeruleus  (1000) caeruleus  (1000)      783 2024-04-01 21:18:17.000000 cgat-0.7.0/cgat.egg-info/PKG-INFO
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3683 2024-04-01 21:18:17.000000 cgat-0.7.0/cgat.egg-info/SOURCES.txt
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        1 2024-04-01 21:18:17.000000 cgat-0.7.0/cgat.egg-info/dependency_links.txt
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       40 2024-04-01 21:18:17.000000 cgat-0.7.0/cgat.egg-info/entry_points.txt
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        1 2024-04-01 08:12:17.000000 cgat-0.7.0/cgat.egg-info/not-zip-safe
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        5 2024-04-01 21:18:17.000000 cgat-0.7.0/cgat.egg-info/top_level.txt
--rwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)    26056 2024-04-01 08:10:13.000000 cgat-0.7.0/install.sh
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 08:10:13.000000 cgat-0.7.0/requires.txt
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       38 2024-04-01 21:18:17.087669 cgat-0.7.0/setup.cfg
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10750 2024-04-01 08:10:13.000000 cgat-0.7.0/setup.py
-drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.087669 cgat-0.7.0/tests/
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      795 2024-04-01 08:10:14.000000 cgat-0.7.0/tests/testComponents.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6974 2024-04-01 08:10:14.000000 cgat-0.7.0/tests/test_commandline.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3267 2024-04-01 08:10:14.000000 cgat-0.7.0/tests/test_import.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11530 2024-04-01 08:10:14.000000 cgat-0.7.0/tests/test_scripts.py
--rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2277 2024-04-01 08:10:14.000000 cgat-0.7.0/tests/test_style.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.272001 cgat-0.7.1/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1188 2024-04-01 08:10:13.000000 cgat-0.7.1/LICENSE
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      680 2024-04-01 08:10:13.000000 cgat-0.7.1/MANIFEST.in
+-rw-r--r--   0 caeruleus  (1000) caeruleus  (1000)      761 2024-04-04 14:46:03.272001 cgat-0.7.1/PKG-INFO
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2721 2024-04-01 08:10:13.000000 cgat-0.7.1/README.md
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      734 2024-04-01 08:10:13.000000 cgat-0.7.1/THANKS.txt
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.260001 cgat-0.7.1/cgat/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2765 2024-04-04 14:37:59.000000 cgat-0.7.1/cgat/AGP.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2016 2024-04-04 08:06:46.000000 cgat-0.7.1/cgat/AString.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.260001 cgat-0.7.1/cgat/BamTools/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    84091 2024-04-04 08:06:46.000000 cgat-0.7.1/cgat/BamTools/bamtools.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    73647 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/BamTools/geneprofile.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    13457 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/BamTools/peakshape.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    17233 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    29497 2024-04-04 12:43:35.000000 cgat-0.7.1/cgat/Blat.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.260001 cgat-0.7.1/cgat/Components/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4766 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Components/Components.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3847 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Components/connected_components.cpp
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1734 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Components/connected_components.h
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3878 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/FastaIterator.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12895 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Fastq.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.260001 cgat-0.7.1/cgat/FastqTools/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3528 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/FastqTools/fastqtools.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3108 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/GFF3.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    31953 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/GTF.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)   185318 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/GeneModelAnalysis.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    49913 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/Genomics.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1053 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Glam2.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1492 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Glam2Scan.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19547 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Histogram.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1395 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Histogram2D.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    41337 2024-04-04 12:43:35.000000 cgat-0.7.1/cgat/IndexedFasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4570 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/IndexedGenome.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11505 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Intervals.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1756 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Iterators.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5499 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/MEME.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7369 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Masker.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12153 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/MatrixTools.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2312 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Motifs.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.264001 cgat-0.7.1/cgat/NCL/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5656 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/NCL/__init__.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4148 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/NCL/_cnestedlist.pxd
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19606 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/NCL/cnestedlist.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3933 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/NCL/default.h
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    32028 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/NCL/intervaldb.c
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4921 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/NCL/intervaldb.h
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1563 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/RLE.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5705 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/RateEstimation.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    40094 2024-04-04 12:43:35.000000 cgat-0.7.1/cgat/SequenceProperties.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6141 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/SetTools.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7596 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Sra.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    34513 2024-04-04 08:06:46.000000 cgat-0.7.1/cgat/Stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    20140 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Tree.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    44920 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/TreeTools.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3137 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/VCF.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.264001 cgat-0.7.1/cgat/VCFTools/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    25310 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/VCFTools/vcftools.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19027 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/Variants.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/__init__.py
+-rwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)     3480 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/cgat.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    28781 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/dictzip.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7542 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/makeGeneset.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.272001 cgat-0.7.1/cgat/tools/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/__init__.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    25343 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2bam.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1895 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2bam_split_reads.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6227 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3410 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2depth.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    16746 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4895 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    38204 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2geneprofile.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    37840 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    16966 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2wiggle.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2502 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam2window_stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9672 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam_compare_alignments.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9070 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam_pileup2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3866 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam_vs_bam.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8170 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam_vs_bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9174 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bam_vs_gtf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8328 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bams2bam.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3208 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bcl2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    22414 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5688 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4029 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed2gff.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2181 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed2graph.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5363 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    24191 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4857 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/bed_vs_bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10208 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/beds2beds.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4295 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/beds2counts.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10672 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/cgat2dot.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5393 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/cgat_get_options.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2586 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/cgat_rebuild_extensions.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1033 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/cgat_script_template.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1470 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/csv2csv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10096 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/csvs2csv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9275 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/data2histogram.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7781 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/diff_bam.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11704 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/tools/diff_bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    15078 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/diff_chains.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9500 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/diff_fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14426 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/tools/diff_gtf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6238 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/extract_stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10207 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    21393 2024-04-01 12:48:18.000000 cgat-0.7.1/cgat/tools/fasta2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14562 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5500 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2kmercontent.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2682 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12477 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3771 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2variants.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2536 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fasta2vcf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2281 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastas2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1884 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastq2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    17342 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastq2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5343 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastq2summary.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6364 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastq2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12133 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastq2tpm.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1337 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastq2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5041 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastqs2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3534 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastqs2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9491 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/fastqs2fastqs.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2597 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/genome_bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5443 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11034 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff2coverage.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14023 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    30644 2024-04-04 13:58:31.000000 cgat-0.7.1/cgat/tools/gff2gff.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9967 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff2histogram.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4537 2024-04-04 12:43:35.000000 cgat-0.7.1/cgat/tools/gff2psl.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7200 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14982 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12848 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gff32gtf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    18122 2024-04-04 08:06:46.000000 cgat-0.7.1/cgat/tools/gtf2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    40355 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gtf2gff.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    52205 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gtf2gtf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    39563 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gtf2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11698 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gtf2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11190 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/gtfs2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4123 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/index2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12771 2024-04-01 13:26:07.000000 cgat-0.7.1/cgat/tools/index_fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6509 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/split_fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7956 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/split_file.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4570 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/split_gff.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3071 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/table2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2346 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/table2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9522 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/tables2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11183 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/vcf2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14736 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/vcf2vcf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8970 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/vcf_compare_phase.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6901 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/vcf_stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3447 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/vcf_vs_vcf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6581 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/vcfstats2db.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6204 2024-04-01 08:10:13.000000 cgat-0.7.1/cgat/tools/wig2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       22 2024-04-04 14:21:30.000000 cgat-0.7.1/cgat/version.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.272001 cgat-0.7.1/cgat.egg-info/
+-rw-r--r--   0 caeruleus  (1000) caeruleus  (1000)      761 2024-04-04 14:46:03.000000 cgat-0.7.1/cgat.egg-info/PKG-INFO
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3604 2024-04-04 14:46:03.000000 cgat-0.7.1/cgat.egg-info/SOURCES.txt
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        1 2024-04-04 14:46:03.000000 cgat-0.7.1/cgat.egg-info/dependency_links.txt
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       40 2024-04-04 14:46:03.000000 cgat-0.7.1/cgat.egg-info/entry_points.txt
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        1 2024-04-04 14:30:05.000000 cgat-0.7.1/cgat.egg-info/not-zip-safe
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        5 2024-04-04 14:46:03.000000 cgat-0.7.1/cgat.egg-info/top_level.txt
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       38 2024-04-04 14:46:03.272001 cgat-0.7.1/setup.cfg
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9667 2024-04-04 14:06:34.000000 cgat-0.7.1/setup.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-04 14:46:03.272001 cgat-0.7.1/tests/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      795 2024-04-01 08:10:14.000000 cgat-0.7.1/tests/testComponents.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6048 2024-04-04 14:15:54.000000 cgat-0.7.1/tests/test_commandline.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3267 2024-04-01 08:10:14.000000 cgat-0.7.1/tests/test_import.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11491 2024-04-04 12:43:35.000000 cgat-0.7.1/tests/test_scripts.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2277 2024-04-01 08:10:14.000000 cgat-0.7.1/tests/test_style.py
```

### Comparing `cgat-0.7.0/LICENSE` & `cgat-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/MANIFEST.in` & `cgat-0.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/PKG-INFO` & `cgat-0.7.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgat
-Version: 0.7.0
+Version: 0.7.1
 Summary: cgat : the Computational Genomics Analysis Toolkit
 Home-page: http://www.cgat.org/cgat/Tools/
 Author: Andreas Heger
 Author-email: andreas.heger@gmail.com
 License: MIT
 Keywords: computational genomics
 Platform: any
@@ -15,10 +15,9 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 License-File: LICENSE
-License-File: COPYING
 
 cgat : the Computational Genomics Analysis Toolkit
```

### Comparing `cgat-0.7.0/README.md` & `cgat-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/THANKS.txt` & `cgat-0.7.1/THANKS.txt`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/AGP.py` & `cgat-0.7.1/cgat/AGP.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,24 +5,40 @@
 files.
 
 Code
 ----
 
 """
 
+import functools
 
+
+def deprecated_class(cls):
+    orig_init = cls.__init__
+
+    @functools.wraps(orig_init)
+    def new_init(self, *args, **kwargs):
+        warnings.warn(f"{cls.__name__} is deprecated and will be removed in the next release.", DeprecationWarning)
+        orig_init(self, *args, **kwargs)
+
+    cls.__init__ = new_init
+    return cls
+
+
+@deprecated_class
 class ObjectPosition(object):
 
     def map(self, start, end):
         if self.mOrientation:
             return start + self.start, end + self.start
         else:
             return end + self.start, start + self.start
 
 
+@deprecated_class
 class AGP(object):
     """Parser for AGP formatted files."""
 
     def readFromFile(self, infile):
         """read an agp file.
 
         Example line::
```

### Comparing `cgat-0.7.0/cgat/AString.py` & `cgat-0.7.1/cgat/AString.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/BamTools/bamtools.pyx` & `cgat-0.7.1/cgat/BamTools/bamtools.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/BamTools/geneprofile.pyx` & `cgat-0.7.1/cgat/BamTools/geneprofile.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/BamTools/peakshape.pyx` & `cgat-0.7.1/cgat/BamTools/peakshape.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Bed.py` & `cgat-0.7.1/cgat/Bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Blat.py` & `cgat-0.7.1/cgat/Blat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,72 @@
 '''Blat.py - tools for working with PSL formatted files and data
 =============================================================
 
+IMPORTANT NOTICE:
+Several functions within this module are scheduled for
+deprecation in May 2024.
+Details regarding the specific functions to be deprecated
+can be found in the documentation of each function.
+
+
 This module provides a class to parse :term:`PSL` formatted
 files such as those output by the BLAT tool.
 
 This module defines the :class:`Blat.Match` class representing a
-single entry and a series of iterators to iterate of :term:`PSL`
+single entry and a series of iterators to iterate of :term:`SL`
 formatted files (:func:`iterator`, :func:`iterator_target_overlap`,
 ...).
 
 Reference
 ---------
 
 '''
 import copy
 import string
 import collections
+import warnings
+import functools
 
 try:
     import alignlib_lite
 except ImportError:
     pass
 
 from cgat import Components as Components
 from cgatcore import experiment as E
 
 
+def deprecated_class(cls):
+    orig_init = cls.__init__
+
+    @functools.wraps(orig_init)
+    def new_init(self, *args, **kwargs):
+        warnings.warn(f"{cls.__name__} is deprecated and will be removed in May 2024.", DeprecationWarning)
+        orig_init(self, *args, **kwargs)
+
+    cls.__init__ = new_init
+    return cls
+
+
+@deprecated_class
 class Error(Exception):
     """Base class for exceptions in this module."""
 
     def __str__(self):
         return str(self._message)
 
     def _get_message(self):
         return self._message
 
     def _set_message(self, message):
         self._message = message
     message = property(_get_message, _set_message)
 
 
+@deprecated_class
 class ParsingError(Error):
 
     """Exception raised for errors while parsing
 
     Attributes:
         message -- explanation of the error
     """
@@ -57,14 +80,15 @@
 HEADER = """psLayout version 3
 
 match   mis-    rep.    N's     Q gap   Q gap   T gap   T gap   strand  Q       Q       Q       Q       T       T       T       T       block   blockSizes      qStarts  tStarts
         match                   count   bases   count   bases           name    size    start   end     name    size    start   end     count
 ---------------------------------------------------------------------------------------------------------------------------------------------------------------"""
 
 
+@deprecated_class
 class Match:
 
     """a :term:`psl` formatted alignment.
 
     Block coordinates are on the forward strand for target and on
     the forward/reverse strand for the query depending on the strand.
 
@@ -475,14 +499,15 @@
                 "qGapCount", "qGapBases", "tGapCount", "tGapBases", "strand",
                 "qName", "qSize", "qStart", "qEnd",
                 "tName", "tSize", "tStart", "tEnd",
                 "blockCount", "blockSizes",
                 "qStarts", "tStarts")
 
 
+@deprecated_class
 class MatchPSLX(Match):
 
     def __init__(self):
         Match.__init__(self)
         self.mQuerySequence = []
         self.mSbjctSequence = []
 
@@ -597,14 +622,15 @@
             continue
 
         match = Match()
         match.fromTable(line[:-1].split("\t"))
         yield match
 
 
+@deprecated_class
 class BlatIterator:
 
     def __init__(self, f, *args, **kwargs):
         self.mIterator = _iterate(f)
 
     def __iter__(self):
         return self
```

### Comparing `cgat-0.7.0/cgat/Components/Components.pyx` & `cgat-0.7.1/cgat/Components/Components.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Components/connected_components.cpp` & `cgat-0.7.1/cgat/Components/connected_components.cpp`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Components/connected_components.h` & `cgat-0.7.1/cgat/Components/connected_components.h`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/FastaIterator.py` & `cgat-0.7.1/cgat/FastaIterator.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Fastq.py` & `cgat-0.7.1/cgat/Fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/FastqTools/fastqtools.pyx` & `cgat-0.7.1/cgat/FastqTools/fastqtools.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/GFF3.py` & `cgat-0.7.1/cgat/GFF3.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/GTF.py` & `cgat-0.7.1/cgat/GTF.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/GeneModelAnalysis.pyx` & `cgat-0.7.1/cgat/GeneModelAnalysis.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Genomics.py` & `cgat-0.7.1/cgat/Genomics.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Glam2.py` & `cgat-0.7.1/cgat/Glam2.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Glam2Scan.py` & `cgat-0.7.1/cgat/Glam2Scan.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Histogram.py` & `cgat-0.7.1/cgat/Histogram.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Histogram2D.py` & `cgat-0.7.1/cgat/Histogram2D.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/IndexedFasta.py` & `cgat-0.7.1/cgat/IndexedFasta.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 only of internal use.
 
 Reference
 ----------
 
 '''
 
-from __future__ import generator_stop
 import os
 import sys
 import array
 import string
 import re
 import struct
 import math
```

### Comparing `cgat-0.7.0/cgat/IndexedGenome.py` & `cgat-0.7.1/cgat/IndexedGenome.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Intervals.py` & `cgat-0.7.1/cgat/Intervals.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Iterators.py` & `cgat-0.7.1/cgat/Iterators.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/MEME.py` & `cgat-0.7.1/cgat/MEME.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Masker.py` & `cgat-0.7.1/cgat/Masker.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/MatrixTools.py` & `cgat-0.7.1/cgat/MatrixTools.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Motifs.py` & `cgat-0.7.1/cgat/Motifs.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/NCL/__init__.py` & `cgat-0.7.1/cgat/NCL/__init__.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/NCL/_cnestedlist.pxd` & `cgat-0.7.1/cgat/NCL/_cnestedlist.pxd`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/NCL/cnestedlist.pyx` & `cgat-0.7.1/cgat/NCL/cnestedlist.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/NCL/default.h` & `cgat-0.7.1/cgat/NCL/default.h`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/NCL/intervaldb.c` & `cgat-0.7.1/cgat/NCL/intervaldb.c`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/NCL/intervaldb.h` & `cgat-0.7.1/cgat/NCL/intervaldb.h`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/RLE.py` & `cgat-0.7.1/cgat/RLE.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/RateEstimation.py` & `cgat-0.7.1/cgat/RateEstimation.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/SequenceProperties.py` & `cgat-0.7.1/cgat/SequenceProperties.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 """
 
 import re
 import math
 import hashlib
 import base64
 import itertools
-import six
 
 from cgat import Genomics as Genomics
 
 
 class SequenceProperties(object):
     """Base class.
 
@@ -133,15 +132,15 @@
         self.mHid = ""
 
     def loadSequence(self, sequence, seqtype="na"):
         """load hid sequence properties from a sequence."""
         SequenceProperties.loadSequence(self, sequence, seqtype)
 
         # do the encryption
-        h = hashlib.md5(six.b(sequence)).digest()
+        h = hashlib.md5(sequence.encode()).digest()
         # map to printable letters: hid has length 22, so the padded '=' are
         # truncated. You have to add them, if you ever want to decode,
         # but who would do such a thing :=)
         r = base64.encodebytes(h)[0:22].decode("ascii")
 
         # finally substitute some characters:
         # '/' for '_', so we have legal file names
```

### Comparing `cgat-0.7.0/cgat/SetTools.py` & `cgat-0.7.1/cgat/SetTools.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Sra.py` & `cgat-0.7.1/cgat/Sra.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Stats.py` & `cgat-0.7.1/cgat/Stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Tree.py` & `cgat-0.7.1/cgat/Tree.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/TreeTools.py` & `cgat-0.7.1/cgat/TreeTools.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/VCF.py` & `cgat-0.7.1/cgat/VCF.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/VCFTools/vcftools.pyx` & `cgat-0.7.1/cgat/VCFTools/vcftools.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/Variants.py` & `cgat-0.7.1/cgat/Variants.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/cgat.py` & `cgat-0.7.1/cgat/cgat.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/dictzip.py` & `cgat-0.7.1/cgat/dictzip.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/makeGeneset.py` & `cgat-0.7.1/cgat/makeGeneset.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam2bam.py` & `cgat-0.7.1/cgat/tools/bam2bam.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam2bam_split_reads.py` & `cgat-0.7.1/cgat/tools/bam2bam_split_reads.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam2bed.py` & `cgat-0.7.1/cgat/tools/bam2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam2depth.py` & `cgat-0.7.1/cgat/tools/bam2depth.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam2fasta.py` & `cgat-0.7.1/cgat/tools/bam2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam2fastq.py` & `cgat-0.7.1/cgat/tools/bam2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam2geneprofile.py` & `cgat-0.7.1/cgat/tools/bam2geneprofile.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam2stats.py` & `cgat-0.7.1/cgat/tools/bam2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam2wiggle.py` & `cgat-0.7.1/cgat/tools/bam2wiggle.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam2window_stats.py` & `cgat-0.7.1/cgat/tools/bam2window_stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam_compare_alignments.py` & `cgat-0.7.1/cgat/tools/bam_compare_alignments.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam_pileup2tsv.py` & `cgat-0.7.1/cgat/tools/bam_pileup2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam_vs_bam.py` & `cgat-0.7.1/cgat/tools/bam_vs_bam.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam_vs_bed.py` & `cgat-0.7.1/cgat/tools/bam_vs_bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bam_vs_gtf.py` & `cgat-0.7.1/cgat/tools/bam_vs_gtf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bams2bam.py` & `cgat-0.7.1/cgat/tools/bams2bam.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bcl2fastq.py` & `cgat-0.7.1/cgat/tools/bcl2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bed2bed.py` & `cgat-0.7.1/cgat/tools/bed2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bed2fasta.py` & `cgat-0.7.1/cgat/tools/bed2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bed2gff.py` & `cgat-0.7.1/cgat/tools/bed2gff.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bed2graph.py` & `cgat-0.7.1/cgat/tools/bed2graph.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bed2stats.py` & `cgat-0.7.1/cgat/tools/bed2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bed2table.py` & `cgat-0.7.1/cgat/tools/bed2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/bed_vs_bed.py` & `cgat-0.7.1/cgat/tools/bed_vs_bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/beds2beds.py` & `cgat-0.7.1/cgat/tools/beds2beds.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/beds2counts.py` & `cgat-0.7.1/cgat/tools/beds2counts.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/cgat2dot.py` & `cgat-0.7.1/cgat/tools/cgat2dot.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/cgat_get_options.py` & `cgat-0.7.1/cgat/tools/cgat_get_options.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/cgat_rebuild_extensions.py` & `cgat-0.7.1/cgat/tools/cgat_rebuild_extensions.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/cgat_script_template.py` & `cgat-0.7.1/cgat/tools/cgat_script_template.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/csv2csv.py` & `cgat-0.7.1/cgat/tools/csv2csv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/csvs2csv.py` & `cgat-0.7.1/cgat/tools/csvs2csv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/data2histogram.py` & `cgat-0.7.1/cgat/tools/data2histogram.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/diff_bam.py` & `cgat-0.7.1/cgat/tools/diff_bam.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/diff_bed.py` & `cgat-0.7.1/cgat/tools/diff_bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/diff_chains.py` & `cgat-0.7.1/cgat/tools/diff_chains.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/diff_fasta.py` & `cgat-0.7.1/cgat/tools/diff_fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/diff_gtf.py` & `cgat-0.7.1/cgat/tools/diff_gtf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/extract_stats.py` & `cgat-0.7.1/cgat/tools/extract_stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fasta2bed.py` & `cgat-0.7.1/cgat/tools/fasta2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fasta2fasta.py` & `cgat-0.7.1/cgat/tools/fasta2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fasta2fastq.py` & `cgat-0.7.1/cgat/tools/fasta2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fasta2kmercontent.py` & `cgat-0.7.1/cgat/tools/fasta2kmercontent.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fasta2stats.py` & `cgat-0.7.1/cgat/tools/fasta2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fasta2table.py` & `cgat-0.7.1/cgat/tools/fasta2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fasta2variants.py` & `cgat-0.7.1/cgat/tools/fasta2variants.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fasta2vcf.py` & `cgat-0.7.1/cgat/tools/fasta2vcf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fastas2fasta.py` & `cgat-0.7.1/cgat/tools/fastas2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fastq2fasta.py` & `cgat-0.7.1/cgat/tools/fastq2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fastq2fastq.py` & `cgat-0.7.1/cgat/tools/fastq2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fastq2summary.py` & `cgat-0.7.1/cgat/tools/fastq2summary.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fastq2table.py` & `cgat-0.7.1/cgat/tools/fastq2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fastq2tpm.py` & `cgat-0.7.1/cgat/tools/fastq2tpm.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fastq2tsv.py` & `cgat-0.7.1/cgat/tools/fastq2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fastqs2fasta.py` & `cgat-0.7.1/cgat/tools/fastqs2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fastqs2fastq.py` & `cgat-0.7.1/cgat/tools/fastqs2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/fastqs2fastqs.py` & `cgat-0.7.1/cgat/tools/fastqs2fastqs.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/genome_bed.py` & `cgat-0.7.1/cgat/tools/genome_bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/gff2bed.py` & `cgat-0.7.1/cgat/tools/gff2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/gff2coverage.py` & `cgat-0.7.1/cgat/tools/gff2coverage.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/gff2fasta.py` & `cgat-0.7.1/cgat/tools/gff2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/gff2gff.py` & `cgat-0.7.1/cgat/tools/gff2gff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 '''gff2gff.py - manipulate gff files
 =================================
 
 :Tags: Genomics Intervals GFF Manipulation
 
+Note: The script can parse AGP files but this functionality
+is scheduled for deprecation in the next release.
 
 Purpose
 -------
 
 This scripts reads a :term:`gff` formatted file, applies a
 transformation and outputs the new intervals in :term:`gff` format.
 The type of transformation chosen is given through the `--method``
```

### Comparing `cgat-0.7.0/cgat/tools/gff2histogram.py` & `cgat-0.7.1/cgat/tools/gff2histogram.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/gff2psl.py` & `cgat-0.7.1/cgat/tools/gff2psl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 '''
 gff2psl.py - convert from gff to psl
 ====================================
 
 :Tags: Genomics Intervals GFF PSL Conversion
 
+Note: This script is scheduled for deprecation in May 2024.
+
 Purpose
 -------
 
 This scripts converts from a :term:`gff` formatted
 file to a :term:`psl` formatted file.
 The output can be modified by the following command line options:
 
@@ -43,20 +45,27 @@
 import cgat.IndexedFasta as IndexedFasta
 import cgat.Blat as Blat
 import cgat.GTF as GTF
 import alignlib_lite
 import cgat.Intervals as Intervals
 
 
+def print_deprecation_warning():
+    warning_message = ("""WARNING: 'gff2psl.py' is deprecated and will be removed in May 2024.""")
+    print(warning_message, file=sys.stderr)
+
+
 def main(argv=None):
     """script main.
 
     parses command line options in sys.argv, unless *argv* is given.
     """
 
+    print_deprecation_warning()
+
     if argv is None:
         argv = sys.argv
 
     parser = E.ArgumentParser(description=__doc__)
 
     parser.add_argument("--version", action='version', version="1.0")
```

### Comparing `cgat-0.7.0/cgat/tools/gff2stats.py` & `cgat-0.7.1/cgat/tools/gff2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/gff2table.py` & `cgat-0.7.1/cgat/tools/gff2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/gff32gtf.py` & `cgat-0.7.1/cgat/tools/gff32gtf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/gtf2fasta.py` & `cgat-0.7.1/cgat/tools/gtf2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/gtf2gff.py` & `cgat-0.7.1/cgat/tools/gtf2gff.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/gtf2gtf.py` & `cgat-0.7.1/cgat/tools/gtf2gtf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/gtf2table.py` & `cgat-0.7.1/cgat/tools/gtf2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/gtf2tsv.py` & `cgat-0.7.1/cgat/tools/gtf2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/gtfs2tsv.py` & `cgat-0.7.1/cgat/tools/gtfs2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/index2bed.py` & `cgat-0.7.1/cgat/tools/index2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/index_fasta.py` & `cgat-0.7.1/cgat/tools/index_fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/split_fasta.py` & `cgat-0.7.1/cgat/tools/split_fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/split_file.py` & `cgat-0.7.1/cgat/tools/split_file.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/split_gff.py` & `cgat-0.7.1/cgat/tools/split_gff.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/table2stats.py` & `cgat-0.7.1/cgat/tools/table2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/table2table.py` & `cgat-0.7.1/cgat/tools/table2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/tables2table.py` & `cgat-0.7.1/cgat/tools/tables2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/vcf2tsv.py` & `cgat-0.7.1/cgat/tools/vcf2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/vcf2vcf.py` & `cgat-0.7.1/cgat/tools/vcf2vcf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/vcf_compare_phase.py` & `cgat-0.7.1/cgat/tools/vcf_compare_phase.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/vcf_stats.py` & `cgat-0.7.1/cgat/tools/vcf_stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/vcf_vs_vcf.py` & `cgat-0.7.1/cgat/tools/vcf_vs_vcf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/vcfstats2db.py` & `cgat-0.7.1/cgat/tools/vcfstats2db.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat/tools/wig2bed.py` & `cgat-0.7.1/cgat/tools/wig2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/cgat.egg-info/PKG-INFO` & `cgat-0.7.1/cgat.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgat
-Version: 0.7.0
+Version: 0.7.1
 Summary: cgat : the Computational Genomics Analysis Toolkit
 Home-page: http://www.cgat.org/cgat/Tools/
 Author: Andreas Heger
 Author-email: andreas.heger@gmail.com
 License: MIT
 Keywords: computational genomics
 Platform: any
@@ -15,10 +15,9 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 License-File: LICENSE
-License-File: COPYING
 
 cgat : the Computational Genomics Analysis Toolkit
```

### Comparing `cgat-0.7.0/cgat.egg-info/SOURCES.txt` & `cgat-0.7.1/cgat.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,36 @@
-COPYING
 LICENSE
 MANIFEST.in
 README.md
 THANKS.txt
-install.sh
-requires.txt
 setup.py
 cgat/AGP.py
 cgat/AString.py
 cgat/Bed.py
 cgat/Blat.py
-cgat/CBioPortal.py
 cgat/FastaIterator.py
 cgat/Fastq.py
 cgat/GFF3.py
 cgat/GTF.py
 cgat/GeneModelAnalysis.pyx
 cgat/Genomics.py
 cgat/Glam2.py
 cgat/Glam2Scan.py
 cgat/Histogram.py
 cgat/Histogram2D.py
-cgat/IGV.py
 cgat/IndexedFasta.py
 cgat/IndexedGenome.py
 cgat/Intervals.py
 cgat/Iterators.py
 cgat/MEME.py
 cgat/Masker.py
 cgat/MatrixTools.py
 cgat/Motifs.py
 cgat/RLE.py
 cgat/RateEstimation.py
-cgat/SVGdraw.py
 cgat/SequenceProperties.py
 cgat/SetTools.py
 cgat/Sra.py
 cgat/Stats.py
 cgat/Tree.py
 cgat/TreeTools.py
 cgat/VCF.py
```

### Comparing `cgat-0.7.0/setup.py` & `cgat-0.7.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -133,45 +133,14 @@
     return None
 
 REPO_REQUIREMENT = re.compile(
     r'^-e (?P<link>(?P<vcs>git|svn|hg|bzr).+#egg=(?P<package>.+)-(?P<version>\d(?:\.\d)*))$')
 HTTPS_REQUIREMENT = re.compile(
     r'^-e (?P<link>.*).+#(?P<package>.+)-(?P<version>\d(?:\.\d)*)$')
 install_requires = []
-dependency_links = []
-
-for requirement in (
-        l.strip() for l in open('requires.txt') if not l.startswith("#")):
-    match = REPO_REQUIREMENT.match(requirement)
-    if match:
-        assert which(match.group('vcs')) is not None, \
-            ("VCS '%(vcs)s' must be installed in order to "
-             "install %(link)s" % match.groupdict())
-        install_requires.append("%(package)s==%(version)s" % match.groupdict())
-        dependency_links.append(match.group('link'))
-        continue
-
-    if requirement.startswith("https"):
-        install_requires.append(requirement)
-        continue
-
-    match = HTTPS_REQUIREMENT.match(requirement)
-    if match:
-        install_requires.append("%(package)s>=%(version)s" % match.groupdict())
-        dependency_links.append(match.group('link'))
-        continue
-
-    install_requires.append(requirement)
-
-if major == 2:
-    install_requires.extend(['web.py>=0.37',
-                             'xlwt>=0.7.4',
-                             'matplotlib-venn>=0.5'])
-elif major == 3:
-    pass
 
 cgat_packages = find_packages()
 cgat_package_dirs = {'cgat': 'cgat'}
 
 ##########################################################
 ##########################################################
 # classifiers
@@ -313,15 +282,14 @@
     package_dir=cgat_package_dirs,
     include_package_data=True,
     entry_points={
         'console_scripts': ['cgat = cgat.cgat:main']
     },
     # dependencies
     install_requires=install_requires,
-    dependency_links=dependency_links,
     # extension modules
     ext_modules=extensions,
     cmdclass={'build_ext': build_ext},
     # other options
     zip_safe=False,
     test_suite="tests",
 )
```

### Comparing `cgat-0.7.0/tests/testComponents.py` & `cgat-0.7.1/tests/testComponents.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/tests/test_commandline.py` & `cgat-0.7.1/tests/test_commandline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,249 +1,187 @@
-'''test_commandline - test coding style confirmation of CGAT code
-===========================================================
+'''
+test_commandline - Tests coding style conformity of CGAT code collection.
+==========================================================================
 
 :Author: Andreas Heger
 :Release: $Id$
 :Date: |today|
 :Tags: Python
 
 Purpose
 -------
-
-This script test the command line usage of all scripts in the
-CGAT code collection.
-
-This script is best run within nosetests::
+This script tests the command line usage of all scripts in the CGAT code collection.
+It's recommended to run this within nosetests for efficiency and coverage:
 
    nosetests tests/test_commandline.py --nocapture
 
+Before running these tests, ensure to execute:
 
-.. note::
-
-   Make sure to run::
-
-       python setup.py develop
-
-   Before running these tests.
+   python setup.py develop
 
+to make all package scripts available for import and testing.
 '''
+
 import glob
 import os
 import importlib
 import yaml
 import re
 import sys
 import copy
-import platform
+import argparse
 
 from nose.tools import ok_
 import cgatcore.experiment as E
 import cgatcore.iotools as iotools
 import TestUtils
 
-# handle to original E.Start function
-ORIGINAL_START = None
+# Preserve the original E.Start function for later restoration
+ORIGINAL_START = E.start
 
-# Parser object collected from child script
+# Placeholders for parser object and tested script's module
 PARSER = None
+TESTED_MODULE = None
 
-# DIRECTORIES to examine for python modules/scripts
+# Directories to examine for Python modules/scripts
 EXPRESSIONS = (
-    ('tools', 'cgat/tools/*.py'),)
+    ('tools', 'cgat/tools/*.py'),
+)
 
+# Files to exclude from checks
 EXCLUDE = [
     "__init__.py",
     "version.py",
     "cgat.py",
-    "gtf2table.py",  # fails with pysam include issue
-    "bed2table.py",  # fails with pysam include issue
-    "fasta2bed.py",   # fails because of pybedtools rebuild
+    "gtf2table.py",   # Fails with pysam include issue
+    "bed2table.py",   # Fails with pysam include issue
+    "fasta2bed.py",   # Fails due to pybedtools rebuild requirements
 ]
 
-# Filename with the black/white list of options.
-# The file is a tab-separated with the first column
-# an option name and the second field a marker.
-# Possible markers are:
-# ok = whitelist - this option is ok.
-# 'bad', 'rename', '?', '' - this option is not ok.
+# Filename for the black/white list of options
 FILENAME_OPTIONLIST = "tests/option_list.tsv"
 
 
 class DummyError(Exception):
+    """Custom exception for controlling test flow."""
     pass
 
 
 def filter_files(files):
-    '''filter list of files according to filters set in
-    configuration file tests/_test_commandline.yml'''
-
-    # directory location of tests
+    '''Filter list of files according to filters set in the configuration file tests/_test_commandline.yml'''
     testing_dir = TestUtils.get_tests_directory()
-
-    # the config file
     config_file = os.path.join(testing_dir, "_test_commandline.yml")
 
     if os.path.exists(config_file):
-        config = yaml.safe_load(open(config_file))
-        if config is not None:
-            if "restrict" in config and config["restrict"]:
+        with open(config_file) as cf:
+            config = yaml.safe_load(cf)
+            if config and "restrict" in config:
                 values = config["restrict"]
                 if "manifest" in values:
-                    # take scripts defined in the MANIFEST.in file
-                    scriptdirs = [x for x in open("MANIFEST.in")
-                                  if x.startswith("include CGAT/tools") and
-                                  x.endswith(".py\n")]
-
-                    take = set([re.sub("include\s*", "",
-                                       x[:-1]) for x in scriptdirs])
+                    scriptdirs = [x.strip() for x in open("MANIFEST.in")
+                                  if x.startswith("include CGAT/tools") and x.endswith(".py\n")]
+                    take = set(re.sub("include\s*", "", x) for x in scriptdirs)
                     files = [x for x in files if x in take]
-
                 if "regex" in values:
                     rx = re.compile(values["regex"])
-                    files = filter(rx.search, files)
+                    files = list(filter(rx.search, files))
     return files
 
 
 def LocalStart(parser, *args, **kwargs):
-    '''stub for E.start - set return_parser argument to true'''
+    '''Stub for E.start - captures the parser for inspection.'''
     global PARSER
-    d = copy.copy(kwargs)
-    d.update({'return_parser': True})
-    PARSER = ORIGINAL_START(parser, **d)
+    kwargs.update({'return_parser': True})
+    PARSER = ORIGINAL_START(parser, **kwargs)
     raise DummyError()
 
 
 def load_script(script_name):
+    '''Attempts to import a script as a module for inspection.'''
+    script_path = os.path.splitext(script_name)[0]
+    script_dir, script_base = os.path.split(script_path)
+    module_name = ".".join(filter(None, [script_dir.replace(os.sep, '.'), script_base]))
+
+    # Remove compiled files to ensure fresh import
+    compiled_script = script_path + ".pyc"
+    if os.path.exists(compiled_script):
+        os.remove(compiled_script)
 
-    # call other script
-    prefix, suffix = os.path.splitext(script_name)
-
-    dirname = os.path.relpath(os.path.dirname(script_name))
-    basename = os.path.basename(script_name)[:-3]
-
-    if os.path.exists(prefix + ".pyc"):
-        try:
-            os.remove(prefix + ".pyc")
-        except OSError:
-            pass
-
-    modulename = ".".join((re.sub("/", ".", dirname), basename))
     try:
-        module = importlib.import_module(modulename)
-    except ImportError as msg:
-        sys.stderr.write('could not import %s - skipped: %s\n' %
-                         (modulename, msg))
-        module = None
-
-    return module, modulename
-
-
-def check_option(option, script_name, map_option2action):
-    '''import script and get command line options.
-
-    Test command line options for conformity.
-    '''
-    if option in map_option2action:
-        ok_(option in map_option2action,
-            'option %s:%s unknown')
-        ok_(map_option2action[option] == "ok",
-            'option %s:%s wrong: action="%s"' %
-            (script_name, option, map_option2action[option]))
+        module = importlib.import_module(module_name)
+    except ImportError as e:
+        sys.stderr.write(f'ImportError for {module_name}: {e}\n')
+        return None, None
 
-
-def fail_(msg):
-    '''create test that fails with *msg*.'''
-    ok_(False, msg)
+    return module, module_name
 
 
 def test_cmdline():
-    '''test style of scripts
-    '''
-
-    # start script in order to build the command line parser
+    '''Test command line interfaces of scripts for style and conformity.'''
     global ORIGINAL_START
-    if ORIGINAL_START is None:
-        ORIGINAL_START = E.start
-    # read the first two columns
-    map_option2action = iotools.read_map(
+
+    # Load option actions from list
+    option_actions = iotools.read_map(
         iotools.open_file(FILENAME_OPTIONLIST),
         columns=(0, 1),
-        has_header=True)
-
-    files = []
-    for label, expression in EXPRESSIONS:
-        f = glob.glob(expression)
-        files.extend(sorted(f))
+        has_header=True
+    )
 
+    # Compile list of scripts to test
+    files = [f for label, expr in EXPRESSIONS for f in glob.glob(expr)]
     files = filter_files(files)
 
-    # make sure to use the current working directory as
-    # primary lookup.
+    # Prioritise the current directory for module lookup
     sys.path.insert(0, ".")
 
-    # files = [
-    #    'scripts/check_db.py',
-    #    'scripts/cgat_build_report_page.py']
-
-    for f in files:
-        if os.path.isdir(f):
-            continue
-        if os.path.basename(f) in EXCLUDE:
+    for script in files:
+        if os.path.isdir(script) or os.path.basename(script) in EXCLUDE:
             continue
 
-        script_name = os.path.abspath(f)
-        pyxfile = (os.path.join(os.path.dirname(f), "_") +
-                   os.path.basename(f) + "x")
-
-        fail_.description = script_name
-        # check if script contains getopt
-        with iotools.open_file(script_name) as inf:
-            if "getopt" in inf.read():
-                yield (fail_,
-                       "script uses getopt directly: %s" % script_name)
-                continue
-
-        module, modulename = load_script(script_name)
-        if module is None:
-            yield (fail_,
-                   "module could not be imported: %s\n" % script_name)
+        script_name = os.path.abspath(script)
+        module, module_name = load_script(script)
+        if not module:
+            yield fail_, f"Module {script_name} could not be imported."
             continue
+
+        # Replace the start function to capture parser
         E.start = LocalStart
 
+        # Attempt to run script's main function to access its parser
         try:
-            module.main(argv=["dummy", "--help"])
-        except AttributeError:
-            yield (fail_,
-                   "no main method in %s\n" % script_name)
-            ok_(False, "no main method in %s" % script_name)
-        except SystemExit:
-            yield (fail_,
-                   "script does not use E.start() %s\n" % script_name)
+            module.main(argv=["--help"])
         except DummyError:
+            # Expected flow interruption by LocalStart
             pass
+        except Exception as e:
+            yield fail_, f"Error invoking main of {script_name}: {e}"
+            continue
+
+        if PARSER:
+            for action in PARSER._actions:  # Iterate through the actions stored in the parser
+                if isinstance(action, argparse._HelpAction):  # Skip help actions
+                    continue
+                opt_strings = action.option_strings  # Get the list of CLI flags
+                if not opt_strings:  # This skips positional arguments
+                    continue
+                for opt_string in opt_strings:
+                    if opt_string.startswith("--"):
+                        opt_string = opt_string[2:]
+                    yield check_option, opt_string, script_name, option_actions
+
+        # Reset module to avoid conflicts
+        if module_name in sys.modules:
+            del sys.modules[module_name]
+
+
+def check_option(option, script_name, option_actions):
+    print(f"Checking option: {option} in script: {script_name}")  # Diagnostic print
+    assert option in option_actions, f"Option {option} in script {script_name} is unknown or not allowed."
+    assert option_actions[option] == "ok", f"Option {option} in script {script_name} is not allowed."
+
+
+def fail_(msg):
+    '''Generate a failing test with the provided message.'''
+    ok_(False, msg)
 
-        for option in PARSER.parse_args(parser):
-            print("=================")
-            print(option)
-            # ignore options added by optparse
-            if option.dest is None:
-                continue
-
-            optstring = option.get_opt_string()
-            if optstring.startswith("--"):
-                optstring = optstring[2:]
-
-            check_option.description = script_name + ":" + optstring
-
-            yield(check_option, optstring, os.path.abspath(f),
-                  map_option2action)
-
-        # clear up
-        del sys.modules[modulename]
-
-        # scripts with pyximport need special handling.
-        #
-        # Multiple imports of pyximport seems to create
-        # some confusion - here, clear up sys.meta_path after
-        # each script
-        if os.path.exists(pyxfile):
-            sys.meta_path = []
+# Reset E.start to its original function after testing
+E.start = ORIGINAL_START
```

### Comparing `cgat-0.7.0/tests/test_import.py` & `cgat-0.7.1/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `cgat-0.7.0/tests/test_scripts.py` & `cgat-0.7.1/tests/test_scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,14 @@
    The starting number of this task starting at 1
 
 CGAT_TASK_STEPSIZE
    The number of tests to run within a chunk
 
 """
 
-from __future__ import print_function
-
 import subprocess
 import tempfile
 import os
 import shutil
 import re
 import glob
 import gzip
```

### Comparing `cgat-0.7.0/tests/test_style.py` & `cgat-0.7.1/tests/test_style.py`

 * *Files identical despite different names*

