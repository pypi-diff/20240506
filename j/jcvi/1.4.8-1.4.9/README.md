# Comparing `tmp/jcvi-1.4.8.tar.gz` & `tmp/jcvi-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcvi-1.4.8.tar", last modified: Wed May  1 05:02:02 2024, max compression
+gzip compressed data, was "jcvi-1.4.9.tar", last modified: Mon May  6 04:23:29 2024, max compression
```

## Comparing `jcvi-1.4.8.tar` & `jcvi-1.4.9.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.321407 jcvi-1.4.8/
--rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.4.8/LICENSE
--rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.4.8/MANIFEST.in
--rw-r--r--   0 bao        (501) staff       (20)     8915 2024-05-01 05:02:02.321506 jcvi-1.4.8/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     8250 2024-04-30 16:06:02.000000 jcvi-1.4.8/README.md
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.297102 jcvi-1.4.8/jcvi/
--rw-r--r--   0 bao        (501) staff       (20)      816 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/__init__.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.299092 jcvi-1.4.8/jcvi/algorithms/
--rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/algorithms/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      263 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/algorithms/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     6421 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/algorithms/ec.py
--rw-r--r--   0 bao        (501) staff       (20)     6412 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/algorithms/formula.py
--rw-r--r--   0 bao        (501) staff       (20)    14137 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/algorithms/graph.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6275 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/algorithms/lis.py
--rwxr-xr-x   0 bao        (501) staff       (20)    24107 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/algorithms/lpsolve.py
--rw-r--r--   0 bao        (501) staff       (20)     6102 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/algorithms/matrix.py
--rw-r--r--   0 bao        (501) staff       (20)     1296 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/algorithms/maxsum.py
--rwxr-xr-x   0 bao        (501) staff       (20)     4978 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/algorithms/supermap.py
--rw-r--r--   0 bao        (501) staff       (20)    12550 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/algorithms/tsp.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.300792 jcvi-1.4.8/jcvi/annotation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/annotation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      258 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/annotation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    21401 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/annotation/ahrd.py
--rw-r--r--   0 bao        (501) staff       (20)     7917 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/annotation/automaton.py
--rwxr-xr-x   0 bao        (501) staff       (20)     6395 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/annotation/depth.py
--rw-r--r--   0 bao        (501) staff       (20)     7033 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/annotation/evm.py
--rw-r--r--   0 bao        (501) staff       (20)    14679 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/annotation/maker.py
--rw-r--r--   0 bao        (501) staff       (20)    19482 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/annotation/pasa.py
--rw-r--r--   0 bao        (501) staff       (20)    12807 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/annotation/qc.py
--rw-r--r--   0 bao        (501) staff       (20)    42705 2024-05-01 05:00:35.000000 jcvi-1.4.8/jcvi/annotation/reformat.py
--rw-r--r--   0 bao        (501) staff       (20)    12632 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/annotation/stats.py
--rw-r--r--   0 bao        (501) staff       (20)     6781 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/annotation/train.py
--rw-r--r--   0 bao        (501) staff       (20)     5040 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/annotation/trinity.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.303890 jcvi-1.4.8/jcvi/apps/
--rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/apps/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      249 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    20394 2024-05-01 05:00:35.000000 jcvi-1.4.8/jcvi/apps/align.py
--rw-r--r--   0 bao        (501) staff       (20)    66673 2024-05-01 05:00:35.000000 jcvi-1.4.8/jcvi/apps/base.py
--rw-r--r--   0 bao        (501) staff       (20)    12248 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/biomart.py
--rwxr-xr-x   0 bao        (501) staff       (20)     3516 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/blastplus.py
--rw-r--r--   0 bao        (501) staff       (20)     5228 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/bowtie.py
--rw-r--r--   0 bao        (501) staff       (20)     7676 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/bwa.py
--rw-r--r--   0 bao        (501) staff       (20)     7237 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/cdhit.py
--rw-r--r--   0 bao        (501) staff       (20)     2611 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/emboss.py
--rw-r--r--   0 bao        (501) staff       (20)    21311 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/fetch.py
--rw-r--r--   0 bao        (501) staff       (20)    19442 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/gbsubmit.py
--rw-r--r--   0 bao        (501) staff       (20)     6881 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/gmap.py
--rw-r--r--   0 bao        (501) staff       (20)    18461 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/grid.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7214 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/lastz.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2992 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/mask.py
--rw-r--r--   0 bao        (501) staff       (20)    35460 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/phylo.py
--rw-r--r--   0 bao        (501) staff       (20)     1854 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/r.py
--rw-r--r--   0 bao        (501) staff       (20)     4873 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/restriction.py
--rw-r--r--   0 bao        (501) staff       (20)     3767 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/softlink.py
--rw-r--r--   0 bao        (501) staff       (20)    33029 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/uclust.py
--rw-r--r--   0 bao        (501) staff       (20)     5194 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/uniprot.py
--rw-r--r--   0 bao        (501) staff       (20)     3636 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/apps/vecscreen.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.306753 jcvi-1.4.8/jcvi/assembly/
--rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/assembly/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      253 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    65586 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)    15425 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/allpaths.py
--rw-r--r--   0 bao        (501) staff       (20)    13251 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/automaton.py
--rw-r--r--   0 bao        (501) staff       (20)     5535 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/base.py
--rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.4.8/jcvi/assembly/chic.pyx
--rw-r--r--   0 bao        (501) staff       (20)     4558 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/coverage.py
--rw-r--r--   0 bao        (501) staff       (20)     8650 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/gaps.py
--rw-r--r--   0 bao        (501) staff       (20)    20008 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/geneticmap.py
--rw-r--r--   0 bao        (501) staff       (20)    34665 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/goldenpath.py
--rw-r--r--   0 bao        (501) staff       (20)    56179 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/hic.py
--rw-r--r--   0 bao        (501) staff       (20)    43053 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/kmer.py
--rw-r--r--   0 bao        (501) staff       (20)    12475 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/opticalmap.py
--rw-r--r--   0 bao        (501) staff       (20)    27263 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/patch.py
--rw-r--r--   0 bao        (501) staff       (20)    15706 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/postprocess.py
--rw-r--r--   0 bao        (501) staff       (20)    21503 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/preprocess.py
--rw-r--r--   0 bao        (501) staff       (20)     6275 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/sim.py
--rw-r--r--   0 bao        (501) staff       (20)     8836 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/soap.py
--rw-r--r--   0 bao        (501) staff       (20)    16163 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/assembly/syntenypath.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.309042 jcvi-1.4.8/jcvi/compara/
--rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/compara/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      247 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/compara/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)     4218 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/compara/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9765 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/compara/blastfilter.py
--rw-r--r--   0 bao        (501) staff       (20)    28531 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/compara/catalog.py
--rw-r--r--   0 bao        (501) staff       (20)    26317 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/compara/fractionation.py
--rw-r--r--   0 bao        (501) staff       (20)    33973 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/compara/ks.py
--rw-r--r--   0 bao        (501) staff       (20)     9189 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/compara/pad.py
--rw-r--r--   0 bao        (501) staff       (20)     8324 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/compara/pedigree.py
--rw-r--r--   0 bao        (501) staff       (20)     3048 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/compara/phylogeny.py
--rwxr-xr-x   0 bao        (501) staff       (20)     7933 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/compara/quota.py
--rw-r--r--   0 bao        (501) staff       (20)    10310 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/compara/reconstruct.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9136 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/compara/synfind.py
--rwxr-xr-x   0 bao        (501) staff       (20)    57581 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/compara/synteny.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.312365 jcvi-1.4.8/jcvi/formats/
--rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/formats/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      258 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    63425 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/agp.py
--rw-r--r--   0 bao        (501) staff       (20)    33922 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)    71610 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/bed.py
--rw-r--r--   0 bao        (501) staff       (20)    43167 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/blast.py
--rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.4.8/jcvi/formats/cblast.pyx
--rw-r--r--   0 bao        (501) staff       (20)     3163 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/cdt.py
--rw-r--r--   0 bao        (501) staff       (20)     8534 2024-05-01 05:00:35.000000 jcvi-1.4.8/jcvi/formats/chain.py
--rw-r--r--   0 bao        (501) staff       (20)     4620 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/contig.py
--rw-r--r--   0 bao        (501) staff       (20)    15170 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/coords.py
--rw-r--r--   0 bao        (501) staff       (20)     6516 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/excel.py
--rw-r--r--   0 bao        (501) staff       (20)    75587 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/fasta.py
--rw-r--r--   0 bao        (501) staff       (20)    29570 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/fastq.py
--rw-r--r--   0 bao        (501) staff       (20)    15510 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/genbank.py
--rw-r--r--   0 bao        (501) staff       (20)   119884 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/gff.py
--rw-r--r--   0 bao        (501) staff       (20)     3962 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/html.py
--rw-r--r--   0 bao        (501) staff       (20)     4595 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/maf.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2816 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/obo.py
--rw-r--r--   0 bao        (501) staff       (20)     2880 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/paf.py
--rw-r--r--   0 bao        (501) staff       (20)     2749 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/pdf.py
--rwxr-xr-x   0 bao        (501) staff       (20)    10351 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/psl.py
--rw-r--r--   0 bao        (501) staff       (20)     2746 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/formats/pyblast.py
--rw-r--r--   0 bao        (501) staff       (20)    28218 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/sam.py
--rw-r--r--   0 bao        (501) staff       (20)     8018 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/formats/sizes.py
--rw-r--r--   0 bao        (501) staff       (20)    25449 2024-05-01 04:19:07.000000 jcvi-1.4.8/jcvi/formats/vcf.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.314935 jcvi-1.4.8/jcvi/graphics/
--rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/graphics/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      267 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    16228 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/align.py
--rw-r--r--   0 bao        (501) staff       (20)    15231 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/assembly.py
--rw-r--r--   0 bao        (501) staff       (20)    24973 2024-05-01 05:00:35.000000 jcvi-1.4.8/jcvi/graphics/base.py
--rwxr-xr-x   0 bao        (501) staff       (20)     9984 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/blastplot.py
--rw-r--r--   0 bao        (501) staff       (20)    22261 2024-05-01 05:00:35.000000 jcvi-1.4.8/jcvi/graphics/chromosome.py
--rw-r--r--   0 bao        (501) staff       (20)     7097 2024-05-01 05:00:35.000000 jcvi-1.4.8/jcvi/graphics/coverage.py
--rwxr-xr-x   0 bao        (501) staff       (20)    14852 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/dotplot.py
--rw-r--r--   0 bao        (501) staff       (20)    21811 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/glyph.py
--rw-r--r--   0 bao        (501) staff       (20)    24787 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/grabseeds.py
--rw-r--r--   0 bao        (501) staff       (20)     5017 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/heatmap.py
--rw-r--r--   0 bao        (501) staff       (20)     9589 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/histogram.py
--rw-r--r--   0 bao        (501) staff       (20)    13317 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/karyotype.py
--rw-r--r--   0 bao        (501) staff       (20)    34110 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/landscape.py
--rw-r--r--   0 bao        (501) staff       (20)     3862 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/mummerplot.py
--rw-r--r--   0 bao        (501) staff       (20)    22488 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/synteny.py
--rw-r--r--   0 bao        (501) staff       (20)     5473 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/table.py
--rw-r--r--   0 bao        (501) staff       (20)    20370 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/tree.py
--rw-r--r--   0 bao        (501) staff       (20)     6182 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/graphics/wheel.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.316894 jcvi-1.4.8/jcvi/projects/
--rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/projects/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      257 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/projects/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    22374 2024-05-01 05:00:35.000000 jcvi-1.4.8/jcvi/projects/age.py
--rw-r--r--   0 bao        (501) staff       (20)    15889 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/projects/allmaps.py
--rw-r--r--   0 bao        (501) staff       (20)     6738 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/projects/bites.py
--rw-r--r--   0 bao        (501) staff       (20)    14086 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/projects/ies.py
--rw-r--r--   0 bao        (501) staff       (20)     7085 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/projects/jcvi.py
--rw-r--r--   0 bao        (501) staff       (20)    22160 2024-05-01 05:00:35.000000 jcvi-1.4.8/jcvi/projects/misc.py
--rw-r--r--   0 bao        (501) staff       (20)    24998 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/projects/napus.py
--rw-r--r--   0 bao        (501) staff       (20)    12708 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/projects/pineapple.py
--rw-r--r--   0 bao        (501) staff       (20)    67821 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/projects/str.py
--rw-r--r--   0 bao        (501) staff       (20)    25729 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/projects/sugarcane.py
--rw-r--r--   0 bao        (501) staff       (20)    23885 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/projects/synfind.py
--rw-r--r--   0 bao        (501) staff       (20)    21557 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/projects/tgbs.py
--rw-r--r--   0 bao        (501) staff       (20)    11690 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/projects/vanilla.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.318584 jcvi-1.4.8/jcvi/utils/
--rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/utils/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      256 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/utils/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    24193 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/utils/aws.py
--rw-r--r--   0 bao        (501) staff       (20)    12647 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/utils/cbook.py
--rw-r--r--   0 bao        (501) staff       (20)      355 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/utils/console.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.320170 jcvi-1.4.8/jcvi/utils/data/
--rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.4.8/jcvi/utils/data/Airswing.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.4.8/jcvi/utils/data/Collegia.ttf
--rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.4.8/jcvi/utils/data/HookedUp.ttf
--rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.4.8/jcvi/utils/data/Humor-Sans.ttf
--rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.4.8/jcvi/utils/data/TREDs.meta.csv
--rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/utils/data/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.4.8/jcvi/utils/data/adapters.fasta
--rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.4.8/jcvi/utils/data/blosum80.mat
--rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.4.8/jcvi/utils/data/chrY.hg38.unique_ccn.gc
--rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.4.8/jcvi/utils/data/colorchecker.txt
--rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.4.8/jcvi/utils/data/hg38.band.txt
--rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.4.8/jcvi/utils/data/hg38.chrom.sizes
--rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.4.8/jcvi/utils/data/instance.json
--rw-r--r--   0 bao        (501) staff       (20)     9726 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/utils/db.py
--rw-r--r--   0 bao        (501) staff       (20)     4145 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/utils/ez_setup.py
--rwxr-xr-x   0 bao        (501) staff       (20)     2884 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/utils/grouper.py
--rw-r--r--   0 bao        (501) staff       (20)    10437 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/utils/orderedcollections.py
--rw-r--r--   0 bao        (501) staff       (20)    14596 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/utils/range.py
--rw-r--r--   0 bao        (501) staff       (20)     3946 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/utils/table.py
--rw-r--r--   0 bao        (501) staff       (20)     4675 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/utils/taxonomy.py
--rw-r--r--   0 bao        (501) staff       (20)     1522 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/utils/validator.py
--rwxr-xr-x   0 bao        (501) staff       (20)     1376 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/utils/webcolors.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.321272 jcvi-1.4.8/jcvi/variation/
--rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.8/jcvi/variation/__init__.py
--rw-r--r--   0 bao        (501) staff       (20)      256 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/variation/__main__.py
--rw-r--r--   0 bao        (501) staff       (20)    45325 2024-05-01 05:00:35.000000 jcvi-1.4.8/jcvi/variation/cnv.py
--rw-r--r--   0 bao        (501) staff       (20)     7022 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/variation/deconvolute.py
--rw-r--r--   0 bao        (501) staff       (20)     9360 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/variation/delly.py
--rw-r--r--   0 bao        (501) staff       (20)    11736 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/variation/impute.py
--rw-r--r--   0 bao        (501) staff       (20)     3440 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/variation/phase.py
--rw-r--r--   0 bao        (501) staff       (20)    10785 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/variation/snp.py
--rw-r--r--   0 bao        (501) staff       (20)    48803 2024-05-01 04:07:52.000000 jcvi-1.4.8/jcvi/variation/str.py
--rw-r--r--   0 bao        (501) staff       (20)      176 2024-05-01 05:02:02.000000 jcvi-1.4.8/jcvi/version.py
-drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-01 05:02:02.297790 jcvi-1.4.8/jcvi.egg-info/
--rw-r--r--   0 bao        (501) staff       (20)     8915 2024-05-01 05:02:02.000000 jcvi-1.4.8/jcvi.egg-info/PKG-INFO
--rw-r--r--   0 bao        (501) staff       (20)     4543 2024-05-01 05:02:02.000000 jcvi-1.4.8/jcvi.egg-info/SOURCES.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2024-05-01 05:02:02.000000 jcvi-1.4.8/jcvi.egg-info/dependency_links.txt
--rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.4.8/jcvi.egg-info/not-zip-safe
--rw-r--r--   0 bao        (501) staff       (20)      221 2024-05-01 05:02:02.000000 jcvi-1.4.8/jcvi.egg-info/requires.txt
--rw-r--r--   0 bao        (501) staff       (20)        5 2024-05-01 05:02:02.000000 jcvi-1.4.8/jcvi.egg-info/top_level.txt
--rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.4.8/pyproject.toml
--rw-r--r--   0 bao        (501) staff       (20)     1242 2024-05-01 05:02:02.321850 jcvi-1.4.8/setup.cfg
--rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.4.8/setup.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.099320 jcvi-1.4.9/
+-rw-r--r--   0 bao        (501) staff       (20)     1292 2020-03-03 07:11:04.000000 jcvi-1.4.9/LICENSE
+-rw-r--r--   0 bao        (501) staff       (20)       91 2022-11-27 15:24:30.000000 jcvi-1.4.9/MANIFEST.in
+-rw-r--r--   0 bao        (501) staff       (20)     8915 2024-05-06 04:23:29.099424 jcvi-1.4.9/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     8250 2024-04-30 16:06:02.000000 jcvi-1.4.9/README.md
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.073690 jcvi-1.4.9/jcvi/
+-rw-r--r--   0 bao        (501) staff       (20)      816 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/__init__.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.076019 jcvi-1.4.9/jcvi/algorithms/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/algorithms/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      263 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/algorithms/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     6421 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/algorithms/ec.py
+-rw-r--r--   0 bao        (501) staff       (20)     6412 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/algorithms/formula.py
+-rw-r--r--   0 bao        (501) staff       (20)    14137 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/algorithms/graph.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6275 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/algorithms/lis.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    24107 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/algorithms/lpsolve.py
+-rw-r--r--   0 bao        (501) staff       (20)     6102 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/algorithms/matrix.py
+-rw-r--r--   0 bao        (501) staff       (20)     1296 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/algorithms/maxsum.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     4978 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/algorithms/supermap.py
+-rw-r--r--   0 bao        (501) staff       (20)    12550 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/algorithms/tsp.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.077619 jcvi-1.4.9/jcvi/annotation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/annotation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      258 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/annotation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    21401 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/annotation/ahrd.py
+-rw-r--r--   0 bao        (501) staff       (20)     7917 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/annotation/automaton.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     6395 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/annotation/depth.py
+-rw-r--r--   0 bao        (501) staff       (20)     7033 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/annotation/evm.py
+-rw-r--r--   0 bao        (501) staff       (20)    14679 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/annotation/maker.py
+-rw-r--r--   0 bao        (501) staff       (20)    19482 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/annotation/pasa.py
+-rw-r--r--   0 bao        (501) staff       (20)    12807 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/annotation/qc.py
+-rw-r--r--   0 bao        (501) staff       (20)    42705 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/annotation/reformat.py
+-rw-r--r--   0 bao        (501) staff       (20)    12632 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/annotation/stats.py
+-rw-r--r--   0 bao        (501) staff       (20)     6781 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/annotation/train.py
+-rw-r--r--   0 bao        (501) staff       (20)     5040 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/annotation/trinity.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.080555 jcvi-1.4.9/jcvi/apps/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/apps/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      249 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/apps/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    20394 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    66711 2024-05-06 04:23:09.000000 jcvi-1.4.9/jcvi/apps/base.py
+-rw-r--r--   0 bao        (501) staff       (20)    12248 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/biomart.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     3516 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/blastplus.py
+-rw-r--r--   0 bao        (501) staff       (20)     5228 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/bowtie.py
+-rw-r--r--   0 bao        (501) staff       (20)     7676 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/bwa.py
+-rw-r--r--   0 bao        (501) staff       (20)     7237 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/cdhit.py
+-rw-r--r--   0 bao        (501) staff       (20)     2611 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/emboss.py
+-rw-r--r--   0 bao        (501) staff       (20)    21311 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/fetch.py
+-rw-r--r--   0 bao        (501) staff       (20)    19442 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/gbsubmit.py
+-rw-r--r--   0 bao        (501) staff       (20)     6881 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/gmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    18461 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/grid.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7214 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/lastz.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2992 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/mask.py
+-rw-r--r--   0 bao        (501) staff       (20)    35460 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/phylo.py
+-rw-r--r--   0 bao        (501) staff       (20)     1854 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/r.py
+-rw-r--r--   0 bao        (501) staff       (20)     4873 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/restriction.py
+-rw-r--r--   0 bao        (501) staff       (20)     3767 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/softlink.py
+-rw-r--r--   0 bao        (501) staff       (20)    33029 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/uclust.py
+-rw-r--r--   0 bao        (501) staff       (20)     5194 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/uniprot.py
+-rw-r--r--   0 bao        (501) staff       (20)     3636 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/apps/vecscreen.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.083180 jcvi-1.4.9/jcvi/assembly/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/assembly/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      253 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/assembly/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    65586 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    15425 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/allpaths.py
+-rw-r--r--   0 bao        (501) staff       (20)    13251 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/automaton.py
+-rw-r--r--   0 bao        (501) staff       (20)     5535 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/base.py
+-rw-r--r--   0 bao        (501) staff       (20)     3457 2022-09-27 05:18:33.000000 jcvi-1.4.9/jcvi/assembly/chic.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     4558 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/coverage.py
+-rw-r--r--   0 bao        (501) staff       (20)     8650 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/gaps.py
+-rw-r--r--   0 bao        (501) staff       (20)    20008 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/geneticmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    34665 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/goldenpath.py
+-rw-r--r--   0 bao        (501) staff       (20)    56179 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/hic.py
+-rw-r--r--   0 bao        (501) staff       (20)    43053 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/kmer.py
+-rw-r--r--   0 bao        (501) staff       (20)    12475 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/opticalmap.py
+-rw-r--r--   0 bao        (501) staff       (20)    27263 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/patch.py
+-rw-r--r--   0 bao        (501) staff       (20)    15706 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/postprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)    21503 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/preprocess.py
+-rw-r--r--   0 bao        (501) staff       (20)     6275 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/sim.py
+-rw-r--r--   0 bao        (501) staff       (20)     8836 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/soap.py
+-rw-r--r--   0 bao        (501) staff       (20)    16163 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/assembly/syntenypath.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.085241 jcvi-1.4.9/jcvi/compara/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/compara/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      247 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/compara/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)     4218 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/compara/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9765 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/compara/blastfilter.py
+-rw-r--r--   0 bao        (501) staff       (20)    28322 2024-05-06 04:23:09.000000 jcvi-1.4.9/jcvi/compara/catalog.py
+-rw-r--r--   0 bao        (501) staff       (20)    26317 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/compara/fractionation.py
+-rw-r--r--   0 bao        (501) staff       (20)    33973 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/compara/ks.py
+-rw-r--r--   0 bao        (501) staff       (20)     9189 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/compara/pad.py
+-rw-r--r--   0 bao        (501) staff       (20)     8324 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/compara/pedigree.py
+-rw-r--r--   0 bao        (501) staff       (20)     3048 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/compara/phylogeny.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     7933 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/compara/quota.py
+-rw-r--r--   0 bao        (501) staff       (20)    10310 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/compara/reconstruct.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9136 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/compara/synfind.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    57581 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/compara/synteny.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.089063 jcvi-1.4.9/jcvi/formats/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/formats/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      258 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/formats/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    63425 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/agp.py
+-rw-r--r--   0 bao        (501) staff       (20)    33922 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    71610 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/bed.py
+-rw-r--r--   0 bao        (501) staff       (20)    43167 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/blast.py
+-rw-r--r--   0 bao        (501) staff       (20)     7010 2022-09-27 05:18:33.000000 jcvi-1.4.9/jcvi/formats/cblast.pyx
+-rw-r--r--   0 bao        (501) staff       (20)     3163 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/formats/cdt.py
+-rw-r--r--   0 bao        (501) staff       (20)     8534 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/chain.py
+-rw-r--r--   0 bao        (501) staff       (20)     4620 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/contig.py
+-rw-r--r--   0 bao        (501) staff       (20)    15170 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/coords.py
+-rw-r--r--   0 bao        (501) staff       (20)     6516 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/excel.py
+-rw-r--r--   0 bao        (501) staff       (20)    75587 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/fasta.py
+-rw-r--r--   0 bao        (501) staff       (20)    29570 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/fastq.py
+-rw-r--r--   0 bao        (501) staff       (20)    15510 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/genbank.py
+-rw-r--r--   0 bao        (501) staff       (20)   119884 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/gff.py
+-rw-r--r--   0 bao        (501) staff       (20)     3962 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/html.py
+-rw-r--r--   0 bao        (501) staff       (20)     4595 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/maf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2816 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/obo.py
+-rw-r--r--   0 bao        (501) staff       (20)     2880 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/paf.py
+-rw-r--r--   0 bao        (501) staff       (20)     2749 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/formats/pdf.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    10351 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/psl.py
+-rw-r--r--   0 bao        (501) staff       (20)     2746 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/pyblast.py
+-rw-r--r--   0 bao        (501) staff       (20)    28218 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/sam.py
+-rw-r--r--   0 bao        (501) staff       (20)     8018 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/sizes.py
+-rw-r--r--   0 bao        (501) staff       (20)    25449 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/formats/vcf.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.091750 jcvi-1.4.9/jcvi/graphics/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/graphics/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      267 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/graphics/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    16228 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/graphics/align.py
+-rw-r--r--   0 bao        (501) staff       (20)    15231 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/graphics/assembly.py
+-rw-r--r--   0 bao        (501) staff       (20)    24808 2024-05-06 04:23:09.000000 jcvi-1.4.9/jcvi/graphics/base.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     9984 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/graphics/blastplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    22261 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/graphics/chromosome.py
+-rw-r--r--   0 bao        (501) staff       (20)     7097 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/graphics/coverage.py
+-rwxr-xr-x   0 bao        (501) staff       (20)    15127 2024-05-06 04:23:09.000000 jcvi-1.4.9/jcvi/graphics/dotplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    21811 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/graphics/glyph.py
+-rw-r--r--   0 bao        (501) staff       (20)    24787 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/graphics/grabseeds.py
+-rw-r--r--   0 bao        (501) staff       (20)     5017 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/graphics/heatmap.py
+-rw-r--r--   0 bao        (501) staff       (20)     9589 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/graphics/histogram.py
+-rw-r--r--   0 bao        (501) staff       (20)    13292 2024-05-06 04:23:09.000000 jcvi-1.4.9/jcvi/graphics/karyotype.py
+-rw-r--r--   0 bao        (501) staff       (20)    34110 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/graphics/landscape.py
+-rw-r--r--   0 bao        (501) staff       (20)     3862 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/graphics/mummerplot.py
+-rw-r--r--   0 bao        (501) staff       (20)    22500 2024-05-06 04:23:09.000000 jcvi-1.4.9/jcvi/graphics/synteny.py
+-rw-r--r--   0 bao        (501) staff       (20)     5473 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/graphics/table.py
+-rw-r--r--   0 bao        (501) staff       (20)    20370 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/graphics/tree.py
+-rw-r--r--   0 bao        (501) staff       (20)     6182 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/graphics/wheel.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.093891 jcvi-1.4.9/jcvi/projects/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/projects/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      257 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/projects/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    22374 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/projects/age.py
+-rw-r--r--   0 bao        (501) staff       (20)    15889 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/projects/allmaps.py
+-rw-r--r--   0 bao        (501) staff       (20)     6738 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/projects/bites.py
+-rw-r--r--   0 bao        (501) staff       (20)    14086 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/projects/ies.py
+-rw-r--r--   0 bao        (501) staff       (20)     9040 2024-05-06 04:23:09.000000 jcvi-1.4.9/jcvi/projects/jcvi.py
+-rw-r--r--   0 bao        (501) staff       (20)    22140 2024-05-06 04:23:09.000000 jcvi-1.4.9/jcvi/projects/misc.py
+-rw-r--r--   0 bao        (501) staff       (20)    24975 2024-05-06 04:23:09.000000 jcvi-1.4.9/jcvi/projects/napus.py
+-rw-r--r--   0 bao        (501) staff       (20)    12703 2024-05-06 04:23:09.000000 jcvi-1.4.9/jcvi/projects/pineapple.py
+-rw-r--r--   0 bao        (501) staff       (20)    67821 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/projects/str.py
+-rw-r--r--   0 bao        (501) staff       (20)    25729 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/projects/sugarcane.py
+-rw-r--r--   0 bao        (501) staff       (20)    23885 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/projects/synfind.py
+-rw-r--r--   0 bao        (501) staff       (20)    21557 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/projects/tgbs.py
+-rw-r--r--   0 bao        (501) staff       (20)    11690 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/projects/vanilla.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.095711 jcvi-1.4.9/jcvi/utils/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/utils/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      256 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/utils/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    24193 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/utils/aws.py
+-rw-r--r--   0 bao        (501) staff       (20)    12647 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/utils/cbook.py
+-rw-r--r--   0 bao        (501) staff       (20)      355 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/utils/console.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.098087 jcvi-1.4.9/jcvi/utils/data/
+-rwxr-xr-x   0 bao        (501) staff       (20)    16912 2020-01-29 05:28:41.000000 jcvi-1.4.9/jcvi/utils/data/Airswing.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)   103940 2020-01-29 05:28:41.000000 jcvi-1.4.9/jcvi/utils/data/Collegia.ttf
+-rwxr-xr-x   0 bao        (501) staff       (20)    20468 2020-01-29 05:28:41.000000 jcvi-1.4.9/jcvi/utils/data/HookedUp.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    25832 2020-01-29 05:28:41.000000 jcvi-1.4.9/jcvi/utils/data/Humor-Sans.ttf
+-rw-r--r--   0 bao        (501) staff       (20)    28065 2020-01-29 05:28:41.000000 jcvi-1.4.9/jcvi/utils/data/TREDs.meta.csv
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/utils/data/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      911 2020-01-29 05:28:41.000000 jcvi-1.4.9/jcvi/utils/data/adapters.fasta
+-rw-r--r--   0 bao        (501) staff       (20)     3321 2020-01-29 05:28:41.000000 jcvi-1.4.9/jcvi/utils/data/blosum80.mat
+-rw-r--r--   0 bao        (501) staff       (20)     7686 2020-01-29 05:28:41.000000 jcvi-1.4.9/jcvi/utils/data/chrY.hg38.unique_ccn.gc
+-rw-r--r--   0 bao        (501) staff       (20)      282 2020-01-29 05:28:41.000000 jcvi-1.4.9/jcvi/utils/data/colorchecker.txt
+-rw-r--r--   0 bao        (501) staff       (20)    45544 2020-01-29 05:28:41.000000 jcvi-1.4.9/jcvi/utils/data/hg38.band.txt
+-rw-r--r--   0 bao        (501) staff       (20)    11672 2020-01-29 05:28:41.000000 jcvi-1.4.9/jcvi/utils/data/hg38.chrom.sizes
+-rw-r--r--   0 bao        (501) staff       (20)     1000 2020-01-29 05:28:41.000000 jcvi-1.4.9/jcvi/utils/data/instance.json
+-rw-r--r--   0 bao        (501) staff       (20)     9726 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/utils/db.py
+-rw-r--r--   0 bao        (501) staff       (20)     4145 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/utils/ez_setup.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     2884 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/utils/grouper.py
+-rw-r--r--   0 bao        (501) staff       (20)    10437 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/utils/orderedcollections.py
+-rw-r--r--   0 bao        (501) staff       (20)    14596 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/utils/range.py
+-rw-r--r--   0 bao        (501) staff       (20)     3946 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/utils/table.py
+-rw-r--r--   0 bao        (501) staff       (20)     4675 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/utils/taxonomy.py
+-rw-r--r--   0 bao        (501) staff       (20)     1522 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/utils/validator.py
+-rwxr-xr-x   0 bao        (501) staff       (20)     1376 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/utils/webcolors.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.099204 jcvi-1.4.9/jcvi/variation/
+-rw-r--r--   0 bao        (501) staff       (20)        0 2024-05-01 01:14:54.000000 jcvi-1.4.9/jcvi/variation/__init__.py
+-rw-r--r--   0 bao        (501) staff       (20)      256 2024-05-01 04:07:52.000000 jcvi-1.4.9/jcvi/variation/__main__.py
+-rw-r--r--   0 bao        (501) staff       (20)    45266 2024-05-06 04:23:09.000000 jcvi-1.4.9/jcvi/variation/cnv.py
+-rw-r--r--   0 bao        (501) staff       (20)     7022 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/variation/deconvolute.py
+-rw-r--r--   0 bao        (501) staff       (20)     9360 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/variation/delly.py
+-rw-r--r--   0 bao        (501) staff       (20)    11736 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/variation/impute.py
+-rw-r--r--   0 bao        (501) staff       (20)     3440 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/variation/phase.py
+-rw-r--r--   0 bao        (501) staff       (20)    10785 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/variation/snp.py
+-rw-r--r--   0 bao        (501) staff       (20)    48803 2024-05-05 17:03:15.000000 jcvi-1.4.9/jcvi/variation/str.py
+-rw-r--r--   0 bao        (501) staff       (20)      176 2024-05-06 04:23:28.000000 jcvi-1.4.9/jcvi/version.py
+drwxr-xr-x   0 bao        (501) staff       (20)        0 2024-05-06 04:23:29.074553 jcvi-1.4.9/jcvi.egg-info/
+-rw-r--r--   0 bao        (501) staff       (20)     8915 2024-05-06 04:23:28.000000 jcvi-1.4.9/jcvi.egg-info/PKG-INFO
+-rw-r--r--   0 bao        (501) staff       (20)     4543 2024-05-06 04:23:29.000000 jcvi-1.4.9/jcvi.egg-info/SOURCES.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2024-05-06 04:23:28.000000 jcvi-1.4.9/jcvi.egg-info/dependency_links.txt
+-rw-r--r--   0 bao        (501) staff       (20)        1 2022-11-26 21:54:22.000000 jcvi-1.4.9/jcvi.egg-info/not-zip-safe
+-rw-r--r--   0 bao        (501) staff       (20)      221 2024-05-06 04:23:28.000000 jcvi-1.4.9/jcvi.egg-info/requires.txt
+-rw-r--r--   0 bao        (501) staff       (20)        5 2024-05-06 04:23:28.000000 jcvi-1.4.9/jcvi.egg-info/top_level.txt
+-rw-r--r--   0 bao        (501) staff       (20)      359 2022-11-26 21:23:29.000000 jcvi-1.4.9/pyproject.toml
+-rw-r--r--   0 bao        (501) staff       (20)     1242 2024-05-06 04:23:29.099802 jcvi-1.4.9/setup.cfg
+-rw-r--r--   0 bao        (501) staff       (20)      553 2022-11-26 21:23:29.000000 jcvi-1.4.9/setup.py
```

### Comparing `jcvi-1.4.8/LICENSE` & `jcvi-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/PKG-INFO` & `jcvi-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jcvi-1.4.8/README.md` & `jcvi-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/__init__.py` & `jcvi-1.4.9/jcvi/__init__.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/algorithms/ec.py` & `jcvi-1.4.9/jcvi/algorithms/ec.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/algorithms/formula.py` & `jcvi-1.4.9/jcvi/algorithms/formula.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/algorithms/graph.py` & `jcvi-1.4.9/jcvi/algorithms/graph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/algorithms/lis.py` & `jcvi-1.4.9/jcvi/algorithms/lis.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/algorithms/lpsolve.py` & `jcvi-1.4.9/jcvi/algorithms/lpsolve.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/algorithms/matrix.py` & `jcvi-1.4.9/jcvi/algorithms/matrix.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/algorithms/maxsum.py` & `jcvi-1.4.9/jcvi/algorithms/maxsum.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/algorithms/supermap.py` & `jcvi-1.4.9/jcvi/algorithms/supermap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/algorithms/tsp.py` & `jcvi-1.4.9/jcvi/algorithms/tsp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/annotation/ahrd.py` & `jcvi-1.4.9/jcvi/annotation/ahrd.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/annotation/automaton.py` & `jcvi-1.4.9/jcvi/annotation/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/annotation/depth.py` & `jcvi-1.4.9/jcvi/annotation/depth.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/annotation/evm.py` & `jcvi-1.4.9/jcvi/annotation/evm.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/annotation/maker.py` & `jcvi-1.4.9/jcvi/annotation/maker.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/annotation/pasa.py` & `jcvi-1.4.9/jcvi/annotation/pasa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/annotation/qc.py` & `jcvi-1.4.9/jcvi/annotation/qc.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/annotation/reformat.py` & `jcvi-1.4.9/jcvi/annotation/reformat.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/annotation/stats.py` & `jcvi-1.4.9/jcvi/annotation/stats.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/annotation/train.py` & `jcvi-1.4.9/jcvi/annotation/train.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/annotation/trinity.py` & `jcvi-1.4.9/jcvi/annotation/trinity.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/align.py` & `jcvi-1.4.9/jcvi/apps/align.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/base.py` & `jcvi-1.4.9/jcvi/apps/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
             "--params",
             dest="extra",
             default=params,
             help="Extra parameters to pass {0}".format(dest_prog)
             + " (these WILL NOT be validated)",
         )
 
-    def set_outfile(self, outfile="stdout"):
+    def set_outfile(self, outfile: Optional[str] = "stdout"):
         """
         Add --outfile options to print out to filename.
         """
         self.add_argument("-o", "--outfile", default=outfile, help="Outfile name")
 
     def set_outdir(self, outdir="."):
         self.add_argument("--outdir", default=outdir, help="Specify output directory")
@@ -654,14 +654,15 @@
             "--theme",
             choices=[str(x) for x in range(len(set1))],
             default=str(theme),
             help="Color index within the palette for contig grid boundaries. Palette contains: {}".format(
                 "|".join(set1)
             ),
         )
+        return group
 
     def set_depth(self, depth=50):
         self.add_argument("--depth", default=depth, type=float, help="Desired depth")
 
     def set_rclip(self, rclip=0):
         self.add_argument(
             "--rclip",
```

### Comparing `jcvi-1.4.8/jcvi/apps/biomart.py` & `jcvi-1.4.9/jcvi/apps/biomart.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/blastplus.py` & `jcvi-1.4.9/jcvi/apps/blastplus.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/bowtie.py` & `jcvi-1.4.9/jcvi/apps/bowtie.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/bwa.py` & `jcvi-1.4.9/jcvi/apps/bwa.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/cdhit.py` & `jcvi-1.4.9/jcvi/apps/cdhit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/emboss.py` & `jcvi-1.4.9/jcvi/apps/emboss.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/fetch.py` & `jcvi-1.4.9/jcvi/apps/fetch.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/gbsubmit.py` & `jcvi-1.4.9/jcvi/apps/gbsubmit.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/gmap.py` & `jcvi-1.4.9/jcvi/apps/gmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/grid.py` & `jcvi-1.4.9/jcvi/apps/grid.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/lastz.py` & `jcvi-1.4.9/jcvi/apps/lastz.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/mask.py` & `jcvi-1.4.9/jcvi/apps/mask.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/phylo.py` & `jcvi-1.4.9/jcvi/apps/phylo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/r.py` & `jcvi-1.4.9/jcvi/apps/r.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/restriction.py` & `jcvi-1.4.9/jcvi/apps/restriction.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/softlink.py` & `jcvi-1.4.9/jcvi/apps/softlink.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/uclust.py` & `jcvi-1.4.9/jcvi/apps/uclust.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/uniprot.py` & `jcvi-1.4.9/jcvi/apps/uniprot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/apps/vecscreen.py` & `jcvi-1.4.9/jcvi/apps/vecscreen.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/allmaps.py` & `jcvi-1.4.9/jcvi/assembly/allmaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/allpaths.py` & `jcvi-1.4.9/jcvi/assembly/allpaths.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/automaton.py` & `jcvi-1.4.9/jcvi/assembly/automaton.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/base.py` & `jcvi-1.4.9/jcvi/assembly/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/chic.pyx` & `jcvi-1.4.9/jcvi/assembly/chic.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/coverage.py` & `jcvi-1.4.9/jcvi/assembly/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/gaps.py` & `jcvi-1.4.9/jcvi/assembly/gaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/geneticmap.py` & `jcvi-1.4.9/jcvi/assembly/geneticmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/goldenpath.py` & `jcvi-1.4.9/jcvi/assembly/goldenpath.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/hic.py` & `jcvi-1.4.9/jcvi/assembly/hic.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/kmer.py` & `jcvi-1.4.9/jcvi/assembly/kmer.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/opticalmap.py` & `jcvi-1.4.9/jcvi/assembly/opticalmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/patch.py` & `jcvi-1.4.9/jcvi/assembly/patch.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/postprocess.py` & `jcvi-1.4.9/jcvi/assembly/postprocess.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/preprocess.py` & `jcvi-1.4.9/jcvi/assembly/preprocess.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/sim.py` & `jcvi-1.4.9/jcvi/assembly/sim.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/soap.py` & `jcvi-1.4.9/jcvi/assembly/soap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/assembly/syntenypath.py` & `jcvi-1.4.9/jcvi/assembly/syntenypath.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/compara/base.py` & `jcvi-1.4.9/jcvi/compara/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/compara/blastfilter.py` & `jcvi-1.4.9/jcvi/compara/blastfilter.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/compara/catalog.py` & `jcvi-1.4.9/jcvi/compara/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,26 @@
     OptionParser,
     glob,
     logger,
     mkdir,
     need_update,
     sh,
 )
-from ..formats.base import must_open, BaseFile
+from ..apps.align import last as last_main, diamond_blastp_main, blast_main
+from ..compara.blastfilter import main as blastfilter_main
+from ..compara.quota import main as quota_main
+from ..compara.synteny import scan, mcscan, liftover
+from ..formats.base import BaseFile, DictFile, must_open
 from ..formats.bed import Bed
-from ..formats.blast import BlastLine
+from ..formats.blast import (
+    BlastLine,
+    cscore,
+    filter as blast_filter,
+    filtered_blastfile_name,
+)
 from ..formats.fasta import Fasta
 from ..utils.cbook import gene_name
 from ..utils.grouper import Grouper
 
 from .base import AnchorFile
 from .synteny import check_beds
 
@@ -261,16 +270,14 @@
 
 def sort_layout(thread, listfile, column=0):
     """
     Sort the syntelog table according to chromomomal positions. First orient the
     contents against threadbed, then for contents not in threadbed, insert to
     the nearest neighbor.
     """
-    from jcvi.formats.base import DictFile
-
     outfile = listfile.rsplit(".", 1)[0] + ".sorted.list"
     threadorder = thread.order
     fw = open(outfile, "w")
     lt = DictFile(listfile, keypos=column, valuepos=None)
     threaded = []
     imported = set()
     for t in thread:
@@ -500,17 +507,14 @@
 
 def omgprepare(args):
     """
     %prog omgprepare ploidy anchorsfile blastfile
 
     Prepare to run Sankoff's OMG algorithm to get orthologs.
     """
-    from jcvi.formats.blast import cscore
-    from jcvi.formats.base import DictFile
-
     p = OptionParser(omgprepare.__doc__)
     p.add_argument("--norbh", action="store_true", help="Disable RBH hits")
     p.add_argument(
         "--pctid", default=0, type=int, help="Percent id cutoff for RBH hits"
     )
     p.add_argument("--cscore", default=90, type=int, help="C-score cutoff for RBH hits")
     p.set_stripnames()
@@ -564,16 +568,14 @@
         npairs += 1
     fw.close()
 
     logger.debug("Write %d pairs to `%s`.", npairs, weightsfile)
 
 
 def make_ortholog(blocksfile, rbhfile, orthofile):
-    from jcvi.formats.base import DictFile
-
     # Generate mapping both ways
     adict = DictFile(rbhfile)
     bdict = DictFile(rbhfile, keypos=1, valuepos=0)
     adict.update(bdict)
 
     fp = open(blocksfile)
     fw = open(orthofile, "w")
@@ -599,21 +601,14 @@
     Run a sensitive pipeline to find orthologs between two species a and b.
     The pipeline runs LAST and generate .lifted.anchors.
 
     `--full` mode would assume 1-to-1 quota synteny blocks as the backbone of
     such predictions. Extra orthologs will be recruited from reciprocal best
     match (RBH).
     """
-    from jcvi.apps.align import last as last_main
-    from jcvi.apps.align import diamond_blastp_main, blast_main
-    from jcvi.compara.blastfilter import main as blastfilter_main
-    from jcvi.compara.quota import main as quota_main
-    from jcvi.compara.synteny import scan, mcscan, liftover
-    from jcvi.formats.blast import cscore, filter, filtered_blastfile_name
-
     p = OptionParser(ortholog.__doc__)
     p.add_argument(
         "--dbtype",
         default="nucl",
         choices=("nucl", "prot"),
         help="Molecule type of subject database",
     )
@@ -665,15 +660,14 @@
     )
     p.add_argument(
         "--ignore_zero_anchor",
         default=False,
         action="store_true",
         help="Ignore this pair of ortholog identification instead of throwing an error when performing many pairs of cataloging.",
     )
-
     p.add_argument(
         "--align_soft",
         default="last",
         choices=("last", "blast", "diamond_blastp"),
         help="Sequence alignment software. Default <last> for both <nucl> and <prot>. Users could also use <blast> for both <nucl> and <prot>, or <diamond_blastp> for <prot>.",
     )
 
@@ -709,15 +703,15 @@
         else:
             last_main([bfasta, afasta, cpus_flag], dbtype)
 
     self_remove = opts.self_remove
     if a == b:
         lastself = filtered_blastfile_name(last, self_remove, 0, inverse=True)
         if need_update(last, lastself, warn=True):
-            filter(
+            blast_filter(
                 [last, "--hitlen=0", f"--pctid={self_remove}", "--inverse", "--noself"]
             )
         last = lastself
 
     filtered_last = last + ".filtered"
     if need_update(last, filtered_last, warn=True):
         # If we are doing filtering based on another file then we don't run cscore anymore
@@ -748,15 +742,15 @@
                 scan(dargs)
             except ValueError as e:
                 if ignore_zero_anchor:
                     logger.debug(str(e))
                     logger.debug("Ignoring this error and continuing...")
                     return
                 else:
-                    raise ValueError(e)
+                    raise ValueError(e) from e
         if quota:
             quota_main([lifted_anchors, "--quota={0}".format(quota), "--screen"])
         if need_update(anchors, pdf, warn=True) and not opts.no_dotplot:
             from jcvi.graphics.dotplot import dotplot_main
 
             dargs = [anchors]
             if opts.nostdpf:
```

### Comparing `jcvi-1.4.8/jcvi/compara/fractionation.py` & `jcvi-1.4.9/jcvi/compara/fractionation.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/compara/ks.py` & `jcvi-1.4.9/jcvi/compara/ks.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/compara/pad.py` & `jcvi-1.4.9/jcvi/compara/pad.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/compara/pedigree.py` & `jcvi-1.4.9/jcvi/compara/pedigree.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/compara/phylogeny.py` & `jcvi-1.4.9/jcvi/compara/phylogeny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/compara/quota.py` & `jcvi-1.4.9/jcvi/compara/quota.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/compara/reconstruct.py` & `jcvi-1.4.9/jcvi/compara/reconstruct.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/compara/synfind.py` & `jcvi-1.4.9/jcvi/compara/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/compara/synteny.py` & `jcvi-1.4.9/jcvi/compara/synteny.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/agp.py` & `jcvi-1.4.9/jcvi/formats/agp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/base.py` & `jcvi-1.4.9/jcvi/formats/base.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/bed.py` & `jcvi-1.4.9/jcvi/formats/bed.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/blast.py` & `jcvi-1.4.9/jcvi/formats/blast.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/cblast.pyx` & `jcvi-1.4.9/jcvi/formats/cblast.pyx`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/cdt.py` & `jcvi-1.4.9/jcvi/formats/cdt.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/chain.py` & `jcvi-1.4.9/jcvi/formats/chain.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/contig.py` & `jcvi-1.4.9/jcvi/formats/contig.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/coords.py` & `jcvi-1.4.9/jcvi/formats/coords.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/excel.py` & `jcvi-1.4.9/jcvi/formats/excel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/fasta.py` & `jcvi-1.4.9/jcvi/formats/fasta.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/fastq.py` & `jcvi-1.4.9/jcvi/formats/fastq.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/genbank.py` & `jcvi-1.4.9/jcvi/formats/genbank.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/gff.py` & `jcvi-1.4.9/jcvi/formats/gff.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/html.py` & `jcvi-1.4.9/jcvi/formats/html.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/maf.py` & `jcvi-1.4.9/jcvi/formats/maf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/obo.py` & `jcvi-1.4.9/jcvi/formats/obo.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/paf.py` & `jcvi-1.4.9/jcvi/formats/paf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/pdf.py` & `jcvi-1.4.9/jcvi/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/psl.py` & `jcvi-1.4.9/jcvi/formats/psl.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/pyblast.py` & `jcvi-1.4.9/jcvi/formats/pyblast.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/sam.py` & `jcvi-1.4.9/jcvi/formats/sam.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/sizes.py` & `jcvi-1.4.9/jcvi/formats/sizes.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/formats/vcf.py` & `jcvi-1.4.9/jcvi/formats/vcf.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/align.py` & `jcvi-1.4.9/jcvi/graphics/align.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/assembly.py` & `jcvi-1.4.9/jcvi/graphics/assembly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/base.py` & `jcvi-1.4.9/jcvi/graphics/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,14 @@
 # -*- coding: UTF-8 -*-
 
 import copy
 import os.path as op
 from os import remove
 
 import sys
-import logging
-
-from ..apps.base import get_logger
-
-get_logger("matplotlib", logging.WARNING)
-get_logger("numexpr", logging.WARNING)
-get_logger("PIL", logging.INFO)
 
 from functools import partial
 from typing import Optional, List, Tuple, Union
 
 import numpy as np
 import matplotlib as mpl
 import seaborn as sns
```

### Comparing `jcvi-1.4.8/jcvi/graphics/blastplot.py` & `jcvi-1.4.9/jcvi/graphics/blastplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/chromosome.py` & `jcvi-1.4.9/jcvi/graphics/chromosome.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/coverage.py` & `jcvi-1.4.9/jcvi/graphics/coverage.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/dotplot.py` & `jcvi-1.4.9/jcvi/graphics/dotplot.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 see more here: http://matplotlib.sourceforge.net/users/usetex.html
 """
 
 import os.path as op
 import string
 import sys
 
+from copy import deepcopy
 from random import sample
+from typing import Optional
 
 from ..apps.base import OptionParser, logger, need_update
 from ..compara.base import AnchorFile
 from ..compara.synteny import batch_scan, check_beds, get_orientation
 from ..utils.cbook import seqid_parse, thousands
 
 from .base import (
@@ -217,52 +219,59 @@
     set_human_axis(ax)
 
     plt.setp(ax.get_xticklabels() + ax.get_yticklabels(), color="gray", size=10)
 
     return xlim, ylim
 
 
-def downsample(data, sample_number=10000):
+def downsample(data, sample_number: int = 10000):
+    """
+    Downsample the data to a manageable size for plotting.
+    """
     npairs = len(data)
     # Only show random subset
     if npairs > sample_number:
         logger.debug(
-            "Showing a random subset of {0} data points (total {1}) "
-            "for clarity.".format(sample_number, npairs)
+            "Showing a random subset of %d data points (total %d) for clarity.",
+            sample_number,
+            npairs,
         )
         data = sample(data, sample_number)
     return data
 
 
 def dotplot(
-    anchorfile,
+    anchorfile: str,
     qbed,
     sbed,
     fig,
     root,
     ax,
-    vmin=0,
-    vmax=1,
-    is_self=False,
-    synteny=False,
-    cmap_text=None,
+    vmin: float = 0,
+    vmax: float = 1,
+    is_self: bool = False,
+    synteny: bool = False,
+    cmap_text: Optional[str] = None,
     cmap="copper",
     genomenames=None,
-    sample_number=10000,
-    minfont=5,
-    palette=None,
-    chrlw=0.1,
-    title=None,
-    sep=True,
-    sepcolor="g",
-    stdpf=True,
-    chpf=True,
+    sample_number: int = 10000,
+    minfont: int = 5,
+    palette: Optional[Palette] = None,
+    chrlw: float = 0.1,
+    title: Optional[str] = None,
+    sep: bool = True,
+    sepcolor: str = "g",
+    stdpf: bool = True,
+    chpf: bool = True,
     usetex: bool = True,
 ):
-    fp = open(anchorfile)
+    """
+    Draw a dotplot from an anchor file.
+    """
+    fp = open(anchorfile, encoding="utf-8")
     # add genome names
     if genomenames:
         gx, gy = genomenames.split("_")
     else:
         to_ax_label = lambda fname: op.basename(fname).split(".")[0]
         gx, gy = [to_ax_label(x.filename) for x in (qbed, sbed)]
 
@@ -270,15 +279,15 @@
     gx, gy = markup(gx), markup(gy)
 
     qorder = qbed.order
     sorder = sbed.order
 
     data = []
     if cmap_text:
-        logger.debug("Capping values within [{0:.1f}, {1:.1f}]".format(vmin, vmax))
+        logger.debug("Capping values within [%.1f, %.1f]", vmin, vmax)
 
     block_id = 0
     block_color = "k"
     for row in fp:
         atoms = row.split()
         if row[0] == "#":
             block_id += 1
@@ -333,15 +342,15 @@
         clusters = batch_scan(data, qbed, sbed)
         draw_box(clusters, ax)
 
     if cmap_text:
         draw_cmap(root, cmap_text, vmin, vmax, cmap=cmap)
 
     xsize, ysize = len(qbed), len(sbed)
-    logger.debug("xsize=%d ysize=%d" % (xsize, ysize))
+    logger.debug("xsize=%d ysize=%d", xsize, ysize)
     qbreaks = qbed.get_breaks()
     sbreaks = sbed.get_breaks()
     xlim, _ = plot_breaks_and_labels(
         fig,
         root,
         ax,
         gx,
@@ -370,27 +379,26 @@
         xstart, ystart = 0.1, 0.05
         for category, c in sorted(colors.items()):
             root.add_patch(Rectangle((xstart, ystart), 0.03, 0.02, lw=0, fc=c))
             root.text(xstart + 0.04, ystart, category, color=c)
             xstart += 0.1
 
     if title is None:
-        title = "Inter-genomic comparison: {0} vs {1}".format(gx, gy)
+        title = f"Inter-genomic comparison: {gx} vs {gy}"
         if is_self:
-            title = "Intra-genomic comparison within {0}".format(gx)
-            npairs /= 2
-        title += " ({0} gene pairs)".format(thousands(npairs))
+            title = f"Intra-genomic comparison within {gx}"
+            npairs //= 2
+        title += f" ({thousands(npairs)} gene pairs)"
     root.set_title(title, x=0.5, y=0.96, color="k")
     if title:
-        logger.debug("Dot plot title: {}".format(title))
+        logger.debug("Dot plot title: %s", title)
     normalize_axes(root)
 
 
 def subset_bed(bed, seqids):
-    from copy import deepcopy
 
     newbed = deepcopy(bed)
     del newbed[:]
     for b in bed:
         if b.seqid not in seqids:
             continue
         newbed.append(b)
@@ -469,15 +477,15 @@
     if palette:
         palette = Palette(palettefile=palette)
     elif opts.colororientation:
         palette = Palette.from_block_orientation(anchorfile, qbed, sbed)
 
     cmaptext = opts.cmaptext
     if anchorfile.endswith(".ks"):
-        from jcvi.apps.ks import KsFile
+        from ..compara.ks import KsFile
 
         logger.debug("Anchors contain Ks values")
         cmaptext = cmaptext or "*Ks* values"
         anchorksfile = anchorfile + ".anchors"
         if need_update(anchorfile, anchorksfile):
             ksfile = KsFile(anchorfile)
             ksfile.print_to_anchors(anchorksfile)
@@ -488,28 +496,28 @@
         if is_self:
             qseqids = sseqids = set()
         else:
             qseqids, sseqids = set(), set()
 
         for pair in ac.iter_pairs():
             q, s = pair[:2]
-            qi, q = qorder[q]
-            si, s = sorder[s]
+            _, q = qorder[q]
+            _, s = sorder[s]
             qseqids.add(q.seqid)
             sseqids.add(s.seqid)
 
         if is_self:
             qbed = sbed = subset_bed(qbed, qseqids)
         else:
             qbed = subset_bed(qbed, qseqids)
             sbed = subset_bed(sbed, sseqids)
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])  # the whole canvas
-    ax = fig.add_axes([0.1, 0.1, 0.8, 0.8])  # the dot plot
+    root = fig.add_axes((0, 0, 1, 1))  # the whole canvas
+    ax = fig.add_axes((0.1, 0.1, 0.8, 0.8))  # the dot plot
 
     dotplot(
         anchorfile,
         qbed,
         sbed,
         fig,
         root,
```

### Comparing `jcvi-1.4.8/jcvi/graphics/glyph.py` & `jcvi-1.4.9/jcvi/graphics/glyph.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/grabseeds.py` & `jcvi-1.4.9/jcvi/graphics/grabseeds.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/heatmap.py` & `jcvi-1.4.9/jcvi/graphics/heatmap.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/histogram.py` & `jcvi-1.4.9/jcvi/graphics/histogram.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/karyotype.py` & `jcvi-1.4.9/jcvi/graphics/karyotype.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,23 @@
 
 from typing import Optional
 
 from ..apps.base import OptionParser, logger
 from ..compara.synteny import SimpleFile
 from ..formats.bed import Bed
 
-from .base import AbstractLayout, markup, mpl, plt, savefig, update_figname
+from .base import (
+    AbstractLayout,
+    markup,
+    mpl,
+    normalize_axes,
+    plt,
+    savefig,
+    update_figname,
+)
 from .chromosome import Chromosome, HorizontalChromosome
 from .glyph import TextCircle
 from .synteny import Shade, ymid_offset
 
 
 class LayoutLine(object):
     def __init__(self, row, delimiter=",", generank=True):
@@ -326,15 +334,14 @@
                 style=self.style,
             )
 
 
 class Karyotype(object):
     def __init__(
         self,
-        fig,
         root,
         seqidsfile,
         layoutfile,
         gap=0.01,
         height=0.01,
         lw=1,
         generank=True,
@@ -438,32 +445,28 @@
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     seqidsfile, layoutfile = args
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
     Karyotype(
-        fig,
         root,
         seqidsfile,
         layoutfile,
         keep_chrlabels=opts.keep_chrlabels,
         plot_circles=(not opts.nocircles),
         shadestyle=opts.shadestyle,
         chrstyle=opts.chrstyle,
         generank=(not opts.basepair),
         seed=iopts.seed,
     )
-
-    root.set_xlim(0, 1)
-    root.set_ylim(0, 1)
-    root.set_axis_off()
+    normalize_axes(root)
 
     image_name = update_figname(opts.outfile, iopts.format)
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jcvi-1.4.8/jcvi/graphics/landscape.py` & `jcvi-1.4.9/jcvi/graphics/landscape.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/mummerplot.py` & `jcvi-1.4.9/jcvi/graphics/mummerplot.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/synteny.py` & `jcvi-1.4.9/jcvi/graphics/synteny.py`

 * *Files 2% similar despite different names*

```diff
@@ -440,15 +440,15 @@
         genelabelsize: int = 0,
         genelabelrotation: int = 25,
         pad: float = 0.05,
         vpad: float = 0.015,
         scalebar: bool = False,
         shadestyle: str = "curve",
         glyphstyle: str = "arrow",
-        glyphcolor: BasePalette = OrientationPalette(),
+        glyphcolor: str = "orientation",
         seed: Optional[int] = None,
         prune_features=True,
     ):
         _, h = fig.get_figwidth(), fig.get_figheight()
         bed = Bed(bedfile)
         order = bed.order
         bf = BlockFile(datafile)
@@ -587,21 +587,21 @@
                 )
                 xstart += xiv
                 RoundLabel(ax, 0.5, 0.3, label, fill=True, fc="lavender", color=color)
 
 
 def draw_gene_legend(
     ax,
-    x1,
-    x2,
-    ytop,
-    d=0.04,
-    text=False,
-    repeat=False,
-    glyphstyle="box",
+    x1: float,
+    x2: float,
+    ytop: float,
+    d: float = 0.04,
+    text: bool = False,
+    repeat: bool = False,
+    glyphstyle: str = "box",
 ):
     """
     Draw a legend for gene glyphs.
     """
     forward, backward = OrientationPalette.forward, OrientationPalette.backward
     ax.plot([x1, x1 + d], [ytop, ytop], ":", color=forward, lw=2)
     ax.plot([x1 + d], [ytop], ">", color=forward, mec=forward)
@@ -643,16 +643,15 @@
         + "However, plot may appear visually crowded. "
         + "Reasonably good values are 2 to 6 [Default: disabled]",
     )
     p.add_argument(
         "--genelabelrotation",
         default=25,
         type=int,
-        help="Rotate gene labels at this angle (anti-clockwise), useful for debugging. "
-        + "[Default: 25]",
+        help="Rotate gene labels at this angle (anti-clockwise), useful for debugging.",
     )
     p.add_argument(
         "--scalebar",
         default=False,
         action="store_true",
         help="Add scale bar to the plot",
     )
@@ -679,30 +678,30 @@
         default="",
         help="Prefix for the output file",
     )
     p.add_argument(
         "--noprune",
         default=False,
         action="store_true",
-        help="If set, do not exclude small features from annotation track (<1% of region)",
+        help="If set, do not exclude small features from annotation track (<1%% of region)",
     )
     opts, args, iopts = p.set_image_options(figsize="8x7")
 
     if len(args) != 3:
         sys.exit(not p.print_help())
 
     datafile, bedfile, layoutfile = args
     switch = opts.switch
     tree = opts.tree
     gene_labels = None if not opts.genelabels else set(opts.genelabels.split(","))
     prune_features = not opts.noprune
 
     pf = datafile.rsplit(".", 1)[0]
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
     Synteny(
         fig,
         root,
         datafile,
         bedfile,
         layoutfile,
         switch=switch,
```

### Comparing `jcvi-1.4.8/jcvi/graphics/table.py` & `jcvi-1.4.9/jcvi/graphics/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/tree.py` & `jcvi-1.4.9/jcvi/graphics/tree.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/graphics/wheel.py` & `jcvi-1.4.9/jcvi/graphics/wheel.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/projects/age.py` & `jcvi-1.4.9/jcvi/projects/age.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/projects/allmaps.py` & `jcvi-1.4.9/jcvi/projects/allmaps.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/projects/bites.py` & `jcvi-1.4.9/jcvi/projects/bites.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/projects/ies.py` & `jcvi-1.4.9/jcvi/projects/ies.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/projects/jcvi.py` & `jcvi-1.4.9/jcvi/projects/jcvi.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,17 +10,88 @@
 import networkx as nx
 
 from ..apps.base import ActionDispatcher, OptionParser, logger
 from ..assembly.geneticmap import draw_geneticmap_heatmap
 from ..assembly.hic import draw_hic_heatmap
 from ..assembly.kmer import draw_ks_histogram
 from ..compara.pedigree import Pedigree, calculate_inbreeding
-from ..graphics.base import cm, load_image, normalize_axes, panel_labels, plt, savefig
+from ..compara.synteny import check_beds
+from ..graphics.base import (
+    cm,
+    load_image,
+    normalize_axes,
+    panel_labels,
+    plt,
+    savefig,
+    set1,
+    setup_theme,
+)
 from ..graphics.chromosome import draw_chromosomes
+from ..graphics.dotplot import dotplot
+from ..graphics.karyotype import Karyotype
 from ..graphics.landscape import draw_heatmaps, draw_multi_depth, draw_stacks
+from ..graphics.synteny import Synteny, draw_gene_legend
+
+
+def synteny(args):
+    """
+    %prog synteny grape.peach.anchors seqids layout blocks grape_peach.bed blocks.layout
+
+    Plot synteny composite figure, including:
+    A. Synteny dotplot
+    B. Karyotype plot
+    """
+    p = OptionParser(synteny.__doc__)
+    p.set_beds()
+    opts, args, iopts = p.set_image_options(args, figsize="14x7")
+    setup_theme(style="dark")
+
+    if len(args) != 6:
+        sys.exit(not p.print_help())
+
+    anchorfile, seqidsfile, layoutfile, datafile, bedfile, blockslayoutfile = args
+
+    fig = plt.figure(1, (iopts.w, iopts.h))
+    root = fig.add_axes((0, 0, 1, 1))
+
+    ax1_root = fig.add_axes((0, 0, 0.5, 1))
+    ax1_canvas = fig.add_axes((0.05, 0.1, 0.4, 0.8))  # the dot plot
+    ax2_root = fig.add_axes((0.5, 0.5, 0.5, 0.5))
+    ax3_root = fig.add_axes((0.5, 0, 0.5, 0.5))
+
+    # Panel A
+    logger.info("Plotting synteny dotplot")
+    qbed, sbed, _, _, is_self = check_beds(anchorfile, p, opts)
+    dotplot(
+        anchorfile,
+        qbed,
+        sbed,
+        fig,
+        ax1_root,
+        ax1_canvas,
+        is_self=is_self,
+        chrlw=0.5,
+        sepcolor=set1[3],
+    )
+
+    # Panel B
+    logger.info("Plotting karyotype plot")
+    Karyotype(ax2_root, seqidsfile, layoutfile)
+
+    # Panel C
+    logger.info("Plotting synteny blocks")
+    Synteny(fig, ax3_root, datafile, bedfile, blockslayoutfile, pad=0.1, vpad=0.03)
+    draw_gene_legend(root, 0.69, 0.8, 0.34)
+
+    labels = ((0.02, 0.95, "A"), (0.52, 0.95, "B"), (0.52, 0.45, "C"))
+    panel_labels(root, labels)
+    normalize_axes(root, ax1_root, ax2_root, ax3_root)
+
+    image_name = "synteny.pdf"
+    savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def diversity(args):
     """
     %prog diversity pedigree.ped VAR?_srtd.wgs.regions.bed.gz
 
     Plot diversity composite figure, including:
@@ -146,14 +217,16 @@
         ax2_root_extent,
         stacks,
         fastafile,
         window,
         shift,
         top=5,
     )
+
+    # Panel C
     draw_heatmaps(
         fig,
         ax3_root,
         ax3_root_extent,
         fastafile,
         "Chr2",
         stacks,
@@ -162,18 +235,15 @@
         shift,
         cmap=cm.viridis,
     )
 
     ax2_root.set_axis_off()
     ax3_root.set_axis_off()
 
-    labels = (
-        (0.02, 0.95, "A"),
-        (0.42, 0.95, "B"),
-    )
+    labels = ((0.02, 0.95, "A"), (0.42, 0.95, "B"), (0.42, 0.48, "C"))
     panel_labels(root, labels)
     normalize_axes(root, ax1_root)
 
     image_name = "landscape.pdf"
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
@@ -248,14 +318,15 @@
     image_name = "genomebuild.pdf"
     savefig(image_name, dpi=iopts.dpi, iopts=iopts)
 
 
 def main():
 
     actions = (
+        ("synteny", "Plot synteny composite figure"),
         ("diversity", "Plot diversity composite figure"),
         ("genomebuild", "Plot genome build composite figure"),
         ("landscape", "Plot landscape composite figure"),
     )
     p = ActionDispatcher(actions)
     p.dispatch(globals())
```

### Comparing `jcvi-1.4.8/jcvi/projects/misc.py` & `jcvi-1.4.9/jcvi/projects/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,17 +151,17 @@
 
     if len(args) != 5:
         sys.exit(not p.print_help())
 
     seqidsfile, klayout, datafile, bedfile, slayout = args
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
-    Karyotype(fig, root, seqidsfile, klayout)
+    Karyotype(root, seqidsfile, klayout)
     Synteny(fig, root, datafile, bedfile, slayout)
 
     # legend showing the orientation of the genes
     draw_gene_legend(root, 0.42, 0.52, 0.48)
 
     labels = ((0.04, 0.96, "A"), (0.04, 0.52, "B"))
     panel_labels(root, labels)
@@ -272,17 +272,17 @@
     opts, args, iopts = p.set_image_options(args, figsize="8x6")
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     seqids, layout = args
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
-    K = Karyotype(fig, root, seqids, layout)
+    K = Karyotype(root, seqids, layout)
     L = K.layout
 
     xs = 0.79
     dt = dict(rectangle=False, circle=False)
     # Embed a phylogenetic tree to the right
     coords = {}
     coords["Amborella"] = (xs, L[0].y)
@@ -500,17 +500,17 @@
         sys.exit(not p.print_help())
 
     seqidsfile, klayout, datafile, bedfile, slayout = args
     switch = opts.switch
     tree = opts.tree
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
-    Karyotype(fig, root, seqidsfile, klayout)
+    Karyotype(root, seqidsfile, klayout)
     Synteny(fig, root, datafile, bedfile, slayout, switch=switch, tree=tree)
 
     # legend showing the orientation of the genes
     draw_gene_legend(root, 0.5, 0.68, 0.5)
 
     # annotate the WGD events
     fc = "lightslategrey"
@@ -547,17 +547,17 @@
         sys.exit(p.print_help())
 
     seqidsfile, klayout, datafile, bedfile, slayout = args
     switch = opts.switch
     depthfile = opts.depthfile
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
-    kt = Karyotype(fig, root, seqidsfile, klayout)
+    kt = Karyotype(root, seqidsfile, klayout)
     Synteny(fig, root, datafile, bedfile, slayout, switch=switch)
 
     light = "lightslategrey"
     # Show the dup depth along the cotton chromosomes
     if depthfile:
         ymin, ymax = 0.9, 0.95
         root.text(0.11, 0.96, "Cotton duplication level", color="gray", size=10)
@@ -678,15 +678,15 @@
     Illustrate the methods used in Maggie's epoch paper, in particular, how to
     classifiy S/G/F/FB/FN for the genes.
     """
     p = OptionParser(__doc__)
     p.parse_args(args)
 
     fig = plt.figure(1, (6, 4))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
     # Separators
     linestyle = dict(lw=2, color="b", alpha=0.2, zorder=2)
     root.plot((0, 1), (0.5, 0.5), "--", **linestyle)
     for i in (1.0 / 3, 2.0 / 3):
         root.plot((i, i), (0.5, 1), "--", **linestyle)
     for i in (1.0 / 6, 3.0 / 6, 5.0 / 6):
```

### Comparing `jcvi-1.4.8/jcvi/projects/napus.py` & `jcvi-1.4.9/jcvi/projects/napus.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
             hlsuffix=hlsuffix,
         )
         w2s += w2 + gap
 
     # Synteny panel
     seqidsfile = make_seqids(chrs)
     klayout = make_layout(chrs, chr_sum_sizes, ratio, template_cov)
-    Karyotype(fig, root, seqidsfile, klayout, gap=gap, generank=False, sizes=sizes)
+    Karyotype(root, seqidsfile, klayout, gap=gap, generank=False, sizes=sizes)
 
     root.set_xlim(0, 1)
     root.set_ylim(0, 1)
     root.set_axis_off()
 
     chr2 = "_".join(chr2)
     if opts.reverse:
@@ -308,15 +308,14 @@
 
     # Synteny panel
     seqidsfile = make_seqids(chrs)
     klayout = make_layout(chrs, chr_sum_sizes, ratio, template_f3a, shift=0.05)
     height = 0.07
     r = height / 4
     K = Karyotype(
-        fig,
         root,
         seqidsfile,
         klayout,
         gap=gap,
         height=height,
         lw=2,
         generank=False,
@@ -694,17 +693,17 @@
 
     if len(args) != 2:
         sys.exit(not p.print_help())
 
     seqidsfile, klayout = args
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
-    Karyotype(fig, root, seqidsfile, klayout)
+    Karyotype(root, seqidsfile, klayout)
 
     fc = "darkslategrey"
     radius = 0.012
     ot = -0.05  # use this to adjust vertical position of the left panel
     TextCircle(root, 0.1, 0.9 + ot, r"$\gamma$", radius=radius, fc=fc)
     root.text(0.1, 0.88 + ot, r"$\times3$", ha="center", va="top", color=fc)
     TextCircle(root, 0.08, 0.79 + ot, r"$\alpha$", radius=radius, fc=fc)
```

### Comparing `jcvi-1.4.8/jcvi/projects/pineapple.py` & `jcvi-1.4.9/jcvi/projects/pineapple.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,17 +304,17 @@
 
     if len(args) != 5:
         sys.exit(not p.print_help())
 
     seqidsfile, klayout, datafile, bedfile, slayout = args
 
     fig = plt.figure(1, (iopts.w, iopts.h))
-    root = fig.add_axes([0, 0, 1, 1])
+    root = fig.add_axes((0, 0, 1, 1))
 
-    Karyotype(fig, root, seqidsfile, klayout)
+    Karyotype(root, seqidsfile, klayout)
     Synteny(fig, root, datafile, bedfile, slayout, switch=opts.switch)
 
     # legend showing the orientation of the genes
     draw_gene_legend(root, 0.27, 0.37, 0.52)
 
     # annotate the WGD events
     fc = "lightslategrey"
```

### Comparing `jcvi-1.4.8/jcvi/projects/str.py` & `jcvi-1.4.9/jcvi/projects/str.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/projects/sugarcane.py` & `jcvi-1.4.9/jcvi/projects/sugarcane.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/projects/synfind.py` & `jcvi-1.4.9/jcvi/projects/synfind.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/projects/tgbs.py` & `jcvi-1.4.9/jcvi/projects/tgbs.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/projects/vanilla.py` & `jcvi-1.4.9/jcvi/projects/vanilla.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/aws.py` & `jcvi-1.4.9/jcvi/utils/aws.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/cbook.py` & `jcvi-1.4.9/jcvi/utils/cbook.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/data/Airswing.ttf` & `jcvi-1.4.9/jcvi/utils/data/Airswing.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/data/Collegia.ttf` & `jcvi-1.4.9/jcvi/utils/data/Collegia.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/data/HookedUp.ttf` & `jcvi-1.4.9/jcvi/utils/data/HookedUp.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/data/Humor-Sans.ttf` & `jcvi-1.4.9/jcvi/utils/data/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/data/TREDs.meta.csv` & `jcvi-1.4.9/jcvi/utils/data/TREDs.meta.csv`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/data/adapters.fasta` & `jcvi-1.4.9/jcvi/utils/data/adapters.fasta`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/data/blosum80.mat` & `jcvi-1.4.9/jcvi/utils/data/blosum80.mat`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/data/chrY.hg38.unique_ccn.gc` & `jcvi-1.4.9/jcvi/utils/data/chrY.hg38.unique_ccn.gc`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/data/hg38.band.txt` & `jcvi-1.4.9/jcvi/utils/data/hg38.band.txt`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/data/hg38.chrom.sizes` & `jcvi-1.4.9/jcvi/utils/data/hg38.chrom.sizes`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/data/instance.json` & `jcvi-1.4.9/jcvi/utils/data/instance.json`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/db.py` & `jcvi-1.4.9/jcvi/utils/db.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/ez_setup.py` & `jcvi-1.4.9/jcvi/utils/ez_setup.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/grouper.py` & `jcvi-1.4.9/jcvi/utils/grouper.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/orderedcollections.py` & `jcvi-1.4.9/jcvi/utils/orderedcollections.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/range.py` & `jcvi-1.4.9/jcvi/utils/range.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/table.py` & `jcvi-1.4.9/jcvi/utils/table.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/taxonomy.py` & `jcvi-1.4.9/jcvi/utils/taxonomy.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/validator.py` & `jcvi-1.4.9/jcvi/utils/validator.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/utils/webcolors.py` & `jcvi-1.4.9/jcvi/utils/webcolors.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/variation/cnv.py` & `jcvi-1.4.9/jcvi/variation/cnv.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,26 +22,23 @@
 from pybedtools import BedTool, cleanup, set_tempdir
 
 from ..algorithms.formula import get_kmeans
 from ..apps.base import (
     ActionDispatcher,
     OptionParser,
     getfilesize,
-    get_logger,
     logger,
     mkdir,
     popen,
     sh,
 )
 from ..apps.grid import MakeManager
 from ..utils.aws import glob_s3, push_to_s3, sync_from_s3
 from ..utils.cbook import percentage
 
-get_logger("matplotlib", logging.WARNING)
-
 autosomes = [f"chr{x}" for x in range(1, 23)]
 sexsomes = ["chrX", "chrY"]
 allsomes = autosomes + sexsomes
 # See: http://www.ncbi.nlm.nih.gov/projects/genome/assembly/grc/human/
 PAR = [("chrX", 10001, 2781479), ("chrX", 155701383, 156030895)]
```

### Comparing `jcvi-1.4.8/jcvi/variation/deconvolute.py` & `jcvi-1.4.9/jcvi/variation/deconvolute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/variation/delly.py` & `jcvi-1.4.9/jcvi/variation/delly.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/variation/impute.py` & `jcvi-1.4.9/jcvi/variation/impute.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/variation/phase.py` & `jcvi-1.4.9/jcvi/variation/phase.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/variation/snp.py` & `jcvi-1.4.9/jcvi/variation/snp.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi/variation/str.py` & `jcvi-1.4.9/jcvi/variation/str.py`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/jcvi.egg-info/PKG-INFO` & `jcvi-1.4.9/jcvi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcvi
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python utility libraries on genome assembly, annotation and comparative genomics
 Home-page: http://github.com/tanghaibao/jcvi
 Author: Haibao Tang, Vivek Krishnakumar, Jingping Li
 Author-email: tanghaibao@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jcvi-1.4.8/jcvi.egg-info/SOURCES.txt` & `jcvi-1.4.9/jcvi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/setup.cfg` & `jcvi-1.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `jcvi-1.4.8/setup.py` & `jcvi-1.4.9/setup.py`

 * *Files identical despite different names*

