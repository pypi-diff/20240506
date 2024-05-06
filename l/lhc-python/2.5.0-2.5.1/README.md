# Comparing `tmp/lhc-python-2.5.0.tar.gz` & `tmp/lhc_python-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lhc-python-2.5.0.tar", last modified: Thu Dec 16 11:09:21 2021, max compression
+gzip compressed data, was "lhc_python-2.5.1.tar", last modified: Mon May  6 11:09:29 2024, max compression
```

## Comparing `lhc-python-2.5.0.tar` & `lhc_python-2.5.1.tar`

### file list

```diff
@@ -1,255 +1,194 @@
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.716764 lhc-python-2.5.0/
--rw-rw-rw-   0        0        0    18363 2021-04-19 09:29:36.000000 lhc-python-2.5.0/LICENSE.txt
--rw-rw-rw-   0        0        0       63 2021-04-19 09:29:36.000000 lhc-python-2.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4048 2021-12-16 11:09:21.715763 lhc-python-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3531 2021-04-19 09:29:36.000000 lhc-python-2.5.0/README.md
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.110914 lhc-python-2.5.0/lhc/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.127883 lhc-python-2.5.0/lhc/binf/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.154831 lhc-python-2.5.0/lhc/binf/align/
--rw-rw-rw-   0        0        0      417 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/binf/align/__init__.py
--rw-rw-rw-   0        0        0     1728 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/align/__main__.py
--rw-rw-rw-   0        0        0     3176 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/align/aligner.py
--rw-rw-rw-   0        0        0     1689 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/align/alignment.py
--rw-rw-rw-   0        0        0      514 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/align/character_map.py
--rw-rw-rw-   0        0        0      364 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/align/global_alignment.py
--rw-rw-rw-   0        0        0      306 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/align/local_alignment.py
--rw-rw-rw-   0        0        0     3649 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/align/score.py
--rw-rw-rw-   0        0        0     1348 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/align/semiglobal_alignment.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.160820 lhc-python-2.5.0/lhc/binf/alignment/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/alignment/__init__.py
--rw-rw-rw-   0        0        0     1060 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/binf/alignment/__main__.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.178286 lhc-python-2.5.0/lhc/binf/alignment/tools/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/alignment/tools/__init__.py
--rw-rw-rw-   0        0        0     5181 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/binf/alignment/tools/call_variants.py
--rw-rw-rw-   0        0        0     1404 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/binf/alignment/tools/get_consensus.py
--rw-rw-rw-   0        0        0     3614 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/alignment/tools/mismatch_filter.py
--rw-rw-rw-   0        0        0     1957 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/alignment/tools/strand.py
--rw-rw-rw-   0        0        0     1794 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/binf/alignment/tools/trim_gaps.py
--rw-rw-rw-   0        0        0     6075 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/binf/genetic_code.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.191264 lhc-python-2.5.0/lhc/binf/genomic_coordinate/
--rw-rw-rw-   0        0        0      154 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/genomic_coordinate/__init__.py
--rw-rw-rw-   0        0        0     6381 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/binf/genomic_coordinate/genomic_interval.py
--rw-rw-rw-   0        0        0     3155 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/binf/genomic_coordinate/genomic_position.py
--rw-rw-rw-   0        0        0     3463 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/binf/genomic_coordinate/nested_genomic_interval.py
--rw-rw-rw-   0        0        0      827 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/identifier.py
--rw-rw-rw-   0        0        0      700 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/iupac.py
--rw-rw-rw-   0        0        0      808 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/kmer.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.199746 lhc-python-2.5.0/lhc/binf/loci/
--rw-rw-rw-   0        0        0       98 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/loci/__init__.py
--rw-rw-rw-   0        0        0     1163 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/loci/__main__.py
--rw-rw-rw-   0        0        0     1894 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/loci/make_loci.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.250149 lhc-python-2.5.0/lhc/binf/loci/tools/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/loci/tools/__init__.py
--rw-rw-rw-   0        0        0     3805 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/loci/tools/closest.py
--rw-rw-rw-   0        0        0     1951 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/loci/tools/deduplicate.py
--rw-rw-rw-   0        0        0     2143 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/loci/tools/extend.py
--rw-rw-rw-   0        0        0     2392 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/binf/loci/tools/filter.py
--rw-rw-rw-   0        0        0     5686 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/loci/tools/flank.py
--rw-rw-rw-   0        0        0     1525 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/loci/tools/generate.py
--rw-rw-rw-   0        0        0     2690 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/loci/tools/kmer_filter.py
--rw-rw-rw-   0        0        0     3664 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/loci/tools/query.py
--rw-rw-rw-   0        0        0     3755 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/loci/tools/shear.py
--rw-rw-rw-   0        0        0     1424 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/loci/tools/stats.py
--rw-rw-rw-   0        0        0     1386 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/loci/tools/view.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.256138 lhc-python-2.5.0/lhc/binf/misc/
--rw-rw-rw-   0        0        0        0 2021-11-17 17:37:03.000000 lhc-python-2.5.0/lhc/binf/misc/__init__.py
--rw-rw-rw-   0        0        0      607 2021-11-17 17:37:03.000000 lhc-python-2.5.0/lhc/binf/misc/__main__.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.261631 lhc-python-2.5.0/lhc/binf/misc/tools/
--rw-rw-rw-   0        0        0        0 2021-11-17 17:37:03.000000 lhc-python-2.5.0/lhc/binf/misc/tools/__init__.py
--rw-rw-rw-   0        0        0      659 2021-11-17 17:37:03.000000 lhc-python-2.5.0/lhc/binf/misc/tools/cs_to_table.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.276100 lhc-python-2.5.0/lhc/binf/sequence/
--rw-rw-rw-   0        0        0      612 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/binf/sequence/__init__.py
--rw-rw-rw-   0        0        0      809 2021-11-17 17:37:03.000000 lhc-python-2.5.0/lhc/binf/sequence/__main__.py
--rw-rw-rw-   0        0        0    16323 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/sequence/dicodonshuffle.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.284088 lhc-python-2.5.0/lhc/binf/sequence/digen/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/sequence/digen/__init__.py
--rw-rw-rw-   0        0        0     3685 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/sequence/digen/digen.py
--rw-rw-rw-   0        0        0      201 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/sequence/digen/setup.py
--rw-rw-rw-   0        0        0      202 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/sequence/reverse_complement.py
--rw-rw-rw-   0        0        0     1423 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/sequence/sequence_generator.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.304046 lhc-python-2.5.0/lhc/binf/sequence/tools/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/sequence/tools/__init__.py
--rw-rw-rw-   0        0        0     4123 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/binf/sequence/tools/extract.py
--rw-rw-rw-   0        0        0     2538 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/sequence/tools/filter.py
--rw-rw-rw-   0        0        0     3815 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/binf/sequence/tools/split.py
--rw-rw-rw-   0        0        0      773 2021-11-17 17:37:03.000000 lhc-python-2.5.0/lhc/binf/sequence/tools/stat_.py
--rw-rw-rw-   0        0        0     1645 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/binf/sequence/tools/unique.py
--rw-rw-rw-   0        0        0     1353 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/sequence/tools/view.py
--rw-rw-rw-   0        0        0      474 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/binf/skew.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.325007 lhc-python-2.5.0/lhc/binf/variant/
--rw-rw-rw-   0        0        0      283 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/binf/variant/__init__.py
--rw-rw-rw-   0        0        0      534 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/binf/variant/__main__.py
--rw-rw-rw-   0        0        0     1443 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/binf/variant/amino_acid_variant.py
--rw-rw-rw-   0        0        0     1796 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/binf/variant/coding_variant.py
--rw-rw-rw-   0        0        0     2218 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/binf/variant/codon_variant.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.329998 lhc-python-2.5.0/lhc/binf/variant/tools/
--rw-rw-rw-   0        0        0        0 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/binf/variant/tools/__init__.py
--rw-rw-rw-   0        0        0     3125 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/binf/variant/tools/annotate.py
--rw-rw-rw-   0        0        0     1114 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/binf/variant/variant.py
--rw-rw-rw-   0        0        0     1515 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/binf/variant/variant_effect.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.353453 lhc-python-2.5.0/lhc/collections/
--rw-rw-rw-   0        0        0      321 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/collections/__init__.py
--rw-rw-rw-   0        0        0      943 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/collections/inorder_access_interval_set.py
--rw-rw-rw-   0        0        0      742 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/collections/inorder_access_set.py
--rw-rw-rw-   0        0        0     1892 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/collections/interval_map.py
--rw-rw-rw-   0        0        0     1232 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/collections/interval_set.py
--rw-rw-rw-   0        0        0     2743 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/collections/multi_dimension_map.py
--rw-rw-rw-   0        0        0     3315 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/collections/tracked_map.py
--rw-rw-rw-   0        0        0     3369 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/collections/tracked_set.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.355948 lhc-python-2.5.0/lhc/data/
--rw-rw-rw-   0        0        0    10876 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/data/gc.prt
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.369921 lhc-python-2.5.0/lhc/filetools/
--rw-rw-rw-   0        0        0      114 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/filetools/__init__.py
--rw-rw-rw-   0        0        0     1629 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/filetools/filepool.py
--rw-rw-rw-   0        0        0      560 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/filetools/shared_connection.py
--rw-rw-rw-   0        0        0     2664 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/filetools/shared_file.py
--rw-rw-rw-   0        0        0     3308 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/filetools/shared_filepool.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.381400 lhc-python-2.5.0/lhc/graph/
--rw-rw-rw-   0        0        0      107 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/graph/__init__.py
--rw-rw-rw-   0        0        0     5714 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/graph/graph.py
--rw-rw-rw-   0        0        0     1989 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/graph/hyper_graph.py
--rw-rw-rw-   0        0        0     2578 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/graph/n_partite_graph.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.389884 lhc-python-2.5.0/lhc/indices/
--rw-rw-rw-   0        0        0       41 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/indices/__init__.py
--rw-rw-rw-   0        0        0     2751 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/indices/tbi.py
--rw-rw-rw-   0        0        0     3291 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/indices/tracked_index.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.397868 lhc-python-2.5.0/lhc/interval/
--rw-rw-rw-   0        0        0       68 2021-11-21 06:40:07.000000 lhc-python-2.5.0/lhc/interval/__init__.py
--rw-rw-rw-   0        0        0      954 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/interval/binner.py
--rw-rw-rw-   0        0        0     7119 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/interval/interval.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.403857 lhc-python-2.5.0/lhc/intervaltools/
--rw-rw-rw-   0        0        0      152 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/intervaltools/__init__.py
--rw-rw-rw-   0        0        0      463 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/intervaltools/set.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.412342 lhc-python-2.5.0/lhc/io/
--rw-rw-rw-   0        0        0       29 2021-11-18 18:04:09.000000 lhc-python-2.5.0/lhc/io/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.415338 lhc-python-2.5.0/lhc/io/alignment/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/alignment/__init__.py
--rw-rw-rw-   0        0        0      538 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/cut.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.430306 lhc-python-2.5.0/lhc/io/fasta/
--rw-rw-rw-   0        0        0      124 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fasta/__init__.py
--rw-rw-rw-   0        0        0     4481 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fasta/__main__.py
--rw-rw-rw-   0        0        0      788 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fasta/index.py
--rw-rw-rw-   0        0        0     2189 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fasta/inorder_access_set.py
--rw-rw-rw-   0        0        0     2095 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fasta/iterator.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.438791 lhc-python-2.5.0/lhc/io/fasta/tools/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fasta/tools/__init__.py
--rw-rw-rw-   0        0        0     2427 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fasta/tools/index.py
--rw-rw-rw-   0        0        0     2195 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fasta/tools/wrap.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.446776 lhc-python-2.5.0/lhc/io/fastq/
--rw-rw-rw-   0        0        0       66 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fastq/__init__.py
--rw-rw-rw-   0        0        0     3493 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fastq/__main__.py
--rw-rw-rw-   0        0        0     1823 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fastq/iterator.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.455259 lhc-python-2.5.0/lhc/io/fastq/tools/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fastq/tools/__init__.py
--rw-rw-rw-   0        0        0     3594 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fastq/tools/filter.py
--rw-rw-rw-   0        0        0     5702 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/fastq/tools/split.py
--rw-rw-rw-   0        0        0      705 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/io/file.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.466737 lhc-python-2.5.0/lhc/io/gbk/
--rw-rw-rw-   0        0        0       77 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/gbk/__init__.py
--rw-rw-rw-   0        0        0      567 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/gbk/__main__.py
--rw-rw-rw-   0        0        0     6390 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/io/gbk/iterator.py
--rw-rw-rw-   0        0        0      582 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/gbk/sequence_set.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.475222 lhc-python-2.5.0/lhc/io/gbk/tools/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/gbk/tools/__init__.py
--rw-rw-rw-   0        0        0     4250 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/gbk/tools/extract.py
--rw-rw-rw-   0        0        0      913 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/gbk/tools/split.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.514148 lhc-python-2.5.0/lhc/io/locus/
--rw-rw-rw-   0        0        0     1181 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/io/locus/__init__.py
--rw-rw-rw-   0        0        0     1242 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/io/locus/bed.py
--rw-rw-rw-   0        0        0     4987 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/io/locus/embl.py
--rw-rw-rw-   0        0        0     5586 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/io/locus/gbk.py
--rw-rw-rw-   0        0        0     1596 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/io/locus/gff.py
--rw-rw-rw-   0        0        0     2008 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/io/locus/gtf.py
--rw-rw-rw-   0        0        0     3356 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/io/locus/locus_file.py
--rw-rw-rw-   0        0        0     2188 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/io/locus/paf.py
--rw-rw-rw-   0        0        0      638 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/io/locus/region.py
--rw-rw-rw-   0        0        0     1660 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/io/locus/repeat_masker.py
--rw-rw-rw-   0        0        0     1958 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/io/locus/sam.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.526126 lhc-python-2.5.0/lhc/io/maf/
--rw-rw-rw-   0        0        0       35 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/maf/__init__.py
--rw-rw-rw-   0        0        0     1479 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/maf/__main__.py
--rw-rw-rw-   0        0        0      444 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/maf/index.py
--rw-rw-rw-   0        0        0     1876 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/maf/iterator.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.531614 lhc-python-2.5.0/lhc/io/methpat/
--rw-rw-rw-   0        0        0        0 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/io/methpat/__init__.py
--rw-rw-rw-   0        0        0      503 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/io/methpat/__main__.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.546586 lhc-python-2.5.0/lhc/io/sequence/
--rw-rw-rw-   0        0        0      817 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/io/sequence/__init__.py
--rw-rw-rw-   0        0        0      499 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/io/sequence/embl.py
--rw-rw-rw-   0        0        0     1296 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/io/sequence/fasta.py
--rw-rw-rw-   0        0        0      678 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/io/sequence/fastq.py
--rw-rw-rw-   0        0        0     2711 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/io/sequence/sequence_file.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.570541 lhc-python-2.5.0/lhc/io/txt/
--rw-rw-rw-   0        0        0      219 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/__init__.py
--rw-rw-rw-   0        0        0      903 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/__main__.py
--rw-rw-rw-   0        0        0      941 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/filter.py
--rw-rw-rw-   0        0        0     3457 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/format_parser.py
--rw-rw-rw-   0        0        0      743 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/formatters.py
--rw-rw-rw-   0        0        0      826 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/indexed_set.py
--rw-rw-rw-   0        0        0     1532 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/iterator.py
--rw-rw-rw-   0        0        0      330 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/set_.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.592998 lhc-python-2.5.0/lhc/io/txt/tools/
--rw-rw-rw-   0        0        0       21 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/tools/__init__.py
--rw-rw-rw-   0        0        0     1188 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/tools/check_format.py
--rw-rw-rw-   0        0        0     1766 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/tools/compress.py
--rw-rw-rw-   0        0        0      809 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/tools/decompress.py
--rw-rw-rw-   0        0        0     1099 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/tools/fetch.py
--rw-rw-rw-   0        0        0     2269 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/tools/index.py
--rw-rw-rw-   0        0        0      766 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/tools/join.py
--rw-rw-rw-   0        0        0     2573 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/txt/tools/sort.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.600982 lhc-python-2.5.0/lhc/io/variant/
--rw-rw-rw-   0        0        0      673 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/io/variant/__init__.py
--rw-rw-rw-   0        0        0     3374 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/io/variant/variant_file.py
--rw-rw-rw-   0        0        0     2793 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/io/variant/vcf.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.619447 lhc-python-2.5.0/lhc/io/vcf/
--rw-rw-rw-   0        0        0      329 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/vcf/__init__.py
--rw-rw-rw-   0        0        0     1889 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/vcf/__main__.py
--rw-rw-rw-   0        0        0     1784 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/vcf/index.py
--rw-rw-rw-   0        0        0     2035 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/io/vcf/iterator.py
--rw-rw-rw-   0        0        0     8569 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/io/vcf/merger.py
--rw-rw-rw-   0        0        0      649 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/vcf/set_.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.650888 lhc-python-2.5.0/lhc/io/vcf/tools/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/vcf/tools/__init__.py
--rw-rw-rw-   0        0        0     1253 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/vcf/tools/compare.py
--rw-rw-rw-   0        0        0     2032 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/vcf/tools/difference.py
--rw-rw-rw-   0        0        0     4722 2021-11-03 22:00:30.000000 lhc-python-2.5.0/lhc/io/vcf/tools/filter.py
--rw-rw-rw-   0        0        0      400 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/vcf/tools/index.py
--rw-rw-rw-   0        0        0     3210 2021-12-16 10:49:33.000000 lhc-python-2.5.0/lhc/io/vcf/tools/merge.py
--rw-rw-rw-   0        0        0     1306 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/vcf/tools/sample.py
--rw-rw-rw-   0        0        0     1871 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/vcf/tools/shift.py
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/vcf/tools/sort.py
--rw-rw-rw-   0        0        0     2355 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/vcf/tools/split_alt.py
--rw-rw-rw-   0        0        0     1860 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/io/vcf/tools/trim_alt.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.662365 lhc-python-2.5.0/lhc/itertools/
--rw-rw-rw-   0        0        0      105 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/itertools/__init__.py
--rw-rw-rw-   0        0        0      311 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/itertools/chunked_iterator.py
--rw-rw-rw-   0        0        0     1503 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/itertools/merge_sorted.py
--rw-rw-rw-   0        0        0     2289 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/itertools/sorted_iterator_merger.py
--rw-rw-rw-   0        0        0      196 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/math.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.674344 lhc-python-2.5.0/lhc/misc/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/misc/__init__.py
--rw-rw-rw-   0        0        0     6004 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/misc/performance_measures.py
--rw-rw-rw-   0        0        0     2069 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/misc/string.py
--rw-rw-rw-   0        0        0     2499 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/misc/tools.py
--rw-rw-rw-   0        0        0      150 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/order.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.679832 lhc-python-2.5.0/lhc/random/
--rw-rw-rw-   0        0        0        0 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/random/__init__.py
--rw-rw-rw-   0        0        0     1962 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/random/reservoir.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.688814 lhc-python-2.5.0/lhc/tools/
--rw-rw-rw-   0        0        0       69 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/tools/__init__.py
--rw-rw-rw-   0        0        0     2400 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lhc/tools/sorter.py
--rw-rw-rw-   0        0        0      836 2021-12-16 10:49:29.000000 lhc-python-2.5.0/lhc/tools/tokeniser.py
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.703789 lhc-python-2.5.0/lhc_python.egg-info/
--rw-rw-rw-   0        0        0     4048 2021-12-16 11:09:20.000000 lhc-python-2.5.0/lhc_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5766 2021-12-16 11:09:20.000000 lhc-python-2.5.0/lhc_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-16 11:09:20.000000 lhc-python-2.5.0/lhc_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2021-12-16 11:09:20.000000 lhc-python-2.5.0/lhc_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2021-12-16 11:09:20.000000 lhc-python-2.5.0/lhc_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.090453 lhc-python-2.5.0/lib/
-drwxrwxrwx   0        0        0        0 2021-12-16 11:09:21.708777 lhc-python-2.5.0/lib/bitap/
--rw-rw-rw-   0        0        0     1986 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lib/bitap/bitap.cpp
--rw-rw-rw-   0        0        0     1265 2021-04-19 09:29:36.000000 lhc-python-2.5.0/lib/bitap/bitapmodule.cpp
--rw-rw-rw-   0        0        0       42 2021-12-16 11:09:21.717263 lhc-python-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1248 2021-12-16 10:49:33.000000 lhc-python-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.423778 lhc_python-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-05-06 11:09:20.000000 lhc_python-2.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-05-06 11:09:29.423778 lhc_python-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-06 11:09:20.000000 lhc_python-2.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-06 11:09:20.000000 lhc_python-2.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 11:09:29.423778 lhc_python-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-06 11:09:20.000000 lhc_python-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.395778 lhc_python-2.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.399778 lhc_python-2.5.1/src/lhc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.399778 lhc_python-2.5.1/src/lhc/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.399778 lhc_python-2.5.1/src/lhc/cli/alignments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/alignments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/alignments/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/alignments/cs_to_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/alignments/mismatch_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/alignments/strand.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.403778 lhc_python-2.5.1/src/lhc/cli/loci/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/closest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/deduplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/difference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/extend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/flank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/intersect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/kmer_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/union.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/loci/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.403778 lhc_python-2.5.1/src/lhc/cli/multiple_alignments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/multiple_alignments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/multiple_alignments/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/multiple_alignments/align_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/multiple_alignments/call_variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/multiple_alignments/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/multiple_alignments/get_consensus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/multiple_alignments/trim_gaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.403778 lhc_python-2.5.1/src/lhc/cli/sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/sequences/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/sequences/barcode_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/sequences/barcode_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/sequences/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/sequences/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/sequences/interleave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/sequences/reverse_complement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/sequences/rmdup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/sequences/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/sequences/stat_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/sequences/unique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/sequences/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.407778 lhc_python-2.5.1/src/lhc/cli/variants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/variants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/variants/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/variants/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/variants/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/variants/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/variants/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/variants/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/variants/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/variants/shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/variants/split_alt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/cli/variants/trim_alt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.407778 lhc_python-2.5.1/src/lhc/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/collections/interval_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/collections/one_pass_interval_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/collections/sequence_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/collections/tabix_file_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.407778 lhc_python-2.5.1/src/lhc/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/data/Emolwt.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    10644 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/data/gc.prt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.407778 lhc_python-2.5.1/src/lhc/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.407778 lhc_python-2.5.1/src/lhc/entities/genomic_coordinate/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/genomic_coordinate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/genomic_coordinate/genomic_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/genomic_coordinate/genomic_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/genomic_coordinate/nested_genomic_interval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.411778 lhc_python-2.5.1/src/lhc/entities/interval/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/interval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/interval/binner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/interval/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/interval/set_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.411778 lhc_python-2.5.1/src/lhc/entities/locus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/locus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/locus/make_loci.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.411778 lhc_python-2.5.1/src/lhc/entities/multiple_alignment/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/multiple_alignment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/multiple_alignment/aligner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/multiple_alignment/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/multiple_alignment/character_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/multiple_alignment/global_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/multiple_alignment/local_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/multiple_alignment/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/multiple_alignment/semiglobal_alignment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.411778 lhc_python-2.5.1/src/lhc/entities/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15843 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/sequence/dicodonshuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/sequence/reverse_complement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/sequence/sequence_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.411778 lhc_python-2.5.1/src/lhc/entities/variant/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/variant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/variant/amino_acid_variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/variant/coding_variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/variant/codon_variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/variant/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/variant/variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/entities/variant/variant_effect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.415778 lhc_python-2.5.1/src/lhc/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/graph/hyper_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/graph/n_partite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/graph/n_partite_graph_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.415778 lhc_python-2.5.1/src/lhc/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.415778 lhc_python-2.5.1/src/lhc/io/alignment/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/alignment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/alignment/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/alignment/alignment_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/alignment/clustal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/alignment/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/alignment/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/filepool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.415778 lhc_python-2.5.1/src/lhc/io/locus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/locus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/locus/bed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/locus/embl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/locus/gbk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/locus/gff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/locus/gtf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/locus/locus_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/locus/paf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/locus/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/locus/repeat_masker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/locus/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.419778 lhc_python-2.5.1/src/lhc/io/methpat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/methpat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/methpat/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.419778 lhc_python-2.5.1/src/lhc/io/methpat/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/methpat/tools/extract_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.419778 lhc_python-2.5.1/src/lhc/io/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/sequence/embl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/sequence/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/sequence/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/sequence/sequence_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.419778 lhc_python-2.5.1/src/lhc/io/variant/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/variant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/variant/maf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/variant/variant_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/io/variant/vcf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.419778 lhc_python-2.5.1/src/lhc/itertools/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/itertools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/itertools/chunked_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/itertools/merge_sorted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/itertools/sorted_iterator_merger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.423778 lhc_python-2.5.1/src/lhc/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/misc/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/misc/genetic_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/misc/iupac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/misc/kmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/misc/natural_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/misc/performance_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/misc/reservoir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/misc/skew.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/misc/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lhc/misc/tokeniser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.423778 lhc_python-2.5.1/src/lhc_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-05-06 11:09:29.000000 lhc_python-2.5.1/src/lhc_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-06 11:09:29.000000 lhc_python-2.5.1/src/lhc_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:09:29.000000 lhc_python-2.5.1/src/lhc_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 11:09:29.000000 lhc_python-2.5.1/src/lhc_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 11:09:29.000000 lhc_python-2.5.1/src/lhc_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.395778 lhc_python-2.5.1/src/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.423778 lhc_python-2.5.1/src/lib/bitap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lib/bitap/bitap.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lib/bitap/bitap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lib/bitap/bitapmodule.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:29.423778 lhc_python-2.5.1/src/lib/digen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lib/digen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lib/digen/digen.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lib/digen/digen.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lib/digen/digen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lib/digen/digenmodule.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-06 11:09:20.000000 lhc_python-2.5.1/src/lib/digen/setup.py
```

### Comparing `lhc-python-2.5.0/LICENSE.txt` & `lhc_python-2.5.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,339 +1,339 @@
-GNU GENERAL PUBLIC LICENSE
-                       Version 2, June 1991
-
- Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
- 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The licenses for most software are designed to take away your
-freedom to share and change it.  By contrast, the GNU General Public
-License is intended to guarantee your freedom to share and change free
-software--to make sure the software is free for all its users.  This
-General Public License applies to most of the Free Software
-Foundation's software and to any other program whose authors commit to
-using it.  (Some other Free Software Foundation software is covered by
-the GNU Lesser General Public License instead.)  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-this service if you wish), that you receive source code or can get it
-if you want it, that you can change the software or use pieces of it
-in new free programs; and that you know you can do these things.
-
-  To protect your rights, we need to make restrictions that forbid
-anyone to deny you these rights or to ask you to surrender the rights.
-These restrictions translate to certain responsibilities for you if you
-distribute copies of the software, or if you modify it.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must give the recipients all the rights that
-you have.  You must make sure that they, too, receive or can get the
-source code.  And you must show them these terms so they know their
-rights.
-
-  We protect your rights with two steps: (1) copyright the software, and
-(2) offer you this license which gives you legal permission to copy,
-distribute and/or modify the software.
-
-  Also, for each author's protection and ours, we want to make certain
-that everyone understands that there is no warranty for this free
-software.  If the software is modified by someone else and passed on, we
-want its recipients to know that what they have is not the original, so
-that any problems introduced by others will not reflect on the original
-authors' reputations.
-
-  Finally, any free program is threatened constantly by software
-patents.  We wish to avoid the danger that redistributors of a free
-program will individually obtain patent licenses, in effect making the
-program proprietary.  To prevent this, we have made it clear that any
-patent must be licensed for everyone's free use or not licensed at all.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                    GNU GENERAL PUBLIC LICENSE
-   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
-
-  0. This License applies to any program or other work which contains
-a notice placed by the copyright holder saying it may be distributed
-under the terms of this General Public License.  The "Program", below,
-refers to any such program or work, and a "work based on the Program"
-means either the Program or any derivative work under copyright law:
-that is to say, a work containing the Program or a portion of it,
-either verbatim or with modifications and/or translated into another
-language.  (Hereinafter, translation is included without limitation in
-the term "modification".)  Each licensee is addressed as "you".
-
-Activities other than copying, distribution and modification are not
-covered by this License; they are outside its scope.  The act of
-running the Program is not restricted, and the output from the Program
-is covered only if its contents constitute a work based on the
-Program (independent of having been made by running the Program).
-Whether that is true depends on what the Program does.
-
-  1. You may copy and distribute verbatim copies of the Program's
-source code as you receive it, in any medium, provided that you
-conspicuously and appropriately publish on each copy an appropriate
-copyright notice and disclaimer of warranty; keep intact all the
-notices that refer to this License and to the absence of any warranty;
-and give any other recipients of the Program a copy of this License
-along with the Program.
-
-You may charge a fee for the physical act of transferring a copy, and
-you may at your option offer warranty protection in exchange for a fee.
-
-  2. You may modify your copy or copies of the Program or any portion
-of it, thus forming a work based on the Program, and copy and
-distribute such modifications or work under the terms of Section 1
-above, provided that you also meet all of these conditions:
-
-    a) You must cause the modified files to carry prominent notices
-    stating that you changed the files and the date of any change.
-
-    b) You must cause any work that you distribute or publish, that in
-    whole or in part contains or is derived from the Program or any
-    part thereof, to be licensed as a whole at no charge to all third
-    parties under the terms of this License.
-
-    c) If the modified program normally reads commands interactively
-    when run, you must cause it, when started running for such
-    interactive use in the most ordinary way, to print or display an
-    announcement including an appropriate copyright notice and a
-    notice that there is no warranty (or else, saying that you provide
-    a warranty) and that users may redistribute the program under
-    these conditions, and telling the user how to view a copy of this
-    License.  (Exception: if the Program itself is interactive but
-    does not normally print such an announcement, your work based on
-    the Program is not required to print an announcement.)
-
-These requirements apply to the modified work as a whole.  If
-identifiable sections of that work are not derived from the Program,
-and can be reasonably considered independent and separate works in
-themselves, then this License, and its terms, do not apply to those
-sections when you distribute them as separate works.  But when you
-distribute the same sections as part of a whole which is a work based
-on the Program, the distribution of the whole must be on the terms of
-this License, whose permissions for other licensees extend to the
-entire whole, and thus to each and every part regardless of who wrote it.
-
-Thus, it is not the intent of this section to claim rights or contest
-your rights to work written entirely by you; rather, the intent is to
-exercise the right to control the distribution of derivative or
-collective works based on the Program.
-
-In addition, mere aggregation of another work not based on the Program
-with the Program (or with a work based on the Program) on a volume of
-a storage or distribution medium does not bring the other work under
-the scope of this License.
-
-  3. You may copy and distribute the Program (or a work based on it,
-under Section 2) in object code or executable form under the terms of
-Sections 1 and 2 above provided that you also do one of the following:
-
-    a) Accompany it with the complete corresponding machine-readable
-    source code, which must be distributed under the terms of Sections
-    1 and 2 above on a medium customarily used for software interchange; or,
-
-    b) Accompany it with a written offer, valid for at least three
-    years, to give any third party, for a charge no more than your
-    cost of physically performing source distribution, a complete
-    machine-readable copy of the corresponding source code, to be
-    distributed under the terms of Sections 1 and 2 above on a medium
-    customarily used for software interchange; or,
-
-    c) Accompany it with the information you received as to the offer
-    to distribute corresponding source code.  (This alternative is
-    allowed only for noncommercial distribution and only if you
-    received the program in object code or executable form with such
-    an offer, in accord with Subsection b above.)
-
-The source code for a work means the preferred form of the work for
-making modifications to it.  For an executable work, complete source
-code means all the source code for all modules it contains, plus any
-associated interface definition files, plus the scripts used to
-control compilation and installation of the executable.  However, as a
-special exception, the source code distributed need not include
-anything that is normally distributed (in either source or binary
-form) with the major components (compiler, kernel, and so on) of the
-operating system on which the executable runs, unless that component
-itself accompanies the executable.
-
-If distribution of executable or object code is made by offering
-access to copy from a designated place, then offering equivalent
-access to copy the source code from the same place counts as
-distribution of the source code, even though third parties are not
-compelled to copy the source along with the object code.
-
-  4. You may not copy, modify, sublicense, or distribute the Program
-except as expressly provided under this License.  Any attempt
-otherwise to copy, modify, sublicense or distribute the Program is
-void, and will automatically terminate your rights under this License.
-However, parties who have received copies, or rights, from you under
-this License will not have their licenses terminated so long as such
-parties remain in full compliance.
-
-  5. You are not required to accept this License, since you have not
-signed it.  However, nothing else grants you permission to modify or
-distribute the Program or its derivative works.  These actions are
-prohibited by law if you do not accept this License.  Therefore, by
-modifying or distributing the Program (or any work based on the
-Program), you indicate your acceptance of this License to do so, and
-all its terms and conditions for copying, distributing or modifying
-the Program or works based on it.
-
-  6. Each time you redistribute the Program (or any work based on the
-Program), the recipient automatically receives a license from the
-original licensor to copy, distribute or modify the Program subject to
-these terms and conditions.  You may not impose any further
-restrictions on the recipients' exercise of the rights granted herein.
-You are not responsible for enforcing compliance by third parties to
-this License.
-
-  7. If, as a consequence of a court judgment or allegation of patent
-infringement or for any other reason (not limited to patent issues),
-conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot
-distribute so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you
-may not distribute the Program at all.  For example, if a patent
-license would not permit royalty-free redistribution of the Program by
-all those who receive copies directly or indirectly through you, then
-the only way you could satisfy both it and this License would be to
-refrain entirely from distribution of the Program.
-
-If any portion of this section is held invalid or unenforceable under
-any particular circumstance, the balance of the section is intended to
-apply and the section as a whole is intended to apply in other
-circumstances.
-
-It is not the purpose of this section to induce you to infringe any
-patents or other property right claims or to contest validity of any
-such claims; this section has the sole purpose of protecting the
-integrity of the free software distribution system, which is
-implemented by public license practices.  Many people have made
-generous contributions to the wide range of software distributed
-through that system in reliance on consistent application of that
-system; it is up to the author/donor to decide if he or she is willing
-to distribute software through any other system and a licensee cannot
-impose that choice.
-
-This section is intended to make thoroughly clear what is believed to
-be a consequence of the rest of this License.
-
-  8. If the distribution and/or use of the Program is restricted in
-certain countries either by patents or by copyrighted interfaces, the
-original copyright holder who places the Program under this License
-may add an explicit geographical distribution limitation excluding
-those countries, so that distribution is permitted only in or among
-countries not thus excluded.  In such case, this License incorporates
-the limitation as if written in the body of this License.
-
-  9. The Free Software Foundation may publish revised and/or new versions
-of the General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-Each version is given a distinguishing version number.  If the Program
-specifies a version number of this License which applies to it and "any
-later version", you have the option of following the terms and conditions
-either of that version or of any later version published by the Free
-Software Foundation.  If the Program does not specify a version number of
-this License, you may choose any version ever published by the Free Software
-Foundation.
-
-  10. If you wish to incorporate parts of the Program into other free
-programs whose distribution conditions are different, write to the author
-to ask for permission.  For software which is copyrighted by the Free
-Software Foundation, write to the Free Software Foundation; we sometimes
-make exceptions for this.  Our decision will be guided by the two goals
-of preserving the free status of all derivatives of our free software and
-of promoting the sharing and reuse of software generally.
-
-                            NO WARRANTY
-
-  11. BECAUSE THE PROGRAM IS LICENSED FREE OF CHARGE, THERE IS NO WARRANTY
-FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW.  EXCEPT WHEN
-OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES
-PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED
-OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
-MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.  THE ENTIRE RISK AS
-TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU.  SHOULD THE
-PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING,
-REPAIR OR CORRECTION.
-
-  12. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY AND/OR
-REDISTRIBUTE THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
-INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING
-OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED
-TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY
-YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER
-PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGES.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-convey the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    {description}
-    Copyright (C) {year}  {fullname}
-
-    This program is free software; you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation; either version 2 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License along
-    with this program; if not, write to the Free Software Foundation, Inc.,
-    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
-
-Also add information on how to contact you by electronic and paper mail.
-
-If the program is interactive, make it output a short notice like this
-when it starts in an interactive mode:
-
-    Gnomovision version 69, Copyright (C) year name of author
-    Gnomovision comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, the commands you use may
-be called something other than `show w' and `show c'; they could even be
-mouse-clicks or menu items--whatever suits your program.
-
-You should also get your employer (if you work as a programmer) or your
-school, if any, to sign a "copyright disclaimer" for the program, if
-necessary.  Here is a sample; alter the names:
-
-  Yoyodyne, Inc., hereby disclaims all copyright interest in the program
-  `Gnomovision' (which makes passes at compilers) written by James Hacker.
-
-  {signature of Ty Coon}, 1 April 1989
-  Ty Coon, President of Vice
-
-This General Public License does not permit incorporating your program into
-proprietary programs.  If your program is a subroutine library, you may
-consider it more useful to permit linking proprietary applications with the
-library.  If this is what you want to do, use the GNU Lesser General
+GNU GENERAL PUBLIC LICENSE
+                       Version 2, June 1991
+
+ Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
+ 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The licenses for most software are designed to take away your
+freedom to share and change it.  By contrast, the GNU General Public
+License is intended to guarantee your freedom to share and change free
+software--to make sure the software is free for all its users.  This
+General Public License applies to most of the Free Software
+Foundation's software and to any other program whose authors commit to
+using it.  (Some other Free Software Foundation software is covered by
+the GNU Lesser General Public License instead.)  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+this service if you wish), that you receive source code or can get it
+if you want it, that you can change the software or use pieces of it
+in new free programs; and that you know you can do these things.
+
+  To protect your rights, we need to make restrictions that forbid
+anyone to deny you these rights or to ask you to surrender the rights.
+These restrictions translate to certain responsibilities for you if you
+distribute copies of the software, or if you modify it.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must give the recipients all the rights that
+you have.  You must make sure that they, too, receive or can get the
+source code.  And you must show them these terms so they know their
+rights.
+
+  We protect your rights with two steps: (1) copyright the software, and
+(2) offer you this license which gives you legal permission to copy,
+distribute and/or modify the software.
+
+  Also, for each author's protection and ours, we want to make certain
+that everyone understands that there is no warranty for this free
+software.  If the software is modified by someone else and passed on, we
+want its recipients to know that what they have is not the original, so
+that any problems introduced by others will not reflect on the original
+authors' reputations.
+
+  Finally, any free program is threatened constantly by software
+patents.  We wish to avoid the danger that redistributors of a free
+program will individually obtain patent licenses, in effect making the
+program proprietary.  To prevent this, we have made it clear that any
+patent must be licensed for everyone's free use or not licensed at all.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                    GNU GENERAL PUBLIC LICENSE
+   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
+
+  0. This License applies to any program or other work which contains
+a notice placed by the copyright holder saying it may be distributed
+under the terms of this General Public License.  The "Program", below,
+refers to any such program or work, and a "work based on the Program"
+means either the Program or any derivative work under copyright law:
+that is to say, a work containing the Program or a portion of it,
+either verbatim or with modifications and/or translated into another
+language.  (Hereinafter, translation is included without limitation in
+the term "modification".)  Each licensee is addressed as "you".
+
+Activities other than copying, distribution and modification are not
+covered by this License; they are outside its scope.  The act of
+running the Program is not restricted, and the output from the Program
+is covered only if its contents constitute a work based on the
+Program (independent of having been made by running the Program).
+Whether that is true depends on what the Program does.
+
+  1. You may copy and distribute verbatim copies of the Program's
+source code as you receive it, in any medium, provided that you
+conspicuously and appropriately publish on each copy an appropriate
+copyright notice and disclaimer of warranty; keep intact all the
+notices that refer to this License and to the absence of any warranty;
+and give any other recipients of the Program a copy of this License
+along with the Program.
+
+You may charge a fee for the physical act of transferring a copy, and
+you may at your option offer warranty protection in exchange for a fee.
+
+  2. You may modify your copy or copies of the Program or any portion
+of it, thus forming a work based on the Program, and copy and
+distribute such modifications or work under the terms of Section 1
+above, provided that you also meet all of these conditions:
+
+    a) You must cause the modified files to carry prominent notices
+    stating that you changed the files and the date of any change.
+
+    b) You must cause any work that you distribute or publish, that in
+    whole or in part contains or is derived from the Program or any
+    part thereof, to be licensed as a whole at no charge to all third
+    parties under the terms of this License.
+
+    c) If the modified program normally reads commands interactively
+    when run, you must cause it, when started running for such
+    interactive use in the most ordinary way, to print or display an
+    announcement including an appropriate copyright notice and a
+    notice that there is no warranty (or else, saying that you provide
+    a warranty) and that users may redistribute the program under
+    these conditions, and telling the user how to view a copy of this
+    License.  (Exception: if the Program itself is interactive but
+    does not normally print such an announcement, your work based on
+    the Program is not required to print an announcement.)
+
+These requirements apply to the modified work as a whole.  If
+identifiable sections of that work are not derived from the Program,
+and can be reasonably considered independent and separate works in
+themselves, then this License, and its terms, do not apply to those
+sections when you distribute them as separate works.  But when you
+distribute the same sections as part of a whole which is a work based
+on the Program, the distribution of the whole must be on the terms of
+this License, whose permissions for other licensees extend to the
+entire whole, and thus to each and every part regardless of who wrote it.
+
+Thus, it is not the intent of this section to claim rights or contest
+your rights to work written entirely by you; rather, the intent is to
+exercise the right to control the distribution of derivative or
+collective works based on the Program.
+
+In addition, mere aggregation of another work not based on the Program
+with the Program (or with a work based on the Program) on a volume of
+a storage or distribution medium does not bring the other work under
+the scope of this License.
+
+  3. You may copy and distribute the Program (or a work based on it,
+under Section 2) in object code or executable form under the terms of
+Sections 1 and 2 above provided that you also do one of the following:
+
+    a) Accompany it with the complete corresponding machine-readable
+    source code, which must be distributed under the terms of Sections
+    1 and 2 above on a medium customarily used for software interchange; or,
+
+    b) Accompany it with a written offer, valid for at least three
+    years, to give any third party, for a charge no more than your
+    cost of physically performing source distribution, a complete
+    machine-readable copy of the corresponding source code, to be
+    distributed under the terms of Sections 1 and 2 above on a medium
+    customarily used for software interchange; or,
+
+    c) Accompany it with the information you received as to the offer
+    to distribute corresponding source code.  (This alternative is
+    allowed only for noncommercial distribution and only if you
+    received the program in object code or executable form with such
+    an offer, in accord with Subsection b above.)
+
+The source code for a work means the preferred form of the work for
+making modifications to it.  For an executable work, complete source
+code means all the source code for all modules it contains, plus any
+associated interface definition files, plus the scripts used to
+control compilation and installation of the executable.  However, as a
+special exception, the source code distributed need not include
+anything that is normally distributed (in either source or binary
+form) with the major components (compiler, kernel, and so on) of the
+operating system on which the executable runs, unless that component
+itself accompanies the executable.
+
+If distribution of executable or object code is made by offering
+access to copy from a designated place, then offering equivalent
+access to copy the source code from the same place counts as
+distribution of the source code, even though third parties are not
+compelled to copy the source along with the object code.
+
+  4. You may not copy, modify, sublicense, or distribute the Program
+except as expressly provided under this License.  Any attempt
+otherwise to copy, modify, sublicense or distribute the Program is
+void, and will automatically terminate your rights under this License.
+However, parties who have received copies, or rights, from you under
+this License will not have their licenses terminated so long as such
+parties remain in full compliance.
+
+  5. You are not required to accept this License, since you have not
+signed it.  However, nothing else grants you permission to modify or
+distribute the Program or its derivative works.  These actions are
+prohibited by law if you do not accept this License.  Therefore, by
+modifying or distributing the Program (or any work based on the
+Program), you indicate your acceptance of this License to do so, and
+all its terms and conditions for copying, distributing or modifying
+the Program or works based on it.
+
+  6. Each time you redistribute the Program (or any work based on the
+Program), the recipient automatically receives a license from the
+original licensor to copy, distribute or modify the Program subject to
+these terms and conditions.  You may not impose any further
+restrictions on the recipients' exercise of the rights granted herein.
+You are not responsible for enforcing compliance by third parties to
+this License.
+
+  7. If, as a consequence of a court judgment or allegation of patent
+infringement or for any other reason (not limited to patent issues),
+conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot
+distribute so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you
+may not distribute the Program at all.  For example, if a patent
+license would not permit royalty-free redistribution of the Program by
+all those who receive copies directly or indirectly through you, then
+the only way you could satisfy both it and this License would be to
+refrain entirely from distribution of the Program.
+
+If any portion of this section is held invalid or unenforceable under
+any particular circumstance, the balance of the section is intended to
+apply and the section as a whole is intended to apply in other
+circumstances.
+
+It is not the purpose of this section to induce you to infringe any
+patents or other property right claims or to contest validity of any
+such claims; this section has the sole purpose of protecting the
+integrity of the free software distribution system, which is
+implemented by public license practices.  Many people have made
+generous contributions to the wide range of software distributed
+through that system in reliance on consistent application of that
+system; it is up to the author/donor to decide if he or she is willing
+to distribute software through any other system and a licensee cannot
+impose that choice.
+
+This section is intended to make thoroughly clear what is believed to
+be a consequence of the rest of this License.
+
+  8. If the distribution and/or use of the Program is restricted in
+certain countries either by patents or by copyrighted interfaces, the
+original copyright holder who places the Program under this License
+may add an explicit geographical distribution limitation excluding
+those countries, so that distribution is permitted only in or among
+countries not thus excluded.  In such case, this License incorporates
+the limitation as if written in the body of this License.
+
+  9. The Free Software Foundation may publish revised and/or new versions
+of the General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+Each version is given a distinguishing version number.  If the Program
+specifies a version number of this License which applies to it and "any
+later version", you have the option of following the terms and conditions
+either of that version or of any later version published by the Free
+Software Foundation.  If the Program does not specify a version number of
+this License, you may choose any version ever published by the Free Software
+Foundation.
+
+  10. If you wish to incorporate parts of the Program into other free
+programs whose distribution conditions are different, write to the author
+to ask for permission.  For software which is copyrighted by the Free
+Software Foundation, write to the Free Software Foundation; we sometimes
+make exceptions for this.  Our decision will be guided by the two goals
+of preserving the free status of all derivatives of our free software and
+of promoting the sharing and reuse of software generally.
+
+                            NO WARRANTY
+
+  11. BECAUSE THE PROGRAM IS LICENSED FREE OF CHARGE, THERE IS NO WARRANTY
+FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW.  EXCEPT WHEN
+OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES
+PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED
+OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
+MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.  THE ENTIRE RISK AS
+TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU.  SHOULD THE
+PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING,
+REPAIR OR CORRECTION.
+
+  12. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY AND/OR
+REDISTRIBUTE THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
+INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING
+OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED
+TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY
+YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER
+PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGES.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+convey the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    {description}
+    Copyright (C) {year}  {fullname}
+
+    This program is free software; you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation; either version 2 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License along
+    with this program; if not, write to the Free Software Foundation, Inc.,
+    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
+
+Also add information on how to contact you by electronic and paper mail.
+
+If the program is interactive, make it output a short notice like this
+when it starts in an interactive mode:
+
+    Gnomovision version 69, Copyright (C) year name of author
+    Gnomovision comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, the commands you use may
+be called something other than `show w' and `show c'; they could even be
+mouse-clicks or menu items--whatever suits your program.
+
+You should also get your employer (if you work as a programmer) or your
+school, if any, to sign a "copyright disclaimer" for the program, if
+necessary.  Here is a sample; alter the names:
+
+  Yoyodyne, Inc., hereby disclaims all copyright interest in the program
+  `Gnomovision' (which makes passes at compilers) written by James Hacker.
+
+  {signature of Ty Coon}, 1 April 1989
+  Ty Coon, President of Vice
+
+This General Public License does not permit incorporating your program into
+proprietary programs.  If your program is a subroutine library, you may
+consider it more useful to permit linking proprietary applications with the
+library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.
```

### Comparing `lhc-python-2.5.0/lhc/binf/align/__main__.py` & `lhc_python-2.5.1/src/lhc/cli/multiple_alignments/align_pairwise.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,52 @@
-import argparse
-import os
-import sys
-
-from lhc.io.fasta import iter_fasta
-from lhc.binf.align import Aligner, Mode, DEFAULT_NUCLEOTIDE_SCORING_MATRIX, DEFAULT_NUCLEOTIDE_ALPHABET
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser():
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser) -> argparse.ArgumentParser:
-    parser.add_argument('sequence1')
-    parser.add_argument('sequence2')
-    parser.add_argument('-m', '--mode', choices=['global', 'local', 'semiglobal'], default='global')
-    parser.add_argument('--molecule', choices=['DNA', 'AA'], default='DNA')
-    parser.set_defaults(func=init_align)
-    return parser
-
-
-def init_align(args):
-    if args.molecule == 'AA':
-        raise NotImplementedError('Not yet implemented: Scoring matrices and alphabet missing for proteins')
-
-    aligner = Aligner(
-        mode=Mode.LOCAL if args.mode == 'local' else Mode.GLOBAL if args.mode == 'global' else Mode.SEMI,
-        scoring_matrix=DEFAULT_NUCLEOTIDE_SCORING_MATRIX if args.molecule == 'DNA' else DEFAULT_NUCLEOTIDE_SCORING_MATRIX,
-        alphabet=DEFAULT_NUCLEOTIDE_ALPHABET if args.molecule == 'DNA' else DEFAULT_NUCLEOTIDE_ALPHABET
-    )
-
-    sequence1 = next(iter_fasta(args.sequence1)).seq if args.sequence1.endswith('.fasta') and os.path.exists(args.sequence1) else\
-        args.sequence1
-    sequence2 = next(iter_fasta(args.sequence2)).seq if args.sequence1.endswith('.fasta') and os.path.exists(args.sequence2) else\
-        args.sequence2
-
-    alignment = aligner.align(sequence1, sequence2)
-    sys.stdout.write(str(alignment))
-    sys.stdout.write('\n')
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+import os
+import sys
+
+from lhc.io.sequence import iter_sequences
+from lhc.entities.multiple_alignment import Aligner, Mode, DEFAULT_NUCLEOTIDE_SCORING_MATRIX, DEFAULT_NUCLEOTIDE_ALPHABET
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser():
+    return define_parser(argparse.ArgumentParser())
+
+
+def get_description() -> str:
+    return 'Align two sequences'
+
+
+def define_parser(parser) -> argparse.ArgumentParser:
+    parser.add_argument('sequence1')
+    parser.add_argument('sequence2')
+    parser.add_argument('-m', '--mode', choices=['global', 'local', 'semiglobal'], default='global')
+    parser.add_argument('--molecule', choices=['DNA', 'AA'], default='DNA')
+    parser.set_defaults(func=init_align)
+    return parser
+
+
+def init_align(args):
+    if args.molecule == 'AA':
+        raise NotImplementedError('Not yet implemented: Scoring matrices and alphabet missing for proteins')
+
+    aligner = Aligner(
+        mode=Mode.LOCAL if args.mode == 'local' else Mode.GLOBAL if args.mode == 'global' else Mode.SEMI,
+        scoring_matrix=DEFAULT_NUCLEOTIDE_SCORING_MATRIX if args.molecule == 'DNA' else DEFAULT_NUCLEOTIDE_SCORING_MATRIX,
+        alphabet=DEFAULT_NUCLEOTIDE_ALPHABET if args.molecule == 'DNA' else DEFAULT_NUCLEOTIDE_ALPHABET
+    )
+
+    sequence1 = next(iter_sequences(args.sequence1)).seq if args.sequence1.endswith('.fasta') and os.path.exists(args.sequence1) else\
+        args.sequence1
+    sequence2 = next(iter_sequences(args.sequence2)).seq if args.sequence1.endswith('.fasta') and os.path.exists(args.sequence2) else\
+        args.sequence2
+
+    alignment = aligner.align(sequence1, sequence2)
+    sys.stdout.write(str(alignment))
+    sys.stdout.write('\n')
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `lhc-python-2.5.0/lhc/binf/align/aligner.py` & `lhc_python-2.5.1/src/lhc/entities/multiple_alignment/aligner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import numpy
-import sys
-
-from enum import Enum
-from lhc.binf.align.alignment import Alignment
-from lhc.binf.align.global_alignment import GlobalAlignment
-from lhc.binf.align.local_alignment import LocalAlignment
-from lhc.binf.align.semiglobal_alignment import SemiGlobalAlignment
-from lhc.binf.align.character_map import CharacterMap
-
-DEFAULT_NUCLEOTIDE_ALPHABET = 'ATGCSWRYKMBVHDN_'
-
-DEFAULT_NUCLEOTIDE_SCORING_MATRIX = numpy.array([
-    [ 5, -4, -4, -4, -4,  1,  1, -4, -4,  1, -4, -1, -1, -1, -2, -5],
-    [-4,  5, -4, -4, -4,  1, -4,  1,  1, -4, -1, -4, -1, -1, -2, -5],
-    [-4, -4,  5, -4,  1, -4,  1, -4,  1, -4, -1, -1, -4, -1, -2, -5],
-    [-4, -4, -4,  5,  1, -4, -4,  1, -4,  1, -1, -1, -1, -4, -2, -5],
-    [-4, -4,  1,  1, -1, -4, -2, -2, -2, -2, -1, -1, -3, -3, -1, -5],
-    [ 1,  1, -4, -4, -4, -1, -2, -2, -2, -2, -3, -3, -1, -1, -1, -5],
-    [ 1, -4,  1, -4, -2, -2, -1, -4, -2, -2, -3, -1, -3, -1, -1, -5],
-    [-4,  1, -4,  1, -2, -2, -4, -1, -2, -2, -1, -3, -1, -3, -1, -5],
-    [-4,  1,  1, -4, -2, -2, -2, -2, -1, -4, -1, -3, -3, -1, -1, -5],
-    [ 1, -4, -4,  1, -2, -2, -2, -2, -4, -1, -3, -1, -1, -3, -1, -5],
-    [-4, -1, -1, -1, -1, -3, -3, -1, -1, -3, -1, -2, -2, -2, -1, -5],
-    [-1, -4, -1, -1, -1, -3, -1, -3, -3, -1, -2, -1, -2, -2, -1, -5],
-    [-1, -1, -4, -1, -3, -1, -3, -1, -3, -1, -2, -2, -1, -2, -1, -5],
-    [-1, -1, -1, -4, -3, -1, -1, -3, -1, -3, -2, -2, -2, -1, -1, -5],
-    [-2, -2, -2, -2, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -5],
-    [-5, -5, -5, -5, -5, -5, -5, -5, -5, -5, -5, -5, -5, -5, -5, -5]])
-
-
-class Mode(Enum):
-    LOCAL = 1
-    GLOBAL = 2
-    SEMI = 3
-
-
-class Aligner:
-
-    def __init__(
-        self,
-        mode: Mode,
-        scoring_matrix=DEFAULT_NUCLEOTIDE_SCORING_MATRIX,
-        alphabet=DEFAULT_NUCLEOTIDE_ALPHABET
-    ):
-        if scoring_matrix.shape[0] != len(alphabet):
-            raise ValueError('Scoring matrix must be square of alphabet length')
-        self.mode = mode
-        self.scoring_matrix = scoring_matrix
-        self.character_map = CharacterMap(alphabet)
-
-    def align(self, sequence1: str, sequence2: str) -> Alignment:
-        end = 0 if self.mode == Mode.LOCAL else -sys.maxsize
-        scores = [end, 0, 0, 0]
-
-        alignment = SemiGlobalAlignment(sequence1, sequence2) if self.mode == Mode.SEMI else \
-            LocalAlignment(sequence1, sequence2) if self.mode == Mode.LOCAL else \
-            GlobalAlignment(sequence1, sequence2)
-        s1 = self.character_map.translate(sequence1)
-        s2 = self.character_map.translate(sequence2)
-        gap = self.character_map.translate('_')[0]
-        for i, ci in enumerate(s1):
-            for j, cj in enumerate(s2):
-                scores[Alignment.DIAG] = alignment.scores[i - 1, j - 1] + self.scoring_matrix[ci, cj]
-                scores[Alignment.LEFT] = alignment.scores[i, j - 1] + self.scoring_matrix[gap, cj]
-                scores[Alignment.UP] = alignment.scores[i - 1, j] + self.scoring_matrix[ci, gap]
-                idx = scores.index(max(scores))
-                alignment.set_entry(i, j, scores[idx], idx)
-        return alignment
+import numpy
+import sys
+
+from enum import Enum
+from lhc.entities.multiple_alignment.alignment import Alignment
+from lhc.entities.multiple_alignment.global_alignment import GlobalAlignment
+from lhc.entities.multiple_alignment.local_alignment import LocalAlignment
+from lhc.entities.multiple_alignment.semiglobal_alignment import SemiGlobalAlignment
+from lhc.entities.multiple_alignment.character_map import CharacterMap
+
+DEFAULT_NUCLEOTIDE_ALPHABET = 'ATGCSWRYKMBVHDN_'
+
+DEFAULT_NUCLEOTIDE_SCORING_MATRIX = numpy.array([
+    [ 5, -4, -4, -4, -4,  1,  1, -4, -4,  1, -4, -1, -1, -1, -2, -5],
+    [-4,  5, -4, -4, -4,  1, -4,  1,  1, -4, -1, -4, -1, -1, -2, -5],
+    [-4, -4,  5, -4,  1, -4,  1, -4,  1, -4, -1, -1, -4, -1, -2, -5],
+    [-4, -4, -4,  5,  1, -4, -4,  1, -4,  1, -1, -1, -1, -4, -2, -5],
+    [-4, -4,  1,  1, -1, -4, -2, -2, -2, -2, -1, -1, -3, -3, -1, -5],
+    [ 1,  1, -4, -4, -4, -1, -2, -2, -2, -2, -3, -3, -1, -1, -1, -5],
+    [ 1, -4,  1, -4, -2, -2, -1, -4, -2, -2, -3, -1, -3, -1, -1, -5],
+    [-4,  1, -4,  1, -2, -2, -4, -1, -2, -2, -1, -3, -1, -3, -1, -5],
+    [-4,  1,  1, -4, -2, -2, -2, -2, -1, -4, -1, -3, -3, -1, -1, -5],
+    [ 1, -4, -4,  1, -2, -2, -2, -2, -4, -1, -3, -1, -1, -3, -1, -5],
+    [-4, -1, -1, -1, -1, -3, -3, -1, -1, -3, -1, -2, -2, -2, -1, -5],
+    [-1, -4, -1, -1, -1, -3, -1, -3, -3, -1, -2, -1, -2, -2, -1, -5],
+    [-1, -1, -4, -1, -3, -1, -3, -1, -3, -1, -2, -2, -1, -2, -1, -5],
+    [-1, -1, -1, -4, -3, -1, -1, -3, -1, -3, -2, -2, -2, -1, -1, -5],
+    [-2, -2, -2, -2, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -5],
+    [-5, -5, -5, -5, -5, -5, -5, -5, -5, -5, -5, -5, -5, -5, -5, -5]])
+
+
+class Mode(Enum):
+    LOCAL = 1
+    GLOBAL = 2
+    SEMI = 3
+
+
+class Aligner:
+
+    def __init__(
+        self,
+        mode: Mode,
+        scoring_matrix=DEFAULT_NUCLEOTIDE_SCORING_MATRIX,
+        alphabet=DEFAULT_NUCLEOTIDE_ALPHABET
+    ):
+        if scoring_matrix.shape[0] != len(alphabet):
+            raise ValueError('Scoring matrix must be square of alphabet length')
+        self.mode = mode
+        self.scoring_matrix = scoring_matrix
+        self.character_map = CharacterMap(alphabet)
+
+    def align(self, sequence1: str, sequence2: str) -> Alignment:
+        end = 0 if self.mode == Mode.LOCAL else -sys.maxsize
+        scores = [end, 0, 0, 0]
+
+        alignment = SemiGlobalAlignment(sequence1, sequence2) if self.mode == Mode.SEMI else \
+            LocalAlignment(sequence1, sequence2) if self.mode == Mode.LOCAL else \
+            GlobalAlignment(sequence1, sequence2)
+        s1 = self.character_map.translate(sequence1)
+        s2 = self.character_map.translate(sequence2)
+        gap = self.character_map.translate('_')[0]
+        for i, ci in enumerate(s1):
+            for j, cj in enumerate(s2):
+                scores[Alignment.DIAG] = alignment.scores[i - 1, j - 1] + self.scoring_matrix[ci, cj]
+                scores[Alignment.LEFT] = alignment.scores[i, j - 1] + self.scoring_matrix[gap, cj]
+                scores[Alignment.UP] = alignment.scores[i - 1, j] + self.scoring_matrix[ci, gap]
+                idx = scores.index(max(scores))
+                alignment.set_entry(i, j, scores[idx], idx)
+        return alignment
```

### Comparing `lhc-python-2.5.0/lhc/binf/align/alignment.py` & `lhc_python-2.5.1/src/lhc/entities/multiple_alignment/alignment.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import numpy
-
-
-class Alignment:
-    END = 0
-    DIAG = 1
-    LEFT = 2
-    UP = 3
-
-    def __init__(self, s1: str, s2: str):
-        self.s1 = s1
-        self.s2 = s2
-
-        self.scores = numpy.zeros((len(s1) + 1, len(s2) + 1), numpy.int32)
-        self.pointers = numpy.zeros((len(s1) + 1, len(s2) + 1), numpy.int32)
-        self.stop = [len(s1) - 1, len(s2) - 1]
-        self.max = [len(s1) - 1, len(s2) - 1]
-
-    def __str__(self) -> str:
-        si = self.s1
-        sj = self.s2
-        i, j = self.stop
-
-        a = []
-        ai = []
-        aj = []
-
-        pointer = self.pointers[i, j]
-        while pointer != Alignment.END:
-            if pointer == Alignment.LEFT:
-                ai.append('-')
-                aj.append(sj[j])
-                a.append(' ')
-                j -= 1
-            elif pointer == Alignment.UP:
-                ai.append(si[i])
-                aj.append('-')
-                a.append(' ')
-                i -= 1
-            elif pointer == Alignment.DIAG:
-                ai.append(si[i])
-                aj.append(sj[j])
-                a.append('|' if si[i] == sj[j] else '.')
-                i -= 1
-                j -= 1
-            pointer = self.pointers[i, j]
-
-        return ''.join(reversed(ai)) + '\n' + ''.join(reversed(a)) + '\n' + ''.join(reversed(aj))
-
-    def get_entry(self, i: int, j: int):
-        return self.scores[i, j], self.pointers[i, j]
-
-    def set_entry(self, i: int, j: int, score: int, pointer: int):
-        self.scores[i, j] = score
-        self.pointers[i, j] = pointer
-
-    def get_score(self) -> int:
-        return self.scores[self.max[0], self.max[1]]
+import numpy
+
+
+class Alignment:
+    END = 0
+    DIAG = 1
+    LEFT = 2
+    UP = 3
+
+    def __init__(self, s1: str, s2: str):
+        self.s1 = s1
+        self.s2 = s2
+
+        self.scores = numpy.zeros((len(s1) + 1, len(s2) + 1), numpy.int32)
+        self.pointers = numpy.zeros((len(s1) + 1, len(s2) + 1), numpy.int32)
+        self.stop = [len(s1) - 1, len(s2) - 1]
+        self.max = [len(s1) - 1, len(s2) - 1]
+
+    def __str__(self) -> str:
+        si = self.s1
+        sj = self.s2
+        i, j = self.stop
+
+        a = []
+        ai = []
+        aj = []
+
+        pointer = self.pointers[i, j]
+        while pointer != Alignment.END:
+            if pointer == Alignment.LEFT:
+                ai.append('-')
+                aj.append(sj[j])
+                a.append(' ')
+                j -= 1
+            elif pointer == Alignment.UP:
+                ai.append(si[i])
+                aj.append('-')
+                a.append(' ')
+                i -= 1
+            elif pointer == Alignment.DIAG:
+                ai.append(si[i])
+                aj.append(sj[j])
+                a.append('|' if si[i] == sj[j] else '.')
+                i -= 1
+                j -= 1
+            pointer = self.pointers[i, j]
+
+        return ''.join(reversed(ai)) + '\n' + ''.join(reversed(a)) + '\n' + ''.join(reversed(aj))
+
+    def get_entry(self, i: int, j: int):
+        return self.scores[i, j], self.pointers[i, j]
+
+    def set_entry(self, i: int, j: int, score: int, pointer: int):
+        self.scores[i, j] = score
+        self.pointers[i, j] = pointer
+
+    def get_score(self) -> int:
+        return self.scores[self.max[0], self.max[1]]
```

### Comparing `lhc-python-2.5.0/lhc/binf/align/score.py` & `lhc_python-2.5.1/src/lhc/entities/multiple_alignment/score.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import numpy
-
-EDNA_ALPHABET = 'ATGCSWRYKMBVHDN'
-
-EDNA_SCORING_MATRIX = numpy.array([
-    [ 5, -4, -4, -4, -4,  1,  1, -4, -4,  1, -4, -1, -1, -1, -2],
-    [-4,  5, -4, -4, -4,  1, -4,  1,  1, -4, -1, -4, -1, -1, -2],
-    [-4, -4,  5, -4,  1, -4,  1, -4,  1, -4, -1, -1, -4, -1, -2],
-    [-4, -4, -4,  5,  1, -4, -4,  1, -4,  1, -1, -1, -1, -4, -2],
-    [-4, -4,  1,  1, -1, -4, -2, -2, -2, -2, -1, -1, -3, -3, -1],
-    [ 1,  1, -4, -4, -4, -1, -2, -2, -2, -2, -3, -3, -1, -1, -1],
-    [ 1, -4,  1, -4, -2, -2, -1, -4, -2, -2, -3, -1, -3, -1, -1],
-    [-4,  1, -4,  1, -2, -2, -4, -1, -2, -2, -1, -3, -1, -3, -1],
-    [-4,  1,  1, -4, -2, -2, -2, -2, -1, -4, -1, -3, -3, -1, -1],
-    [ 1, -4, -4,  1, -2, -2, -2, -2, -4, -1, -3, -1, -1, -3, -1],
-    [-4, -1, -1, -1, -1, -3, -3, -1, -1, -3, -1, -2, -2, -2, -1],
-    [-1, -4, -1, -1, -1, -3, -1, -3, -3, -1, -2, -1, -2, -2, -1],
-    [-1, -1, -4, -1, -3, -1, -3, -1, -3, -1, -2, -2, -1, -2, -1],
-    [-1, -1, -1, -4, -3, -1, -1, -3, -1, -3, -2, -2, -2, -1, -1],
-    [-2, -2, -2, -2, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1]
-])
-
-BLOSUM_ALPHABET = 'ARNDCQEGHILKMFPSTWYVBZX*'
-
-BLOSUM62 = numpy.array([
-    [ 4, -1, -2, -2,  0, -1, -1,  0, -2, -1, -1, -1, -1, -2, -1,  1,  0, -3, -2,  0, -2, -1,  0, -4],
-    [-1,  5,  0, -2, -3,  1,  0, -2,  0, -3, -2,  2, -1, -3, -2, -1, -1, -3, -2, -3, -1,  0, -1, -4],
-    [-2,  0,  6,  1, -3,  0,  0,  0,  1, -3, -3,  0, -2, -3, -2,  1,  0, -4, -2, -3,  3,  0, -1, -4],
-    [-2, -2,  1,  6, -3,  0,  2, -1, -1, -3, -4, -1, -3, -3, -1,  0, -1, -4, -3, -3,  4,  1, -1, -4],
-    [ 0, -3, -3, -3,  9, -3, -4, -3, -3, -1, -1, -3, -1, -2, -3, -1, -1, -2, -2, -1, -3, -3, -2, -4],
-    [-1,  1,  0,  0, -3,  5,  2, -2,  0, -3, -2,  1,  0, -3, -1,  0, -1, -2, -1, -2,  0,  3, -1, -4],
-    [-1,  0,  0,  2, -4,  2,  5, -2,  0, -3, -3,  1, -2, -3, -1,  0, -1, -3, -2, -2,  1,  4, -1, -4],
-    [ 0, -2,  0, -1, -3, -2, -2,  6, -2, -4, -4, -2, -3, -3, -2,  0, -2, -2, -3, -3, -1, -2, -1, -4],
-    [-2,  0,  1, -1, -3,  0,  0, -2,  8, -3, -3, -1, -2, -1, -2, -1, -2, -2,  2, -3,  0,  0, -1, -4],
-    [-1, -3, -3, -3, -1, -3, -3, -4, -3,  4,  2, -3,  1,  0, -3, -2, -1, -3, -1,  3, -3, -3, -1, -4],
-    [-1, -2, -3, -4, -1, -2, -3, -4, -3,  2,  4, -2,  2,  0, -3, -2, -1, -2, -1,  1, -4, -3, -1, -4],
-    [-1,  2,  0, -1, -3,  1,  1, -2, -1, -3, -2,  5, -1, -3, -1,  0, -1, -3, -2, -2,  0,  1, -1, -4],
-    [-1, -1, -2, -3, -1,  0, -2, -3, -2,  1,  2, -1,  5,  0, -2, -1, -1, -1, -1,  1, -3, -1, -1, -4],
-    [-2, -3, -3, -3, -2, -3, -3, -3, -1,  0,  0, -3,  0,  6, -4, -2, -2,  1,  3, -1, -3, -3, -1, -4],
-    [-1, -2, -2, -1, -3, -1, -1, -2, -2, -3, -3, -1, -2, -4,  7, -1, -1, -4, -3, -2, -2, -1, -2, -4],
-    [ 1, -1,  1,  0, -1,  0,  0,  0, -1, -2, -2,  0, -1, -2, -1,  4,  1, -3, -2, -2,  0,  0,  0, -4],
-    [ 0, -1,  0, -1, -1, -1, -1, -2, -2, -1, -1, -1, -1, -2, -1,  1,  5, -2, -2,  0, -1, -1,  0, -4],
-    [-3, -3, -4, -4, -2, -2, -3, -2, -2, -3, -2, -3, -1,  1, -4, -3, -2, 11,  2, -3, -4, -3, -2, -4],
-    [-2, -2, -2, -3, -2, -1, -2, -3,  2, -1, -1, -2, -1,  3, -3, -2, -2,  2,  7, -1, -3, -2, -1, -4],
-    [ 0, -3, -3, -3, -1, -2, -2, -3, -3,  3,  1, -2,  1, -1, -2, -2,  0, -3, -1,  4, -3, -2, -1, -4],
-    [-2, -1,  3,  4, -3,  0,  1, -1,  0, -3, -4,  0, -3, -3, -2,  0, -1, -4, -3, -3,  4,  1, -1, -4],
-    [-1,  0,  0,  1, -3,  3,  4, -2,  0, -3, -3,  1, -1, -3, -1,  0, -1, -3, -2, -2,  1,  4, -1, -4],
-    [ 0, -1, -1, -1, -2, -1, -1, -1, -1, -1, -1, -1, -1, -1, -2,  0,  0, -2, -1, -1, -1, -1, -1, -4],
-    [-4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4,  1]
-])
+import numpy
+
+EDNA_ALPHABET = 'ATGCSWRYKMBVHDN'
+
+EDNA_SCORING_MATRIX = numpy.array([
+    [ 5, -4, -4, -4, -4,  1,  1, -4, -4,  1, -4, -1, -1, -1, -2],
+    [-4,  5, -4, -4, -4,  1, -4,  1,  1, -4, -1, -4, -1, -1, -2],
+    [-4, -4,  5, -4,  1, -4,  1, -4,  1, -4, -1, -1, -4, -1, -2],
+    [-4, -4, -4,  5,  1, -4, -4,  1, -4,  1, -1, -1, -1, -4, -2],
+    [-4, -4,  1,  1, -1, -4, -2, -2, -2, -2, -1, -1, -3, -3, -1],
+    [ 1,  1, -4, -4, -4, -1, -2, -2, -2, -2, -3, -3, -1, -1, -1],
+    [ 1, -4,  1, -4, -2, -2, -1, -4, -2, -2, -3, -1, -3, -1, -1],
+    [-4,  1, -4,  1, -2, -2, -4, -1, -2, -2, -1, -3, -1, -3, -1],
+    [-4,  1,  1, -4, -2, -2, -2, -2, -1, -4, -1, -3, -3, -1, -1],
+    [ 1, -4, -4,  1, -2, -2, -2, -2, -4, -1, -3, -1, -1, -3, -1],
+    [-4, -1, -1, -1, -1, -3, -3, -1, -1, -3, -1, -2, -2, -2, -1],
+    [-1, -4, -1, -1, -1, -3, -1, -3, -3, -1, -2, -1, -2, -2, -1],
+    [-1, -1, -4, -1, -3, -1, -3, -1, -3, -1, -2, -2, -1, -2, -1],
+    [-1, -1, -1, -4, -3, -1, -1, -3, -1, -3, -2, -2, -2, -1, -1],
+    [-2, -2, -2, -2, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1, -1]
+])
+
+BLOSUM_ALPHABET = 'ARNDCQEGHILKMFPSTWYVBZX*'
+
+BLOSUM62 = numpy.array([
+    [ 4, -1, -2, -2,  0, -1, -1,  0, -2, -1, -1, -1, -1, -2, -1,  1,  0, -3, -2,  0, -2, -1,  0, -4],
+    [-1,  5,  0, -2, -3,  1,  0, -2,  0, -3, -2,  2, -1, -3, -2, -1, -1, -3, -2, -3, -1,  0, -1, -4],
+    [-2,  0,  6,  1, -3,  0,  0,  0,  1, -3, -3,  0, -2, -3, -2,  1,  0, -4, -2, -3,  3,  0, -1, -4],
+    [-2, -2,  1,  6, -3,  0,  2, -1, -1, -3, -4, -1, -3, -3, -1,  0, -1, -4, -3, -3,  4,  1, -1, -4],
+    [ 0, -3, -3, -3,  9, -3, -4, -3, -3, -1, -1, -3, -1, -2, -3, -1, -1, -2, -2, -1, -3, -3, -2, -4],
+    [-1,  1,  0,  0, -3,  5,  2, -2,  0, -3, -2,  1,  0, -3, -1,  0, -1, -2, -1, -2,  0,  3, -1, -4],
+    [-1,  0,  0,  2, -4,  2,  5, -2,  0, -3, -3,  1, -2, -3, -1,  0, -1, -3, -2, -2,  1,  4, -1, -4],
+    [ 0, -2,  0, -1, -3, -2, -2,  6, -2, -4, -4, -2, -3, -3, -2,  0, -2, -2, -3, -3, -1, -2, -1, -4],
+    [-2,  0,  1, -1, -3,  0,  0, -2,  8, -3, -3, -1, -2, -1, -2, -1, -2, -2,  2, -3,  0,  0, -1, -4],
+    [-1, -3, -3, -3, -1, -3, -3, -4, -3,  4,  2, -3,  1,  0, -3, -2, -1, -3, -1,  3, -3, -3, -1, -4],
+    [-1, -2, -3, -4, -1, -2, -3, -4, -3,  2,  4, -2,  2,  0, -3, -2, -1, -2, -1,  1, -4, -3, -1, -4],
+    [-1,  2,  0, -1, -3,  1,  1, -2, -1, -3, -2,  5, -1, -3, -1,  0, -1, -3, -2, -2,  0,  1, -1, -4],
+    [-1, -1, -2, -3, -1,  0, -2, -3, -2,  1,  2, -1,  5,  0, -2, -1, -1, -1, -1,  1, -3, -1, -1, -4],
+    [-2, -3, -3, -3, -2, -3, -3, -3, -1,  0,  0, -3,  0,  6, -4, -2, -2,  1,  3, -1, -3, -3, -1, -4],
+    [-1, -2, -2, -1, -3, -1, -1, -2, -2, -3, -3, -1, -2, -4,  7, -1, -1, -4, -3, -2, -2, -1, -2, -4],
+    [ 1, -1,  1,  0, -1,  0,  0,  0, -1, -2, -2,  0, -1, -2, -1,  4,  1, -3, -2, -2,  0,  0,  0, -4],
+    [ 0, -1,  0, -1, -1, -1, -1, -2, -2, -1, -1, -1, -1, -2, -1,  1,  5, -2, -2,  0, -1, -1,  0, -4],
+    [-3, -3, -4, -4, -2, -2, -3, -2, -2, -3, -2, -3, -1,  1, -4, -3, -2, 11,  2, -3, -4, -3, -2, -4],
+    [-2, -2, -2, -3, -2, -1, -2, -3,  2, -1, -1, -2, -1,  3, -3, -2, -2,  2,  7, -1, -3, -2, -1, -4],
+    [ 0, -3, -3, -3, -1, -2, -2, -3, -3,  3,  1, -2,  1, -1, -2, -2,  0, -3, -1,  4, -3, -2, -1, -4],
+    [-2, -1,  3,  4, -3,  0,  1, -1,  0, -3, -4,  0, -3, -3, -2,  0, -1, -4, -3, -3,  4,  1, -1, -4],
+    [-1,  0,  0,  1, -3,  3,  4, -2,  0, -3, -3,  1, -1, -3, -1,  0, -1, -3, -2, -2,  1,  4, -1, -4],
+    [ 0, -1, -1, -1, -2, -1, -1, -1, -1, -1, -1, -1, -1, -1, -2,  0,  0, -2, -1, -1, -1, -1, -1, -4],
+    [-4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4, -4,  1]
+])
```

### Comparing `lhc-python-2.5.0/lhc/binf/align/semiglobal_alignment.py` & `lhc_python-2.5.1/src/lhc/entities/multiple_alignment/semiglobal_alignment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from lhc.binf.align.alignment import Alignment
-
-
-class SemiGlobalAlignment(Alignment):
-
-    def __init__(self, s1: str, s2: str):
-        super().__init__(s1, s2)
-        if len(s1) < len(s2):
-            for i in range(1, len(s1) + 1):
-                self.set_entry(i - 1, -1, -i, Alignment.UP)
-            for j in range(1, len(s2) + 1):
-                self.set_entry(-1, j - 1, 0, Alignment.LEFT)
-        else:
-            for i in range(1, len(s1) + 1):
-                self.set_entry(i - 1, -1, 0, Alignment.UP)
-            for j in range(1, len(s2) + 1):
-                self.set_entry(-1, j - 1, -j, Alignment.LEFT)
-
-    def set_entry(self, i: int, j: int, score: int, pointer: int):
-        if len(self.s1) < len(self.s2) and i == len(self.s1) - 1:
-            if score > self.get_score():
-                super().set_entry(i, j, score, pointer)
-                self.max = [i, j]
-            else:
-                super().set_entry(i, j, score, Alignment.LEFT)
-        elif len(self.s2) < len(self.s1) and j == len(self.s2) - 1:
-            if score > self.get_score():
-                super().set_entry(i, j, score, pointer)
-                self.max = [i, j]
-            else:
-                super().set_entry(i, j, score, Alignment.UP)
-        else:
-            super().set_entry(i, j, score, pointer)
+from lhc.entities.multiple_alignment.alignment import Alignment
+
+
+class SemiGlobalAlignment(Alignment):
+
+    def __init__(self, s1: str, s2: str):
+        super().__init__(s1, s2)
+        if len(s1) < len(s2):
+            for i in range(1, len(s1) + 1):
+                self.set_entry(i - 1, -1, -i, Alignment.UP)
+            for j in range(1, len(s2) + 1):
+                self.set_entry(-1, j - 1, 0, Alignment.LEFT)
+        else:
+            for i in range(1, len(s1) + 1):
+                self.set_entry(i - 1, -1, 0, Alignment.UP)
+            for j in range(1, len(s2) + 1):
+                self.set_entry(-1, j - 1, -j, Alignment.LEFT)
+
+    def set_entry(self, i: int, j: int, score: int, pointer: int):
+        if len(self.s1) < len(self.s2) and i == len(self.s1) - 1:
+            if score > self.get_score():
+                super().set_entry(i, j, score, pointer)
+                self.max = [i, j]
+            else:
+                super().set_entry(i, j, score, Alignment.LEFT)
+        elif len(self.s2) < len(self.s1) and j == len(self.s2) - 1:
+            if score > self.get_score():
+                super().set_entry(i, j, score, pointer)
+                self.max = [i, j]
+            else:
+                super().set_entry(i, j, score, Alignment.UP)
+        else:
+            super().set_entry(i, j, score, pointer)
```

### Comparing `lhc-python-2.5.0/lhc/binf/alignment/tools/get_consensus.py` & `lhc_python-2.5.1/src/lhc/cli/multiple_alignments/get_consensus.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,49 @@
-import argparse
-
-from collections import Counter
-from lhc.io.sequence import open_sequence_file, Sequence
-from typing import Iterator
-
-
-def get_consensus(sequences: Iterator[Sequence]) -> Sequence:
-    consensus = []
-    positions = zip(*sequences)
-    for position in positions:
-        identity = sorted(Counter(position).items(), key=lambda item: item[1])[-1][0]
-        if identity != '-':
-            consensus.append(identity)
-    return Sequence('consensus', ''.join(consensus))
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser() -> argparse.ArgumentParser:
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-    parser.add_argument('input', nargs='?')
-    parser.add_argument('output', nargs='?')
-    parser.add_argument('-i', '--input-format')
-    parser.add_argument('-o', '--output-format')
-    parser.set_defaults(func=init_get_consensus)
-    return parser
-
-
-def init_get_consensus(args):
-    with open_sequence_file(args.input, format=args.input_format) as alignment_file,\
-        open_sequence_file(args.output, mode='w', format=args.output_format) as consensus_file:
-        consensus = get_consensus(alignment_file)
-        consensus_file.write(consensus)
-
-
-if __name__ == '__main__':
-    import sys
-    sys.exit(main())
+import argparse
+
+from collections import Counter
+from lhc.io.sequence import open_sequence_file, Sequence
+from typing import Iterator
+
+
+def get_consensus(sequences: Iterator[Sequence]) -> Sequence:
+    consensus = []
+    positions = zip(*sequences)
+    for position in positions:
+        identity = sorted(Counter(position).items(), key=lambda item: item[1])[-1][0]
+        if identity != '-':
+            consensus.append(identity)
+    return Sequence('consensus', ''.join(consensus))
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser() -> argparse.ArgumentParser:
+    return define_parser(argparse.ArgumentParser(description=get_description()))
+
+
+def get_description() -> str:
+    return 'Get consensus sequences from multiple alignments.'
+
+
+def define_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
+    parser.add_argument('input', nargs='?')
+    parser.add_argument('output', nargs='?')
+    parser.add_argument('-i', '--input-format')
+    parser.add_argument('-o', '--output-format', default='fasta')
+    parser.set_defaults(func=init_get_consensus)
+    return parser
+
+
+def init_get_consensus(args):
+    with open_sequence_file(args.input, format=args.input_format) as alignment_file,\
+        open_sequence_file(args.output, mode='w', format=args.output_format) as consensus_file:
+        consensus = get_consensus(alignment_file)
+        consensus_file.write(consensus)
+
+
+if __name__ == '__main__':
+    import sys
+    sys.exit(main())
```

### Comparing `lhc-python-2.5.0/lhc/binf/alignment/tools/mismatch_filter.py` & `lhc_python-2.5.1/src/lhc/cli/alignments/mismatch_filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,108 @@
-import argparse
-import sys
-
-from lhc.tools.tokeniser import Tokeniser
-from collections import namedtuple
-
-
-SamEntry = namedtuple('SamEntry', ('query_name', 'flag', 'rname', 'pos', 'mapq', 'cigar', 'rnext', 'pnext', 'tlen', 'seq', 'qual', 'tags', 'original'))
-Variant = namedtuple('Variant', ('type', 'value'))
-
-
-def mismatch_filter(alignments, *, percent=0.01, count=100):
-    for alignment in alignments:
-        if 'cs' in alignment.tags:
-            mismatches = 0
-            length = 0
-            for variant in alignment.tags['cs']:
-                if variant.type == 'match':
-                    length += variant.value
-                elif variant.type == 'mismatch':
-                    mismatches += 1
-                    length += 1
-                elif variant.type == 'insertion':
-                    length += len(variant.value)
-            if mismatches / length < percent and mismatches < count:
-                yield alignment
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser():
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser):
-    parser.add_argument('input', nargs='?')
-    parser.add_argument('output', nargs='?')
-    parser.add_argument('-p', '--percent', default=0.01, type=float)
-    parser.add_argument('-c', '--count', default=100, type=int)
-    parser.set_defaults(func=init_filter)
-    return parser
-
-
-def init_filter(args):
-    input = open(args.input) if args.input else sys.stdin
-    output = open(args.output, 'w') if args.output else sys.stdout
-    for alignment in mismatch_filter(iter_sam(input), percent=args.percent, count=args.count):
-        output.write(alignment.original)
-
-
-def iter_sam(stream):
-    for line in stream:
-        if line.startswith('@'):
-            yield SamEntry(None, None, None, None, None, None, None, None, None, None, None, {'cs': parse_cs_tag(':1')}, original=line)
-        else:
-            parts = line.strip().split('\t', 11)
-            parts[1] = int(parts[1])
-            parts[3] = int(parts[3])
-            parts[4] = int(parts[4])
-            parts[11] = dict(parse_tag(definition) for definition in parts[11].split('\t'))
-            if 'cs' in parts[11]:
-                parts[11]['cs'] = parse_cs_tag(parts[11]['cs'])
-            parts.append(line)
-            yield SamEntry(*parts)
-
-
-def parse_tag(definition):
-    key, type, value = definition.split(':', 2)
-    if type == 'i':
-        value = int(value)
-    elif type == 'f':
-        value = float(value)
-    elif type not in 'AZ':
-        raise ValueError('Unknown tag type "{}". Tag: "{}", value: "{}"'.format(type, key, value))
-    return key, value
-
-
-def parse_cs_tag(definition):
-    tokeniser = Tokeniser({
-        'sequence': 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ_',
-        'number': '0123456789',
-        'variant': ':*+-'
-    })
-    tokens = tokeniser.tokenise(definition)
-    variants = []
-    for variant, value in zip(tokens, tokens):
-        if variant.value == ':':
-            variants.append(Variant('match', int(value.value)))
-        elif variant.value == '*':
-            variants.append(Variant('mismatch', value.value))
-        elif variant.value == '+':
-            variants.append(Variant('insertion', value.value))
-        elif variant.value == '-':
-            variants.append(Variant('deletion', value.value))
-        else:
-            raise ValueError('Unknown variant type: "{}"'.format(variant.value))
-    return variants
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+import sys
+
+from lhc.misc.tokeniser import Tokeniser
+from collections import namedtuple
+
+
+SamEntry = namedtuple('SamEntry', ('query_name', 'flag', 'rname', 'pos', 'mapq', 'cigar', 'rnext', 'pnext', 'tlen', 'seq', 'qual', 'tags', 'original'))
+Variant = namedtuple('Variant', ('type', 'value'))
+
+
+def mismatch_filter(alignments, *, percent=0.01, count=100):
+    for alignment in alignments:
+        if 'cs' in alignment.tags:
+            mismatches = 0
+            length = 0
+            for variant in alignment.tags['cs']:
+                if variant.type == 'match':
+                    length += variant.value
+                elif variant.type == 'mismatch':
+                    mismatches += 1
+                    length += 1
+                elif variant.type == 'insertion':
+                    length += len(variant.value)
+            if mismatches / length < percent and mismatches < count:
+                yield alignment
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser():
+    return define_parser(argparse.ArgumentParser(description=get_description()))
+
+
+def get_description() -> str:
+    return 'Filter aligned reads based on the number of mismatches.'
+
+
+def define_parser(parser):
+    parser.add_argument('input', nargs='?')
+    parser.add_argument('output', nargs='?')
+    parser.add_argument('-p', '--percent', default=0.01, type=float)
+    parser.add_argument('-c', '--count', default=100, type=int)
+    parser.set_defaults(func=init_filter)
+    return parser
+
+
+def init_filter(args):
+    input = open(args.input) if args.input else sys.stdin
+    output = open(args.output, 'w') if args.output else sys.stdout
+    for alignment in mismatch_filter(iter_sam(input), percent=args.percent, count=args.count):
+        output.write(alignment.original)
+
+
+def iter_sam(stream):
+    for line in stream:
+        if line.startswith('@'):
+            yield SamEntry(None, None, None, None, None, None, None, None, None, None, None, {'cs': parse_cs_tag(':1')}, original=line)
+        else:
+            parts = line.strip().split('\t', 11)
+            parts[1] = int(parts[1])
+            parts[3] = int(parts[3])
+            parts[4] = int(parts[4])
+            parts[11] = dict(parse_tag(definition) for definition in parts[11].split('\t'))
+            if 'cs' in parts[11]:
+                parts[11]['cs'] = parse_cs_tag(parts[11]['cs'])
+            parts.append(line)
+            yield SamEntry(*parts)
+
+
+def parse_tag(definition):
+    key, type, value = definition.split(':', 2)
+    if type == 'i':
+        value = int(value)
+    elif type == 'f':
+        value = float(value)
+    elif type not in 'AZ':
+        raise ValueError('Unknown tag type "{}". Tag: "{}", value: "{}"'.format(type, key, value))
+    return key, value
+
+
+def parse_cs_tag(definition):
+    tokeniser = Tokeniser({
+        'sequences': 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ_',
+        'number': '0123456789',
+        'variants': ':*+-'
+    })
+    tokens = tokeniser.tokenise(definition)
+    variants = []
+    for variant, value in zip(tokens, tokens):
+        if variant.value == ':':
+            variants.append(Variant('match', int(value.value)))
+        elif variant.value == '*':
+            variants.append(Variant('mismatch', value.value))
+        elif variant.value == '+':
+            variants.append(Variant('insertion', value.value))
+        elif variant.value == '-':
+            variants.append(Variant('deletion', value.value))
+        else:
+            raise ValueError('Unknown variants type: "{}"'.format(variant.value))
+    return variants
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `lhc-python-2.5.0/lhc/binf/alignment/tools/trim_gaps.py` & `lhc_python-2.5.1/src/lhc/cli/sequences/unique.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,52 @@
-import argparse
-
-from collections import Counter
-from lhc.io.sequence import open_sequence_file, Sequence
-from typing import Iterator, List
-
-
-def trim_gaps(sequences: List[Sequence], gap_threshold: 0.1) -> Iterator[Sequence]:
-    positions = list(zip(*sequences))
-    fr = 0
-    to = 0
-    for position in positions:
-        count = Counter(position)
-        if count['-'] / sum(count.values()) < gap_threshold:
-            break
-        fr += 1
-    for position in reversed(positions):
-        count = Counter(position)
-        if count['-'] / sum(count.values()) < gap_threshold:
-            break
-        to -= 1
-    yield from (Sequence(sequence.identifier, sequence.sequence[fr:to]) for sequence in sequences)
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser() -> argparse.ArgumentParser:
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-    parser.add_argument('input', nargs='?')
-    parser.add_argument('output', nargs='?')
-    parser.add_argument('-i', '--input-format')
-    parser.add_argument('-o', '--output-format')
-    parser.add_argument('-g', '--gap-threshold', type=float, default=0.1)
-    parser.set_defaults(func=init_trim)
-    return parser
-
-
-def init_trim(args):
-    with open_sequence_file(args.input, format=args.input_format) as alignment_file,\
-            open_sequence_file(args.output, mode='w', format=args.output_format) as trimmed_alignment_file:
-        trimmed_alignment = trim_gaps(list(alignment_file), args.gap_threshold)
-        for sequence in trimmed_alignment:
-            trimmed_alignment_file.write(sequence)
-
-
-if __name__ == '__main__':
-    import sys
-    sys.exit(main())
+import argparse
+
+from typing import Iterable, Iterator
+from lhc.io.sequence import open_sequence_file, Sequence
+
+
+def unique(sequences: Iterable[Sequence], key_name: str = 'identifier') -> Iterator[Sequence]:
+    visited = set()
+    for sequence in sequences:
+        key = getattr(sequence, key_name)
+        if key not in visited:
+            yield Sequence(sequence.identifier, sequence.sequence, data=sequence.data)
+            visited.add(key)
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser() -> argparse.ArgumentParser:
+    return define_parser(argparse.ArgumentParser(get_description()))
+
+
+def get_description() -> str:
+    return 'Remove duplicate sequnces based on the identifiers.'
+
+
+def define_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
+    parser.add_argument('input', nargs='?',
+                        help='sequences to view (default: stdin).')
+    parser.add_argument('output', nargs='?',
+                        help='sequences file to write viewed sequences to (default: stdout).')
+    parser.add_argument('-i', '--input-format',
+                        help='file format of input file (useful for reading from stdin).')
+    parser.add_argument('-o', '--output-format', default='fasta',
+                        help='file format of output file (useful for writing to stdout).')
+    parser.add_argument('-k', '--key', choices=('identifier', 'sequences'), default='identifier')
+    parser.set_defaults(func=init_view)
+    return parser
+
+
+def init_view(args: argparse.Namespace):
+    with open_sequence_file(args.input, format=args.input_format) as input_sequences,\
+            open_sequence_file(args.output, 'w', format=args.output_format) as output_sequences:
+        for sequence in unique(input_sequences, args.key):
+            output_sequences.write(sequence)
+
+
+if __name__ == '__main__':
+    import sys
+    sys.exit(main())
```

### Comparing `lhc-python-2.5.0/lhc/binf/genetic_code.py` & `lhc_python-2.5.1/src/lhc/misc/genetic_code.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-import pkgutil
-
-
-class RedundantCode(object):
-    BASES = set('actgu')
-    REDUNDANT_BASES = set('bdhkmnrsvwy')
-    AMINO_ACIDS = set('ACDEFGHIKLMNPQRSTVWY*.BZX')
-    CODE = {'a': 'a', 'c': 'c', 'g': 'g', 't': 't', 'u': 'u',
-            'm': 'ac', 'r': 'ag', 'w': 'at',
-            'k': 'gt', 'y': 'tc', 's': 'cg',
-            'b': 'cgt', 'd': 'agt', 'h': 'act', 'v': 'acg', 'n': 'acgt'}
-    REV = {'a': 'a', 'c': 'c', 'g': 'g', 't': 't', 'u': 'u',
-           'ac': 'm', 'ag': 'r', 'at': 'w',
-           'gt': 'k', 'tc': 'y', 'cg': 's',
-           'cgt': 'b', 'agt': 'd', 'act': 'h', 'acg': 'v', 'acgt': 'n'}
-
-    def decode_codon(self, codon):
-        codon = codon.lower()
-        code = RedundantCode.CODE
-        res = []
-        for b1 in code[codon[0]]:
-            for b2 in code[codon[1]]:
-                for b3 in code[codon[2]]:
-                    res.append(b1+b2+b3)
-        return res
-
-    def encode_codon(self, codons):
-        rev = self.REV
-        b1 = set()
-        b2 = set()
-        b3 = set()
-        for codon in codons:
-            b1.add(codon[0])
-            b2.add(codon[1])
-            b3.add(codon[2])
-        
-        return rev[''.join(sorted(list(b1)))] +\
-            rev[''.join(sorted(list(b2)))] +\
-            rev[''.join(sorted(list(b3)))]
-
-    def valid_codon(self, codon):
-        for c in codon:
-            if c not in self.CODE:
-                return False
-        return True
-
-
-class GeneticCode(object):
-
-    NCODONS = 64
-    REDUNDANT_CODE = RedundantCode()
-    BASE2IDX = {'a': 0, 'c': 1, 'g': 2, 't': 3, 'u': 3}
-    IDX2BASE = 'acgt'
-    
-    AMINO_ACIDS = set("ACDEFGHIKLMNPQRSTVWY*")
-
-    def __init__(self, na2aa):
-        self.__aa2na = {}
-        self.__init_aa2na(na2aa)
-
-        self.__na2aa = None
-        self.__init_na2aa(na2aa)
-    
-    def __contains__(self, key):
-        if not isinstance(key, str):
-            raise TypeError('Expected codon or amino acid. Got {}: {}'.format(type(key), key))
-        
-        if key.upper() in GeneticCode.REDUNDANT_CODE.AMINO_ACIDS:
-            return True
-        return GeneticCode.REDUNDANT_CODE.valid_codon(key)
-    
-    def __getitem__(self, key):
-        if isinstance(key, list):
-            key = ''.join(key)
-        if not isinstance(key, str):
-            raise TypeError('Expected codon or amino acid. Got {}: {}'.format(type(key), key))
-        elif len(key) != 1 and len(key) != 3:
-            raise TypeError('Expected codon or amino acid. Got {}: len: {}'.format(type(key), key, len(key)))
-        
-        if key.upper() in GeneticCode.REDUNDANT_CODE.AMINO_ACIDS:
-            return self.__aa2na[key.upper()]
-        decode_codon = GeneticCode.REDUNDANT_CODE.decode_codon  # SPEED_HACK
-        res = set([self.__na2aa[self._codon2index(codon)]
-                   for codon in decode_codon(key)])
-        if len(res) > 1:
-            # raise ValueError('Codon "%s" does not match a specific codon family: %s'%\
-            # (key, str(list(res))))
-            res = ['X']
-        return list(res)[0]
-
-    def get_codons(self, aa):
-        if aa not in GeneticCode.REDUNDANT_CODE.AMINO_ACIDS:
-            aa = self[aa]
-        return self.__aa2na[aa]
-
-    def get_amino_acid(self, codon):
-        return self.__na2aa[self._codon2index(codon)]
-    
-    def translate(self, na):
-        return ''.join([self[na[i * 3:(i * 3) + 3]] for i in range(len(na) // 3)])
-    
-    def __init_aa2na(self, na2aa):
-        setdefault = self.__aa2na.setdefault  # SPEED_HACK
-        for key, val in list(na2aa.items()):
-            setdefault(val, []).append(key)
-
-    def __init_na2aa(self, na2aa):
-        self.__na2aa = GeneticCode.NCODONS * [None]
-        for key, val in list(na2aa.items()):
-            self.__na2aa[self._codon2index(key)] = val
-
-    def _codon2index(self, codon):
-        codon = codon.lower()
-        return 16 * self.BASE2IDX[codon[0]] +\
-            4 * self.BASE2IDX[codon[1]] +\
-            self.BASE2IDX[codon[2]]
-        
-    def _index2codon(self, index):
-        codon = [self.IDX2BASE[index/16],
-                 self.IDX2BASE[(index % 16)/4],
-                 self.IDX2BASE[index % 4]]
-        return "".join(codon)
-
-
-class GeneticCodes:
-    def __init__(self, fname=None):
-        if fname is None:
-            data = pkgutil.get_data('lhc', 'data/gc.prt').decode('utf-8')
-        else:
-            with open(fname, encoding='utf-8') as fileobj:
-                data = fileobj.read()
-        self.codes = {}
-        self.name2id = {}
-        self._parse_file(data)
-
-    def __getitem__(self, key):
-        if isinstance(key, str):
-            key = self.name2id[key]
-        return self.codes[key]
-
-    def get_code(self, id) -> GeneticCode:
-        return self[id]
-    
-    def translate(self, seq, id=1):
-        return self[id].translate(seq)
-    
-    def get_valid_names(self):
-        return list(self.name2id.keys())
-    
-    def _parse_file(self, data):
-        lines = iter(data.split('\n'))
-        line = next(lines)
-        names = []
-        while True:
-            if line[2:6] == 'name':
-                names.append(line[line.find('"') + 1: line.rfind('"')])
-            elif line[2:4] == 'id':
-                id_ = int(line[5:line.find(',')].strip())
-                na2aa = self._parse_code(lines)
-                self.codes[id_] = GeneticCode(na2aa)
-                for name in names:
-                    self.name2id[name] = id_
-                names = []
-            try:
-                line = next(lines)
-            except StopIteration:
-                break
-
-    def _parse_code(self, lines):
-        na2aa = {}  #  'NNN': 'X'}
-        aa_line = next(lines)
-        next(lines)
-        _1 = next(lines)
-        _2 = next(lines)
-        _3 = next(lines)
-        i = 12
-        while aa_line[i] != '"':
-            codon = (_1[i] + _2[i] + _3[i]).lower()
-            na2aa[codon] = aa_line[i]
-            i += 1
-        return na2aa
+import pkgutil
+
+
+class RedundantCode(object):
+    BASES = set('actgu')
+    REDUNDANT_BASES = set('bdhkmnrsvwy')
+    AMINO_ACIDS = set('ACDEFGHIKLMNPQRSTVWY*.BZX')
+    CODE = {'a': 'a', 'c': 'c', 'g': 'g', 't': 't', 'u': 'u',
+            'm': 'ac', 'r': 'ag', 'w': 'at',
+            'k': 'gt', 'y': 'tc', 's': 'cg',
+            'b': 'cgt', 'd': 'agt', 'h': 'act', 'v': 'acg', 'n': 'acgt'}
+    REV = {'a': 'a', 'c': 'c', 'g': 'g', 't': 't', 'u': 'u',
+           'ac': 'm', 'ag': 'r', 'at': 'w',
+           'gt': 'k', 'tc': 'y', 'cg': 's',
+           'cgt': 'b', 'agt': 'd', 'act': 'h', 'acg': 'v', 'acgt': 'n'}
+
+    def decode_codon(self, codon):
+        codon = codon.lower()
+        code = RedundantCode.CODE
+        res = []
+        for b1 in code[codon[0]]:
+            for b2 in code[codon[1]]:
+                for b3 in code[codon[2]]:
+                    res.append(b1+b2+b3)
+        return res
+
+    def encode_codon(self, codons):
+        rev = self.REV
+        b1 = set()
+        b2 = set()
+        b3 = set()
+        for codon in codons:
+            b1.add(codon[0])
+            b2.add(codon[1])
+            b3.add(codon[2])
+        
+        return rev[''.join(sorted(list(b1)))] +\
+            rev[''.join(sorted(list(b2)))] +\
+            rev[''.join(sorted(list(b3)))]
+
+    def valid_codon(self, codon):
+        for c in codon:
+            if c not in self.CODE:
+                return False
+        return True
+
+
+class GeneticCode(object):
+
+    NCODONS = 64
+    REDUNDANT_CODE = RedundantCode()
+    BASE2IDX = {'a': 0, 'c': 1, 'g': 2, 't': 3, 'u': 3}
+    IDX2BASE = 'acgt'
+    
+    AMINO_ACIDS = set("ACDEFGHIKLMNPQRSTVWY*")
+
+    def __init__(self, na2aa):
+        self.__aa2na = {}
+        self.__init_aa2na(na2aa)
+
+        self.__na2aa = None
+        self.__init_na2aa(na2aa)
+    
+    def __contains__(self, key):
+        if not isinstance(key, str):
+            raise TypeError('Expected codon or amino acid. Got {}: {}'.format(type(key), key))
+        
+        if key.upper() in GeneticCode.REDUNDANT_CODE.AMINO_ACIDS:
+            return True
+        return GeneticCode.REDUNDANT_CODE.valid_codon(key)
+    
+    def __getitem__(self, key):
+        if isinstance(key, list):
+            key = ''.join(key)
+        if not isinstance(key, str):
+            raise TypeError('Expected codon or amino acid. Got {}: {}'.format(type(key), key))
+        elif len(key) != 1 and len(key) != 3:
+            raise TypeError('Expected codon or amino acid. Got {}: len: {}'.format(type(key), key, len(key)))
+        
+        if key.upper() in GeneticCode.REDUNDANT_CODE.AMINO_ACIDS:
+            return self.__aa2na[key.upper()]
+        decode_codon = GeneticCode.REDUNDANT_CODE.decode_codon  # SPEED_HACK
+        res = set([self.__na2aa[self._codon2index(codon)]
+                   for codon in decode_codon(key)])
+        if len(res) > 1:
+            # raise ValueError('Codon "%s" does not match a specific codon family: %s'%\
+            # (key, str(list(res))))
+            res = ['X']
+        return list(res)[0]
+
+    def get_codons(self, aa):
+        if aa not in GeneticCode.REDUNDANT_CODE.AMINO_ACIDS:
+            aa = self[aa]
+        return self.__aa2na[aa]
+
+    def get_amino_acid(self, codon):
+        return self.__na2aa[self._codon2index(codon)]
+    
+    def translate(self, na):
+        return ''.join([self[na[i * 3:(i * 3) + 3]] for i in range(len(na) // 3)])
+    
+    def __init_aa2na(self, na2aa):
+        setdefault = self.__aa2na.setdefault  # SPEED_HACK
+        for key, val in list(na2aa.items()):
+            setdefault(val, []).append(key)
+
+    def __init_na2aa(self, na2aa):
+        self.__na2aa = GeneticCode.NCODONS * [None]
+        for key, val in list(na2aa.items()):
+            self.__na2aa[self._codon2index(key)] = val
+
+    def _codon2index(self, codon):
+        codon = codon.lower()
+        return 16 * self.BASE2IDX[codon[0]] +\
+            4 * self.BASE2IDX[codon[1]] +\
+            self.BASE2IDX[codon[2]]
+        
+    def _index2codon(self, index):
+        codon = [self.IDX2BASE[index/16],
+                 self.IDX2BASE[(index % 16)/4],
+                 self.IDX2BASE[index % 4]]
+        return "".join(codon)
+
+
+class GeneticCodes:
+    def __init__(self, fname=None):
+        if fname is None:
+            data = pkgutil.get_data('lhc', 'data/gc.prt').decode('utf-8')
+        else:
+            with open(fname, encoding='utf-8') as fileobj:
+                data = fileobj.read()
+        self.codes = {}
+        self.name2id = {}
+        self._parse_file(data)
+
+    def __getitem__(self, key):
+        if isinstance(key, str):
+            key = self.name2id[key]
+        return self.codes[key]
+
+    def get_code(self, id) -> GeneticCode:
+        return self[id]
+    
+    def translate(self, seq, id=1):
+        return self[id].translate(seq)
+    
+    def get_valid_names(self):
+        return list(self.name2id.keys())
+    
+    def _parse_file(self, data):
+        lines = iter(data.split('\n'))
+        line = next(lines)
+        names = []
+        while True:
+            if line[2:6] == 'name':
+                names.append(line[line.find('"') + 1: line.rfind('"')])
+            elif line[2:4] == 'id':
+                id_ = int(line[5:line.find(',')].strip())
+                na2aa = self._parse_code(lines)
+                self.codes[id_] = GeneticCode(na2aa)
+                for name in names:
+                    self.name2id[name] = id_
+                names = []
+            try:
+                line = next(lines)
+            except StopIteration:
+                break
+
+    def _parse_code(self, lines):
+        na2aa = {}  #  'NNN': 'X'}
+        aa_line = next(lines)
+        next(lines)
+        _1 = next(lines)
+        _2 = next(lines)
+        _3 = next(lines)
+        i = 12
+        while aa_line[i] != '"':
+            codon = (_1[i] + _2[i] + _3[i]).lower()
+            na2aa[codon] = aa_line[i]
+            i += 1
+        return na2aa
```

### Comparing `lhc-python-2.5.0/lhc/binf/genomic_coordinate/genomic_interval.py` & `lhc_python-2.5.1/src/lhc/entities/genomic_coordinate/genomic_interval.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-from copy import deepcopy
-from .genomic_position import GenomicPosition
-from lhc.binf.sequence.reverse_complement import reverse_complement
-from lhc.interval import Interval
-
-
-class GenomicInterval(Interval):
-
-    __slots__ = ('start', 'stop', 'data')
-
-    def __init__(self, start, stop, *, chromosome=None, strand='+', data=None):
-        """
-        Create a genomic interval. Either provide two GenomicPositions or two integers and specify a chromosome.
-
-        :param start: the start position of the interval (inclusive, 0-indexed)
-        :type start: int | GenomicPosition
-        :param stop: the stop position of the interval (not inclusive)
-        :type stop: int | GenomicPosition
-        :param str chromosome: chromosome identifier for interval
-        :param str strand: either '+' or '-'
-        :param data: extra data to be associated with the interval
-        """
-        start = start if isinstance(start, GenomicPosition) else GenomicPosition(start, chromosome=chromosome, strand=strand)
-        stop = stop if isinstance(stop, GenomicPosition) else GenomicPosition(stop, chromosome=chromosome, strand=strand)
-        super().__init__(start, stop, data=data)
-
-    def __str__(self):
-        return '{}:{!r}-{!r}'.format(self.chromosome, self.start.position + 1, self.stop.position)
-
-    @property
-    def chromosome(self):
-        return self.start.chromosome
-
-    @chromosome.setter
-    def chromosome(self, chromosome):
-        self.start.chromosome = chromosome
-        self.stop.chromosome = chromosome
-
-    @property
-    def strand(self):
-        return self.start.strand
-
-    def switch_strand(self):
-        strand = '-' if self.start.strand == '+' else '+'
-        self.start.strand = strand
-        self.stop.strand = strand
-
-    # Set-like operation functions
-
-    def union(self, other, *, ignore_strand=False):
-        """
-        Union of two intervals
-        :param GenomicInterval other: interval to union with
-        :return: union of two intervals íf overlapping or touching
-        :rtype: GenomicInterval
-        """
-        if not ignore_strand:
-            self._assert_same_chromosome_and_strand(other)
-        interval = deepcopy(self)
-        interval.union_update(other)
-        return interval
-
-    def union_update(self, other, *, ignore_strand=False):
-        """
-
-        :param GenomicInterval other:
-        :return:
-        """
-        if not ignore_strand:
-            self._assert_same_chromosome_and_strand(other)
-        self._assert_same_chromosome_and_strand(other)
-        super().union_update(other)
-
-    def intersect(self, other, *, ignore_strand=False):
-        if not ignore_strand:
-            self._assert_same_chromosome_and_strand(other)
-        interval = deepcopy(self)
-        interval.intersect_update(other)
-        return interval
-
-    def intersect_update(self, other, *, ignore_strand=False):
-        if not ignore_strand:
-            self._assert_same_chromosome_and_strand(other)
-        super().intersect_update(other)
-
-    def difference(self, other, *, ignore_strand=False):
-        if not ignore_strand:
-            self._assert_same_chromosome_and_strand(other)
-        if not self.overlaps(other):
-            return Interval.INTERVAL_PAIR(self, None)
-
-        left = right = None
-        if self.start < other.start:
-            left = GenomicInterval(self.start.position, other.start.position, chromosome=self.chromosome,
-                                   strand=self.strand, data=self.data)
-        if other.stop < self.stop:
-            right = GenomicInterval(other.stop.position, self.stop.position, chromosome=self.chromosome,
-                                    strand=self.strand, data=self.data)
-        return Interval.INTERVAL_PAIR(left, right)
-
-    # Interval arithmetic functions
-
-    def add(self, other):
-        self._assert_same_chromosome_and_strand(other)
-        interval = super().add(other)
-        return GenomicInterval(interval.start.position, interval.stop.position, chromosome=self.chromosome,
-                               strand=self.strand, data=self.data)
-
-    def subtract(self, other):
-        self._assert_same_chromosome_and_strand(other)
-        interval = super().subtract(other)
-        return GenomicInterval(interval.start.position, interval.stop.position, chromosome=self.chromosome,
-                               strand=self.strand, data=self.data)
-
-    def multiply(self, other):
-        self._assert_same_chromosome_and_strand(other)
-        interval = super().multiply(other)
-        return GenomicInterval(interval.start.position, interval.stop.position, chromosome=self.chromosome,
-                               strand=self.strand, data=self.data)
-
-    def divide(self, other):
-        self._assert_same_chromosome_and_strand(other)
-        interval = super().divide(other)
-        return GenomicInterval(interval.start.position, interval.stop.position, chromosome=self.chromosome,
-                               strand=self.strand, data=self.data)
-
-    # Position functions
-
-    def get_rel_pos(self, pos):
-        if pos < self.start or pos >= self.stop:
-            raise ValueError('Position outside interval bounds.')
-        return pos - self.start if self.strand == '+'\
-            else self.stop - pos - 1
-
-    def get_sub_seq(self, sequence_set, fr=None, to=None):
-        fr = self.start.position if fr is None else max(self.start.position, fr)
-        to = self.stop.position if to is None else min(self.stop.position, to)
-        res = sequence_set.fetch(str(self.chromosome), fr + 1, to)
-        if self.strand == '-':
-            res = reverse_complement(res)
-        return res
-
-    def get_5p(self):
-        return self.start if self.strand == '+' else\
-            self.stop
-
-    def get_3p(self):
-        return self.stop if self.strand == '+' else\
-            self.start
-
-    def _assert_same_chromosome_and_strand(self, other):
-        if self.chromosome != other.chromosome or self.strand != other.strand:
-            raise ValueError('Genomic intervals must be on same chromosome and strand.')
-
-    def __getstate__(self):
-        return self.start, self.stop, self.data
-
-    def __setstate__(self, state):
-        self.start, self.stop, self.data = state
+from copy import deepcopy
+from .genomic_position import GenomicPosition
+from lhc.entities.sequence.reverse_complement import reverse_complement
+from lhc.entities.interval import Interval
+
+
+class GenomicInterval(Interval):
+
+    __slots__ = ('start', 'stop', 'data')
+
+    def __init__(self, start, stop, *, chromosome=None, strand='+', data=None):
+        """
+        Create a genomic interval. Either provide two GenomicPositions or two integers and specify a chromosome.
+
+        :param start: the start position of the interval (inclusive, 0-indexed)
+        :type start: int | GenomicPosition
+        :param stop: the stop position of the interval (not inclusive)
+        :type stop: int | GenomicPosition
+        :param str chromosome: chromosome identifier for interval
+        :param str strand: either '+' or '-'
+        :param data: extra data to be associated with the interval
+        """
+        start = start if isinstance(start, GenomicPosition) else GenomicPosition(start, chromosome=chromosome, strand=strand)
+        stop = stop if isinstance(stop, GenomicPosition) else GenomicPosition(stop, chromosome=chromosome, strand=strand)
+        super().__init__(start, stop, data=data)
+
+    def __str__(self):
+        return '{}:{!r}-{!r}'.format(self.chromosome, self.start.position + 1, self.stop.position)
+
+    @property
+    def chromosome(self):
+        return self.start.chromosome
+
+    @chromosome.setter
+    def chromosome(self, chromosome):
+        self.start.chromosome = chromosome
+        self.stop.chromosome = chromosome
+
+    @property
+    def strand(self):
+        return self.start.strand
+
+    def switch_strand(self):
+        strand = '-' if self.start.strand == '+' else '+'
+        self.start.strand = strand
+        self.stop.strand = strand
+
+    # Set-like operation functions
+
+    def union(self, other, *, ignore_strand=False):
+        """
+        Union of two intervals
+        :param GenomicInterval other: interval to union with
+        :return: union of two intervals íf overlapping or touching
+        :rtype: GenomicInterval
+        """
+        if not ignore_strand:
+            self._assert_same_chromosome_and_strand(other)
+        interval = deepcopy(self)
+        interval.union_update(other)
+        return interval
+
+    def union_update(self, other, *, ignore_strand=False):
+        """
+
+        :param GenomicInterval other:
+        :return:
+        """
+        if not ignore_strand:
+            self._assert_same_chromosome_and_strand(other)
+        self._assert_same_chromosome_and_strand(other)
+        super().union_update(other)
+
+    def intersect(self, other, *, ignore_strand=False):
+        if not ignore_strand:
+            self._assert_same_chromosome_and_strand(other)
+        interval = deepcopy(self)
+        interval.intersect_update(other)
+        return interval
+
+    def intersect_update(self, other, *, ignore_strand=False):
+        if not ignore_strand:
+            self._assert_same_chromosome_and_strand(other)
+        super().intersect_update(other)
+
+    def difference(self, other, *, ignore_strand=False):
+        if not ignore_strand:
+            self._assert_same_chromosome_and_strand(other)
+        if not self.overlaps(other):
+            return Interval.INTERVAL_PAIR(self, None)
+
+        left = right = None
+        if self.start < other.start:
+            left = GenomicInterval(self.start.position, other.start.position, chromosome=self.chromosome,
+                                   strand=self.strand, data=self.data)
+        if other.stop < self.stop:
+            right = GenomicInterval(other.stop.position, self.stop.position, chromosome=self.chromosome,
+                                    strand=self.strand, data=self.data)
+        return Interval.INTERVAL_PAIR(left, right)
+
+    # Interval arithmetic functions
+
+    def add(self, other):
+        self._assert_same_chromosome_and_strand(other)
+        interval = super().add(other)
+        return GenomicInterval(interval.start.position, interval.stop.position, chromosome=self.chromosome,
+                               strand=self.strand, data=self.data)
+
+    def subtract(self, other):
+        self._assert_same_chromosome_and_strand(other)
+        interval = super().subtract(other)
+        return GenomicInterval(interval.start.position, interval.stop.position, chromosome=self.chromosome,
+                               strand=self.strand, data=self.data)
+
+    def multiply(self, other):
+        self._assert_same_chromosome_and_strand(other)
+        interval = super().multiply(other)
+        return GenomicInterval(interval.start.position, interval.stop.position, chromosome=self.chromosome,
+                               strand=self.strand, data=self.data)
+
+    def divide(self, other):
+        self._assert_same_chromosome_and_strand(other)
+        interval = super().divide(other)
+        return GenomicInterval(interval.start.position, interval.stop.position, chromosome=self.chromosome,
+                               strand=self.strand, data=self.data)
+
+    # Position functions
+
+    def get_rel_pos(self, pos):
+        if pos < self.start or pos >= self.stop:
+            raise ValueError('Position outside interval bounds.')
+        return pos - self.start if self.strand == '+'\
+            else self.stop - pos - 1
+
+    def get_sub_seq(self, sequence_set, fr=None, to=None):
+        fr = self.start.position if fr is None else max(self.start.position, fr)
+        to = self.stop.position if to is None else min(self.stop.position, to)
+        res = sequence_set.fetch(str(self.chromosome), fr, to)
+        if self.strand == '-':
+            res = reverse_complement(res)
+        return res
+
+    def get_5p(self):
+        return self.start if self.strand == '+' else\
+            self.stop
+
+    def get_3p(self):
+        return self.stop if self.strand == '+' else\
+            self.start
+
+    def _assert_same_chromosome_and_strand(self, other):
+        if self.chromosome != other.chromosome or self.strand != other.strand:
+            raise ValueError('Genomic intervals must be on same chromosome and strand.')
+
+    def __getstate__(self):
+        return self.start, self.stop, self.data
+
+    def __setstate__(self, state):
+        self.start, self.stop, self.data = state
```

### Comparing `lhc-python-2.5.0/lhc/binf/genomic_coordinate/genomic_position.py` & `lhc_python-2.5.1/src/lhc/entities/genomic_coordinate/genomic_position.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from functools import total_ordering
-from lhc.order import natural_key
-
-
-class ChromosomeIdentifier:
-    def __init__(self, chromosome: str):
-        self.chromosome = chromosome
-        self.parts = tuple(natural_key(chromosome))
-
-    def __str__(self):
-        return self.chromosome
-
-    def __hash__(self):
-        return hash(self.chromosome)
-
-    def __eq__(self, other):
-        if isinstance(other, str):
-            return self.chromosome == other
-        return self.parts == other.parts
-
-    def __lt__(self, other):
-        if isinstance(other, str):
-            return self.chromosome < other
-        return self.parts < other.parts
-
-
-@total_ordering
-class GenomicPosition:
-
-    def __init__(self, position, *, chromosome=None, strand='+', data=None):
-        self.chromosome = None if chromosome is None else chromosome if isinstance(chromosome, ChromosomeIdentifier) else ChromosomeIdentifier(chromosome)
-        self.position = position
-        self.strand = strand
-        self.data = data
-
-    def __str__(self):
-        return str(self.position)
-
-    def __repr__(self):
-        return 'GenomicPosition({})'.format(self)
-
-    def __hash__(self):
-        return hash((self.chromosome, self.position))
-
-    def __eq__(self, other):
-        if isinstance(other, int) or self.chromosome is None or other.chromosome is None:
-            return self.position == other
-        return self.chromosome == other.chromosome and self.position == other.position and\
-            self.strand == other.strand
-
-    def __lt__(self, other):
-        if isinstance(other, int) or self.chromosome is None or other.chromosome is None:
-            return self.position < other
-        return (self.chromosome < other.chromosome) or\
-            (self.chromosome == other.chromosome) and (self.position < other.position)
-
-    def __add__(self, other):
-        """
-        Add an integer to the current position
-        :param int other: integer to add
-        :return: new position
-        :rtype: GenomicPosition
-        """
-        return GenomicPosition(self.position + other, chromosome=self.chromosome, strand=self.strand)
-
-    def __sub__(self, other):
-        """
-        Subtract either an integer from the current position
-        :param int other: integer to subtract
-        :return: new position
-        :rtype: GenomicPosition
-        """
-        if isinstance(other, GenomicPosition):
-            return self.get_distance_to(other)
-        return GenomicPosition(self.position - other, chromosome=self.chromosome, strand=self.strand)
-
-    def __truediv__(self, other: int):
-        return self.position / other
-
-    def get_distance_to(self, other):
-        """
-        Get the distance between two positions
-        :param GenomicPosition other: other position
-        :return: distance between positions
-        :rtype: int
-        """
-        if self.chromosome != other.chromosome:
-            raise ValueError('Positions on different chromosomes: "{}" and "{}"'.format(self.chromosome, other.chromosome))
-        return self.position - other.position
+from functools import total_ordering
+from lhc.misc.natural_key import natural_key
+
+
+class ChromosomeIdentifier:
+    def __init__(self, chromosome: str):
+        self.chromosome = chromosome
+        self.parts = tuple(natural_key(chromosome))
+
+    def __str__(self):
+        return self.chromosome
+
+    def __hash__(self):
+        return hash(self.chromosome)
+
+    def __eq__(self, other):
+        if isinstance(other, str):
+            return self.chromosome == other
+        return self.parts == other.parts
+
+    def __lt__(self, other):
+        if isinstance(other, str):
+            return self.chromosome < other
+        return self.parts < other.parts
+
+
+@total_ordering
+class GenomicPosition:
+
+    def __init__(self, position, *, chromosome=None, strand='+', data=None):
+        self.chromosome = None if chromosome is None else chromosome if isinstance(chromosome, ChromosomeIdentifier) else ChromosomeIdentifier(chromosome)
+        self.position = position
+        self.strand = strand
+        self.data = data
+
+    def __str__(self):
+        return str(self.position)
+
+    def __repr__(self):
+        return 'GenomicPosition({})'.format(self)
+
+    def __hash__(self):
+        return hash((self.chromosome, self.position))
+
+    def __eq__(self, other):
+        if isinstance(other, int) or self.chromosome is None or other.chromosome is None:
+            return self.position == other
+        return self.chromosome == other.chromosome and self.position == other.position and\
+            self.strand == other.strand
+
+    def __lt__(self, other):
+        if isinstance(other, int) or self.chromosome is None or other.chromosome is None:
+            return self.position < other
+        return (self.chromosome < other.chromosome) or\
+            (self.chromosome == other.chromosome) and (self.position < other.position)
+
+    def __add__(self, other):
+        """
+        Add an integer to the current position
+        :param int other: integer to add
+        :return: new position
+        :rtype: GenomicPosition
+        """
+        return GenomicPosition(self.position + other, chromosome=self.chromosome, strand=self.strand)
+
+    def __sub__(self, other):
+        """
+        Subtract either an integer from the current position
+        :param int other: integer to subtract
+        :return: new position
+        :rtype: GenomicPosition
+        """
+        if isinstance(other, GenomicPosition):
+            return self.get_distance_to(other)
+        return GenomicPosition(self.position - other, chromosome=self.chromosome, strand=self.strand)
+
+    def __truediv__(self, other: int):
+        return self.position / other
+
+    def get_distance_to(self, other):
+        """
+        Get the distance between two positions
+        :param GenomicPosition other: other position
+        :return: distance between positions
+        :rtype: int
+        """
+        if self.chromosome != other.chromosome:
+            raise ValueError('Positions on different chromosomes: "{}" and "{}"'.format(self.chromosome, other.chromosome))
+        return self.position - other.position
```

### Comparing `lhc-python-2.5.0/lhc/binf/genomic_coordinate/nested_genomic_interval.py` & `lhc_python-2.5.1/src/lhc/entities/genomic_coordinate/nested_genomic_interval.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,89 @@
-from typing import List
-
-from .genomic_interval import GenomicInterval
-from lhc.binf.sequence.reverse_complement import reverse_complement
-
-
-class NestedGenomicInterval(GenomicInterval):
-    def __init__(self, start, stop, *, chromosome=None, strand='+', data=None):
-        super().__init__(start, stop, chromosome=chromosome, strand=strand, data=data)
-        self.parent = None
-        self.children = []  # type: List['NestedGenomicInterval']
-
-    def __str__(self):
-        if self.chromosome is None:
-            return '{}-{}'.format(self.start.position + 1, self.stop.position)
-        return '{}:{}-{}'.format(self.chromosome, self.start.position + 1, self.stop.position)
-
-    def __repr__(self):
-        return 'NestedGenomicInterval({})'.format(self)
-
-    def __len__(self):
-        if len(self.children) == 0:
-            return self.stop - self.start
-        return sum(len(child) for child in self.children)
-
-    def add_child(self, child: 'NestedGenomicInterval'):
-        child.parent = self
-        self.children.append(child)
-        if child.start < self.start:
-            self.start = child.start
-            if self.parent:
-                self.parent.start = child.start
-        if child.stop > self.stop:
-            self.stop = child.stop
-            if self.parent:
-                self.parent.stop = child.stop
-
-    def switch_strand(self):
-        super().switch_strand()
-        for child in self.children:
-            child.switch_strand()
-
-    # Position functions
-    
-    def get_abs_pos(self, pos):
-        intervals = self.children if self.strand == '+' else reversed(self.children)
-        fr = 0
-        for interval in intervals:
-            length = len(interval)
-            if fr <= pos < fr + length:
-                return interval.get_abs_pos(pos - fr)
-            fr += length
-        raise IndexError('relative position {} not contained within {}'.format(pos, self))
-    
-    def get_rel_pos(self, pos, types=None):
-        if len(self.children) == 0:
-            if types is None or self.data['type'] in types:
-                return pos - self.start.position
-            else:
-                raise ValueError('Position in interval but not of right type.')
-
-        rel_pos = 0
-        intervals = iter(self.children) if self.strand == '+' else reversed(self.children)
-        for interval in intervals:
-            if interval.start.position <= pos < interval.stop.position:
-                return rel_pos + interval.get_rel_pos(pos, types=types)
-            if types is None or interval.data['type'] in types:
-                rel_pos += len(interval)
-        raise IndexError('absolute position {} not contained within {}'.format(pos, self))
-    
-    # Sequence functions
-    
-    def get_sub_seq(self, sequence_set, *, types=None):
-        res = ''
-        if len(self.children) > 0:
-            res = ''.join(child.get_sub_seq(sequence_set, types=types) for child in self.children)
-        elif types is None or self.data['type'] in types:
-            res = super().get_sub_seq(sequence_set)
-        return res if self.strand == '+' else reverse_complement(res)
-
-    def get_5p(self):
-        return self.children[0].get_5p() if self.strand == '+' else\
-            self.children[-1].get_5p()
-
-    def get_3p(self):
-        return self.children[-1].get_3p() if self.strand == '+' else\
-            self.children[0].get_3p()
+from typing import List
+
+from .genomic_interval import GenomicInterval
+from lhc.entities.sequence.reverse_complement import reverse_complement
+
+
+class NestedGenomicInterval(GenomicInterval):
+    def __init__(self, start, stop, *, chromosome=None, strand='+', data=None):
+        super().__init__(start, stop, chromosome=chromosome, strand=strand, data=data)
+        self.parent = None
+        self.children = []  # type: List['NestedGenomicInterval']
+
+    def __str__(self):
+        if self.chromosome is None:
+            return '{}-{}'.format(self.start.position, self.stop.position)
+        return '{}:{}-{}'.format(self.chromosome, self.start.position, self.stop.position)
+
+    def __repr__(self):
+        return 'NestedGenomicInterval({})'.format(self)
+
+    def __len__(self):
+        if len(self.children) == 0:
+            return self.stop - self.start
+        return sum(len(child) for child in self.children)
+
+    def add_child(self, child: 'NestedGenomicInterval'):
+        child.parent = self
+        self.children.append(child)
+        if child.start < self.start:
+            self.start = child.start
+            if self.parent:
+                self.parent.start = child.start
+        if child.stop > self.stop:
+            self.stop = child.stop
+            if self.parent:
+                self.parent.stop = child.stop
+
+    def switch_strand(self):
+        super().switch_strand()
+        for child in self.children:
+            child.switch_strand()
+
+    # Position functions
+    
+    def get_abs_pos(self, pos):
+        intervals = self.children if self.strand == '+' else reversed(self.children)
+        fr = 0
+        for interval in intervals:
+            length = len(interval)
+            if fr <= pos < fr + length:
+                return interval.get_abs_pos(pos - fr)
+            fr += length
+        raise IndexError('relative position {} not contained within {}'.format(pos, self))
+    
+    def get_rel_pos(self, pos, types=None):
+        if len(self.children) == 0:
+            if types is None or self.data['type'] in types:
+                return pos - self.start.position
+            else:
+                raise ValueError('Position in interval but not of right type.')
+
+        rel_pos = 0
+        intervals = iter(self.children) if self.strand == '+' else reversed(self.children)
+        for interval in intervals:
+            if interval.start.position <= pos < interval.stop.position:
+                return rel_pos + interval.get_rel_pos(pos, types=types)
+            if types is None or interval.data['type'] in types:
+                rel_pos += len(interval)
+        raise IndexError('absolute position {} not contained within {}'.format(pos, self))
+    
+    # Sequence functions
+    
+    def get_sub_seq(self, sequence_set, *, types=None):
+        res = ''
+        if len(self.children) > 0:
+            res = ''.join(child.get_sub_seq(sequence_set, types=types) for child in self.children)
+            if self.strand == '-':
+                res = reverse_complement(res)
+        elif types is None or self.data['type'] in types:
+            res = super().get_sub_seq(sequence_set)
+        return res
+
+    def get_5p(self):
+        return self.children[0].get_5p() if self.strand == '+' else\
+            self.children[-1].get_5p()
+
+    def get_3p(self):
+        return self.children[-1].get_3p() if self.strand == '+' else\
+            self.children[0].get_3p()
```

### Comparing `lhc-python-2.5.0/lhc/binf/iupac.py` & `lhc_python-2.5.1/src/lhc/misc/iupac.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-RAW = """A	Ala	Alanine
-C	Cys	Cysteine
-D	Asp	Aspartic Acid
-E	Glu	Glutamic Acid
-F	Phe	Phenylalanine
-G	Gly	Glycine
-H	His	Histidine
-I	Ile	Isoleucine
-K	Lys	Lysine
-L	Leu	Leucine
-M	Met	Methionine
-N	Asn	Asparagine
-P	Pro	Proline
-Q	Gln	Glutamine
-R	Arg	Arginine
-S	Ser	Serine
-T	Thr	Threonine
-V	Val	Valine
-W	Trp	Tryptophan
-Y	Tyr	Tyrosine
-*	*	Stop"""
-
-DATA = [line.split('\t') for line in RAW.split('\n')]
-
-AA_MAP = {}
-for i, parts in enumerate(DATA):
-    for part in parts:
-        AA_MAP[part] = i
-
-
-def get_one_code(key):
-    return DATA[AA_MAP[key]][0]
-
-
-def get_three_code(key):
-    return DATA[AA_MAP[key]][1]
-
-
-def get_full_name(key):
-    return DATA[AA_MAP[key]][2]
+RAW = """A	Ala	Alanine
+C	Cys	Cysteine
+D	Asp	Aspartic Acid
+E	Glu	Glutamic Acid
+F	Phe	Phenylalanine
+G	Gly	Glycine
+H	His	Histidine
+I	Ile	Isoleucine
+K	Lys	Lysine
+L	Leu	Leucine
+M	Met	Methionine
+N	Asn	Asparagine
+P	Pro	Proline
+Q	Gln	Glutamine
+R	Arg	Arginine
+S	Ser	Serine
+T	Thr	Threonine
+V	Val	Valine
+W	Trp	Tryptophan
+Y	Tyr	Tyrosine
+*	*	Stop"""
+
+DATA = [line.split('\t') for line in RAW.split('\n')]
+
+AA_MAP = {}
+for i, parts in enumerate(DATA):
+    for part in parts:
+        AA_MAP[part] = i
+
+
+def get_one_code(key):
+    return DATA[AA_MAP[key]][0]
+
+
+def get_three_code(key):
+    return DATA[AA_MAP[key]][1]
+
+
+def get_full_name(key):
+    return DATA[AA_MAP[key]][2]
```

### Comparing `lhc-python-2.5.0/lhc/binf/kmer.py` & `lhc_python-2.5.1/src/lhc/misc/kmer.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from collections import Counter
-
-
-class KmerCounter(object):
-    def __init__(self, sequence, k=None, step=1):
-        self.sequence = sequence.lower()
-        self.counts = Counter()
-        self.step = step
-        self.ks = set()
-        if k is not None:
-            self.ks.add(k)
-            self._count_k(k)
-
-    def __str__(self):
-        return str(self.counts)
-
-    def __getitem__(self, key):
-        if len(key) not in self.ks:
-            self._count_k(len(key))
-        return self.counts[key.lower()]
-
-    def _count_k(self, k):
-        for i in range(0, len(self.sequence), self.step):
-            kmer = self.sequence[i:i + k]
-            if kmer not in self.counts:
-                self.counts[kmer] = 0
-            self.counts[kmer] += 1
-        self.ks.add(k)
+from collections import Counter
+
+
+class KmerCounter(object):
+    def __init__(self, sequence, k=None, step=1):
+        self.sequence = sequence.lower()
+        self.counts = Counter()
+        self.step = step
+        self.ks = set()
+        if k is not None:
+            self.ks.add(k)
+            self._count_k(k)
+
+    def __str__(self):
+        return str(self.counts)
+
+    def __getitem__(self, key):
+        if len(key) not in self.ks:
+            self._count_k(len(key))
+        return self.counts[key.lower()]
+
+    def _count_k(self, k):
+        for i in range(0, len(self.sequence), self.step):
+            kmer = self.sequence[i:i + k]
+            if kmer not in self.counts:
+                self.counts[kmer] = 0
+            self.counts[kmer] += 1
+        self.ks.add(k)
```

### Comparing `lhc-python-2.5.0/lhc/binf/loci/make_loci.py` & `lhc_python-2.5.1/src/lhc/entities/locus/make_loci.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import heapq
-
-from typing import Dict, Iterable, Iterator, List
-from lhc.binf.genomic_coordinate import GenomicInterval, NestedGenomicInterval
-
-
-def make_loci(loci: Iterable[GenomicInterval], *, tolerance: int = 100000) -> Iterator[NestedGenomicInterval]:
-    tops = []  # type: List[NestedGenomicInterval]
-    parents = {}  # type: Dict[str, NestedGenomicInterval]
-    for locus in loci:
-        gene_id = locus.data['gene_id']
-        transcript_id = locus.data['transcript_id'] if 'transcript_id' in locus.data else locus.data['gene_id'] + '.1'
-        nested_locus = NestedGenomicInterval(locus.start, locus.stop, strand=locus.strand, data=locus.data)
-
-        if 'feature' not in locus.data or locus.data['feature'] == 'gene':
-            heapq.heappush(tops, nested_locus)
-            parents[gene_id] = nested_locus
-        elif locus.data['feature'] == 'transcript':
-            parents[transcript_id] = nested_locus
-            parents[gene_id].add_child(nested_locus)
-        else:
-            if gene_id not in parents:
-                top = NestedGenomicInterval(locus.start, locus.stop, strand=locus.strand, data=locus.data)
-                heapq.heappush(tops, top)
-                parents[gene_id] = top
-            if transcript_id not in parents:
-                parents[transcript_id] = NestedGenomicInterval(locus.start, locus.stop, strand=locus.strand, data=locus.data)
-                parents[gene_id].add_child(parents[transcript_id])
-            parents[transcript_id].add_child(nested_locus)
-
-        while len(tops) > 0 and tops[0].data['gene_id'] != gene_id and tops[0].stop + tolerance < locus.start:
-            gene = tops.pop(0)
-            for transcript in gene.children:
-                del parents[transcript.data['transcript_id']]
-            del parents[gene.data['gene_id']]
-            yield gene
-
-    yield from tops
+import heapq
+
+from typing import Dict, Iterable, Iterator, List
+from lhc.entities.genomic_coordinate import GenomicInterval, NestedGenomicInterval
+
+
+def make_loci(loci: Iterable[GenomicInterval], *, tolerance: int = 100000) -> Iterator[NestedGenomicInterval]:
+    tops = []  # type: List[NestedGenomicInterval]
+    parents = {}  # type: Dict[str, NestedGenomicInterval]
+    for locus in loci:
+        gene_id = locus.data['gene_id']
+        transcript_id = locus.data['transcript_id'] if 'transcript_id' in locus.data else locus.data['gene_id'] + '.1'
+        nested_locus = NestedGenomicInterval(locus.start, locus.stop, strand=locus.strand, data=locus.data)
+
+        if 'feature' not in locus.data or locus.data['feature'] == 'gene':
+            heapq.heappush(tops, nested_locus)
+            parents[gene_id] = nested_locus
+        elif locus.data['feature'] == 'transcript':
+            parents[transcript_id] = nested_locus
+            parents[gene_id].add_child(nested_locus)
+        else:
+            if gene_id not in parents:
+                top = NestedGenomicInterval(locus.start, locus.stop, strand=locus.strand, data=locus.data)
+                heapq.heappush(tops, top)
+                parents[gene_id] = top
+            if transcript_id not in parents:
+                parents[transcript_id] = NestedGenomicInterval(locus.start, locus.stop, strand=locus.strand, data=locus.data)
+                parents[gene_id].add_child(parents[transcript_id])
+            parents[transcript_id].add_child(nested_locus)
+
+        while len(tops) > 0 and tops[0].data['gene_id'] != gene_id and tops[0].stop + tolerance < locus.start:
+            gene = tops.pop(0)
+            for transcript in gene.children:
+                del parents[transcript.data['transcript_id']]
+            del parents[gene.data['gene_id']]
+            yield gene
+
+    yield from tops
```

### Comparing `lhc-python-2.5.0/lhc/binf/loci/tools/closest.py` & `lhc_python-2.5.1/src/lhc/cli/loci/closest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,80 +1,84 @@
-import argparse
-
-from typing import Iterable, Iterator
-from lhc.binf.genomic_coordinate import GenomicInterval
-from lhc.io.locus import open_locus_file
-
-
-def closest(lefts: Iterable[GenomicInterval], rights: Iterable[GenomicInterval]) -> Iterator[GenomicInterval]:
-    rights = iter(rights)
-    lefts = iter(lefts)
-
-    current_closest = [next(rights, None), next(rights, None)]
-    for left in lefts:
-        if current_closest[0] is None:
-            yield left, None, None
-        else:
-            while left.chromosome != current_closest[0].chromosome or current_closest[1] is not None and current_closest[0].chromosome == current_closest[1].chromosome and abs(current_closest[0].start - left.start) >= abs(current_closest[1].start - left.start):
-                current_closest.pop(0)
-                current_closest.append(next(rights, None))
-            yield left, current_closest[0], abs(current_closest[0].start - left.start)
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser() -> argparse.ArgumentParser:
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser) -> argparse.ArgumentParser:
-    parser.add_argument('input', nargs='?',
-                        help='input loci to filter (default: stdin).')
-    parser.add_argument('output', nargs='?',
-                        help='loci file to extract loci to (default: stdout).')
-    parser.add_argument('-m', '--missing',
-                        help='file to write missing loci to')
-    parser.add_argument('-d', '--direction', default='both', choices=('left', 'right', 'both'),
-                        help='which loci to return')
-    parser.add_argument('-l', '--loci', required=True,
-                        help='loci to find intersections with')
-    parser.add_argument('-i', '--input-format',
-                        help='file format of input file (useful for reading from stdin).')
-    parser.add_argument('-o', '--output-format',
-                        help='file format of output file (useful for writing to stdout).')
-    parser.add_argument('-t', '--tolerance', type=int,
-                        help='limit the farthest detected loci to tolerance.')
-    parser.add_argument('--loci-format')
-    parser.add_argument('--input-index', default=1, type=int)
-    parser.add_argument('--output-index', default=1, type=int)
-    parser.add_argument('--loci-index', default=1, type=int)
-    parser.set_defaults(func=init_closest)
-    return parser
-
-
-def init_closest(args):
-    import sys
-
-    with open_locus_file(args.input, format=args.input_format, index=args.input_index) as input,\
-            open_locus_file(args.output, 'w', format=args.output_format, index=args.output_index) as output, \
-            open_locus_file(args.missing, 'we', format=None if args.missing else args.output_format, index=args.output_index) as missing, \
-            open_locus_file(args.loci, index=args.loci_index) as loci:
-        for left, right, distance in closest(input, loci):
-            if args.direction == 'both':
-                right_id = right.data['gene_id'] if right is not None else None
-                if args.tolerance and distance > args.tolerance:
-                    missing.write(left)
-                else:
-                    sys.stdout.write('\t{}\t{}\t{}\t{}\t{}\t{}\n'.format(left.chromosome, left.start.position, left.stop.position, right.start.position, right.stop.position, distance))
-            else:
-                locus = left if args.direction == 'left' else right
-                if args.tolerance and distance > args.tolerance:
-                    missing.write(locus)
-                else:
-                    output.write(locus)
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+
+from typing import Iterable, Iterator
+from lhc.entities.genomic_coordinate import GenomicInterval
+from lhc.io.locus import open_locus_file
+
+
+def closest(lefts: Iterable[GenomicInterval], rights: Iterable[GenomicInterval]) -> Iterator[GenomicInterval]:
+    rights = iter(rights)
+    lefts = iter(lefts)
+
+    current_closest = [next(rights, None), next(rights, None)]
+    for left in lefts:
+        if current_closest[0] is None:
+            yield left, None, None
+        else:
+            while left.chromosome != current_closest[0].chromosome or current_closest[1] is not None and current_closest[0].chromosome == current_closest[1].chromosome and abs(current_closest[0].start - left.start) >= abs(current_closest[1].start - left.start):
+                current_closest.pop(0)
+                current_closest.append(next(rights, None))
+            yield left, current_closest[0], abs(current_closest[0].start - left.start)
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser() -> argparse.ArgumentParser:
+    return define_parser(argparse.ArgumentParser(description=get_description()))
+
+
+def get_description() -> str:
+    return 'Get the closest loci to the given loci.'
+
+
+def define_parser(parser) -> argparse.ArgumentParser:
+    parser.add_argument('input', nargs='?',
+                        help='input loci to filter (default: stdin).')
+    parser.add_argument('output', nargs='?',
+                        help='loci file to extract loci to (default: stdout).')
+    parser.add_argument('-m', '--missing',
+                        help='file to write missing loci to')
+    parser.add_argument('-d', '--direction', default='both', choices=('left', 'right', 'both'),
+                        help='which loci to return')
+    parser.add_argument('-l', '--loci', required=True,
+                        help='loci to find intersections with')
+    parser.add_argument('-i', '--input-format',
+                        help='file format of input file (useful for reading from stdin).')
+    parser.add_argument('-o', '--output-format', default='gtf',
+                        help='file format of output file (useful for writing to stdout).')
+    parser.add_argument('-t', '--tolerance', type=int,
+                        help='limit the farthest detected loci to tolerance.')
+    parser.add_argument('--loci-format')
+    parser.add_argument('--input-index', default=1, type=int)
+    parser.add_argument('--output-index', default=1, type=int)
+    parser.add_argument('--loci-index', default=1, type=int)
+    parser.set_defaults(func=init_closest)
+    return parser
+
+
+def init_closest(args):
+    import sys
+
+    with open_locus_file(args.input, format=args.input_format, index=args.input_index) as input,\
+            open_locus_file(args.output, 'w', format=args.output_format, index=args.output_index) as output, \
+            open_locus_file(args.missing, 'we', format=None if args.missing else args.output_format, index=args.output_index) as missing, \
+            open_locus_file(args.loci, index=args.loci_index) as loci:
+        for left, right, distance in closest(input, loci):
+            if args.direction == 'both':
+                right_id = right.data['gene_id'] if right is not None else None
+                if args.tolerance and distance > args.tolerance:
+                    missing.write(left)
+                else:
+                    sys.stdout.write('\t{}\t{}\t{}\t{}\t{}\t{}\n'.format(left.chromosome, left.start.position, left.stop.position, right.start.position, right.stop.position, distance))
+            else:
+                locus = left if args.direction == 'left' else right
+                if args.tolerance and distance > args.tolerance:
+                    missing.write(locus)
+                else:
+                    output.write(locus)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `lhc-python-2.5.0/lhc/binf/loci/tools/deduplicate.py` & `lhc_python-2.5.1/src/lhc/cli/loci/filter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,68 @@
-import sys
-import argparse
-
-from typing import Iterable, Iterator
-from lhc.binf.genomic_coordinate import GenomicInterval
-from lhc.io.locus import open_locus_file
-
-
-def deduplicate(interval_file: Iterable[GenomicInterval], *, threshold=0) -> Iterator[GenomicInterval]:
-    intervals = iter(interval_file)
-    prev = next(intervals, None)
-    for interval in intervals:
-        if interval.chromosome != prev.chromosome or interval.start - prev.start > threshold:
-            yield prev
-            prev = interval
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser():
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser):
-    parser.add_argument('input', nargs='?',
-                        help='name of the intervals file to be extended (default: stdin).')
-    parser.add_argument('output', nargs='?',
-                        help='name of the extended intervals file (default: stdout).')
-    parser.add_argument('-i', '--input-format',
-                        help='file format of input file (useful for reading from stdin).')
-    parser.add_argument('-o', '--output-format',
-                        help='file format of output file (useful for writing to stdout).')
-    parser.add_argument('-t', '--threshold', type=int, default=0,
-                        help='locus within the threshold are replaced with the upstream locus')
-    parser.set_defaults(func=init_deduplicate)
-    return parser
-
-
-def init_deduplicate(args):
-    args.output_format = args.input_format if args.output_format is None else args.output_format
-    with open_locus_file(args.input, format=args.input_format) as input,\
-            open_locus_file(args.output, 'w', format=args.output_format) as output:
-        for interval in deduplicate(input, threshold=args.threshold):
-            output.write(interval)
-
-
-if __name__ == '__main__':
-    sys.exit(main())
+import sys
+import argparse
+
+from typing import Iterable, Iterator, Optional
+from lhc.entities.genomic_coordinate import GenomicInterval
+from lhc.io.locus import open_locus_file
+
+
+def filter(intervals: Iterable[GenomicInterval], filter_: Optional[str] = None) -> Iterator[GenomicInterval]:
+    filter_fn = eval('lambda: {}'.format(filter_))
+    for interval in intervals:
+        local_variables = {
+            'chromosome': interval.chromosome,
+            'start': interval.start,
+            'stop': interval.stop,
+            'strand': interval.strand
+        }
+        if interval.data:
+            local_variables.update(interval.data)
+        globals().update(local_variables)
+        if filter_fn():
+            yield interval
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser():
+    return define_parser(argparse.ArgumentParser(description=get_description()))
+
+
+def get_description() -> str:
+    return 'Filter loci using the given conditions.'
+
+
+def define_parser(parser):
+    parser.add_argument('input', nargs='?',
+                        help='name of the intervals file to be filtered (default: stdin).')
+    parser.add_argument('output', nargs='?',
+                        help='name of the filtered intervals file (default: stdout).')
+    parser.add_argument('-f', '--filter', required=True,
+                        help='filter to apply (default: none).')
+    parser.add_argument('-i', '--input-format',
+                        help='file format of input file (useful for reading from stdin).')
+    parser.add_argument('-o', '--output-format', default='gtf',
+                        help='file format of output file (useful for writing to stdout).')
+    parser.add_argument('-v', '--inverse', action='store_true',
+                        help='invert filter.')
+    group = parser.add_mutually_exclusive_group()
+    group.add_argument('-r', '--region',
+                       help='apply filter in region (default: none).')
+    group.add_argument('-x', '--exclude',
+                       help='do not apply filter in region (default: none).')
+    parser.set_defaults(func=init_filter)
+    return parser
+
+
+def init_filter(args):
+    with open_locus_file(args.input, format=args.input_format) as input,\
+            open_locus_file(args.output, 'w', format=args.output_format) as output:
+        for interval in filter(input, args.filter_):
+            output.write(interval)
+
+
+if __name__ == '__main__':
+    sys.exit(main())
```

### Comparing `lhc-python-2.5.0/lhc/binf/loci/tools/filter.py` & `lhc_python-2.5.1/src/lhc/cli/loci/view.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,47 @@
-import sys
-import argparse
-
-from typing import Iterable, Iterator
-from lhc.binf.genomic_coordinate import GenomicInterval
-from lhc.io.locus import open_locus_file
-
-
-def filter(intervals: Iterable[GenomicInterval], expression=None) -> Iterator[GenomicInterval]:
-    for interval in intervals:
-        local_variables = {
-            'chromosome': interval.chromosome,
-            'start': interval.start,
-            'stop': interval.stop,
-            'strand': interval.strand
-        }
-        if interval.data:
-            local_variables.update(interval.data)
-        globals().update(local_variables)
-        if expression():
-            yield interval
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser():
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser):
-    parser.add_argument('input', nargs='?',
-                        help='name of the intervals file to be filtered (default: stdin).')
-    parser.add_argument('output', nargs='?',
-                        help='name of the filtered intervals file (default: stdout).')
-    parser.add_argument('-f', '--filter', required=True,
-                        help='filter to apply (default: none).')
-    parser.add_argument('-i', '--input-format',
-                        help='file format of input file (useful for reading from stdin).')
-    parser.add_argument('-o', '--output-format',
-                        help='file format of output file (useful for writing to stdout).')
-    parser.add_argument('-v', '--inverse', action='store_true',
-                        help='invert filter.')
-    group = parser.add_mutually_exclusive_group()
-    group.add_argument('-r', '--region',
-                       help='apply filter in region (default: none).')
-    group.add_argument('-x', '--exclude',
-                       help='do not apply filter in region (default: none).')
-    parser.set_defaults(func=init_filter)
-    return parser
-
-
-def init_filter(args):
-    with open_locus_file(args.input, format=args.input_format) as input,\
-            open_locus_file(args.output, 'w', format=args.output_format) as output:
-        filter_fn = eval('lambda: {}'.format(args.filter))
-        for interval in filter(input, filter_fn):
-            output.write(interval)
-
-
-if __name__ == '__main__':
-    sys.exit(main())
+import sys
+import argparse
+
+from typing import Iterable, Iterator
+from lhc.entities.genomic_coordinate import GenomicInterval
+from lhc.io.locus import open_locus_file
+
+
+def view(intervals: Iterable[GenomicInterval]) -> Iterator[GenomicInterval]:
+    yield from intervals
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser():
+    return define_parser(argparse.ArgumentParser(description=get_description()))
+
+
+def get_description() -> str:
+    return 'View the loci in the given file'
+
+
+def define_parser(parser):
+    parser.add_argument('input', nargs='?',
+                        help='name of the intervals file to be viewed (default: stdin).')
+    parser.add_argument('output', nargs='?',
+                        help='name of the output intervals file (default: stdout).')
+    parser.add_argument('-i', '--input-format',
+                        help='file format of input file (useful for reading from stdin).')
+    parser.add_argument('-o', '--output-format', default='gtf',
+                        help='file format of output file (useful for writing to stdout).')
+    parser.set_defaults(func=init_view)
+    return parser
+
+
+def init_view(args):
+    with open_locus_file(args.input, format=args.input_format) as input,\
+            open_locus_file(args.output, 'w', format=args.output_format) as output:
+        for interval in view(input):
+            output.write(interval)
+
+
+if __name__ == '__main__':
+    sys.exit(main())
```

### Comparing `lhc-python-2.5.0/lhc/binf/loci/tools/flank.py` & `lhc_python-2.5.1/src/lhc/cli/loci/flank.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,100 @@
-import sys
-import argparse
-
-from copy import copy
-from typing import Iterable, Iterator
-from lhc.binf.genomic_coordinate import GenomicInterval
-from lhc.io.locus import open_locus_file
-
-
-def flank(intervals: Iterable[GenomicInterval], *, point_one=0, point_two=0, point_three=0, point_four=0, orientation='same') -> Iterator[GenomicInterval]:
-    """
-    Create flanking intervals for each interval in `intervals`.
-    :param intervals: intervals to flank
-    :param five_prime: how much upstream to flank
-    :param three_prime: how much downstream to flank
-    :return: tuple of five- and three-prime flanks
-    """
-    for interval in intervals:
-        strand = interval.strand if orientation == 'same' else '-' if interval.strand == '+' else '+'
-        five_prime_interval = None if point_one == point_two else \
-            GenomicInterval(interval.start + point_one, interval.start + point_two, chromosome=interval.chromosome,
-                            strand=strand, data=copy(interval.data)) if interval.strand == '+' else \
-            GenomicInterval(interval.stop - point_two, interval.stop - point_one, chromosome=interval.chromosome,
-                            strand=strand, data=copy(interval.data))
-        three_prime_interval = None if point_three == point_four else \
-            GenomicInterval(interval.stop + point_three, interval.stop + point_four, chromosome=interval.chromosome,
-                            strand=strand, data=copy(interval.data)) if interval.strand == '+' else \
-            GenomicInterval(interval.start - point_four, interval.start - point_three, chromosome=interval.chromosome,
-                            strand=strand, data=copy(interval.data))
-        if five_prime_interval and five_prime_interval.start >= 0:
-            five_prime_interval.data['gene_id'] += '_5p_flank'
-            five_prime_interval.data['transcript_id'] = five_prime_interval.data['gene_id'] + five_prime_interval.data['transcript_id'][five_prime_interval.data['transcript_id'].find('.'):] if 'transcript_id' in five_prime_interval.data else five_prime_interval.data['gene_id'] + '.1'
-            five_prime_interval.data['exon_id'] = five_prime_interval.data['gene_id'] + five_prime_interval.data['exon_id'][five_prime_interval.data['exon_id'].find('.'):] if 'exon_id' in five_prime_interval.data else five_prime_interval.data['gene_id'] + '.1'
-            five_prime_interval.data['feature'] = '5p_flank'
-        if three_prime_interval and three_prime_interval.start >= 0:
-            three_prime_interval.data['gene_id'] += '_3p_flank'
-            three_prime_interval.data['transcript_id'] = three_prime_interval.data['gene_id'] + three_prime_interval.data['transcript_id'][three_prime_interval.data['transcript_id'].find('.'):] if 'transcript_id' in three_prime_interval.data else three_prime_interval.data['gene_id'] + '.1'
-            three_prime_interval.data['exon_id'] = three_prime_interval.data['gene_id'] + three_prime_interval.data['exon_id'][three_prime_interval.data['exon_id'].find('.'):] if 'exon_id' in three_prime_interval.data else three_prime_interval.data['gene_id'] + '.1'
-            three_prime_interval.data['feature'] = '3p_flank'
-        yield five_prime_interval, three_prime_interval
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser():
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser):
-    parser.add_argument('input', nargs='?',
-                        help='name of the intervals file to be flanked (default: stdin).')
-    parser.add_argument('output', nargs='?',
-                        help='name of the flanked intervals file (default: stdout).')
-    parser.add_argument('-i', '--input-format',
-                        help='file format of input file (useful for reading from stdin).')
-    parser.add_argument('-o', '--output-format',
-                        help='file format of output file (useful for writing to stdout).')
-    parser.add_argument('-1', '--point-one', type=int, default=0,
-                        help='start the 5\' flank relative to the start coordinate')
-    parser.add_argument('-2', '--point-two', type=int, default=0,
-                        help='stop the 5\' flank relative to the start coordinate')
-    parser.add_argument('-3', '--point-three', type=int, default=0,
-                        help='start the 3\' flank relative to the stop coordinate')
-    parser.add_argument('-4', '--point-four', type=int, default=0,
-                        help='stop the 3\' flank relative to the stop coordinate')
-    parser.add_argument('-x', '--orientation', choices=['same', 'opposite'], default='same')
-    parser.set_defaults(func=init_flank)
-    return parser
-
-
-def init_flank(args):
-    assert args.point_one <= args.point_two
-    assert args.point_three <= args.point_four
-    args.output_format = args.input_format if args.output_format is None else args.output_format
-
-    with open_locus_file(args.input, format=args.input_format) as input,\
-            open_locus_file(args.output, 'w', format=args.output_format) as output:
-        flanks = flank(
-            input,
-            point_one=args.point_one,
-            point_two=args.point_two,
-            point_three=args.point_three,
-            point_four=args.point_four,
-            orientation=args.orientation)
-        for five_prime, three_prime in flanks:
-            if five_prime is not None:
-                output.write(five_prime)
-            if three_prime is not None:
-                output.write(three_prime)
-
-
-if __name__ == '__main__':
-    sys.exit(main())
+import sys
+import argparse
+
+from copy import copy
+from typing import Iterable, Iterator
+from lhc.entities.genomic_coordinate import GenomicInterval
+from lhc.io.locus import open_locus_file
+
+
+def flank(intervals: Iterable[GenomicInterval], *, point_one=0, point_two=0, point_three=0, point_four=0, orientation='same') -> Iterator[GenomicInterval]:
+    """
+    Create flanking intervals for each interval in `intervals`.
+    :param intervals: intervals to flank
+    :param five_prime: how much upstream to flank
+    :param three_prime: how much downstream to flank
+    :return: tuple of five- and three-prime flanks
+    """
+    for interval in intervals:
+        strand = interval.strand if orientation == 'same' else '-' if interval.strand == '+' else '+'
+        five_prime_interval = None if point_one == point_two else \
+            GenomicInterval(interval.start + point_one, interval.start + point_two, chromosome=interval.chromosome,
+                            strand=strand, data=copy(interval.data)) if interval.strand == '+' else \
+            GenomicInterval(interval.stop - point_two, interval.stop - point_one, chromosome=interval.chromosome,
+                            strand=strand, data=copy(interval.data))
+        three_prime_interval = None if point_three == point_four else \
+            GenomicInterval(interval.stop + point_three, interval.stop + point_four, chromosome=interval.chromosome,
+                            strand=strand, data=copy(interval.data)) if interval.strand == '+' else \
+            GenomicInterval(interval.start - point_four, interval.start - point_three, chromosome=interval.chromosome,
+                            strand=strand, data=copy(interval.data))
+        if five_prime_interval and five_prime_interval.start >= 0:
+            five_prime_interval.data['gene_id'] += '_5p_flank'
+            five_prime_interval.data['transcript_id'] = five_prime_interval.data['gene_id'] + five_prime_interval.data['transcript_id'][five_prime_interval.data['transcript_id'].find('.'):] if 'transcript_id' in five_prime_interval.data else five_prime_interval.data['gene_id'] + '.1'
+            five_prime_interval.data['exon_id'] = five_prime_interval.data['gene_id'] + five_prime_interval.data['exon_id'][five_prime_interval.data['exon_id'].find('.'):] if 'exon_id' in five_prime_interval.data else five_prime_interval.data['gene_id'] + '.1'
+            five_prime_interval.data['feature'] = '5p_flank'
+        if three_prime_interval and three_prime_interval.start >= 0:
+            three_prime_interval.data['gene_id'] += '_3p_flank'
+            three_prime_interval.data['transcript_id'] = three_prime_interval.data['gene_id'] + three_prime_interval.data['transcript_id'][three_prime_interval.data['transcript_id'].find('.'):] if 'transcript_id' in three_prime_interval.data else three_prime_interval.data['gene_id'] + '.1'
+            three_prime_interval.data['exon_id'] = three_prime_interval.data['gene_id'] + three_prime_interval.data['exon_id'][three_prime_interval.data['exon_id'].find('.'):] if 'exon_id' in three_prime_interval.data else three_prime_interval.data['gene_id'] + '.1'
+            three_prime_interval.data['feature'] = '3p_flank'
+        yield five_prime_interval, three_prime_interval
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser():
+    return define_parser(argparse.ArgumentParser(description=get_description()))
+
+
+def get_description() -> str:
+    return 'Get the intervals flanking the given loci.'
+
+
+def define_parser(parser):
+    parser.add_argument('input', nargs='?',
+                        help='name of the intervals file to be flanked (default: stdin).')
+    parser.add_argument('output', nargs='?',
+                        help='name of the flanked intervals file (default: stdout).')
+    parser.add_argument('-i', '--input-format',
+                        help='file format of input file (useful for reading from stdin).')
+    parser.add_argument('-o', '--output-format', default='gtf',
+                        help='file format of output file (useful for writing to stdout).')
+    parser.add_argument('-1', '--point-one', type=int, default=0,
+                        help='start the 5\' flank relative to the start coordinate')
+    parser.add_argument('-2', '--point-two', type=int, default=0,
+                        help='stop the 5\' flank relative to the start coordinate')
+    parser.add_argument('-3', '--point-three', type=int, default=0,
+                        help='start the 3\' flank relative to the stop coordinate')
+    parser.add_argument('-4', '--point-four', type=int, default=0,
+                        help='stop the 3\' flank relative to the stop coordinate')
+    parser.add_argument('-x', '--orientation', choices=['same', 'opposite'], default='same')
+    parser.set_defaults(func=init_flank)
+    return parser
+
+
+def init_flank(args):
+    assert args.point_one <= args.point_two
+    assert args.point_three <= args.point_four
+    args.output_format = args.input_format if args.output_format is None else args.output_format
+
+    with open_locus_file(args.input, format=args.input_format) as input,\
+            open_locus_file(args.output, 'w', format=args.output_format) as output:
+        flanks = flank(
+            input,
+            point_one=args.point_one,
+            point_two=args.point_two,
+            point_three=args.point_three,
+            point_four=args.point_four,
+            orientation=args.orientation)
+        for five_prime, three_prime in flanks:
+            if five_prime is not None:
+                output.write(five_prime)
+            if three_prime is not None:
+                output.write(three_prime)
+
+
+if __name__ == '__main__':
+    sys.exit(main())
```

### Comparing `lhc-python-2.5.0/lhc/binf/loci/tools/generate.py` & `lhc_python-2.5.1/src/lhc/cli/loci/generate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,50 @@
-import argparse
-
-from typing import Iterator
-from lhc.binf.genomic_coordinate import GenomicInterval
-from lhc.io.fasta import iter_fasta
-from lhc.io.file import open_file
-from lhc.io.locus import open_locus_file
-
-
-def generate_from_fasta(sequences) -> Iterator[GenomicInterval]:
-    pass
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser() -> argparse.ArgumentParser:
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser) -> argparse.ArgumentParser:
-    parser.add_argument('input', nargs='?',
-                        help='input to generate from (default: stdin).')
-    parser.add_argument('output', nargs='?',
-                        help='loci file to extract loci to (default: stdout).')
-    parser.add_argument('-o', '--output-format',
-                        help='file format of output file (useful for writing to stdout).')
-    parser.add_argument('-t', '--type', default='exon',
-                        help='type of locus for file formats that support having a locus type.')
-    parser.set_defaults(func=init_generate)
-    return parser
-
-
-def init_generate(args):
-    with open_file(args.input) as input,\
-            open_locus_file(args.output, 'w', format=args.output_format) as output:
-        for key, header, sequence in iter_fasta(input):
-            output.write(GenomicInterval(0, len(sequence), chromosome=key, data={'gene_id': key, 'feature': args.type}))
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+
+from typing import Iterator
+from lhc.entities.genomic_coordinate import GenomicInterval
+from lhc.io.sequence import open_sequence_file
+from lhc.io.locus import open_locus_file
+
+
+def generate_from_fasta(sequences) -> Iterator[GenomicInterval]:
+    pass
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser() -> argparse.ArgumentParser:
+    return define_parser(argparse.ArgumentParser(description=get_description()))
+
+
+def get_description() -> str:
+    return 'Generate loci matching the given sequences'
+
+
+def define_parser(parser) -> argparse.ArgumentParser:
+    parser.add_argument('input', nargs='?',
+                        help='sequences file (default: stdin).')
+    parser.add_argument('output', nargs='?',
+                        help='loci file to extract loci to (default: stdout).')
+    parser.add_argument('-i', '--input-format',
+                        help='file format of input file (useful for reading from stdin).')
+    parser.add_argument('-o', '--output-format', default='gtf',
+                        help='file format of output file (useful for writing to stdout).')
+    parser.add_argument('-t', '--type', default='exon',
+                        help='type of loci for file formats that support having a loci type.')
+    parser.set_defaults(func=init_generate)
+    return parser
+
+
+def init_generate(args):
+    with open_sequence_file(args.input) as sequences,\
+        open_locus_file(args.output, 'w', format=args.output_format) as output\
+    :
+        for sequence in sequences:
+            output.write(GenomicInterval(0, len(sequence), chromosome=sequence.identifier, data={'gene_id': sequence.identifier, 'feature': args.type}))
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `lhc-python-2.5.0/lhc/binf/misc/tools/cs_to_table.py` & `lhc_python-2.5.1/src/lhc/cli/alignments/cs_to_table.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-import argparse
-import sys
-
-from typing import List
-
-
-def cs_to_table(cs) -> List[List[str]]:
-    return [[]]
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser() -> argparse.ArgumentParser:
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-    parser.add_argument('cs')
-    parser.set_defaults(func=init_cs_to_table)
-    return parser
-
-
-def init_cs_to_table(args: argparse.Namespace):
-    sys.stdout.write('\n'.join('\t'.join(line) for line in cs_to_table(args.cs)))
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+import sys
+
+from typing import List
+
+
+def cs_to_table(cs) -> List[List[str]]:
+    return [[]]
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser() -> argparse.ArgumentParser:
+    return define_parser(argparse.ArgumentParser(get_description()))
+
+
+def get_description() -> str:
+    return 'Convert a CS string (CIGAR string al la minimap) to a table'
+
+
+def define_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
+    parser.add_argument('cs')
+    parser.set_defaults(func=init_cs_to_table)
+    return parser
+
+
+def init_cs_to_table(args: argparse.Namespace):
+    sys.stdout.write('\n'.join('\t'.join(line) for line in cs_to_table(args.cs)))
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `lhc-python-2.5.0/lhc/binf/sequence/__init__.py` & `lhc_python-2.5.1/src/lhc/cli/sequences/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-class Sequence:
-    def __init__(self, identifier, sequence, *, data=None):
-        self.identifier = identifier
-        self.sequence = sequence
-        self.data = {} if data is None else data
-
-    def __str__(self):
-        return self.sequence
-
-    def __iter__(self):
-        return iter(self.sequence)
-
-    def __len__(self):
-        return len(self.sequence)
-
-    def __getitem__(self, item):
-        return self.sequence[item]
-
-
-def translate(sequence: str) -> str:
-    from lhc.binf.genetic_code import GeneticCodes
-    codes = GeneticCodes()
-    return codes.translate(sequence)
+class Sequence:
+    def __init__(self, identifier, sequence, *, data=None):
+        self.identifier = identifier
+        self.sequence = sequence
+        self.data = {} if data is None else data
+
+    def __str__(self):
+        return self.sequence
+
+    def __iter__(self):
+        return iter(self.sequence)
+
+    def __len__(self):
+        return len(self.sequence)
+
+    def __getitem__(self, item):
+        return self.sequence[item]
+
+
+def translate(sequence: str) -> str:
+    from lhc.misc.genetic_code import GeneticCodes
+    codes = GeneticCodes()
+    return codes.translate(sequence)
```

### Comparing `lhc-python-2.5.0/lhc/binf/sequence/dicodonshuffle.py` & `lhc_python-2.5.1/src/lhc/entities/sequence/dicodonshuffle.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,493 +1,493 @@
-#!/usr/bin/python
-
-# Converted from the C. Burge and L. Katz C version to Python
-
-import numpy
-import random
-
-from lhc.io.fasta import iter_fasta
-
-
-class NonStandardException(Exception):
-    def __init__(self):
-        Exception.__init__(self)
-
-
-class InvalidLengthException(Exception):
-    def __init__(self, l):
-        Exception.__init__(self)
-        self.l = l
-
-
-class CodonPair:
-    def __init__(self):
-        self.aa = None
-        self.codon1 = None
-        self.codon2 = None
-
-
-class OrfData:
-    def __init__(self):
-        self.name = None
-        self.start = None
-        self.stop = None
-        self.strand = None
-
-
-def main(argv):
-    orfnum = 0
-    pos = 0
-    extcodonflag = False
-    codonfname = ''
-    seedval = 0
-    max_seq = 1
-
-    orfs = [OrfData() for x in range(max_seq)]
-
-    if len(argv) < 3 or len(argv) > 6:
-        usage(argv[0])
-
-    infname = argv[1]
-
-    for i in range(3, len(argv)):
-        if argv[i] == "-f":
-            extcodonflag = True
-            codonfname = argv[i + 1]
-        if argv[i] == "-r":
-            seedval = int(argv[i + 1])
-
-    if seedval > 0:
-        random.seed(seedval)
-
-    sys.stderr.write("reading sequence ")
-
-    seqs = list(iter_fasta(infname))
-    acc, seq = seqs[0]
-
-    sys.stderr.write(" seqlen %d bp\n" % len(seq))
-
-    try:
-        res = shuffle(seq, codonfname)
-        print(res)
-    except NonStandardException:
-        sys.stderr.write("ERROR : Non-standard base found in file\n")
-    except InvalidLengthException as e:
-        sys.stderr.write("ERROR : len(seq) %d mod 3 = %d\n" % (e.l, e.l % 3))
-
-
-# /* fprintf(stderr,"\n\ndone\n\n"); */
-
-# /****************************************************************************/
-
-def usage(out_name):
-    sys.stdout.write("\nusage: %s seqfile outfile [-r seedval] [-f codonfile]\n" % out_name)
-    sys.stdout.write("\n       seqfile   : sequence file in (pseudo-)GenBank format\n")
-    sys.stdout.write("\n       outfile   : file for final output\n");
-    sys.stdout.write("\n       seedval   : value to use in seeding random number generator\n");
-    sys.stdout.write("\n       codonfile : list of codon frequencies to use (optional)");
-    sys.stdout.write("\n                   Format: XYZ f (64 lines)\n\n");
-    sys.exit(0)
-
-
-# /****************************************************************************/
-
-def ribosome(a, b, c):
-    if a in [0, 'A', 'a']:
-        if b in [0, 'A', 'a']:
-            if c in [0, 'A', 'a'] or c in [2, 'G', 'g']:
-                return 8
-            else:
-                return 11
-        if b in [1, 'C', 'c']:
-            return 16
-        if b in [2, 'G', 'g']:
-            if c in [0, 'A', 'a'] or c in [2, 'G', 'g']:
-                return 14
-            else:
-                return 15
-        if b in [3, 'T', 't', 'U', 'u']:
-            if c in [2, 'G', 'g']:
-                return 10
-            else:
-                return 7
-
-    if a in [1, 'C', 'c']:
-        if b in [0, 'A', 'a']:
-            if c in [0, 'A', 'a'] or c in [2, 'G', 'g']:
-                return 13
-            else:
-                return 6
-        if b in [1, 'C', 'c']:
-            return 12
-        if b in [2, 'G', 'g']:
-            return 14
-        if b in [3, 'T', 't', 'U', 'u']:
-            return 9
-
-    if a in [2, 'G', 'g']:
-        if b in [0, 'A', 'a']:
-            if c in [0, 'A', 'a'] or c in [2, 'G', 'g']:
-                return 3
-            else:
-                return 2
-        if b in [1, 'C', 'c']:
-            return 0
-        if b in [2, 'G', 'g']:
-            return 5
-        if b in [3, 'T', 't', 'U', 'u']:
-            return 17
-
-    if a in [3, 'T', 't', 'U', 'u']:
-        if b in [0, 'A', 'a']:
-            if c in [0, 'A', 'a'] or c in [2, 'G', 'g']:
-                return 20
-            else:
-                return 19
-        if b in [1, 'C', 'c']:
-            return 15
-        if b in [2, 'G', 'g']:
-            if c in [0, 'A', 'a']:
-                return 20
-            if c in [2, 'G', 'g']:
-                return 18
-            if c in [1, 'C', 'c'] or c in [3, 'T', 't', 'U', 'u']:
-                return 1
-        if b in [3, 'T', 't', 'U', 'u']:
-            if c in [0, 'A', 'a'] or c in [2, 'G', 'g']:
-                return 9
-            else:
-                return 4
-    return 21
-
-
-def dcshuffle(seq, codonfname=''):
-    MAX_NUM_SEQ = 1
-
-    aacodon = [None for x in range(22)]
-    nextaacodon = [None for x in range(22)]
-    swapflag = [None for x in range(22)]
-
-    ntrueswap = 0
-
-    shuffledaa = numpy.zeros(20, dtype=numpy.int32)
-
-    tmpcodon = [None for x in range(4)]
-
-    naa = numpy.zeros(22, dtype=numpy.int32)
-
-    s = numpy.zeros(6, dtype=numpy.int32)  # next 6 bases : int form
-    c = [None for x in range(6)]
-
-    mc = numpy.zeros((6, 4), dtype=numpy.int32)  # base count in codon pos. 1-6
-    md = numpy.zeros(6, dtype=numpy.float32)  # demoninator for mc
-    mf = numpy.zeros((6, 4), dtype=numpy.float32)
-    mF = numpy.zeros((6, 4), dtype=numpy.float32)  # mf multiplied by 100
-
-    dic = numpy.zeros((3, 6, 4, 4), dtype=numpy.int32)  # dicount at [p1,p2] of
-    did = numpy.zeros((3, 6), dtype=numpy.float32)
-    dif = numpy.zeros((3, 6, 4, 4), dtype=numpy.float32)
-
-    tric = numpy.zeros((3, 4, 4, 4), dtype=numpy.int32)  # tricount at 123,234,345
-    trid = numpy.zeros(3, dtype=numpy.float32)
-    trif = numpy.zeros((3, 4, 4, 4), dtype=numpy.float32)
-
-    codonc = numpy.zeros((4, 4, 4), dtype=numpy.int32)  # codon count
-    codond = 0
-    codonF = numpy.zeros((4, 4, 4), dtype=numpy.float32)  # frequency multiplied by 100
-    codstemF = numpy.zeros((4, 4), dtype=numpy.float32)  # first two codon positons
-
-    cumcodonF = numpy.zeros((4, 4, 4), dtype=numpy.float32)
-    cumF = numpy.zeros((4, 4, 4), dtype=numpy.float32)
-
-    hexc = numpy.zeros((4, 4, 4, 4, 4, 4), dtype=numpy.int32)
-    hexd = 0.
-    hexf = numpy.zeros((4, 4, 4, 4, 4, 4), dtype=numpy.float32)
-
-    aac = numpy.zeros(22, dtype=numpy.int32)  # 20 = stop, 21 = bogus letter
-    aad = 0.
-    aaf = numpy.zeros(22, dtype=numpy.float32)
-
-    rho = numpy.zeros((3, 6, 4, 4), dtype=numpy.float32)  # rho_ij at [p1,p2]
-
-    nstdflag = 0;
-
-    seq_num = numpy.array([nuc2num(base) for base in seq], dtype=numpy.int32)
-
-    if len(seq) % 3 != 0:
-        raise InvalidLengthException(len(seq))
-
-    for pos in range(0, len(seq_num) - 3, 3):
-
-        s = seq_num[pos:pos + 3]
-        if pos + 6 <= len(seq_num):
-            s = seq_num[pos:pos + 6]
-
-        aa = ribosome(s[0], s[1], s[2])
-        aac[aa] += 1
-        aad += 1
-
-        if aa == 20:
-            pass
-        if aa == 21:
-            nstdflag = 1
-
-        if s[0] < 4 and s[1] < 4 and s[2] < 4:
-            codonc[s[0], s[1], s[2]] += 1
-            codond += 1
-
-        for i in range(6):
-            if s[i] < 4:
-                mc[i, s[i]] += 1
-                md[i] += 1
-
-        for i in range(3):
-            for j in range(i + 1, 6):
-                if s[i] < 4 and s[j] < 4:
-                    dic[i, j, s[i], s[j]] += 1
-                    did[i, j] += 1
-
-        for i in range(3):
-            if s[i] < 4 and s[i + 1] < 4 and s[i + 2] < 4:
-                tric[i, s[i], s[i + 1], s[i + 2]] += 1
-                trid[i] += 1
-
-        if s[0] < 4 and s[1] < 4 and s[2] < 4 and s[3] < 4 and s[4] < 4 and s[5] < 4:
-            hexc[s[0], s[1], s[2], s[3], s[4], s[5]] += 1
-            hexd += 1
-
-    if nstdflag:
-        raise NonStandardException()
-
-    for j in range(4):
-        mf[:, j] = mc[:, j] / md
-    mF = 100 * mf
-
-    for i in range(3):
-        for j in range(6):
-            for k in range(4):
-                for l in range(4):
-                    dif[i, j, k, l] = dic[i, j, k, l] / did[i, j]
-                    rho[i, j, k, l] = dif[i, j, k, l] / mf[i, k] * mf[j, l]
-                    if i == 0 and j == 1:
-                        codstemF[k, l] = 100 * dif[i, j, k, l]
-
-    for i in range(3):
-        for j in range(4):
-            for k in range(4):
-                for l in range(4):
-                    if i == 0:
-                        codonF[j, k, l] = 100 * codonc[j, k, l] / codond
-                    trif[i, j, k, l] = tric[i, j, k, l] / trid[i]
-
-    hexf = hexc / hexd
-    aaf = aac / aad
-
-    res = []
-
-    for i in range(22):
-        if aac[i] > 0:
-            aacodon[i] = aac[i] * ['']
-            nextaacodon[i] = aac[i] * ['']
-            swapflag[i] = aac[i] * ['']
-        else:
-            aacodon[i] = None
-            nextaacodon[i] = None
-
-    for j in range(0, len(seq) - 3, 3):
-        aa = ribosome(seq[j], seq[j + 1], seq[j + 2])
-        # print type(aacodon[aa])
-        # print type(int(naa[aa]))
-        # print aacodon[aa][int(naa[aa])]
-        # sys.exit(1)
-        aacodon[aa][int(naa[aa])] = seq[j:j + 3]
-        nextaa = ribosome(seq[j + 3], seq[j + 4], seq[j + 5])
-        nextaacodon[aa][int(naa[aa])] = seq[j + 3:j + 6]
-        naa[aa] += 1
-
-    for i in range(20):
-        shuffledaa[i] = i
-
-    for j in range(20):
-        r = 20 - j
-        k = int(r * random.random())
-
-        i = shuffledaa[j]
-        shuffledaa[j] = shuffledaa[j + k]
-        shuffledaa[j + k] = i
-
-    # now shuffle the codons for each amino acid
-
-    for h in range(20):  # amino acid i
-        i = int(shuffledaa[h])
-
-        for j in range(aac[i]):  # codon j
-            r = aac[i] - j
-            k = int(r * random.random())
-
-            # consider swapping aacodon[i][j] with aacodon[i][j+k])
-
-            # if codons are identical or if first nucleotides differ, do nothing
-
-            if aacodon[i][j] == aacodon[i][j + k] or aacodon[i][j][0] != aacodon[i][j + k][0]:
-                swapflag[i][j] = 1  # count as a swap */
-            else:
-
-                # if +1 nucleotides are identical, make swap
-
-                if nextaacodon[i][j][0] == nextaacodon[i][j + k][0]:
-                    aacodon[i][j], aacodon[i][j + k] = aacodon[i][j + k], aacodon[i][j]
-                    swapflag[i][j] = 1  # count as a swap
-                    ntrueswap += 1
-                else:
-                    # define dinucleotide pair, identify reciprocal codon pairs
-                    # choose one at random, and make swap and reciprocal swap
-                    W = aacodon[i][j][2]
-                    X = nextaacodon[i][j][0]
-
-                    Y = aacodon[i][j + k][2]
-                    Z = nextaacodon[i][j + k][0]
-
-                    # if WX after YZ alphabetically, then swap WX, YZ dinucleotides
-
-                    if W > Y or (W == Y and X > Z):
-                        W, Y = Y, W
-                        X, Z = Z, X
-
-                    # Reciprocal dinucleotide pair: WZ, YX
-
-                    # Search through all remaining unswapped dicodons, identify reciprocal pairs
-
-                    nreciprocals = 0
-                    for ii in range(20):  # aa ii\
-                        for jj in range(aac[ii]):
-                            if swapflag[ii][jj]:  # exclude previously swapped codons
-                                pass
-                            else:
-                                for kk in range(jj + 1, aac[ii]):
-                                    if aacodon[ii][jj][0] != aacodon[ii][kk][0]:  # exclude L2/L4, S2/S4 cases
-                                        pass
-                                    else:
-                                        R = aacodon[ii][jj][2]
-                                        S = nextaacodon[ii][jj][0]
-                                        T = aacodon[ii][kk][2]
-                                        U = nextaacodon[ii][kk][0]
-
-                                        if (R == W and S == Z and T == Y and U == X) or \
-                                                (T == W and U == Z and R == Y and S == X):  # if reciprocal
-                                            nreciprocals += 1
-
-                    reciprocals = None
-
-                    if nreciprocals > 0:
-                        reciprocals = [CodonPair() for x in range(nreciprocals)]
-
-                        recipnum = 0
-
-                        for ii in range(20):  # aa ii
-                            for jj in range(aac[ii]):
-                                if swapflag[ii][jj]:  # exclude previously swapped codons
-                                    pass
-                                else:
-                                    for kk in range(jj + 1, aac[ii]):
-                                        if aacodon[ii][jj][0] != aacodon[ii][kk][0]:  # exlude L2/L4, S2/S4 cases
-                                            pass
-                                        else:
-                                            R = aacodon[ii][jj][2]
-                                            S = nextaacodon[ii][jj][0]
-                                            T = aacodon[ii][kk][2]
-                                            U = nextaacodon[ii][kk][0]
-                                            if (R == W and S == Z and T == Y and U == X) or \
-                                                    (T == W and U == Z and R == Y and S == X):  # if reciprocal
-                                                reciprocals[recipnum].aa = ii
-                                                reciprocals[recipnum].codon1 = jj
-                                                reciprocals[recipnum].codon2 = kk;
-                                                recipnum += 1
-
-                        if nreciprocals > 0:
-                            recipnum = int(nreciprocals * random.random())
-
-                            ii = reciprocals[recipnum].aa
-                            jj = reciprocals[recipnum].codon1
-                            kk = reciprocals[recipnum].codon2
-
-                            # swap codons, swap reciprocal codons, update swapflags
-
-                            aacodon[i][j], aacodon[i][j + k] = aacodon[i][j + k], aacodon[i][j]
-
-                            swapflag[i][j] = 1  # count as a swap
-                            ntrueswap += 1
-
-                            aacodon[ii][jj], aacodon[ii][kk] = aacodon[ii][kk], aacodon[ii][jj]
-
-                            swapflag[ii][jj] = 1  # count as a swap
-                            ntrueswap += 1
-
-    naa = numpy.zeros(22, dtype=numpy.int32)
-
-    if codonfname:
-        with open(codonfname, encoding='utf-8') as codonfp:
-            cumF = 0.0
-            cumcodonF = numpy.zeros((4, 4, 4), numpy.float32)
-            for i in range(4):
-                for j in range(4):
-                    for k in range(4):
-                        fscanf(codonfp, "%s %f", abc, f);
-                        codonF[i, j, k] = f
-                        cumF += f
-                    cumcodonF[i, j, k] = cumF
-
-    for j in range(0, len(seq) - 3, 3):
-        aa = ribosome(seq[j], seq[j + 1], seq[j + 2])
-
-        if len(codonfname) > 0:
-            codonflag = 0
-
-            while not codonflag:
-                r = 100 * random.random()
-
-                for i in range(4):
-                    for j in range(4):
-                        for k in range(4):
-                            if r < cumcodonF[i, j, k]:
-                                break
-
-                aa2 = ribosome(nuc2num(i), nuc2num(j), nuc2num(k));
-
-                if (aa2 == aa):
-                    codonflag = 1
-
-                res.append("%c%c%c" % (nuc2num(i), nuc2num(j), nuc2num(k)))
-
-        else:
-            if aa == 20:
-                res.append('tga')
-            else:
-                res.append("%s" % aacodon[aa][int(naa[aa])])
-
-        if j % 60 > 57:
-            res.append('\n')
-
-        naa[aa] += 1
-
-    res.append(seq[-3:])
-
-    return ''.join(res)
-
-
-_alphabet = 'acgun'
-alphabet = {'a': 0, 'c': 1, 'g': 2, 't': 3, 'u': 3, 'n': 4}
-
-
-def nuc2num(nuc):
-    if nuc in alphabet:
-        return alphabet[nuc]
-    return 4
-
-
-aa_alphabet = 'ACDEFGHIKLMNPQRSTVWYxX'
-
-
-if __name__ == '__main__':
-    import sys
-
-    sys.exit(main(sys.argv))
+#!/usr/bin/python
+
+# Converted from the C. Burge and L. Katz C version to Python
+
+import numpy
+import random
+
+from lhc.io.sequence import iter_sequences
+
+
+class NonStandardException(Exception):
+    def __init__(self):
+        Exception.__init__(self)
+
+
+class InvalidLengthException(Exception):
+    def __init__(self, l):
+        Exception.__init__(self)
+        self.l = l
+
+
+class CodonPair:
+    def __init__(self):
+        self.aa = None
+        self.codon1 = None
+        self.codon2 = None
+
+
+class OrfData:
+    def __init__(self):
+        self.name = None
+        self.start = None
+        self.stop = None
+        self.strand = None
+
+
+def main(argv):
+    orfnum = 0
+    pos = 0
+    extcodonflag = False
+    codonfname = ''
+    seedval = 0
+    max_seq = 1
+
+    orfs = [OrfData() for x in range(max_seq)]
+
+    if len(argv) < 3 or len(argv) > 6:
+        usage(argv[0])
+
+    infname = argv[1]
+
+    for i in range(3, len(argv)):
+        if argv[i] == "-f":
+            extcodonflag = True
+            codonfname = argv[i + 1]
+        if argv[i] == "-r":
+            seedval = int(argv[i + 1])
+
+    if seedval > 0:
+        random.seed(seedval)
+
+    sys.stderr.write("reading sequences ")
+
+    seqs = list(iter_sequences(infname))
+    acc, seq = seqs[0]
+
+    sys.stderr.write(" seqlen %d bp\n" % len(seq))
+
+    try:
+        res = shuffle(seq, codonfname)
+        print(res)
+    except NonStandardException:
+        sys.stderr.write("ERROR : Non-standard base found in file\n")
+    except InvalidLengthException as e:
+        sys.stderr.write("ERROR : len(seq) %d mod 3 = %d\n" % (e.l, e.l % 3))
+
+
+# /* fprintf(stderr,"\n\ndone\n\n"); */
+
+# /****************************************************************************/
+
+def usage(out_name):
+    sys.stdout.write("\nusage: %s seqfile outfile [-r seedval] [-f codonfile]\n" % out_name)
+    sys.stdout.write("\n       seqfile   : sequences file in (pseudo-)GenBank format\n")
+    sys.stdout.write("\n       outfile   : file for final output\n");
+    sys.stdout.write("\n       seedval   : value to use in seeding random number generator\n");
+    sys.stdout.write("\n       codonfile : list of codon frequencies to use (optional)");
+    sys.stdout.write("\n                   Format: XYZ f (64 lines)\n\n");
+    sys.exit(0)
+
+
+# /****************************************************************************/
+
+def ribosome(a, b, c):
+    if a in [0, 'A', 'a']:
+        if b in [0, 'A', 'a']:
+            if c in [0, 'A', 'a'] or c in [2, 'G', 'g']:
+                return 8
+            else:
+                return 11
+        if b in [1, 'C', 'c']:
+            return 16
+        if b in [2, 'G', 'g']:
+            if c in [0, 'A', 'a'] or c in [2, 'G', 'g']:
+                return 14
+            else:
+                return 15
+        if b in [3, 'T', 't', 'U', 'u']:
+            if c in [2, 'G', 'g']:
+                return 10
+            else:
+                return 7
+
+    if a in [1, 'C', 'c']:
+        if b in [0, 'A', 'a']:
+            if c in [0, 'A', 'a'] or c in [2, 'G', 'g']:
+                return 13
+            else:
+                return 6
+        if b in [1, 'C', 'c']:
+            return 12
+        if b in [2, 'G', 'g']:
+            return 14
+        if b in [3, 'T', 't', 'U', 'u']:
+            return 9
+
+    if a in [2, 'G', 'g']:
+        if b in [0, 'A', 'a']:
+            if c in [0, 'A', 'a'] or c in [2, 'G', 'g']:
+                return 3
+            else:
+                return 2
+        if b in [1, 'C', 'c']:
+            return 0
+        if b in [2, 'G', 'g']:
+            return 5
+        if b in [3, 'T', 't', 'U', 'u']:
+            return 17
+
+    if a in [3, 'T', 't', 'U', 'u']:
+        if b in [0, 'A', 'a']:
+            if c in [0, 'A', 'a'] or c in [2, 'G', 'g']:
+                return 20
+            else:
+                return 19
+        if b in [1, 'C', 'c']:
+            return 15
+        if b in [2, 'G', 'g']:
+            if c in [0, 'A', 'a']:
+                return 20
+            if c in [2, 'G', 'g']:
+                return 18
+            if c in [1, 'C', 'c'] or c in [3, 'T', 't', 'U', 'u']:
+                return 1
+        if b in [3, 'T', 't', 'U', 'u']:
+            if c in [0, 'A', 'a'] or c in [2, 'G', 'g']:
+                return 9
+            else:
+                return 4
+    return 21
+
+
+def dcshuffle(seq, codonfname=''):
+    MAX_NUM_SEQ = 1
+
+    aacodon = [None for x in range(22)]
+    nextaacodon = [None for x in range(22)]
+    swapflag = [None for x in range(22)]
+
+    ntrueswap = 0
+
+    shuffledaa = numpy.zeros(20, dtype=numpy.int32)
+
+    tmpcodon = [None for x in range(4)]
+
+    naa = numpy.zeros(22, dtype=numpy.int32)
+
+    s = numpy.zeros(6, dtype=numpy.int32)  # next 6 bases : int form
+    c = [None for x in range(6)]
+
+    mc = numpy.zeros((6, 4), dtype=numpy.int32)  # base count in codon pos. 1-6
+    md = numpy.zeros(6, dtype=numpy.float32)  # demoninator for mc
+    mf = numpy.zeros((6, 4), dtype=numpy.float32)
+    mF = numpy.zeros((6, 4), dtype=numpy.float32)  # mf multiplied by 100
+
+    dic = numpy.zeros((3, 6, 4, 4), dtype=numpy.int32)  # dicount at [p1,p2] of
+    did = numpy.zeros((3, 6), dtype=numpy.float32)
+    dif = numpy.zeros((3, 6, 4, 4), dtype=numpy.float32)
+
+    tric = numpy.zeros((3, 4, 4, 4), dtype=numpy.int32)  # tricount at 123,234,345
+    trid = numpy.zeros(3, dtype=numpy.float32)
+    trif = numpy.zeros((3, 4, 4, 4), dtype=numpy.float32)
+
+    codonc = numpy.zeros((4, 4, 4), dtype=numpy.int32)  # codon count
+    codond = 0
+    codonF = numpy.zeros((4, 4, 4), dtype=numpy.float32)  # frequency multiplied by 100
+    codstemF = numpy.zeros((4, 4), dtype=numpy.float32)  # first two codon positons
+
+    cumcodonF = numpy.zeros((4, 4, 4), dtype=numpy.float32)
+    cumF = numpy.zeros((4, 4, 4), dtype=numpy.float32)
+
+    hexc = numpy.zeros((4, 4, 4, 4, 4, 4), dtype=numpy.int32)
+    hexd = 0.
+    hexf = numpy.zeros((4, 4, 4, 4, 4, 4), dtype=numpy.float32)
+
+    aac = numpy.zeros(22, dtype=numpy.int32)  # 20 = stop, 21 = bogus letter
+    aad = 0.
+    aaf = numpy.zeros(22, dtype=numpy.float32)
+
+    rho = numpy.zeros((3, 6, 4, 4), dtype=numpy.float32)  # rho_ij at [p1,p2]
+
+    nstdflag = 0;
+
+    seq_num = numpy.array([nuc2num(base) for base in seq], dtype=numpy.int32)
+
+    if len(seq) % 3 != 0:
+        raise InvalidLengthException(len(seq))
+
+    for pos in range(0, len(seq_num) - 3, 3):
+
+        s = seq_num[pos:pos + 3]
+        if pos + 6 <= len(seq_num):
+            s = seq_num[pos:pos + 6]
+
+        aa = ribosome(s[0], s[1], s[2])
+        aac[aa] += 1
+        aad += 1
+
+        if aa == 20:
+            pass
+        if aa == 21:
+            nstdflag = 1
+
+        if s[0] < 4 and s[1] < 4 and s[2] < 4:
+            codonc[s[0], s[1], s[2]] += 1
+            codond += 1
+
+        for i in range(6):
+            if s[i] < 4:
+                mc[i, s[i]] += 1
+                md[i] += 1
+
+        for i in range(3):
+            for j in range(i + 1, 6):
+                if s[i] < 4 and s[j] < 4:
+                    dic[i, j, s[i], s[j]] += 1
+                    did[i, j] += 1
+
+        for i in range(3):
+            if s[i] < 4 and s[i + 1] < 4 and s[i + 2] < 4:
+                tric[i, s[i], s[i + 1], s[i + 2]] += 1
+                trid[i] += 1
+
+        if s[0] < 4 and s[1] < 4 and s[2] < 4 and s[3] < 4 and s[4] < 4 and s[5] < 4:
+            hexc[s[0], s[1], s[2], s[3], s[4], s[5]] += 1
+            hexd += 1
+
+    if nstdflag:
+        raise NonStandardException()
+
+    for j in range(4):
+        mf[:, j] = mc[:, j] / md
+    mF = 100 * mf
+
+    for i in range(3):
+        for j in range(6):
+            for k in range(4):
+                for l in range(4):
+                    dif[i, j, k, l] = dic[i, j, k, l] / did[i, j]
+                    rho[i, j, k, l] = dif[i, j, k, l] / mf[i, k] * mf[j, l]
+                    if i == 0 and j == 1:
+                        codstemF[k, l] = 100 * dif[i, j, k, l]
+
+    for i in range(3):
+        for j in range(4):
+            for k in range(4):
+                for l in range(4):
+                    if i == 0:
+                        codonF[j, k, l] = 100 * codonc[j, k, l] / codond
+                    trif[i, j, k, l] = tric[i, j, k, l] / trid[i]
+
+    hexf = hexc / hexd
+    aaf = aac / aad
+
+    res = []
+
+    for i in range(22):
+        if aac[i] > 0:
+            aacodon[i] = aac[i] * ['']
+            nextaacodon[i] = aac[i] * ['']
+            swapflag[i] = aac[i] * ['']
+        else:
+            aacodon[i] = None
+            nextaacodon[i] = None
+
+    for j in range(0, len(seq) - 3, 3):
+        aa = ribosome(seq[j], seq[j + 1], seq[j + 2])
+        # print type(aacodon[aa])
+        # print type(int(naa[aa]))
+        # print aacodon[aa][int(naa[aa])]
+        # sys.exit(1)
+        aacodon[aa][int(naa[aa])] = seq[j:j + 3]
+        nextaa = ribosome(seq[j + 3], seq[j + 4], seq[j + 5])
+        nextaacodon[aa][int(naa[aa])] = seq[j + 3:j + 6]
+        naa[aa] += 1
+
+    for i in range(20):
+        shuffledaa[i] = i
+
+    for j in range(20):
+        r = 20 - j
+        k = int(r * random.random())
+
+        i = shuffledaa[j]
+        shuffledaa[j] = shuffledaa[j + k]
+        shuffledaa[j + k] = i
+
+    # now shuffle the codons for each amino acid
+
+    for h in range(20):  # amino acid i
+        i = int(shuffledaa[h])
+
+        for j in range(aac[i]):  # codon j
+            r = aac[i] - j
+            k = int(r * random.random())
+
+            # consider swapping aacodon[i][j] with aacodon[i][j+k])
+
+            # if codons are identical or if first nucleotides differ, do nothing
+
+            if aacodon[i][j] == aacodon[i][j + k] or aacodon[i][j][0] != aacodon[i][j + k][0]:
+                swapflag[i][j] = 1  # count as a swap */
+            else:
+
+                # if +1 nucleotides are identical, make swap
+
+                if nextaacodon[i][j][0] == nextaacodon[i][j + k][0]:
+                    aacodon[i][j], aacodon[i][j + k] = aacodon[i][j + k], aacodon[i][j]
+                    swapflag[i][j] = 1  # count as a swap
+                    ntrueswap += 1
+                else:
+                    # define dinucleotide pair, identify reciprocal codon pairs
+                    # choose one at random, and make swap and reciprocal swap
+                    W = aacodon[i][j][2]
+                    X = nextaacodon[i][j][0]
+
+                    Y = aacodon[i][j + k][2]
+                    Z = nextaacodon[i][j + k][0]
+
+                    # if WX after YZ alphabetically, then swap WX, YZ dinucleotides
+
+                    if W > Y or (W == Y and X > Z):
+                        W, Y = Y, W
+                        X, Z = Z, X
+
+                    # Reciprocal dinucleotide pair: WZ, YX
+
+                    # Search through all remaining unswapped dicodons, identify reciprocal pairs
+
+                    nreciprocals = 0
+                    for ii in range(20):  # aa ii\
+                        for jj in range(aac[ii]):
+                            if swapflag[ii][jj]:  # exclude previously swapped codons
+                                pass
+                            else:
+                                for kk in range(jj + 1, aac[ii]):
+                                    if aacodon[ii][jj][0] != aacodon[ii][kk][0]:  # exclude L2/L4, S2/S4 cases
+                                        pass
+                                    else:
+                                        R = aacodon[ii][jj][2]
+                                        S = nextaacodon[ii][jj][0]
+                                        T = aacodon[ii][kk][2]
+                                        U = nextaacodon[ii][kk][0]
+
+                                        if (R == W and S == Z and T == Y and U == X) or \
+                                                (T == W and U == Z and R == Y and S == X):  # if reciprocal
+                                            nreciprocals += 1
+
+                    reciprocals = None
+
+                    if nreciprocals > 0:
+                        reciprocals = [CodonPair() for x in range(nreciprocals)]
+
+                        recipnum = 0
+
+                        for ii in range(20):  # aa ii
+                            for jj in range(aac[ii]):
+                                if swapflag[ii][jj]:  # exclude previously swapped codons
+                                    pass
+                                else:
+                                    for kk in range(jj + 1, aac[ii]):
+                                        if aacodon[ii][jj][0] != aacodon[ii][kk][0]:  # exlude L2/L4, S2/S4 cases
+                                            pass
+                                        else:
+                                            R = aacodon[ii][jj][2]
+                                            S = nextaacodon[ii][jj][0]
+                                            T = aacodon[ii][kk][2]
+                                            U = nextaacodon[ii][kk][0]
+                                            if (R == W and S == Z and T == Y and U == X) or \
+                                                    (T == W and U == Z and R == Y and S == X):  # if reciprocal
+                                                reciprocals[recipnum].aa = ii
+                                                reciprocals[recipnum].codon1 = jj
+                                                reciprocals[recipnum].codon2 = kk;
+                                                recipnum += 1
+
+                        if nreciprocals > 0:
+                            recipnum = int(nreciprocals * random.random())
+
+                            ii = reciprocals[recipnum].aa
+                            jj = reciprocals[recipnum].codon1
+                            kk = reciprocals[recipnum].codon2
+
+                            # swap codons, swap reciprocal codons, update swapflags
+
+                            aacodon[i][j], aacodon[i][j + k] = aacodon[i][j + k], aacodon[i][j]
+
+                            swapflag[i][j] = 1  # count as a swap
+                            ntrueswap += 1
+
+                            aacodon[ii][jj], aacodon[ii][kk] = aacodon[ii][kk], aacodon[ii][jj]
+
+                            swapflag[ii][jj] = 1  # count as a swap
+                            ntrueswap += 1
+
+    naa = numpy.zeros(22, dtype=numpy.int32)
+
+    if codonfname:
+        with open(codonfname, encoding='utf-8') as codonfp:
+            cumF = 0.0
+            cumcodonF = numpy.zeros((4, 4, 4), numpy.float32)
+            for i in range(4):
+                for j in range(4):
+                    for k in range(4):
+                        fscanf(codonfp, "%s %f", abc, f);
+                        codonF[i, j, k] = f
+                        cumF += f
+                    cumcodonF[i, j, k] = cumF
+
+    for j in range(0, len(seq) - 3, 3):
+        aa = ribosome(seq[j], seq[j + 1], seq[j + 2])
+
+        if len(codonfname) > 0:
+            codonflag = 0
+
+            while not codonflag:
+                r = 100 * random.random()
+
+                for i in range(4):
+                    for j in range(4):
+                        for k in range(4):
+                            if r < cumcodonF[i, j, k]:
+                                break
+
+                aa2 = ribosome(nuc2num(i), nuc2num(j), nuc2num(k));
+
+                if (aa2 == aa):
+                    codonflag = 1
+
+                res.append("%c%c%c" % (nuc2num(i), nuc2num(j), nuc2num(k)))
+
+        else:
+            if aa == 20:
+                res.append('tga')
+            else:
+                res.append("%s" % aacodon[aa][int(naa[aa])])
+
+        if j % 60 > 57:
+            res.append('\n')
+
+        naa[aa] += 1
+
+    res.append(seq[-3:])
+
+    return ''.join(res)
+
+
+_alphabet = 'acgun'
+alphabet = {'a': 0, 'c': 1, 'g': 2, 't': 3, 'u': 3, 'n': 4}
+
+
+def nuc2num(nuc):
+    if nuc in alphabet:
+        return alphabet[nuc]
+    return 4
+
+
+aa_alphabet = 'ACDEFGHIKLMNPQRSTVWYxX'
+
+
+if __name__ == '__main__':
+    import sys
+
+    sys.exit(main(sys.argv))
```

### Comparing `lhc-python-2.5.0/lhc/binf/sequence/digen/digen.py` & `lhc_python-2.5.1/src/lib/digen/digen.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,137 +1,140 @@
-#!/usr/bin/python
-
-import numpy
-import random
-
-from sequence.seq_tools import dinuc
-
-
-def convert_frequency(alp):
-    din2idx = dict(('%s%s' % ('acgu'[i / 4], 'acgu'[i % 4]), i) for i in range(16))
-    num = numpy.zeros(16, dtype=numpy.int32)
-    for k, v in alp.items():
-        num[din2idx[k]] = int(v)
-    return num
-
-
-def connectivity(frq):
-    ncmp = 0  # Connectivity
-    vis = numpy.zeros(len(frq), dtype=numpy.bool)  # Visited nodes
-    for i in range(len(frq)):
-        if frq[i] == 0 or vis[i]:
-            continue
-
-        ncmp += 1
-        stk = [i]
-        vis[i] = True
-        while len(stk) > 0:  # Breadth first search.
-            j = stk.pop(0)
-            for k in range(4):
-                up = k * 4 + j / 4
-                if not vis[up] and frq[up] > 0:
-                    stk.append(up)
-                    vis[up] = True
-                dn = k + (j % 4) * 4
-                if not vis[dn] and frq[dn] > 0:
-                    stk.append(dn)
-                    vis[dn] = True
-
-    return ncmp
-
-
-def imbalance(frq):
-    res = numpy.zeros(4)
-    for i in range(len(frq)):
-        res[i / 4] -= frq[i]  # Consumed
-        res[i % 4] += frq[i]  # Produced
-    return res
-
-
-def connected(frq, fr):
-    res = numpy.zeros(len(frq))
-    if frq[fr] == 0:
-        raise Exception('Not a valid start point')
-    res = numpy.zeros(len(frq))
-    n = 0
-    stk = [fr]
-    while len(stk) > 0:
-        top = stk.pop(0)
-        res[top] = 1
-        for j in range(top % 4 * 4, top % 4 * 4 + 4):
-            if frq[j] > 0 and res[j] == 0:
-                stk.append(j)
-
-    return sum(res) == sum(frq > 0)
-
-
-def generate(frq):
-    res = []
-    if connectivity(frq) > 1:
-        return res
-
-    # Calculate the imbalance
-    imb = imbalance(frq)
-    if sum(abs(imb)) == 1 or sum(abs(imb)) > 2:
-        return res
-
-    # Choose the next node
-    if -1 in imb:
-        fr = numpy.where(imb == -1)[0] * 4
-        stk = [(i, frq, [i / 4]) for i in range(fr, fr + 4) if frq[i] > 0][::-1]
-    else:
-        stk = [(i, frq, [i / 4]) for i in range(len(frq)) if frq[i] > 0][::-1]
-
-    # random.shuffle(stk) # Start at a random dinucleotide (if more than one possible start).
-    while len(stk) > 0:
-        i, frq, pth = stk.pop()
-        frq = frq.copy()
-        pth = pth[:]
-
-        # Adjust the frequencies and adjacency matrix
-        frq[i] -= 1
-        pth.append(i % 4)
-        if sum(frq) == 0:
-            return ''.join(['acgu'[j] for j in pth])
-            # res.append(''.join(['acgu'[j] for j in pth]))
-            continue
-
-        # Calculate the imbalance
-        imb = imbalance(frq)
-
-        # Choose the next node
-        if connectivity(frq) > 1 or sum(abs(imb)) > 2:
-            continue
-
-        if -1 in imb:
-            fr = numpy.where(imb == -1)[0] * 4
-            nxt = [(j, frq, pth) for j in range(fr, fr + 4) if frq[j] > 0]
-        else:
-            fr = (i % 4) * 4
-            nxt = [(j, frq, pth) for j in range(fr, fr + 4) if frq[j] > 0]
-
-        # random.shuffle(nxt)
-        stk.extend(reversed(nxt))
-    return res
-
-
-def main(argv):
-    frq = {}
-    for i in range(1, len(argv)):
-        k, v = argv[i].split(':')
-        frq[k] = int(v)
-    frq = convert_frequency(frq)
-    res = digen(frq)
-    if res == None:
-        print('There are no possible sequences with this dinucleotide frequency')
-    else:
-        # for r in res:
-        #    print r, dinuc(r)*len(r)
-        print(res)
-        print(dinuc(res) * len(res))
-    return 0
-
-
-if __name__ == '__main__':
-    import sys
-
-    sys.exit(main(sys.argv))
+#!/usr/bin/python
+
+import numpy
+
+from lhc.misc.kmer import KmerCounter
+
+
+def convert_frequency(alp):
+    din2idx = dict(('%s%s' % ('acgu'[i / 4], 'acgu'[i % 4]), i) for i in range(16))
+    num = numpy.zeros(16, dtype=numpy.int32)
+    for k, v in alp.items():
+        num[din2idx[k]] = int(v)
+    return num
+
+
+def connectivity(frq):
+    ncmp = 0  # Connectivity
+    vis = numpy.zeros(len(frq), dtype=numpy.bool)  # Visited nodes
+    for i in range(len(frq)):
+        if frq[i] == 0 or vis[i]:
+            continue
+
+        ncmp += 1
+        stk = [i]
+        vis[i] = True
+        while len(stk) > 0:  # Breadth first search.
+            j = stk.pop(0)
+            for k in range(4):
+                up = k * 4 + j / 4
+                if not vis[up] and frq[up] > 0:
+                    stk.append(up)
+                    vis[up] = True
+                dn = k + (j % 4) * 4
+                if not vis[dn] and frq[dn] > 0:
+                    stk.append(dn)
+                    vis[dn] = True
+
+    return ncmp
+
+
+def imbalance(frq):
+    res = numpy.zeros(4)
+    for i in range(len(frq)):
+        res[i / 4] -= frq[i]  # Consumed
+        res[i % 4] += frq[i]  # Produced
+    return res
+
+
+def connected(frq, fr):
+    res = numpy.zeros(len(frq))
+    if frq[fr] == 0:
+        raise Exception('Not a valid start point')
+    res = numpy.zeros(len(frq))
+    n = 0
+    stk = [fr]
+    while len(stk) > 0:
+        top = stk.pop(0)
+        res[top] = 1
+        for j in range(top % 4 * 4, top % 4 * 4 + 4):
+            if frq[j] > 0 and res[j] == 0:
+                stk.append(j)
+
+    return sum(res) == sum(frq > 0)
+
+
+def generate(frq):
+    res = []
+    if connectivity(frq) > 1:
+        return res
+
+    # Calculate the imbalance
+    imb = imbalance(frq)
+    if sum(abs(imb)) == 1 or sum(abs(imb)) > 2:
+        return res
+
+    # Choose the next node
+    if -1 in imb:
+        fr = numpy.where(imb == -1)[0] * 4
+        stk = [(i, frq, [i / 4]) for i in range(fr, fr + 4) if frq[i] > 0][::-1]
+    else:
+        stk = [(i, frq, [i / 4]) for i in range(len(frq)) if frq[i] > 0][::-1]
+
+    # random.shuffle(stk) # Start at a random dinucleotide (if more than one possible start).
+    while len(stk) > 0:
+        i, frq, pth = stk.pop()
+        frq = frq.copy()
+        pth = pth[:]
+
+        # Adjust the frequencies and adjacency matrix
+        frq[i] -= 1
+        pth.append(i % 4)
+        if sum(frq) == 0:
+            return ''.join(['acgu'[j] for j in pth])
+            # res.append(''.join(['acgu'[j] for j in pth]))
+            continue
+
+        # Calculate the imbalance
+        imb = imbalance(frq)
+
+        # Choose the next node
+        if connectivity(frq) > 1 or sum(abs(imb)) > 2:
+            continue
+
+        if -1 in imb:
+            fr = numpy.where(imb == -1)[0] * 4
+            nxt = [(j, frq, pth) for j in range(fr, fr + 4) if frq[j] > 0]
+        else:
+            fr = (i % 4) * 4
+            nxt = [(j, frq, pth) for j in range(fr, fr + 4) if frq[j] > 0]
+
+        # random.shuffle(nxt)
+        stk.extend(reversed(nxt))
+    return res
+
+
+def main(argv):
+    frq = {}
+    for i in range(1, len(argv)):
+        k, v = argv[i].split(':')
+        frq[k] = int(v)
+    frq = convert_frequency(frq)
+    res = generate(frq)
+    if res == None:
+        print('There are no possible sequences with this dinucleotide frequency')
+    else:
+        # for r in res:
+        #    print r, dinuc(r)*len(r)
+        print(res)
+        print(dinuc(res))
+    return 0
+
+
+def dinuc(sequence):
+    return KmerCounter(sequence)
+
+
+if __name__ == '__main__':
+    import sys
+
+    sys.exit(main(sys.argv))
```

### Comparing `lhc-python-2.5.0/lhc/binf/sequence/sequence_generator.py` & `lhc_python-2.5.1/src/lhc/entities/sequence/sequence_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import bisect
-import random
-
-
-class SequenceGenerator(object):
-
-    NUCLEOTIDES = (('A', 1), ('C', 1), ('G', 1), ('T', 1))
-    AMINO_ACIDS = (('A', 1), ('C', 1), ('D', 1), ('E', 1), ('F', 1), ('G', 1), ('H', 1), ('I', 1), ('K', 1), ('L', 1),
-                   ('M', 1), ('N', 1), ('P', 1), ('Q', 1), ('R', 1), ('S', 1), ('T', 1), ('V', 1), ('W', 1), ('Y', 1))
-
-    def __init__(self, letters=None):
-        """ Create a sequence generator that can generate sequences with given letter frequencies
-
-        :param letters: letters and probabilities as a list of (letter, weight) tuples.
-        """
-        if letters is None:
-            letters = self.NUCLEOTIDES
-        self.letters, weights = list(zip(*letters))
-        self.cumulative_distribution = self._get_cumulative_distribution(weights)
-
-    def generate(self, length):
-        return ''.join(self._get_letter() for i in range(length))
-
-    def _get_cumulative_distribution(self, weights):
-        total_weight = float(sum(weights))
-        probabilities = [weight / total_weight for weight in weights]
-        return list(cumsum(probabilities))
-
-    def _get_letter(self):
-        quantile = random.random()
-        return self.letters[bisect.bisect(self.cumulative_distribution, quantile)]
-
-
-def cumsum(iterable):
-    running_total = 0
-    for item in iterable:
-        running_total += item
-        yield running_total
+import bisect
+import random
+
+
+class SequenceGenerator(object):
+
+    NUCLEOTIDES = (('A', 1), ('C', 1), ('G', 1), ('T', 1))
+    AMINO_ACIDS = (('A', 1), ('C', 1), ('D', 1), ('E', 1), ('F', 1), ('G', 1), ('H', 1), ('I', 1), ('K', 1), ('L', 1),
+                   ('M', 1), ('N', 1), ('P', 1), ('Q', 1), ('R', 1), ('S', 1), ('T', 1), ('V', 1), ('W', 1), ('Y', 1))
+
+    def __init__(self, letters=None):
+        """ Create a sequences generator that can generate sequences with given letter frequencies
+
+        :param letters: letters and probabilities as a list of (letter, weight) tuples.
+        """
+        if letters is None:
+            letters = self.NUCLEOTIDES
+        self.letters, weights = list(zip(*letters))
+        self.cumulative_distribution = self._get_cumulative_distribution(weights)
+
+    def generate(self, length):
+        return ''.join(self._get_letter() for i in range(length))
+
+    def _get_cumulative_distribution(self, weights):
+        total_weight = float(sum(weights))
+        probabilities = [weight / total_weight for weight in weights]
+        return list(cumsum(probabilities))
+
+    def _get_letter(self):
+        quantile = random.random()
+        return self.letters[bisect.bisect(self.cumulative_distribution, quantile)]
+
+
+def cumsum(iterable):
+    running_total = 0
+    for item in iterable:
+        running_total += item
+        yield running_total
```

### Comparing `lhc-python-2.5.0/lhc/binf/sequence/tools/split.py` & `lhc_python-2.5.1/src/lhc/cli/sequences/split.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,100 @@
-import argparse
-import glob
-import re
-
-from functools import partial
-from textwrap import TextWrapper
-from typing import Callable, Dict, Iterable, Iterator, List, Optional, Tuple
-from lhc.io.fasta.iterator import iter_fasta, FastaEntry
-from lhc.filetools.filepool import FilePool
-
-
-def split(sequences: Iterable[FastaEntry], mappers: List[Callable], *, unmapped='discard') -> Iterator[Tuple[str, FastaEntry]]:
-    def map_to_filename(sequence_: FastaEntry) -> str:
-        for mapper in mappers:
-            filename_ = mapper(sequence_)
-            if filename_:
-                return filename_
-        return None if unmapped == 'discard' else\
-            'unmapped' if unmapped == 'join' else\
-            sequence.key
-
-    for sequence in sequences:
-        if len(sequence.seq) == 0:
-            continue
-        filename = map_to_filename(sequence)
-        if filename:
-            yield filename, sequence
-
-
-def map_by_map(sequence: FastaEntry, map_: Dict[str, str]) -> Optional[str]:
-    return map_.get(sequence.key, None)
-
-
-def map_by_regx(sequence: FastaEntry, regx: re.Pattern, replacement: str, description=False) -> Optional[str]:
-    match = regx.match(sequence.key)
-    if match:
-        return regx.sub(replacement, sequence.key)
-    elif description:
-        match = regx.match(sequence.hdr)
-        if match:
-            return regx.sub(replacement, sequence.hdr)
-    return None
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser():
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser):
-    parser.add_argument('input', nargs='*',
-                        help='sequences to filter (default: stdin).')
-    parser.add_argument('-d', '--description', action='store_true',
-                        help='search also in description field.')
-    parser.add_argument('-o', '--output',
-                        help='prefix for output files')
-    parser.add_argument('-r', '--regular-expression', nargs=2, action='append',
-                        help='split using regular expression')
-    parser.add_argument('-m', '--map',
-                        help='split using a map')
-    parser.add_argument('-u', '--unmapped', choices=['discard', 'keep', 'split'], default='split',
-                        help='whether the unmapped sequences should be discarded, output to a single file or output to multiple files')
-    parser.set_defaults(func=init_split)
-    return parser
-
-
-def init_split(args: argparse.Namespace):
-    wrapper = TextWrapper()
-    mappers = []
-
-    outputs = FilePool(mode='w')
-    if args.map:
-        with open(args.map) as fileobj:
-            mappers.append(partial(map_by_map, map_=dict(line.strip().split() for line in fileobj)))
-    if args.regular_expression:
-        for expression in args.regular_expression:
-            mappers.append(partial(map_by_regx, regx=re.compile(expression[0]), replacement=expression[1], description=args.description))
-
-    sequence_iterators = [('stdin', iter_fasta(sys.stdin))] if args.input is None else ((input, iter_fasta(input)) for input in args.input if input)
-    for input, sequences in sequence_iterators:
-        try:
-            for filename, sequence in split(sequences, mappers, unmapped=args.unmapped):
-                outputs['{}{}.fasta'.format(args.output, filename)].write('>{} "{}"\n{}\n'.format(sequence.hdr, input, '\n'.join(wrapper.wrap(sequence.seq.replace('-', '')))))
-        except ValueError as error:
-            if str(error) == 'Invalid fasta file format.':
-                raise ValueError('"{}" has an invalid fasta file format.'.format(input))
-            else:
-                raise error
-
-
-if __name__ == '__main__':
-    import sys
-    sys.exit(main())
+import argparse
+import re
+
+from functools import partial
+from textwrap import TextWrapper
+from typing import Callable, Dict, Iterator, List, Optional, Tuple
+from lhc.io.sequence import open_sequence_file, Sequence, SequenceFile
+from lhc.io import FilePool
+
+
+def split(sequences: SequenceFile, mappers: List[Callable], *, unmapped='discard') -> Iterator[Tuple[str, Sequence]]:
+    def map_to_filename(sequence_: Sequence) -> str:
+        for mapper in mappers:
+            filename_ = mapper(sequence_)
+            if filename_:
+                return filename_
+        return None if unmapped == 'discard' else\
+            'unmapped' if unmapped == 'join' else\
+            sequence.identifier
+
+    for sequence in sequences:
+        if len(sequence.sequence) == 0:
+            continue
+        filename = map_to_filename(sequence)
+        if filename:
+            yield filename, sequence
+
+
+def map_by_map(sequence: Sequence, map_: Dict[str, str]) -> Optional[str]:
+    return map_.get(sequence.identifier, None)
+
+
+def map_by_regx(sequence: Sequence, regx: re.Pattern, replacement: str, description=False) -> Optional[str]:
+    match = regx.match(sequence.identifier)
+    if match:
+        return regx.sub(replacement, sequence.identifier)
+    elif description:
+        match = regx.match(sequence.identifier)
+        if match:
+            return regx.sub(replacement, sequence.identifier)
+    return None
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser():
+    return define_parser(argparse.ArgumentParser(get_description()))
+
+
+def get_description() -> str:
+    return 'Split a set of sequences into several sets based on the given conditions.'
+
+
+def define_parser(parser):
+    parser.add_argument('input', nargs='*',
+                        help='sequences to filter (default: stdin).')
+    parser.add_argument('-d', '--description', action='store_true',
+                        help='search also in description field.')
+    parser.add_argument('-o', '--output',
+                        help='prefix for output files')
+    parser.add_argument('-r', '--regular-expression', nargs=2, action='append',
+                        help='split using regular expression')
+    parser.add_argument('-m', '--map',
+                        help='split using a map')
+    parser.add_argument('-u', '--unmapped', choices=['discard', 'keep', 'split'], default='split',
+                        help='whether the unmapped sequences should be discarded, output to a single file or output to multiple files')
+    parser.set_defaults(func=init_split)
+    return parser
+
+
+def init_split(args: argparse.Namespace):
+    wrapper = TextWrapper()
+    mappers = []
+
+    outputs = FilePool(mode='w')
+    if args.map:
+        with open(args.map) as fileobj:
+            mappers.append(partial(map_by_map, map_=dict(line.strip().split(maxsplit=1) for line in fileobj)))
+    if args.regular_expression:
+        for expression in args.regular_expression:
+            mappers.append(partial(map_by_regx, regx=re.compile(expression[0]), replacement=expression[1], description=args.description))
+
+    sequence_iterators = [open_sequence_file(input) for input in args.input if input]
+    for input_, sequences in sequence_iterators:
+        try:
+            for filename, sequence in split(sequences, mappers, unmapped=args.unmapped):
+                outputs['{}{}.fasta'.format(args.output, filename)].write('>{} "{}"\n{}\n'.format(sequence.identifier, input_, '\n'.join(wrapper.wrap(sequence.sequence.replace('-', '')))))
+        except ValueError as error:
+            if str(error) == 'Invalid fasta file format.':
+                raise ValueError('"{}" has an invalid fasta file format.'.format(input_))
+            else:
+                raise error
+
+
+if __name__ == '__main__':
+    import sys
+    sys.exit(main())
```

### Comparing `lhc-python-2.5.0/lhc/binf/sequence/tools/view.py` & `lhc_python-2.5.1/src/lhc/cli/sequences/reverse_complement.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,47 @@
-import argparse
-
-from textwrap import TextWrapper
-from typing import Iterable, Iterator
-from lhc.io import open_file
-from lhc.io.fasta.iterator import iter_fasta, FastaEntry
-
-
-def view(sequences: Iterable[FastaEntry]) -> Iterator[FastaEntry]:
-    for sequence in sequences:
-        yield FastaEntry(sequence.key, sequence.hdr, sequence.seq.replace('-', ''))
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser() -> argparse.ArgumentParser:
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-    parser.add_argument('input', nargs='?',
-                        help='sequences to view (default: stdin).')
-    parser.add_argument('output', nargs='?',
-                        help='sequence file to write viewed sequences to (default: stdout).')
-    parser.set_defaults(func=init_view)
-    return parser
-
-
-def init_view(args: argparse.Namespace):
-    wrapper = TextWrapper()
-    with open_file(args.input) as input, open_file(args.output, 'w') as output:
-        sequences = iter_fasta(input)
-        for sequence in view(sequences):
-            output.write('>{}\n{}\n'.format(sequence.hdr, '\n'.join(wrapper.wrap(sequence.seq))))
-
-
-if __name__ == '__main__':
-    import sys
-    sys.exit(main())
+import argparse
+
+from typing import Iterator
+from lhc.io.sequence import open_sequence_file, SequenceFile, Sequence
+from lhc.entities.sequence.reverse_complement import reverse_complement as rc
+
+
+def reverse_complement(sequences: SequenceFile) -> Iterator[Sequence]:
+    for sequence in sequences:
+        yield Sequence(sequence.identifier, rc(sequence.sequence.replace('-', '')))
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser() -> argparse.ArgumentParser:
+    return define_parser(argparse.ArgumentParser(get_description()))
+
+
+def get_description() -> str:
+    return 'View the sequences in the given file.'
+
+
+def define_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
+    parser.add_argument('input', nargs='?',
+                        help='sequences to reverse complement (default: stdin).')
+    parser.add_argument('output', nargs='?',
+                        help='sequences file to write reverse complemented sequences to (default: stdout).')
+    parser.add_argument('-i', '--input-format')
+    parser.add_argument('-o', '--output-format', default='fasta')
+    parser.set_defaults(func=init_reverse_complement)
+    return parser
+
+
+def init_reverse_complement(args: argparse.Namespace):
+    with open_sequence_file(args.input, format=args.input_format) as sequences,\
+        open_sequence_file(args.output, 'w', format=args.output_format) as output\
+    :
+        for sequence in reverse_complement(sequences):
+            output.write(sequence)
+
+
+if __name__ == '__main__':
+    import sys
+    sys.exit(main())
```

### Comparing `lhc-python-2.5.0/lhc/binf/variant/amino_acid_variant.py` & `lhc_python-2.5.1/src/lhc/entities/variant/amino_acid_variant.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from dataclasses import dataclass
-from lhc.binf.genetic_code import GeneticCodes
-
-
-@dataclass
-class AminoAcidVariant:
-    pos: int
-    ref: str
-    alt: str
-    fs: int = 0
-
-    def __str__(self):
-        pos = self.pos
-        ref = self.ref
-        alt = self.alt
-        if self.fs > 0:
-            res = 'p.{}{}{}fs{}'.format(self.ref[0], self.pos + 1, self.alt[0], 'Ter' + str(self.fs) if self.alt[-1] == '*' else '*?')
-        elif len(ref) > len(alt):
-            d = len(ref) - len(alt)
-            rng = pos + 1 if d == 1 else '{}_{}'.format(pos + 1, pos + len(ref) - 1)
-            res = 'p.{}del'.format(rng)
-        elif len(alt) > len(ref):
-            res = 'p.{}_{}ins{}'.format(pos + 1, pos + 2, alt)
-        else:
-            res = 'p.{}{}{}'.format(self.ref, pos + 1, alt)
-        return res
-
-
-def call_amino_acid_variants(codon_variants, genetic_code=None):
-    if genetic_code is None:
-        genetic_code = GeneticCodes().get_code(1)
-    amino_acid_variants = []
-    for variant in codon_variants:
-        if variant is None:
-            amino_acid_variants.append(None)
-            continue
-
-        amino_acid_variants.append(AminoAcidVariant(
-            variant.pos // 3,
-            genetic_code.translate(variant.ref),
-            genetic_code.translate(variant.alt),
-            None if variant.fs is None else variant.fs // 3,
-        ))
-    return amino_acid_variants
+from dataclasses import dataclass
+from lhc.misc.genetic_code import GeneticCodes
+
+
+@dataclass
+class AminoAcidVariant:
+    pos: int
+    ref: str
+    alt: str
+    fs: int = 0
+
+    def __str__(self):
+        pos = self.pos
+        ref = self.ref
+        alt = self.alt
+        if self.fs > 0:
+            res = 'p.{}{}{}fs{}'.format(self.ref[0], self.pos + 1, self.alt[0], 'Ter' + str(self.fs) if self.alt[-1] == '*' else '*?')
+        elif len(ref) > len(alt):
+            d = len(ref) - len(alt)
+            rng = pos + 1 if d == 1 else '{}_{}'.format(pos + 1, pos + len(ref) - 1)
+            res = 'p.{}del'.format(rng)
+        elif len(alt) > len(ref):
+            res = 'p.{}_{}ins{}'.format(pos + 1, pos + 2, alt)
+        else:
+            res = 'p.{}{}{}'.format(self.ref, pos + 1, alt)
+        return res
+
+
+def call_amino_acid_variants(codon_variants, genetic_code=None):
+    if genetic_code is None:
+        genetic_code = GeneticCodes().get_code(1)
+    amino_acid_variants = []
+    for variant in codon_variants:
+        if variant is None:
+            amino_acid_variants.append(None)
+            continue
+
+        amino_acid_variants.append(AminoAcidVariant(
+            variant.pos // 3,
+            genetic_code.translate(variant.ref),
+            genetic_code.translate(variant.alt),
+            None if variant.fs is None else variant.fs // 3,
+        ))
+    return amino_acid_variants
```

### Comparing `lhc-python-2.5.0/lhc/binf/variant/codon_variant.py` & `lhc_python-2.5.1/src/lhc/entities/variant/codon_variant.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from dataclasses import dataclass
-
-
-@dataclass
-class CodonVariant:
-    pos: int
-    ref: str
-    alt: str
-    fs: int = 0
-
-    def __str__(self):
-        if self.fs == 0:
-            return 'c.{}{}>{}'.format(self.pos + 1, self.ref, self.alt)
-        else:
-            return 'c.{}{}{}fs{}'.format(self.ref[:3], self.pos + 1, self.alt[:3], 'Ter' + str(self.fs) if self.alt[-3:].upper() in {'TAA', 'TAG', 'TGA'} else '*?')
-
-
-def call_codon_variants(coding_variants, reference_sequences):
-    codon_variants = []
-    for variant in coding_variants:
-        if variant is None:
-            codon_variants.append(None)
-            continue
-
-        reference_sequence = reference_sequences[variant.id]
-        assert reference_sequence[variant.pos:variant.pos + len(variant.ref)] == variant.ref
-
-        sequence = list(reference_sequence)
-        sequence[variant.pos:variant.pos + len(variant.ref)] = list(variant.alt)
-
-        fr = variant.pos - variant.pos % 3
-        if (len(variant.ref) - len(variant.alt)) % 3 == 0:
-            ref_to = variant.pos + len(variant.ref)
-            ref_to += [0, 2, 1][ref_to % 3]
-            alt_to = variant.pos + len(variant.alt)
-            alt_to += [0, 2, 1][alt_to % 3]
-            fs_pos = 0
-        else:
-            while fr + 3 < len(reference_sequence) and fr + 3 < len(sequence) and reference_sequence[fr:fr+3] == ''.join(sequence[fr:fr+3]):
-                fr += 3
-
-            ref_to = fr + 3
-            while ref_to <= len(reference_sequence) and reference_sequence[ref_to - 3:ref_to].upper() not in {'TAA', 'TAG', 'TGA'}:
-                ref_to += 3
-
-            alt_to = fr + 3
-            while alt_to <= len(sequence) and ''.join(sequence[alt_to - 3:alt_to]).upper() not in {'TAA', 'TAG', 'TGA'}:
-                alt_to += 3
-            fs_pos = alt_to - fr - (3 if ''.join(sequence[alt_to - 3:alt_to]).upper() in {'TAA', 'TAG', 'TGA'} else 0)
-            if fs_pos == 0:
-                ref_to = fr + 3
-        ref_codon = reference_sequence[fr:ref_to]
-        alt_codon = ''.join(sequence[fr:alt_to])
-        codon_variants.append(CodonVariant(fr, ref_codon, alt_codon, fs_pos))
-    return codon_variants
+from dataclasses import dataclass
+
+
+@dataclass
+class CodonVariant:
+    pos: int
+    ref: str
+    alt: str
+    fs: int = 0
+
+    def __str__(self):
+        if self.fs == 0:
+            return 'c.{}{}>{}'.format(self.pos + 1, self.ref, self.alt)
+        else:
+            return 'c.{}{}{}fs{}'.format(self.ref[:3], self.pos + 1, self.alt[:3], 'Ter' + str(self.fs) if self.alt[-3:].upper() in {'TAA', 'TAG', 'TGA'} else '*?')
+
+
+def call_codon_variants(coding_variants, reference_sequences):
+    codon_variants = []
+    for variant in coding_variants:
+        if variant is None:
+            codon_variants.append(None)
+            continue
+
+        reference_sequence = reference_sequences[variant.id]
+        assert reference_sequence[variant.pos:variant.pos + len(variant.ref)] == variant.ref
+
+        sequence = list(reference_sequence)
+        sequence[variant.pos:variant.pos + len(variant.ref)] = list(variant.alt)
+
+        fr = variant.pos - variant.pos % 3
+        if (len(variant.ref) - len(variant.alt)) % 3 == 0:
+            ref_to = variant.pos + len(variant.ref)
+            ref_to += [0, 2, 1][ref_to % 3]
+            alt_to = variant.pos + len(variant.alt)
+            alt_to += [0, 2, 1][alt_to % 3]
+            fs_pos = 0
+        else:
+            while fr + 3 < len(reference_sequence) and fr + 3 < len(sequence) and reference_sequence[fr:fr+3] == ''.join(sequence[fr:fr+3]):
+                fr += 3
+
+            ref_to = fr + 3
+            while ref_to <= len(reference_sequence) and reference_sequence[ref_to - 3:ref_to].upper() not in {'TAA', 'TAG', 'TGA'}:
+                ref_to += 3
+
+            alt_to = fr + 3
+            while alt_to <= len(sequence) and ''.join(sequence[alt_to - 3:alt_to]).upper() not in {'TAA', 'TAG', 'TGA'}:
+                alt_to += 3
+            fs_pos = alt_to - fr - (3 if ''.join(sequence[alt_to - 3:alt_to]).upper() in {'TAA', 'TAG', 'TGA'} else 0)
+            if fs_pos == 0:
+                ref_to = fr + 3
+        ref_codon = reference_sequence[fr:ref_to]
+        alt_codon = ''.join(sequence[fr:alt_to])
+        codon_variants.append(CodonVariant(fr, ref_codon, alt_codon, fs_pos))
+    return codon_variants
```

### Comparing `lhc-python-2.5.0/lhc/binf/variant/tools/annotate.py` & `lhc_python-2.5.1/src/lhc/cli/variants/annotate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,71 @@
-import argparse
-
-from lhc.binf.variant import call_coding_variants, call_codon_variants, call_amino_acid_variants, call_variant_effects
-from lhc.collections import IntervalSet
-from lhc.io import open_file
-from lhc.io.locus import open_locus_file, LocusFile
-from lhc.io.sequence import open_sequence_file, SequenceFile
-from lhc.io.variant import open_variant_file, VariantFile
-
-
-def annotate(variants: VariantFile, reference: SequenceFile, loci: LocusFile):
-    variants = list(variants)
-    locus_set = IntervalSet(locus for locus in loci if locus.data['type'] == 'CDS')
-    locus_sequences = {locus.data['gene']: reference.file.fetch(
-            str(locus.chromosome),
-            locus.start.position,
-            locus.stop.position + 3
-        ) for locus in locus_set}
-    coding_variantss = call_coding_variants(variants, locus_set)
-    codon_variantss = []
-    for coding_variants in coding_variantss:
-        codon_variantss.append(call_codon_variants(coding_variants, locus_sequences))
-    amino_acid_variantss = []
-    for codon_variants in codon_variantss:
-        amino_acid_variantss.append(call_amino_acid_variants(codon_variants))
-    variant_effectss = []
-    for amino_acid_variants in amino_acid_variantss:
-        variant_effectss.append(call_variant_effects(amino_acid_variants))
-    yield from zip(variants, coding_variantss, codon_variantss, amino_acid_variantss, variant_effectss)
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser() -> argparse.ArgumentParser:
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
-    parser.add_argument('input', nargs='?')
-    parser.add_argument('output', nargs='?')
-    parser.add_argument('-i', '--input-format')
-    parser.add_argument('-r', '--reference', required=True)
-    parser.add_argument('-l', '--loci', required=True)
-    parser.set_defaults(func=init_annotate)
-    return parser
-
-
-def init_annotate(args: argparse.Namespace):
-    with open_variant_file(args.input, format=args.input_format) as variants,\
-            open_file(args.output, 'w') as output_file,\
-            open_sequence_file(args.reference, 'q') as reference,\
-            open_locus_file(args.loci) as loci:
-        output_file.write('sample\tallele_frequency\tgenomic_variant\tgene\tamino_acid_variant\tvariant_effect\n')
-        for variant, coding_variants, codon_variants, amino_acid_variants, variant_effects in annotate(variants, reference, loci):
-            for coding_variant, codon_variant, amino_acid_variant, variant_effect in zip(coding_variants, codon_variants, amino_acid_variants, variant_effects):
-                for sample in variant.samples:
-                    if 'AF' not in variant.samples[sample]:
-                        continue
-                    output_file.write('{}\t{}\t{}\t{}\t{}\t{}\n'.format(sample, variant.samples[sample]['AF'], variant, coding_variant.gene, amino_acid_variant, variant_effect))
-
-
-if __name__ == '__main__':
-    import sys
-    sys.exit(main())
+import argparse
+
+from lhc.entities.variant import call_coding_variants, call_codon_variants, call_amino_acid_variants, call_variant_effects
+from lhc.collections import IntervalSet
+from lhc.io import open_file
+from lhc.io.locus import open_locus_file, LocusFile
+from lhc.io.sequence import open_sequence_file, SequenceFile
+from lhc.io.variant import open_variant_file, VariantFile
+
+
+def annotate(variants: VariantFile, reference: SequenceFile, loci: LocusFile):
+    variants = list(variants)
+    locus_set = IntervalSet(locus for locus in loci if locus.data['type'] == 'CDS')
+    locus_sequences = {locus.data['gene']: reference.file.fetch(
+            str(locus.chromosome),
+            locus.start.position,
+            locus.stop.position + 3
+        ) for locus in locus_set}
+    coding_variantss = call_coding_variants(variants, locus_set)
+    codon_variantss = []
+    for coding_variants in coding_variantss:
+        codon_variantss.append(call_codon_variants(coding_variants, locus_sequences))
+    amino_acid_variantss = []
+    for codon_variants in codon_variantss:
+        amino_acid_variantss.append(call_amino_acid_variants(codon_variants))
+    variant_effectss = []
+    for amino_acid_variants in amino_acid_variantss:
+        variant_effectss.append(call_variant_effects(amino_acid_variants))
+    yield from zip(variants, coding_variantss, codon_variantss, amino_acid_variantss, variant_effectss)
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser() -> argparse.ArgumentParser:
+    return define_parser(argparse.ArgumentParser(get_description()))
+
+
+def get_description() -> str:
+    return 'Annotate the given set of genomic variants'
+
+
+def define_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
+    parser.add_argument('input', nargs='?')
+    parser.add_argument('output', nargs='?')
+    parser.add_argument('-i', '--input-format')
+    parser.add_argument('-r', '--reference', required=True)
+    parser.add_argument('-l', '--loci', required=True)
+    parser.set_defaults(func=init_annotate)
+    return parser
+
+
+def init_annotate(args: argparse.Namespace):
+    with open_variant_file(args.input, format=args.input_format) as variants,\
+            open_file(args.output, 'w') as output_file,\
+            open_sequence_file(args.reference, 'q') as reference,\
+            open_locus_file(args.loci) as loci:
+        output_file.write('sample\tallele_frequency\tgenomic_variant\tgene\tamino_acid_variant\tvariant_effect\n')
+        for variant, coding_variants, codon_variants, amino_acid_variants, variant_effects in annotate(variants, reference, loci):
+            for coding_variant, codon_variant, amino_acid_variant, variant_effect in zip(coding_variants, codon_variants, amino_acid_variants, variant_effects):
+                for sample in variant.samples:
+                    if 'AF' not in variant.samples[sample]:
+                        continue
+                    output_file.write('{}\t{}\t{}\t{}\t{}\t{}\n'.format(sample, variant.samples[sample]['AF'], variant, coding_variant.gene, amino_acid_variant, variant_effect))
+
+
+if __name__ == '__main__':
+    import sys
+    sys.exit(main())
```

### Comparing `lhc-python-2.5.0/lhc/binf/variant/variant.py` & `lhc_python-2.5.1/src/lhc/entities/variant/variant.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from dataclasses import dataclass
-from typing import Any, Dict, Optional
-
-
-@dataclass
-class Variant:
-    chr: str
-    pos: int
-    ref: str
-    alt: str
-    id: Optional[str] = None
-    qual: Optional[float] = None
-    filter: Optional[str] = None
-    info: Optional[Dict[str, str]] = None
-    format: Optional[str] = None
-    samples: Optional[Dict[str, Any]] = None
-    lead: Optional[str] = None
-
-    def __str__(self):
-        res = []
-        pos = self.pos
-        ref = self.ref
-        alt = self.alt
-        if len(ref) > len(alt):
-            d = len(ref) - len(alt)
-            rng = str(pos + len(ref) - 1,) if d == 1 else '{}_{}'.format(pos + len(ref) - d, pos + len(ref) - 1)
-            res.append('g.{}del'.format(rng))
-        elif len(alt) > len(ref):
-            res.append('g.{}_{}ins{}'.format(pos, pos + 1, alt))
-        else:
-            if len(ref) > 1 and ref == alt:
-                res.append('g.{}_{}inv'.format(pos + 1, pos + len(ref)))
-            else:
-                res.append('g.{}{}>{}'.format(pos + 1, ref, alt))
-        return ','.join(res)
+from dataclasses import dataclass
+from typing import Any, Dict, Optional
+
+
+@dataclass
+class Variant:
+    chr: str
+    pos: int
+    ref: str
+    alt: str
+    id: Optional[str] = None
+    qual: Optional[float] = None
+    filter: Optional[str] = None
+    info: Optional[Dict[str, str]] = None
+    format: Optional[str] = None
+    samples: Optional[Dict[str, Any]] = None
+    lead: Optional[str] = None
+
+    def __str__(self):
+        res = []
+        pos = self.pos
+        ref = self.ref
+        alt = self.alt
+        if len(ref) > len(alt):
+            d = len(ref) - len(alt)
+            rng = str(pos + len(ref) - 1,) if d == 1 else '{}_{}'.format(pos + len(ref) - d, pos + len(ref) - 1)
+            res.append('g.{}del'.format(rng))
+        elif len(alt) > len(ref):
+            res.append('g.{}_{}ins{}'.format(pos, pos + 1, alt))
+        else:
+            if len(ref) > 1 and ref == alt:
+                res.append('g.{}_{}inv'.format(pos + 1, pos + len(ref)))
+            else:
+                res.append('g.{}{}>{}'.format(pos + 1, ref, alt))
+        return ','.join(res)
```

### Comparing `lhc-python-2.5.0/lhc/binf/variant/variant_effect.py` & `lhc_python-2.5.1/src/lhc/entities/variant/variant_effect.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-def call_variant_effects(amino_acid_variants):
-    variant_effects = []
-    for variant in amino_acid_variants:
-        # intron_variant is still missing
-        if variant is None:
-            variant_effects.append('intergenic_variant')
-        elif variant.fs == 0:
-            if variant.ref == variant.alt:
-                if variant.pos == 0:
-                    variant_effects.append('start_retained_variant')
-                elif variant.ref == '*':
-                    variant_effects.append('stop_retained_variant')
-                else:
-                    variant_effects.append('synonymous_variant')
-            else:
-                if variant.pos == 0:
-                    variant_effects.append('start_lost')
-                elif variant.ref == '*':
-                    variant_effects.append('stop_lost')
-                elif variant.alt == '*':
-                    variant_effects.append('stop_gained')
-                else:
-                    variant_effects.append('missense_variant')
-        elif len(variant.ref) > len(variant.alt):
-            if variant.ref.endswith(variant.alt):
-                variant_effects.append('inframe_deletion')
-            else:
-                variant_effects.append('frameshift_truncation')
-        else:
-            if variant.alt.endswith(variant.ref):
-                variant_effects.append('inframe_insertion')
-            else:
-                variant_effects.append('frameshift_elongation')
-    return variant_effects
+def call_variant_effects(amino_acid_variants):
+    variant_effects = []
+    for variant in amino_acid_variants:
+        # intron_variant is still missing
+        if variant is None:
+            variant_effects.append('intergenic_variant')
+        elif variant.fs == 0:
+            if variant.ref == variant.alt:
+                if variant.pos == 0:
+                    variant_effects.append('start_retained_variant')
+                elif variant.ref == '*':
+                    variant_effects.append('stop_retained_variant')
+                else:
+                    variant_effects.append('synonymous_variant')
+            else:
+                if variant.pos == 0:
+                    variant_effects.append('start_lost')
+                elif variant.ref == '*':
+                    variant_effects.append('stop_lost')
+                elif variant.alt == '*':
+                    variant_effects.append('stop_gained')
+                else:
+                    variant_effects.append('missense_variant')
+        elif len(variant.ref) > len(variant.alt):
+            if variant.ref.endswith(variant.alt):
+                variant_effects.append('inframe_deletion')
+            else:
+                variant_effects.append('frameshift_truncation')
+        else:
+            if variant.alt.endswith(variant.ref):
+                variant_effects.append('inframe_insertion')
+            else:
+                variant_effects.append('frameshift_elongation')
+    return variant_effects
```

### Comparing `lhc-python-2.5.0/lhc/data/gc.prt` & `lhc_python-2.5.1/src/lhc/data/gc.prt`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,232 +1,232 @@
---**************************************************************************
---  This is the NCBI genetic code table
---  Initial base data set from Andrzej Elzanowski while at PIR International
---  Addition of Eubacterial and Alternative Yeast by J.Ostell at NCBI
---  Base 1-3 of each codon have been added as comments to facilitate
---    readability at the suggestion of Peter Rice, EMBL
---  Later additions by Taxonomy Group staff at NCBI
---
---  Version 3.9
---     Code 14 differs from code 9 only by translating UAA to Tyr rather than
---     STOP.  A recent study (Telford et al, 2000) has found no evidence that
---     the codon UAA codes for Tyr in the flatworms, but other opinions exist.
---     There are very few GenBank records that are translated with code 14,
---     but a test translation shows that retranslating these records with code
---     9 can cause premature terminations.  Therefore, GenBank will maintain
---     code 14 until further information becomes available.
---
---  Version 3.8
---     Added GTG start to Echinoderm mitochondrial code, code 9
---
---  Version 3.7
---     Added code 23 Thraustochytrium mitochondrial code
---        formerly OGMP code 93
---        submitted by Gertraude Berger, Ph.D.
---
---  Version 3.6
---     Added code 22 TAG-Leu, TCA-stop
---        found in mitochondrial DNA of Scenedesmus obliquus
---        submitted by Gertraude Berger, Ph.D.
---        Organelle Genome Megasequencing Program, Univ Montreal
---
---  Version 3.5
---     Added code 21, Trematode Mitochondrial
---       (as deduced from: Garey & Wolstenholme,1989; Ohama et al, 1990)
---     Added code 16, Chlorophycean Mitochondrial
---       (TAG can translated to Leucine instaed to STOP in chlorophyceans
---        and fungi)
---
---  Version 3.4
---     Added CTG,TTG as allowed alternate start codons in Standard code.
---        Prats et al. 1989, Hann et al. 1992
---
---  Version 3.3 - 10/13/95
---     Added alternate intiation codon ATC to code 5
---        based on complete mitochondrial genome of honeybee
---        Crozier and Crozier (1993)
---
---  Version 3.2 - 6/24/95
---  Code       Comments
---   10        Alternative Ciliate Macronuclear renamed to Euplotid Macro...
---   15        Bleharisma Macro.. code added
---    5        Invertebrate Mito.. GTG allowed as alternate initiator
---   11        Eubacterial renamed to Bacterial as most alternate starts
---               have been found in Achea
---
---
---  Version 3.1 - 1995
---  Updated as per Andrzej Elzanowski at NCBI
---     Complete documentation in NCBI toolkit documentation
---  Note: 2 genetic codes have been deleted
---
---   Old id   Use id     - Notes
---
---   id 7      id 4      - Kinetoplast code now merged in code id 4
---   id 8      id 1      - all plant chloroplast differences due to RNA edit
---
---*************************************************************************
-
-Genetic-code-table ::= {
- {
-  name "Standard" ,
-  name "SGC0" ,
-  id 1 ,
-  ncbieaa  "FFLLSSSSYY**CC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
-  sncbieaa "---M---------------M---------------M----------------------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- },
- {
-  name "Vertebrate Mitochondrial" ,
-  name "SGC1" ,
-  id 2 ,
-  ncbieaa  "FFLLSSSSYY**CCWWLLLLPPPPHHQQRRRRIIMMTTTTNNKKSS**VVVVAAAADDEEGGGG",
-  sncbieaa "--------------------------------MMMM---------------M------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- },
- {
-  name "Yeast Mitochondrial" ,
-  name "SGC2" ,
-  id 3 ,
-  ncbieaa  "FFLLSSSSYY**CCWWTTTTPPPPHHQQRRRRIIMMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
-  sncbieaa "----------------------------------MM----------------------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- },
- {
-    name "Mold Mitochondrial; Protozoan Mitochondrial; Coelenterate
- Mitochondrial; Mycoplasma; Spiroplasma" ,
-  name "SGC3" ,
-  id 4 ,
-  ncbieaa  "FFLLSSSSYY**CCWWLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
-  sncbieaa "--MM---------------M------------MMMM---------------M------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- },
- {
-  name "Invertebrate Mitochondrial" ,
-  name "SGC4" ,
-  id 5 ,
-  ncbieaa  "FFLLSSSSYY**CCWWLLLLPPPPHHQQRRRRIIMMTTTTNNKKSSSSVVVVAAAADDEEGGGG",
-  sncbieaa "---M----------------------------MMMM---------------M------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- },
- {
-  name "Ciliate Nuclear; Dasycladacean Nuclear; Hexamita Nuclear" ,
-  name "SGC5" ,
-  id 6 ,
-  ncbieaa  "FFLLSSSSYYQQCC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
-  sncbieaa "-----------------------------------M----------------------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- },
- {
-  name "Echinoderm Mitochondrial; Flatworm Mitochondrial" ,
-  name "SGC8" ,
-  id 9 ,
-  ncbieaa  "FFLLSSSSYY**CCWWLLLLPPPPHHQQRRRRIIIMTTTTNNNKSSSSVVVVAAAADDEEGGGG",
-  sncbieaa "-----------------------------------M---------------M------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- },
- {
-  name "Euplotid Nuclear" ,
-  name "SGC9" ,
-  id 10 ,
-  ncbieaa  "FFLLSSSSYY**CCCWLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
-  sncbieaa "-----------------------------------M----------------------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- },
- {
-  name "Bacterial and Plant Plastid" ,
-  id 11 ,
-  ncbieaa  "FFLLSSSSYY**CC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
-  sncbieaa "---M---------------M------------MMMM---------------M------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- },
- {
-  name "Alternative Yeast Nuclear" ,
-  id 12 ,
-  ncbieaa  "FFLLSSSSYY**CC*WLLLSPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
-  sncbieaa "-------------------M---------------M----------------------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- },
- {
-  name "Ascidian Mitochondrial" ,
-  id 13 ,
-  ncbieaa  "FFLLSSSSYY**CCWWLLLLPPPPHHQQRRRRIIMMTTTTNNKKSSGGVVVVAAAADDEEGGGG",
-  sncbieaa "---M------------------------------MM---------------M------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- },
- {
-  name "Alternative Flatworm Mitochondrial" ,
-  id 14 ,
-  ncbieaa  "FFLLSSSSYYY*CCWWLLLLPPPPHHQQRRRRIIIMTTTTNNNKSSSSVVVVAAAADDEEGGGG",
-  sncbieaa "-----------------------------------M----------------------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- } ,
- {
-  name "Blepharisma Macronuclear" ,
-  id 15 ,
-  ncbieaa  "FFLLSSSSYY*QCC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
-  sncbieaa "-----------------------------------M----------------------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- } ,
- {
-  name "Chlorophycean Mitochondrial" ,
-  id 16 ,
-  ncbieaa  "FFLLSSSSYY*LCC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
-  sncbieaa "-----------------------------------M----------------------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- } ,
- {
-  name "Trematode Mitochondrial" ,
-  id 21 ,
-  ncbieaa  "FFLLSSSSYY**CCWWLLLLPPPPHHQQRRRRIIMMTTTTNNNKSSSSVVVVAAAADDEEGGGG",
-  sncbieaa "-----------------------------------M---------------M------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- } ,
- {
-  name "Scenedesmus obliquus Mitochondrial" ,
-  id 22 ,
-  ncbieaa  "FFLLSS*SYY*LCC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
-  sncbieaa "-----------------------------------M----------------------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- } ,
- {
-  name "Thraustochytrium Mitochondrial" ,
-  id 23 ,
-  ncbieaa  "FF*LSSSSYY**CC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
-  sncbieaa "--------------------------------M--M---------------M------------"
-  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
-  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
-  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
- }
-}
+--**************************************************************************
+--  This is the NCBI genetic code table
+--  Initial base data set from Andrzej Elzanowski while at PIR International
+--  Addition of Eubacterial and Alternative Yeast by J.Ostell at NCBI
+--  Base 1-3 of each codon have been added as comments to facilitate
+--    readability at the suggestion of Peter Rice, EMBL
+--  Later additions by Taxonomy Group staff at NCBI
+--
+--  Version 3.9
+--     Code 14 differs from code 9 only by translating UAA to Tyr rather than
+--     STOP.  A recent study (Telford et al, 2000) has found no evidence that
+--     the codon UAA codes for Tyr in the flatworms, but other opinions exist.
+--     There are very few GenBank records that are translated with code 14,
+--     but a test translation shows that retranslating these records with code
+--     9 can cause premature terminations.  Therefore, GenBank will maintain
+--     code 14 until further information becomes available.
+--
+--  Version 3.8
+--     Added GTG start to Echinoderm mitochondrial code, code 9
+--
+--  Version 3.7
+--     Added code 23 Thraustochytrium mitochondrial code
+--        formerly OGMP code 93
+--        submitted by Gertraude Berger, Ph.D.
+--
+--  Version 3.6
+--     Added code 22 TAG-Leu, TCA-stop
+--        found in mitochondrial DNA of Scenedesmus obliquus
+--        submitted by Gertraude Berger, Ph.D.
+--        Organelle Genome Megasequencing Program, Univ Montreal
+--
+--  Version 3.5
+--     Added code 21, Trematode Mitochondrial
+--       (as deduced from: Garey & Wolstenholme,1989; Ohama et al, 1990)
+--     Added code 16, Chlorophycean Mitochondrial
+--       (TAG can translated to Leucine instaed to STOP in chlorophyceans
+--        and fungi)
+--
+--  Version 3.4
+--     Added CTG,TTG as allowed alternate start codons in Standard code.
+--        Prats et al. 1989, Hann et al. 1992
+--
+--  Version 3.3 - 10/13/95
+--     Added alternate intiation codon ATC to code 5
+--        based on complete mitochondrial genome of honeybee
+--        Crozier and Crozier (1993)
+--
+--  Version 3.2 - 6/24/95
+--  Code       Comments
+--   10        Alternative Ciliate Macronuclear renamed to Euplotid Macro...
+--   15        Bleharisma Macro.. code added
+--    5        Invertebrate Mito.. GTG allowed as alternate initiator
+--   11        Eubacterial renamed to Bacterial as most alternate starts
+--               have been found in Achea
+--
+--
+--  Version 3.1 - 1995
+--  Updated as per Andrzej Elzanowski at NCBI
+--     Complete documentation in NCBI toolkit documentation
+--  Note: 2 genetic codes have been deleted
+--
+--   Old id   Use id     - Notes
+--
+--   id 7      id 4      - Kinetoplast code now merged in code id 4
+--   id 8      id 1      - all plant chloroplast differences due to RNA edit
+--
+--*************************************************************************
+
+Genetic-code-table ::= {
+ {
+  name "Standard" ,
+  name "SGC0" ,
+  id 1 ,
+  ncbieaa  "FFLLSSSSYY**CC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
+  sncbieaa "---M---------------M---------------M----------------------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ },
+ {
+  name "Vertebrate Mitochondrial" ,
+  name "SGC1" ,
+  id 2 ,
+  ncbieaa  "FFLLSSSSYY**CCWWLLLLPPPPHHQQRRRRIIMMTTTTNNKKSS**VVVVAAAADDEEGGGG",
+  sncbieaa "--------------------------------MMMM---------------M------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ },
+ {
+  name "Yeast Mitochondrial" ,
+  name "SGC2" ,
+  id 3 ,
+  ncbieaa  "FFLLSSSSYY**CCWWTTTTPPPPHHQQRRRRIIMMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
+  sncbieaa "----------------------------------MM----------------------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ },
+ {
+    name "Mold Mitochondrial; Protozoan Mitochondrial; Coelenterate
+ Mitochondrial; Mycoplasma; Spiroplasma" ,
+  name "SGC3" ,
+  id 4 ,
+  ncbieaa  "FFLLSSSSYY**CCWWLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
+  sncbieaa "--MM---------------M------------MMMM---------------M------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ },
+ {
+  name "Invertebrate Mitochondrial" ,
+  name "SGC4" ,
+  id 5 ,
+  ncbieaa  "FFLLSSSSYY**CCWWLLLLPPPPHHQQRRRRIIMMTTTTNNKKSSSSVVVVAAAADDEEGGGG",
+  sncbieaa "---M----------------------------MMMM---------------M------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ },
+ {
+  name "Ciliate Nuclear; Dasycladacean Nuclear; Hexamita Nuclear" ,
+  name "SGC5" ,
+  id 6 ,
+  ncbieaa  "FFLLSSSSYYQQCC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
+  sncbieaa "-----------------------------------M----------------------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ },
+ {
+  name "Echinoderm Mitochondrial; Flatworm Mitochondrial" ,
+  name "SGC8" ,
+  id 9 ,
+  ncbieaa  "FFLLSSSSYY**CCWWLLLLPPPPHHQQRRRRIIIMTTTTNNNKSSSSVVVVAAAADDEEGGGG",
+  sncbieaa "-----------------------------------M---------------M------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ },
+ {
+  name "Euplotid Nuclear" ,
+  name "SGC9" ,
+  id 10 ,
+  ncbieaa  "FFLLSSSSYY**CCCWLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
+  sncbieaa "-----------------------------------M----------------------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ },
+ {
+  name "Bacterial and Plant Plastid" ,
+  id 11 ,
+  ncbieaa  "FFLLSSSSYY**CC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
+  sncbieaa "---M---------------M------------MMMM---------------M------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ },
+ {
+  name "Alternative Yeast Nuclear" ,
+  id 12 ,
+  ncbieaa  "FFLLSSSSYY**CC*WLLLSPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
+  sncbieaa "-------------------M---------------M----------------------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ },
+ {
+  name "Ascidian Mitochondrial" ,
+  id 13 ,
+  ncbieaa  "FFLLSSSSYY**CCWWLLLLPPPPHHQQRRRRIIMMTTTTNNKKSSGGVVVVAAAADDEEGGGG",
+  sncbieaa "---M------------------------------MM---------------M------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ },
+ {
+  name "Alternative Flatworm Mitochondrial" ,
+  id 14 ,
+  ncbieaa  "FFLLSSSSYYY*CCWWLLLLPPPPHHQQRRRRIIIMTTTTNNNKSSSSVVVVAAAADDEEGGGG",
+  sncbieaa "-----------------------------------M----------------------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ } ,
+ {
+  name "Blepharisma Macronuclear" ,
+  id 15 ,
+  ncbieaa  "FFLLSSSSYY*QCC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
+  sncbieaa "-----------------------------------M----------------------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ } ,
+ {
+  name "Chlorophycean Mitochondrial" ,
+  id 16 ,
+  ncbieaa  "FFLLSSSSYY*LCC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
+  sncbieaa "-----------------------------------M----------------------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ } ,
+ {
+  name "Trematode Mitochondrial" ,
+  id 21 ,
+  ncbieaa  "FFLLSSSSYY**CCWWLLLLPPPPHHQQRRRRIIMMTTTTNNNKSSSSVVVVAAAADDEEGGGG",
+  sncbieaa "-----------------------------------M---------------M------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ } ,
+ {
+  name "Scenedesmus obliquus Mitochondrial" ,
+  id 22 ,
+  ncbieaa  "FFLLSS*SYY*LCC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
+  sncbieaa "-----------------------------------M----------------------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ } ,
+ {
+  name "Thraustochytrium Mitochondrial" ,
+  id 23 ,
+  ncbieaa  "FF*LSSSSYY**CC*WLLLLPPPPHHQQRRRRIIIMTTTTNNKKSSRRVVVVAAAADDEEGGGG",
+  sncbieaa "--------------------------------M--M---------------M------------"
+  -- Base1  TTTTTTTTTTTTTTTTCCCCCCCCCCCCCCCCAAAAAAAAAAAAAAAAGGGGGGGGGGGGGGGG
+  -- Base2  TTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGGTTTTCCCCAAAAGGGG
+  -- Base3  TCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAGTCAG
+ }
+}
```

### Comparing `lhc-python-2.5.0/lhc/filetools/filepool.py` & `lhc_python-2.5.1/src/lhc/io/filepool.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import errno
-import time
-
-
-class FilePool(object):
-    """A pool of files
-    
-    FilePool should be used if you think you might be opening more files than
-    allowed by the operating system (2048 on many systems). If too many files
-    are opened, this pool will close the one that was used the longest time
-    ago.
-    """
-    def __init__(self, mode='r'):
-        self.mode = mode
-        self.last_access = {}
-        self.files = {}
-    
-    def __contains__(self, key):
-        return key in self.files
-    
-    def __getitem__(self, key):
-        if key not in self.files or self.files[key].closed:
-            attempt = 0
-            opened = False
-            while attempt < 5:
-                try:
-                    mode = 'r' if self.mode == 'r' else 'a' if key in self.last_access else 'w'
-                    self.files[key] = open(key, mode, encoding='utf-8')
-                    opened = True
-                except IOError as e:
-                    if e.errno == errno.EMFILE:
-                        oldest = sorted(iter(self.last_access.items()), key=lambda x: x[1])[0][0]
-                        self.files[oldest].close()
-                    else:
-                        raise e
-                attempt += 1
-            if not opened:
-                raise IOError('Unable to open another file')
-        self.last_access[key] = time.time()
-        return self.files[key]
-    
-    def close(self, key=None):
-        if key is None:
-            for file in self.files.values():
-                file.close()
-        else:
-            self.files[key].close()
+import errno
+import time
+
+
+class FilePool(object):
+    """A pool of files
+    
+    FilePool should be used if you think you might be opening more files than
+    allowed by the operating system (2048 on many systems). If too many files
+    are opened, this pool will close the one that was used the longest time
+    ago.
+    """
+    def __init__(self, mode='r'):
+        self.mode = mode
+        self.last_access = {}
+        self.files = {}
+    
+    def __contains__(self, key):
+        return key in self.files
+    
+    def __getitem__(self, key):
+        if key not in self.files or self.files[key].closed:
+            attempt = 0
+            opened = False
+            while attempt < 5:
+                try:
+                    mode = 'r' if self.mode == 'r' else 'a' if key in self.last_access else 'w'
+                    self.files[key] = open(key, mode, encoding='utf-8')
+                    opened = True
+                except IOError as e:
+                    if e.errno == errno.EMFILE:
+                        oldest = sorted(iter(self.last_access.items()), key=lambda x: x[1])[0][0]
+                        self.files[oldest].close()
+                    else:
+                        raise e
+                attempt += 1
+            if not opened:
+                raise IOError('Unable to open another file')
+        self.last_access[key] = time.time()
+        return self.files[key]
+    
+    def close(self, key=None):
+        if key is None:
+            for file in self.files.values():
+                file.close()
+        else:
+            self.files[key].close()
```

### Comparing `lhc-python-2.5.0/lhc/graph/graph.py` & `lhc_python-2.5.1/src/lhc/graph/graph.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,175 +1,179 @@
-from collections import namedtuple
-
-Edge = namedtuple('Edge', ('fr', 'to'))
-
-
-class Vertex(object):
-    __slots__ = ('vertex', 'children', 'parents')
-
-    def __init__(self, vertex):
-        self.children = set()
-        self.parents = set()
-        self.vertex = vertex
-
-    def __iter__(self):
-        yield self.vertex
-        yield self.children
-        yield self.parents
-
-
-class Graph(object):
-    """
-    A graph with directed or undirected edges. Vertices must implement __hash__ and __eq__. Edges can not be labelled.
-    N-partite graphs can be used to label the edges.
-    """
-
-    __slots__ = ('name', 'adjacency', 'directed')
-
-    def __init__(self, es=list(), vs=list(), name=None, directed=True):
-        """
-        Initialise a graph
-
-        :param es: list of (from, to) pairs of existing edges
-        :param vs: list of vertex names (without edges)
-        :param name: name of the graph
-        :param directed: whether the graph is directed or not (default: True)
-        """
-        self.name = 'G' if name is None else name
-        self.adjacency = {}  # {vertex: (vertex, children, parents)}
-        self.directed = directed
-
-        for fr, to in es:
-            self.add_edge(fr, to)
-        for v in vs:
-            self.add_vertex(v)
-
-    @property
-    def es(self):
-        for vertex, children, parents in list(self.adjacency.values()):
-            for child in children:
-                yield Edge(vertex, child)
-
-    @property
-    def vs(self):
-        return list(self.adjacency.keys())
-
-    def __str__(self):
-        """
-        Represent graph in DOT format.
-        :return:
-        """
-        res = ['{} {} {{'.format('digraph' if self.directed else 'graph', self.name)]
-        for v, children, parents in sorted(self.adjacency.values()):
-            for child in children:
-                res.append('    "{}" -> "{}";'.format(v, child))
-        res.append('}')
-        return '\n'.join(res)
-
-    def __len__(self):
-        """
-        The number of vertices
-        :return:
-        """
-        return len(self.adjacency)
-
-    def __contains__(self, item):
-        return item in self.adjacency
-
-    def __delitem__(self, key):
-        vertex, children, parents = self.adjacency.pop(key)
-        for child in children:
-            self.adjacency[child].parents.remove(vertex)
-        for parent in parents:
-            self.adjacency[parent].children.remove(vertex)
-
-    def add_edge(self, fr, to):
-        """ Add an edge to the graph. Multiple edges between the same vertices will quietly be ignored. N-partite graphs
-        can be used to permit multiple edges by partitioning the graph into vertices and edges.
-
-        :param fr: The name of the origin vertex.
-        :param to: The name of the destination vertex.
-        :return:
-        """
-        fr = self.add_vertex(fr)
-        to = self.add_vertex(to)
-        self.adjacency[fr].children.add(to)
-        self.adjacency[to].parents.add(fr)
-
-    def add_vertex(self, v):
-        """
-        Add a vertex to the graph. The vertex must implement __hash__ and __eq__ as it will be stored in a set.
-        :param v: vertex
-        :return: graph owned vertex
-        """
-        if v not in self.adjacency:
-            self.adjacency[v] = Vertex(v)
-        return self.adjacency[v].vertex
-        
-    def get_children(self, v):
-        if v in self.adjacency:
-            return self.adjacency[v].children
-        return set()
-
-    def get_parents(self, v):
-        if v in self.adjacency:
-            return self.adjacency[v].parents
-        return set()
-
-    def get_neighbours(self, v):
-        if v in self.adjacency:
-            return self.adjacency[v].children | self.adjacency[v].parents
-        return set()
-
-    def get_descendants(self, v):
-        res = set()
-        if v not in self.adjacency:
-            return res
-        stk = list(self.get_children(v))
-        while len(stk) > 0:
-            top = stk.pop()
-            res.add(top)
-            stk.extend(self.get_children(top) - res)
-        return res
-
-    def get_ancestors(self, v):
-        res = set()
-        if v not in self.adjacency:
-            return res
-        stk = list(self.get_parents(v))
-        while len(stk) > 0:
-            top = stk.pop()
-            res.add(top)
-            stk.extend(self.get_parents(top) - res)
-        return res
-
-    def decompose(self, removed=None):
-        visited = set()
-        removed = set() if removed is None else removed
-        for vertex, children, parents in self.adjacency.values():
-            if vertex in visited or vertex in removed:
-                continue
-            graph = Graph(vs=[vertex], directed=self.directed)
-            stk = [vertex]
-            while len(stk) > 0:
-                vertex = stk.pop()
-                if vertex in visited or vertex in removed:
-                    continue
-                visited.add(vertex)
-                vertex, children, parents = self.adjacency[vertex]
-                for child in children:
-                    graph.add_edge(vertex, child)
-                stk.extend(self.get_neighbours(vertex) - visited - removed)
-            yield graph
-
-    def update(self, other):
-        for vertex in other.vs:
-            self.add_vertex(vertex)
-        for fr, to in other.es:
-            self.add_edge(fr, to)
-
-    def __getstate__(self):
-        return tuple(getattr(self, slot) for slot in self.__slots__)
-
-    def __setstate__(self, state):
-        for slot, slot_state in zip(self.__slots__, state):
-            setattr(self, slot, slot_state)
+from collections import namedtuple
+
+Edge = namedtuple('Edge', ('fr', 'to'))
+
+
+class Vertex(object):
+    __slots__ = ('vertex', 'children', 'parents')
+
+    def __init__(self, vertex):
+        self.children = set()
+        self.parents = set()
+        self.vertex = vertex
+
+    def __iter__(self):
+        yield self.vertex
+        yield self.children
+        yield self.parents
+
+
+class Graph(object):
+    """
+    A graph with directed or undirected edges. Vertices must implement __hash__ and __eq__. Edges can not be labelled.
+    N-partite graphs can be used to label the edges.
+    """
+
+    __slots__ = ('name', 'adjacency', 'directed')
+
+    def __init__(self, es=None, vs=None, name=None, directed=True):
+        """
+        Initialise a graph
+
+        :param es: list of (from, to) pairs of existing edges
+        :param vs: list of vertex names (without edges)
+        :param name: name of the graph
+        :param directed: whether the graph is directed or not (default: True)
+        """
+        if es is None:
+            es = list()
+        if vs is None:
+            vs = list()
+        self.name = 'G' if name is None else name
+        self.adjacency = {}  # {vertex: (vertex, children, parents)}
+        self.directed = directed
+
+        for fr, to in es:
+            self.add_edge(fr, to)
+        for v in vs:
+            self.add_vertex(v)
+
+    @property
+    def es(self):
+        for vertex, children, parents in list(self.adjacency.values()):
+            for child in children:
+                yield Edge(vertex, child)
+
+    @property
+    def vs(self):
+        return list(self.adjacency.keys())
+
+    def __str__(self):
+        """
+        Represent graph in DOT format.
+        :return:
+        """
+        res = ['{} {} {{'.format('digraph' if self.directed else 'graph', self.name)]
+        for v, children, parents in sorted(self.adjacency.values()):
+            for child in children:
+                res.append('    "{}" -> "{}";'.format(v, child))
+        res.append('}')
+        return '\n'.join(res)
+
+    def __len__(self):
+        """
+        The number of vertices
+        :return:
+        """
+        return len(self.adjacency)
+
+    def __contains__(self, item):
+        return item in self.adjacency
+
+    def __delitem__(self, key):
+        vertex, children, parents = self.adjacency.pop(key)
+        for child in children:
+            self.adjacency[child].parents.remove(vertex)
+        for parent in parents:
+            self.adjacency[parent].children.remove(vertex)
+
+    def add_edge(self, fr, to):
+        """ Add an edge to the graph. Multiple edges between the same vertices will quietly be ignored. N-partite graphs
+        can be used to permit multiple edges by partitioning the graph into vertices and edges.
+
+        :param fr: The name of the origin vertex.
+        :param to: The name of the destination vertex.
+        :return:
+        """
+        fr = self.add_vertex(fr)
+        to = self.add_vertex(to)
+        self.adjacency[fr].children.add(to)
+        self.adjacency[to].parents.add(fr)
+
+    def add_vertex(self, v):
+        """
+        Add a vertex to the graph. The vertex must implement __hash__ and __eq__ as it will be stored in a set.
+        :param v: vertex
+        :return: graph owned vertex
+        """
+        if v not in self.adjacency:
+            self.adjacency[v] = Vertex(v)
+        return self.adjacency[v].vertex
+        
+    def get_children(self, v):
+        if v in self.adjacency:
+            return self.adjacency[v].children
+        return set()
+
+    def get_parents(self, v):
+        if v in self.adjacency:
+            return self.adjacency[v].parents
+        return set()
+
+    def get_neighbours(self, v):
+        if v in self.adjacency:
+            return self.adjacency[v].children | self.adjacency[v].parents
+        return set()
+
+    def get_descendants(self, v):
+        res = set()
+        if v not in self.adjacency:
+            return res
+        stk = list(self.get_children(v))
+        while len(stk) > 0:
+            top = stk.pop()
+            res.add(top)
+            stk.extend(self.get_children(top) - res)
+        return res
+
+    def get_ancestors(self, v):
+        res = set()
+        if v not in self.adjacency:
+            return res
+        stk = list(self.get_parents(v))
+        while len(stk) > 0:
+            top = stk.pop()
+            res.add(top)
+            stk.extend(self.get_parents(top) - res)
+        return res
+
+    def decompose(self, removed=None):
+        visited = set()
+        removed = set() if removed is None else removed
+        for vertex, children, parents in self.adjacency.values():
+            if vertex in visited or vertex in removed:
+                continue
+            graph = Graph(vs=[vertex], directed=self.directed)
+            stk = [vertex]
+            while len(stk) > 0:
+                vertex = stk.pop()
+                if vertex in visited or vertex in removed:
+                    continue
+                visited.add(vertex)
+                vertex, children, parents = self.adjacency[vertex]
+                for child in children:
+                    graph.add_edge(vertex, child)
+                stk.extend(self.get_neighbours(vertex) - visited - removed)
+            yield graph
+
+    def update(self, other):
+        for vertex in other.vs:
+            self.add_vertex(vertex)
+        for fr, to in other.es:
+            self.add_edge(fr, to)
+
+    def __getstate__(self):
+        return tuple(getattr(self, slot) for slot in self.__slots__)
+
+    def __setstate__(self, state):
+        for slot, slot_state in zip(self.__slots__, state):
+            setattr(self, slot, slot_state)
```

### Comparing `lhc-python-2.5.0/lhc/graph/hyper_graph.py` & `lhc_python-2.5.1/src/lhc/graph/hyper_graph.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from .graph import Graph
-
-
-class HyperGraph(object):
-    def __init__(self, name=None):
-        self.name = 'G' if name is None else name
-        self.graph = Graph()
-        self.vs = set()
-        self.es = set()
-    
-    def __str__(self):
-        """ Convert to string
-
-        :return: A string representing the graph in Graphviz format.
-        """
-        res = ['digraph {} {{'.format(self.name)]
-        for e in sorted(self.es):
-            res.append('    {} [shape=box];'.format(e))
-        for e, vs in sorted(self.graph.es.items()):
-            for v in vs:
-                res.append('    "{}" -> "{}";'.format(*v))
-        res.append('}')
-        return '\n'.join(res)
-    
-    def add_vertex(self, v):
-        """ Add a vertex to the graph
-
-        :param v: The vertex name.
-        """
-        self.graph.add_vertex(v)
-        self.vs.add(v)
-
-    def add_outward_edge(self, v, e):
-        """ Add an outward edge to a vertex
-
-        :param v: The source vertex.
-        :param e: The name of the outward edge.
-        """
-        self.add_vertex(v)
-        self.graph.add_vertex(e)
-        self.es.add(e)
-        self.graph.add_edge(e, v)
-
-    def add_inward_edge(self, v, e):
-        """ Add an inward edge to a vertex
-
-        :param v: The destination vertex.
-        :param e: The name of the inward edge.
-        """
-        self.add_vertex(v)
-        self.graph.add_vertex(e)
-        self.es.add(e)
-        self.graph.add_edge(v, e)
-
-    def get_parents(self, n):
-        """ Get the parents of a vertex or edge.
-
-        :param n: A vertex or edge.
-        :return: The children of the given vertex or edge.
-        """
-        return self.graph.get_parents(n)
-
-    def get_children(self, n):
-        """ Get the children of a vertex or edge.
-
-        :param n: A vertex or edge.
-        :return: The children of the given vertex or edge.
-        """
-        return self.graph.get_children(n)
+from .graph import Graph
+
+
+class HyperGraph(object):
+    def __init__(self, name=None):
+        self.name = 'G' if name is None else name
+        self.graph = Graph()
+        self.vs = set()
+        self.es = set()
+    
+    def __str__(self):
+        """ Convert to string
+
+        :return: A string representing the graph in Graphviz format.
+        """
+        res = ['digraph {} {{'.format(self.name)]
+        for e in sorted(self.es):
+            res.append('    {} [shape=box];'.format(e))
+        for e, vs in sorted(self.graph.es.items()):
+            for v in vs:
+                res.append('    "{}" -> "{}";'.format(*v))
+        res.append('}')
+        return '\n'.join(res)
+    
+    def add_vertex(self, v):
+        """ Add a vertex to the graph
+
+        :param v: The vertex name.
+        """
+        self.graph.add_vertex(v)
+        self.vs.add(v)
+
+    def add_outward_edge(self, v, e):
+        """ Add an outward edge to a vertex
+
+        :param v: The source vertex.
+        :param e: The name of the outward edge.
+        """
+        self.add_vertex(v)
+        self.graph.add_vertex(e)
+        self.es.add(e)
+        self.graph.add_edge(e, v)
+
+    def add_inward_edge(self, v, e):
+        """ Add an inward edge to a vertex
+
+        :param v: The destination vertex.
+        :param e: The name of the inward edge.
+        """
+        self.add_vertex(v)
+        self.graph.add_vertex(e)
+        self.es.add(e)
+        self.graph.add_edge(v, e)
+
+    def get_parents(self, n):
+        """ Get the parents of a vertex or edge.
+
+        :param n: A vertex or edge.
+        :return: The children of the given vertex or edge.
+        """
+        return self.graph.get_parents(n)
+
+    def get_children(self, n):
+        """ Get the children of a vertex or edge.
+
+        :param n: A vertex or edge.
+        :return: The children of the given vertex or edge.
+        """
+        return self.graph.get_children(n)
```

### Comparing `lhc-python-2.5.0/lhc/interval/interval.py` & `lhc_python-2.5.1/src/lhc/entities/interval/interval.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,195 +1,185 @@
-from functools import total_ordering
-from collections import namedtuple
-from typing import Any, Tuple
-
-
-@total_ordering
-class Interval(object):
-
-    __slots__ = ('start', 'stop', 'data')
-
-    INTERVAL_PAIR = namedtuple('IntervalPair', ('left', 'right'))
-
-    def __init__(self, start, stop, *, data: Any = None):
-        self.start, self.stop = sorted((start, stop))
-        self.data = data
-
-    def __str__(self):
-        return '[{start!r}, {stop!r})'.format(start=self.start, stop=self.stop)
-    
-    def __len__(self):
-        return self.stop - self.start
-    
-    def __repr__(self):
-        return 'Interval{s}'.format(s=str(self))
-    
-    def __eq__(self, other):
-        return self.start == other.start and\
-            self.stop == other.stop
-    
-    def __lt__(self, other):
-        return self.stop < other.stop if self.start == other.start else self.start < other.start
-    
-    def __hash__(self):
-        return hash((self.start, self.stop))
-
-    def __contains__(self, item) -> bool:
-        """ Used for testing points
-
-        :param item: point for testing
-        :return: if the point is within the interval bounds
-        """
-        return self.start == item if self.start == self.stop else self.start <= item < self.stop
-        
-    # Relative location functions
-    
-    def overlaps(self, other) -> bool:
-        """Test if self and other overlap
-        
-        :param Interval other: the interval being tested
-        :rtype: bool
-        """
-        return self.start < other.stop and other.start < self.stop
-    
-    def contains(self, other) -> bool:
-        """Test if self wholly contains 
-    
-        :param Interval other: the interval being tested
-        :rtype: bool
-        """
-        return self.start <= other.start and other.stop <= self.stop
-    
-    def touches(self, other) -> bool:
-        """Test if self touches (but doesn't overlap) other
-        
-        :param Interval other: the interval being tested
-        :rtype: bool
-        """
-        return self.start == other.stop or self.stop == other.start
-    
-    # Set-like operation functions
-    
-    def union(self, other) -> 'Interval':
-        """Return the interval covering self and other if they overlap
-        
-        :param Interval other: the other interval
-        :rtype: Interval or None
-        """
-        return Interval(min(self.start, other.start),
-                        max(self.stop, other.stop))\
-            if self.overlaps(other) or self.touches(other) else None
-
-    def union_update(self, other):
-        if not self.overlaps(other):
-            raise ValueError('can not union non-overlapping intervals')
-        self.start = min(self.start, other.start)
-        self.stop = max(self.stop, other.stop)
-    
-    def intersect(self, other) -> 'Interval':
-        """Return an interval where self and other intersect
-        
-        :param Interval other: the other interval
-        :rtype: Interval or None 
-        """
-        return Interval(max(self.start, other.start),
-                        min(self.stop, other.stop))\
-            if self.overlaps(other) else None
-
-    def intersect_update(self, other):
-        if not self.overlaps(other):
-            raise ValueError('can not intersect non-overlapping intervals')
-        self.start = max(self.start, other.start)
-        self.stop = min(self.stop, other.stop)
-    
-    def difference(self, other) -> Tuple['Interval', 'Interval']:
-        """Return an interval that covers self but not other
-        
-        :param Interval other: interval to remove
-        :rtype: 2-tuple of interval or None
-        
-        If there is no overlap, the result is at .left and .right is None
-        If self is cut on the lower side, the result is at .right.
-        If self is cut on the upper side, the result is at .left.
-        If self is cut in the middle, the result in in both .left and .right
-        """
-        if not self.overlaps(other):
-            return Interval.INTERVAL_PAIR(self, None)
-        
-        left, right = None
-        if self.start < other.start:
-            left = Interval(self.start, other.start)
-        if other.stop < self.stop:
-            right = Interval(other.stop, self.stop)
-        return Interval.INTERVAL_PAIR(left, right)
-    
-    # Interval arithmetic functions
-    
-    def add(self, other) -> 'Interval':
-        """Return the arithmetic addition of self and other
-        
-        :param Interval other: the other interval
-        """
-        return Interval(self.start + other.start, self.stop + other.stop)
-    
-    def subtract(self, other) -> 'Interval':
-        """Return the arithmetic subtraction of self and other
-        
-        :param Interval other: the other interval
-        """
-        return Interval(self.start - other.stop, self.stop - other.start)
-    
-    def multiply(self, other):
-        """Return the arithmetic multiplication of self and other
-        
-        :param Interval other: the other interval
-        """
-        return Interval(min(self.start * other.start, self.start * other.stop,
-                            self.stop * other.start, self.stop * other.stop),
-                        max(self.start * other.start, self.start * other.stop,
-                            self.stop * other.start, self.stop * other.stop))
-    
-    def divide(self, other):
-        """Return the arithmetic division of self and other
-        
-        :param Interval other: the other interval
-        """
-        return Interval(min(self.start / other.start, self.start / other.stop,
-                            self.stop / other.start, self.stop / other.stop), 
-                        max(self.start / other.start, self.start / other.stop,
-                            self.stop / other.start, self.stop / other.stop))\
-            if other.start != 0 and other.stop != 0 else None
-    
-    # Position functions
-    
-    def get_abs_pos(self, pos):
-        """Get the absolute position of a position relative to a interval
-        
-        :param int pos: the position relative to the interval
-    
-        """
-        if pos < 0 or pos >= self.stop - self.start:
-            err = 'Relative position %d is not contained within %s'
-            raise IndexError(err)
-        return self.start + pos
-    
-    def get_rel_pos(self, pos):
-        """Get the position relative to a interval of a position.
-    
-        :param int pos: the position to calculate relative to the interval
-    
-        """
-        if pos < self.start or pos >= self.stop:
-            err = 'Absolute position {} is not contained within {}'
-            raise IndexError(err.format(pos, self))
-        return pos - self.start
-    
-    # Sequence functions
-    
-    def get_sub_seq(self, seq):
-        return seq[self.start:self.stop]
-
-    def __getstate__(self):
-        return self.start, self.stop, self.data
-
-    def __setstate__(self, state):
-        self.start, self.stop, self.data = state
+import dataclasses
+import functools
+
+from typing import Any, Optional
+
+
+@dataclasses.dataclass
+class IntervalPair:
+    left: Optional['Interval'] = None
+    right: Optional['Interval'] = None
+
+    def __iter__(self):
+        yield self.left
+        yield self.right
+
+
+@functools.total_ordering
+class Interval(object):
+
+    __slots__ = 'start', 'stop', 'data'
+
+    def __init__(self, start, stop, *, data: Any = None):
+        self.start, self.stop = sorted((start, stop))
+        self.data = data
+
+    def __str__(self) -> str:
+        return f'[{self.start}, {self.stop})'
+
+    def __repr__(self) -> str:
+        return f'Interval({self.start}, {self.stop})'
+    
+    def __len__(self) -> int:
+        return self.stop - self.start
+    
+    def __eq__(self, other: 'Interval') -> bool:
+        return self.start == other.start and self.stop == other.stop
+    
+    def __lt__(self, other: 'Interval') -> bool:
+        return self.stop < other.stop if self.start == other.start else self.start < other.start
+    
+    def __hash__(self) -> int:
+        return hash((self.start, self.stop))
+
+    def __contains__(self, item) -> bool:
+        return self.start <= item < self.stop if self.start != self.stop else self.start == item
+        
+    # Relative location functions
+
+    def overlaps(self, other: 'Interval') -> bool:
+        """Test if self overlaps other
+
+        :param Interval other: interval being tested
+        :rtype: bool
+        """
+        return self.start < other.stop and other.start < self.stop
+    
+    def contains(self, other: 'Interval') -> bool:
+        """Test if self wholly contains other
+
+        :param Interval other: interval being tested
+        :rtype: bool
+        """
+        return self.start <= other.start and other.stop <= self.stop
+    
+    def touches(self, other: 'Interval') -> bool:
+        """Test if self touches (but doesn't overlap) other
+
+        :param Interval other: interval being tested
+        :rtype: bool
+        """
+        return self.start == other.stop or self.stop == other.start
+    
+    # Set-like operation functions
+    
+    def union(self, other: 'Interval') -> Optional['Interval']:
+        """Return the interval covering self and other if they overlap
+
+        :param Interval other: interval to union with
+        :rtype: Interval or None
+        """
+        return Interval(min(self.start, other.start), max(self.stop, other.stop))\
+            if self.overlaps(other) or self.touches(other) else None
+    
+    def intersect(self, other: 'Interval') -> Optional['Interval']:
+        """Return an interval where self and other intersect
+
+        :param Interval other: interval to intersect with
+        :rtype: Interval or None 
+        """
+        return Interval(max(self.start, other.start), min(self.stop, other.stop))\
+            if self.overlaps(other) else None
+    
+    def difference(self, other: 'Interval') -> IntervalPair:
+        """Return an interval that covers self but not other
+
+        :param Interval other: interval to difference wit
+        :rtype: 2-tuple of interval or None
+        
+        If there is no overlap, the result is at .left and .right is None
+        If self is cut on the lower side, the result is at .right.
+        If self is cut on the upper side, the result is at .left.
+        If self is cut in the middle, the result in in both .left and .right
+        """
+        if not self.overlaps(other):
+            return IntervalPair(self)
+        
+        left, right = None, None
+        if self.start < other.start:
+            left = Interval(self.start, other.start)
+        if other.stop < self.stop:
+            right = Interval(other.stop, self.stop)
+        return IntervalPair(left, right)
+    
+    # Interval arithmetic functions
+    
+    def add(self, other: 'Interval') -> 'Interval':
+        """Return the arithmetic addition of self and other
+
+        :param Interval other: the other interval
+        """
+        return Interval(self.start + other.start, self.stop + other.stop)
+    
+    def subtract(self, other: 'Interval') -> 'Interval':
+        """Return the arithmetic subtraction of self and other
+        
+        :param Interval other: the other interval
+        """
+        return Interval(self.start - other.stop, self.stop - other.start)
+    
+    def multiply(self, other: 'Interval') -> 'Interval':
+        """Return the arithmetic multiplication of self and other
+        
+        :param Interval other: the other interval
+        """
+        return Interval(min(self.start * other.start, self.start * other.stop,
+                            self.stop * other.start, self.stop * other.stop),
+                        max(self.start * other.start, self.start * other.stop,
+                            self.stop * other.start, self.stop * other.stop))
+    
+    def divide(self, other: 'Interval') -> Optional['Interval']:
+        """Return the arithmetic division of self and other
+        
+        :param Interval other: the other interval
+        """
+        return Interval(min(self.start / other.start, self.start / other.stop,
+                            self.stop / other.start, self.stop / other.stop), 
+                        max(self.start / other.start, self.start / other.stop,
+                            self.stop / other.start, self.stop / other.stop))\
+            if other.start != 0 and other.stop != 0 else None
+    
+    # Position functions
+    
+    def get_abs_pos(self, pos: int) -> int:
+        """Get the absolute position of a position relative to a interval
+        
+        :param int pos: the position relative to the interval
+        """
+        if pos < 0 or pos >= self.stop - self.start:
+            raise IndexError(f'Relative position {pos} is not contained within {self}')
+        return self.start + pos
+    
+    def get_rel_pos(self, pos: int) -> int:
+        """Get the position relative to a interval of a position.
+    
+        :param int pos: the position to calculate relative to the interval
+        """
+        if pos < self.start or pos >= self.stop:
+            raise IndexError(f'Absolute position {pos} is not contained within {self}')
+        return pos - self.start
+    
+    # Sequence functions
+    
+    def get_sub_seq(self, seq: str) -> str:
+        """Get the subsequence
+
+        :param str seq: sequences to get subsequence from
+        :rtype: str
+        """
+        return seq[self.start:self.stop]
+
+    def __getstate__(self):
+        return self.start, self.stop, self.data
+
+    def __setstate__(self, state):
+        self.start, self.stop, self.data = state
```

### Comparing `lhc-python-2.5.0/lhc/io/cut.py` & `lhc_python-2.5.1/src/lhc/io/cut.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import re
-
-from collections import Counter
-
-
-class CodonUsageTable(Counter):
-
-    REGX = re.compile(r'(?P<codon>[ACGTU]{3})\s+(?P<frq>\d+\.\d+)\s+\((\s*\d+)\)')
-
-    def __init__(self, fname):
-        super(CodonUsageTable, self).__init__()
-        with open(fname, encoding='utf-8') as fileobj:
-            for line in fileobj:
-                matches = self.REGX.findall(line)
-                for match in matches:
-                    self[match[0].lower().replace('u', 't')] =\
-                        float(match[2])
+import re
+
+from collections import Counter
+
+
+class CodonUsageTable(Counter):
+
+    REGX = re.compile(r'(?P<codon>[ACGTU]{3})\s+(?P<frq>\d+\.\d+)\s+\((\s*\d+)\)')
+
+    def __init__(self, fname):
+        super(CodonUsageTable, self).__init__()
+        with open(fname, encoding='utf-8') as fileobj:
+            for line in fileobj:
+                matches = self.REGX.findall(line)
+                for match in matches:
+                    self[match[0].lower().replace('u', 't')] =\
+                        float(match[2])
```

### Comparing `lhc-python-2.5.0/lhc/io/fastq/tools/filter.py` & `lhc_python-2.5.1/src/lhc/cli/sequences/barcode_filter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,101 +1,103 @@
-import argparse
-import fileinput
-import gzip
-import os
-
-from multiprocessing import Process
-from lhc.io.fastq import iter_partial_fastq
-from lhc.misc.bitap import bitap_fuzzy
-
-
-class FilterJob(Process):
-    def __init__(
-        self,
-        input_streams,
-        output_streams,
-        filters,
-        mode,
-        group=None,
-        target=None,
-        name=None,
-        args=(),
-        kwargs={}
-    ):
-        super().__init__(group, target, name, args, kwargs)
-
-        self.input_streams = input_streams
-        self.output_streams = output_streams
-        self.filters = filters
-        self.mode = mode
-
-    def run(self):
-        for reads in filter(self.input_streams, self.filters, self.mode):
-            for read, output_stream in zip(reads, self.output_streams):
-                output_stream.write(str(read))
-
-
-def filter(input_streams, filters, mode='all'):
-    fn = all if mode == 'all' else\
-        any if mode == 'any' else\
-        None
-
-    for i, reads in enumerate(zip(*input_streams)):
-        if i % 10000 == 0:
-            print(i)
-        if fn(bitap_fuzzy(query, reads[index].seq, mismatches) is not None for query, mismatches, index in filters):
-            yield reads
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser() -> argparse.ArgumentParser:
-    return define_parser(argparse.ArgumentParser(
-        'Filters synchronised (eg. single-/paired-end) fastq files for the presence of any or all of the filter'
-        ' sequences. Consider using "agrep" instead.'))
-
-
-def define_parser(parser) -> argparse.ArgumentParser:
-    parser.add_argument('read_files', nargs='+')
-    parser.add_argument('-f', '--filter', dest='filters', nargs=3, action='append',
-                        metavar=('SEQUENCE', 'MISMATCHES', 'INDEX'), required=True)
-    parser.add_argument('-j', '--jobs', default=1, type=int)
-    parser.add_argument('-m', '--mode', choices=['all', 'any'], default='all')
-    parser.add_argument('-o', '--output-dir')
-    parser.set_defaults(func=init_filter)
-    return parser
-
-
-def init_filter(args):
-    filters = [(sequence, int(mismatches), int(index)) for sequence, mismatches, index in args.filters]
-
-    output_names = [read_file.rsplit('.', 2)[0] if read_file.endswith('.gz') else
-                    read_file.rsplit('.', 1)[0] for read_file in args.read_files]
-    if args.output_dir is not None:
-        output_names = [os.path.join(args.output_dir, os.path.basename(output_name))
-                        for output_name in output_names]
-
-    jobs = []
-    for i in range(args.jobs):
-        input_streams = [iter_partial_fastq(read_file, i / args.jobs, (i + 1) / args.jobs)
-                         for read_file in args.read_files]
-        output_streams = [open('{}.{}.filtered.fastq'.format(output_name, i), 'w')
-                          for output_name in output_names]
-        jobs.append(FilterJob(input_streams, output_streams, filters, args.mode))
-    for job in jobs:
-        job.start()
-    for job in jobs:
-        job.join()
-    for output_name in output_names:
-        output_stream = gzip.open('{}.filtered.fastq.gz'.format(output_name), 'w')
-        for line in fileinput.input(['{}.{}.filtered.fastq'.format(output_name, i) for i in range(args.jobs)]):
-            output_stream.write(line.encode('utf-8'))
-        for i in range(args.jobs):
-            os.remove('{}.{}.filtered.fastq'.format(output_name, i))
-
-
-if __name__ == '__main__':
-    import sys
-    sys.exit(main())
+import argparse
+import fileinput
+import gzip
+import os
+
+from multiprocessing import Process
+from lhc.io.sequence import open_sequence_file
+from lhc.misc.bitap import bitap_fuzzy
+
+
+class FilterJob(Process):
+    def __init__(
+        self,
+        input_streams,
+        output_streams,
+        filters,
+        mode,
+        group=None,
+        target=None,
+        name=None,
+        args=(),
+        kwargs={}
+    ):
+        super().__init__(group, target, name, args, kwargs)
+
+        self.input_streams = input_streams
+        self.output_streams = output_streams
+        self.filters = filters
+        self.mode = mode
+
+    def run(self):
+        for reads in filter(self.input_streams, self.filters, self.mode):
+            for read, output_stream in zip(reads, self.output_streams):
+                output_stream.write(str(read))
+
+
+def filter(input_streams, filters, mode='all'):
+    fn = all if mode == 'all' else\
+        any if mode == 'any' else\
+        None
+
+    for i, reads in enumerate(zip(*input_streams)):
+        if i % 10000 == 0:
+            print(i)
+        if fn(bitap_fuzzy(query, reads[index].seq, mismatches) is not None for query, mismatches, index in filters):
+            yield reads
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser() -> argparse.ArgumentParser:
+    return define_parser(argparse.ArgumentParser(get_description()))
+
+
+def get_description() -> str:
+    return 'Filters synchronised (eg. single-/paired-end) fastq files for the presence of any or all of the filter sequences. Consider using "agrep" instead.'
+
+
+def define_parser(parser) -> argparse.ArgumentParser:
+    parser.add_argument('read_files', nargs='+')
+    parser.add_argument('-f', '--filter', dest='filters', nargs=3, action='append',
+                        metavar=('SEQUENCE', 'MISMATCHES', 'INDEX'), required=True)
+    parser.add_argument('-j', '--jobs', default=1, type=int)
+    parser.add_argument('-m', '--mode', choices=['all', 'any'], default='all')
+    parser.add_argument('-o', '--output-dir')
+    parser.set_defaults(func=init_filter)
+    return parser
+
+
+def init_filter(args):
+    filters = [(sequence, int(mismatches), int(index)) for sequence, mismatches, index in args.filters]
+
+    output_names = [read_file.rsplit('.', 2)[0] if read_file.endswith('.gz') else
+                    read_file.rsplit('.', 1)[0] for read_file in args.read_files]
+    if args.output_dir is not None:
+        output_names = [os.path.join(args.output_dir, os.path.basename(output_name))
+                        for output_name in output_names]
+
+    jobs = []
+    for i in range(args.jobs):
+        input_streams = [open_sequence_file(read_file, fr=i / args.jobs, to=(i + 1) / args.jobs)
+                         for read_file in args.read_files]
+        output_streams = [open('{}.{}.filtered.fastq'.format(output_name, i), 'w')
+                          for output_name in output_names]
+        jobs.append(FilterJob(input_streams, output_streams, filters, args.mode))
+    for job in jobs:
+        job.start()
+    for job in jobs:
+        job.join()
+    for output_name in output_names:
+        output_stream = gzip.open('{}.filtered.fastq.gz'.format(output_name), 'w')
+        for line in fileinput.input(['{}.{}.filtered.fastq'.format(output_name, i) for i in range(args.jobs)]):
+            output_stream.write(line.encode('utf-8'))
+        for i in range(args.jobs):
+            os.remove('{}.{}.filtered.fastq'.format(output_name, i))
+
+
+if __name__ == '__main__':
+    import sys
+    sys.exit(main())
```

### Comparing `lhc-python-2.5.0/lhc/io/fastq/tools/split.py` & `lhc_python-2.5.1/src/lhc/cli/sequences/barcode_split.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,158 +1,161 @@
-import argparse
-import multiprocessing
-import os
-import sys
-
-from collections import Counter
-from lhc.binf.sequence.reverse_complement import reverse_complement
-from lhc.io.fasta import iter_fasta
-from lhc.io.fastq import iter_fastq
-from lhc.misc.string import hamming
-
-
-def split(args):
-    if args.output is None:
-        args.output = args.input.rsplit('.fastq', 1)[0]
-
-    forward_barcodes_ = [(hdr, seq.lower(), get_seeds(seq.lower(), args.seed_size))
-                         for hdr, seq in iter_fasta(args.barcodes)]
-    reverse_barcodes_ = [(hdr, reverse_complement(seq.lower()), get_seeds(reverse_complement(seq.lower()), args.seed_size))
-                         for hdr, seq in iter_fasta(args.barcodes)]
-    initargs = [forward_barcodes_, reverse_barcodes_, args.max_mismatch]
-    pool = multiprocessing.Pool(args.cpus, initializer=init_worker, initargs=initargs)
-
-    if hasattr(args, 'reverse_reads'):
-        split_paired(args.forward_reads, args.reverse_reads, pool, args.output, args.simultaneous_entries)
-    else:
-        split_single(args.forward_reads, pool, args.output, args.simultaneous_entries)
-
-
-def split_single(reads, pool, output, simultaneous_entries):
-    pool_iterator = iter_fastq(reads)
-    iterator = iter_fastq(reads)
-    out_fhndls = {}
-    for hdrs, entry in zip(pool.imap(find_barcodes_single, pool_iterator, simultaneous_entries), iterator):
-        for hdr in hdrs:
-            if hdr not in out_fhndls:
-                fname = '{}.fastq'.format(hdr)
-                out_fhndls[hdr] = open(os.path.join(output, fname), 'w')
-            out_fhndls[hdr].write(str(entry))
-            sys.exit(1)
-    for out_fhndl in out_fhndls.values():
-        out_fhndl.close()
-
-
-def split_paired(forward, reverse, pool, output, simultaneous_entries):
-    pool_iterator = zip(iter_fastq(forward), iter_fastq(reverse))
-    forward_iterator = iter_fastq(forward)
-    reverse_iterator = iter_fastq(reverse)
-    out_fhndls = {}
-    it = zip(pool.imap(find_barcodes_paired, pool_iterator, simultaneous_entries),
-                        forward_iterator,
-                        reverse_iterator)
-    cnt = Counter()
-    for hdrs, forward_entry, reverse_entry in it:
-        cnt[len(hdrs)] += 1
-        if len(hdrs) == 0:
-            hdrs = ['None']
-        for hdr in hdrs:
-            if hdr not in out_fhndls:
-                forward_fname = '{}.1.fastq'.format(hdr)
-                reverse_fname = '{}.2.fastq'.format(hdr)
-                forward_file = open(os.path.join(output, forward_fname), 'w')
-                reverse_file = open(os.path.join(output, reverse_fname), 'w')
-                out_fhndls[hdr] = (forward_file, reverse_file)
-            out_fhndls[hdr][0].write(str(forward_entry))
-            out_fhndls[hdr][1].write(str(reverse_entry))
-    for out_fhndl in out_fhndls.values():
-        out_fhndl[0].close()
-        out_fhndl[1].close()
-    for n_barcodes, n_reads in cnt.items():
-        print('{} reads had {} barcodes'.format(n_reads, n_barcodes))
- 
-
-def get_seeds(s, k):
-    return [s[i:i + k] for i in range(len(s) - k)]
-
-mismatch = 0
-forward_barcodes = None
-reverse_barcodes = None
-
-
-def init_worker(forward_barcodes_, reverse_barcodes_, mismatch_=0):
-    global mismatch
-    global forward_barcodes
-    global reverse_barcodes
-    
-    mismatch = mismatch_
-    forward_barcodes = forward_barcodes_
-    reverse_barcodes = reverse_barcodes_
-
-
-def find_barcodes_single(entry):
-    forward_hdrs = find_barcodes(entry, forward_barcodes)
-    reverse_hdrs = find_barcodes(entry, reverse_barcodes)
-    return sorted(set(forward_hdrs + reverse_hdrs))
-
-
-def find_barcodes_paired(entries):
-    forward, reverse = entries
-    forward_hdrs = find_barcodes(forward, forward_barcodes)
-    reverse_hdrs = find_barcodes(reverse, reverse_barcodes)
-    return sorted(set(forward_hdrs + reverse_hdrs))
-
-
-def find_barcodes(entry, barcodes):
-    template = entry.seq.lower()
-
-    ## String find
-    if mismatch == 0:
-        return [hdr for hdr, barcode, seeds in barcodes if template.find(barcode) >= 0]
-
-    ## Hamming with seed
-    hdrs = []
-    for hdr, barcode, seeds in barcodes:
-        for i, seed in enumerate(seeds):
-            try:
-                idx = template.index(seed)
-                d = hamming(template[idx - i:idx - i + len(barcode)], barcode)
-                if d <= mismatch:
-                    hdrs.append(hdr) 
-            except ValueError:
-                pass
-    return hdrs
- 
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser():
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser):
-    add_arg = parser.add_argument
-    add_arg('forward_reads',
-            help='Fastq containing forward reads.')
-    add_arg('reverse_reads', nargs='?',
-            help='Fastq containing reverse reads (optional).')
-    add_arg('barcodes',
-            help='Fasta file of barcode sequences')
-    add_arg('-c', '--cpus',
-            help='The number of cpus to use (default: all).')
-    add_arg('-k', '--seed-size', default=5,
-            help='The size of the seed (default: 5).')
-    add_arg('-m', '--max-mismatch', type=float, default=0,
-            help='The number of allowed mismatched (default: 1).')
-    add_arg('-s', '--simultaneous-entries', default=1000,
-            help='The number of entries to submit to each worker at a time (default: 1000).')
-    add_arg('-O', '--output',
-            help='The output directory.')
-    parser.set_defaults(func=split)
-    return parser
-
-
-if __name__ == '__main__':
-    sys.exit(main())
+import argparse
+import multiprocessing
+import os
+import sys
+
+from collections import Counter
+from lhc.entities.sequence.reverse_complement import reverse_complement
+from lhc.io.sequence import open_sequence_file
+from lhc.misc.string import hamming
+
+
+def split_single(reads, pool, output, simultaneous_entries):
+    pool_iterator = open_sequence_file(reads)
+    iterator = open_sequence_file(reads)
+    out_fhndls = {}
+    for hdrs, entry in zip(pool.imap(find_barcodes_single, pool_iterator, simultaneous_entries), iterator):
+        for hdr in hdrs:
+            if hdr not in out_fhndls:
+                fname = '{}.fastq'.format(hdr)
+                out_fhndls[hdr] = open(os.path.join(output, fname), 'w')
+            out_fhndls[hdr].write(str(entry))
+            sys.exit(1)
+    for out_fhndl in out_fhndls.values():
+        out_fhndl.close()
+
+
+def split_paired(forward, reverse, pool, output, simultaneous_entries):
+    pool_iterator = zip(open_sequence_file(forward), open_sequence_file(reverse))
+    forward_iterator = open_sequence_file(forward)
+    reverse_iterator = open_sequence_file(reverse)
+    out_fhndls = {}
+    it = zip(pool.imap(find_barcodes_paired, pool_iterator, simultaneous_entries),
+                        forward_iterator,
+                        reverse_iterator)
+    cnt = Counter()
+    for hdrs, forward_entry, reverse_entry in it:
+        cnt[len(hdrs)] += 1
+        if len(hdrs) == 0:
+            hdrs = ['None']
+        for hdr in hdrs:
+            if hdr not in out_fhndls:
+                forward_fname = '{}.1.fastq'.format(hdr)
+                reverse_fname = '{}.2.fastq'.format(hdr)
+                forward_file = open(os.path.join(output, forward_fname), 'w')
+                reverse_file = open(os.path.join(output, reverse_fname), 'w')
+                out_fhndls[hdr] = (forward_file, reverse_file)
+            out_fhndls[hdr][0].write(str(forward_entry))
+            out_fhndls[hdr][1].write(str(reverse_entry))
+    for out_fhndl in out_fhndls.values():
+        out_fhndl[0].close()
+        out_fhndl[1].close()
+    for n_barcodes, n_reads in cnt.items():
+        print('{} reads had {} barcodes'.format(n_reads, n_barcodes))
+ 
+
+def get_seeds(s, k):
+    return [s[i:i + k] for i in range(len(s) - k)]
+
+mismatch = 0
+forward_barcodes = None
+reverse_barcodes = None
+
+
+def init_worker(forward_barcodes_, reverse_barcodes_, mismatch_=0):
+    global mismatch
+    global forward_barcodes
+    global reverse_barcodes
+    
+    mismatch = mismatch_
+    forward_barcodes = forward_barcodes_
+    reverse_barcodes = reverse_barcodes_
+
+
+def find_barcodes_single(entry):
+    forward_hdrs = find_barcodes(entry, forward_barcodes)
+    reverse_hdrs = find_barcodes(entry, reverse_barcodes)
+    return sorted(set(forward_hdrs + reverse_hdrs))
+
+
+def find_barcodes_paired(entries):
+    forward, reverse = entries
+    forward_hdrs = find_barcodes(forward, forward_barcodes)
+    reverse_hdrs = find_barcodes(reverse, reverse_barcodes)
+    return sorted(set(forward_hdrs + reverse_hdrs))
+
+
+def find_barcodes(entry, barcodes):
+    template = entry.seq.lower()
+
+    ## String find
+    if mismatch == 0:
+        return [hdr for hdr, barcode, seeds in barcodes if template.find(barcode) >= 0]
+
+    ## Hamming with seed
+    hdrs = []
+    for hdr, barcode, seeds in barcodes:
+        for i, seed in enumerate(seeds):
+            try:
+                idx = template.index(seed)
+                d = hamming(template[idx - i:idx - i + len(barcode)], barcode)
+                if d <= mismatch:
+                    hdrs.append(hdr) 
+            except ValueError:
+                pass
+    return hdrs
+ 
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser():
+    return define_parser(argparse.ArgumentParser(get_description()))
+
+
+def get_description() -> str:
+    return 'Split sequences at the given subsequence.'
+
+
+def define_parser(parser):
+    add_arg = parser.add_argument
+    add_arg('forward_reads',
+            help='Fastq containing forward reads.')
+    add_arg('reverse_reads', nargs='?',
+            help='Fastq containing reverse reads (optional).')
+    add_arg('barcodes',
+            help='Fasta file of barcode sequences')
+    add_arg('-c', '--cpus',
+            help='The number of cpus to use (default: all).')
+    add_arg('-k', '--seed-size', default=5,
+            help='The size of the seed (default: 5).')
+    add_arg('-m', '--max-mismatch', type=float, default=0,
+            help='The number of allowed mismatched (default: 1).')
+    add_arg('-s', '--simultaneous-entries', default=1000,
+            help='The number of entries to submit to each worker at a time (default: 1000).')
+    add_arg('-O', '--output',
+            help='The output directory.')
+    parser.set_defaults(func=init_split)
+    return parser
+
+
+def init_split(args):
+    if args.output is None:
+        args.output = args.input.rsplit('.fastq', 1)[0]
+
+    forward_barcodes_ = [(hdr, seq.lower(), get_seeds(seq.lower(), args.seed_size))
+                         for hdr, seq in open_sequence_file(args.barcodes)]
+    reverse_barcodes_ = [(hdr, reverse_complement(seq.lower()), get_seeds(reverse_complement(seq.lower()), args.seed_size))
+                         for hdr, seq in open_sequence_file(args.barcodes)]
+    initargs = [forward_barcodes_, reverse_barcodes_, args.max_mismatch]
+    pool = multiprocessing.Pool(args.cpus, initializer=init_worker, initargs=initargs)
+
+    if hasattr(args, 'reverse_reads'):
+        split_paired(args.forward_reads, args.reverse_reads, pool, args.output, args.simultaneous_entries)
+    else:
+        split_single(args.forward_reads, pool, args.output, args.simultaneous_entries)
+
+
+if __name__ == '__main__':
+    sys.exit(main())
```

### Comparing `lhc-python-2.5.0/lhc/io/file.py` & `lhc_python-2.5.1/src/lhc/io/file.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import gzip
-import sys
-
-from contextlib import contextmanager
-from typing import Optional, IO
-
-
-@contextmanager
-def open_file(filename: Optional[str] = None, mode='r', encoding='utf-8') -> IO:
-    fileobj = sys.stdin if filename is None and 'r' in mode else \
-        sys.stderr if filename is None and 'e' in mode and 'w' in mode else \
-        sys.stdout if filename is None and 'w' in mode else \
-        gzip.open(filename, '{}t'.format(mode), encoding=encoding) if isinstance(filename, str) and filename.endswith('.gz') else \
-        open(filename, mode.replace('e', ''), encoding=encoding) if isinstance(filename, str) else \
-        filename
-    yield fileobj
-    fileobj.close()
+import gzip
+import sys
+
+from contextlib import contextmanager
+from typing import Optional, IO
+
+
+@contextmanager
+def open_file(filename: Optional[str] = None, mode='r', encoding='utf-8') -> IO:
+    fileobj = sys.stdin if filename is None and 'r' in mode else \
+        sys.stderr if filename is None and 'e' in mode and 'w' in mode else \
+        sys.stdout if filename is None and 'w' in mode else \
+        gzip.open(filename, '{}t'.format(mode), encoding=encoding) if isinstance(filename, str) and filename.endswith('.gz') else \
+        open(filename, mode.replace('e', ''), encoding=encoding) if isinstance(filename, str) else \
+        filename
+    yield fileobj
+    fileobj.close()
```

### Comparing `lhc-python-2.5.0/lhc/io/locus/__init__.py` & `lhc_python-2.5.1/src/lhc/io/locus/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from contextlib import contextmanager
-from typing import Optional
-from .locus_file import LocusFile
-from .bed import BedFile
-from .embl import EmblFile
-from .gbk import GbkFile
-from .gff import GffFile
-from .gtf import GtfFile
-from .paf import PafFile
-from .sam import SamFile
-from .region import RegionFile
-from .repeat_masker import RepeatMaskerFile
-
-
-def iter_loci(filename, *, encoding='utf-8', format: Optional[str] = None, index=1):
-    with open_locus_file(filename, encoding=encoding, format=format, index=index) as loci:
-        yield from loci
-
-
-@contextmanager
-def open_locus_file(filename: Optional[str], mode='r', *, encoding='utf-8', format: Optional[str] = None, index=1):
-    file = LocusFile.open_locus_file(filename, mode, encoding=encoding, format=format, index=index)
-    yield file
-    file.close()
-
-
-LocusFile.register_locus_file(BedFile)
-LocusFile.register_locus_file(EmblFile)
-LocusFile.register_locus_file(GbkFile)
-LocusFile.register_locus_file(GffFile)
-LocusFile.register_locus_file(GtfFile)
-LocusFile.register_locus_file(PafFile)
-LocusFile.register_locus_file(RegionFile)
-LocusFile.register_locus_file(RepeatMaskerFile)
+from contextlib import contextmanager
+from typing import Optional
+from .locus_file import LocusFile
+from .bed import BedFile
+from .embl import EmblFile
+from .gbk import GbkFile
+from .gff import GffFile
+from .gtf import GtfFile
+from .paf import PafFile
+from .sam import SamFile
+from .region import RegionFile
+from .repeat_masker import RepeatMaskerFile
+
+
+def iter_loci(filename, *, encoding='utf-8', format: Optional[str] = None, index=1):
+    with open_locus_file(filename, encoding=encoding, format=format, index=index) as loci:
+        yield from loci
+
+
+@contextmanager
+def open_locus_file(filename: Optional[str] = None, mode='r', *, encoding='utf-8', format: Optional[str] = None, index=1):
+    file = LocusFile.open_locus_file(filename, mode, encoding=encoding, format=format, index=index)
+    yield file
+    file.close()
+
+
+LocusFile.register_locus_file(BedFile)
+LocusFile.register_locus_file(EmblFile)
+LocusFile.register_locus_file(GbkFile)
+LocusFile.register_locus_file(GffFile)
+LocusFile.register_locus_file(GtfFile)
+LocusFile.register_locus_file(PafFile)
+LocusFile.register_locus_file(RegionFile)
+LocusFile.register_locus_file(RepeatMaskerFile)
```

### Comparing `lhc-python-2.5.0/lhc/io/locus/bed.py` & `lhc_python-2.5.1/src/lhc/io/locus/bed.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from .locus_file import GenomicInterval, LocusFile
-
-
-class BedFile(LocusFile):
-
-    EXTENSION = ('.bed', '.bed.gz')
-    FORMAT = 'bed'
-
-    def parse(self, line: str, index=1) -> GenomicInterval:
-        parts = line.rstrip('\r\n').split('\t')
-        name = parts[3] if len(parts) > 3 else ''
-        score = parts[4] if len(parts) > 4 else ''
-        strand = parts[5] if len(parts) > 5 else '+'
-        data = {'gene_id': name, 'score': score}
-        for col in parts[6:]:
-            data[col] = None
-        return GenomicInterval(int(parts[1]) - index, int(parts[2]),
-                               chromosome=parts[0],
-                               strand=strand,
-                               data=data)
-
-    def format(self, interval: GenomicInterval, index=1) -> str:
-        return '{chr}\t{start}\t{stop}\t{data[gene_id]}\t{score}\t{strand}{cols}'.format(
-            chr=interval.chromosome,
-            start=interval.start.position + index,
-            stop=interval.stop.position,
-            score=interval.data.get('score', '.'),
-            data=interval.data,
-            strand=interval.strand,
-            cols='\t' + '\t'.join(interval.data['cols']) if 'cols' in interval.data else '')
+from .locus_file import GenomicInterval, LocusFile
+
+
+class BedFile(LocusFile):
+
+    EXTENSION = ('.bed', '.bed.gz')
+    FORMAT = 'bed'
+
+    def parse(self, line: str, index=1) -> GenomicInterval:
+        parts = line.rstrip('\r\n').split('\t')
+        name = parts[3] if len(parts) > 3 else ''
+        score = parts[4] if len(parts) > 4 else ''
+        strand = parts[5] if len(parts) > 5 else '+'
+        data = {'gene_id': name, 'score': score}
+        for col in parts[6:]:
+            data[col] = None
+        return GenomicInterval(int(parts[1]) - index, int(parts[2]),
+                               chromosome=parts[0],
+                               strand=strand,
+                               data=data)
+
+    def format(self, interval: GenomicInterval, index=1) -> str:
+        return '{chr}\t{start}\t{stop}\t{data[gene_id]}\t{score}\t{strand}{cols}'.format(
+            chr=interval.chromosome,
+            start=interval.start.position + index,
+            stop=interval.stop.position,
+            score=interval.data.get('score', '.'),
+            data=interval.data,
+            strand=interval.strand,
+            cols='\t' + '\t'.join(interval.data['cols']) if 'cols' in interval.data else '')
```

### Comparing `lhc-python-2.5.0/lhc/io/locus/embl.py` & `lhc_python-2.5.1/src/lhc/io/locus/embl.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,128 +1,132 @@
-import string
-
-from .locus_file import LocusFile
-from lhc.binf.genomic_coordinate import GenomicPosition, NestedGenomicInterval
-from lhc.tools import Tokeniser, Token
-from typing import List, Optional
-
-
-class EmblFile(LocusFile):
-
-    EXTENSION = ('.embl', '.embl.gz')
-    FORMAT = 'embl'
-
-    def __init__(self, filename: Optional[str] = None, mode: str = 'r', encoding: str = 'utf-8', index=1):
-        super().__init__(filename, mode, encoding, index)
-        self.tokeniser = Tokeniser(
-            {
-                'digit': string.digits,
-                'word': string.ascii_letters + '_.^',
-                'bracket': '()',
-                'separator': ',:',
-                'unknown': '<>',
-            },
-            individual={'(', ')'}
-        )
-
-    def iter(self):
-        line = next(self.file)
-        while not line.startswith(';FT'):
-            line = next(self.file)
-        while line.startswith(';FT'):
-            raw_entry = [line]
-            while True:
-                line = next(self.file)
-                if len(line) < 7 or not line[6] == ' ':
-                    break
-                raw_entry.append(line)
-            yield raw_entry
-
-    def parse(self, lines: List[str], index=1) -> NestedGenomicInterval:
-        interval = self.parse_location(lines[0][20:].strip())
-        interval.data = self.parse_qualifiers(lines[1:])
-        return interval
-
-    def parse_location(self, location_definition: str) -> NestedGenomicInterval:
-        tokens = list(self.tokeniser.tokenise(location_definition))
-        return self.parse_nested_interval(tokens)
-
-    def parse_nested_interval(self, tokens: List[Token]) -> NestedGenomicInterval:
-        """ Parses a super range.
-         SuperRange ::= Interval | Join | Complement
-        """
-        if tokens[0].type in {'digit', 'unknown'}:
-            return self.parse_interval(tokens)
-        elif tokens[0].value in ['join', 'order']:
-            return self.parse_join(tokens)
-        elif tokens[0].value == 'complement':
-            return self.parse_complement(tokens)
-        elif tokens[1].value == ':':
-            chromosome = tokens.pop(0).value
-            tokens.pop(0)  # pop ':'
-            return self.parse_interval(tokens, chromosome=chromosome)
-        raise ValueError('interval {} does not fit pattern.'.format(tokens))
-
-    def parse_interval(self, tokens: List[Token], chromosome=None) -> NestedGenomicInterval:
-        """ Parses an interval
-         Range ::= <num> | <num> ('..' | '^' | '.') <num>
-        """
-        fr = self.parse_digit(tokens) - 1
-        if len(tokens) > 1 and tokens[0].value in {'..', '^', '.'}:
-            tokens.pop(0)  # Pop '..' | '^' | '.'
-            to = self.parse_digit(tokens)
-            return NestedGenomicInterval(fr, to, chromosome=chromosome)
-        return NestedGenomicInterval(fr, fr + 1, chromosome=chromosome)
-
-    def parse_digit(self, tokens: List[Token]) -> GenomicPosition:
-        token = tokens.pop(0)
-        if token.value in '<>':
-            token = tokens.pop(0)
-        return GenomicPosition(int(token.value))
-
-    def parse_join(self, tokens: List[Token]) -> NestedGenomicInterval:
-        """ Parses a join.
-         Join ::= 'join' '(' NestedInterval [',' NestedInterval] ')'
-        """
-        tokens.pop(0)  # Pop 'join'
-        tokens.pop(0)  # Pop '('
-        child = self.parse_nested_interval(tokens)
-        parent = NestedGenomicInterval(child.start.position, child.stop.position)
-        parent.add_child(child)
-        while tokens[0].value == ',':
-            tokens.pop(0)
-            parent.add_child(self.parse_nested_interval(tokens))
-        tokens.pop(0)  # Pop ')'
-        return parent
-
-    def parse_complement(self, tokens: List[Token]) -> NestedGenomicInterval:
-        """ Parses a complement
-         Complement ::= 'complement' '(' NestedInterval ')'
-        """
-        tokens.pop(0)  # Pop 'complement'
-        tokens.pop(0)  # Pop '('
-        res = self.parse_nested_interval(tokens)
-        res.switch_strand()
-        tokens.pop(0)  # Pop ')'
-        return res
-
-    def parse_qualifiers(self, lines):
-        qualifiers = {}
-        i = 0
-        while i < len(lines) and lines[i][20] == '/':
-            key, value = lines[i][21:].strip().split('=')
-            if value.startswith('"') and not value.endswith('"'):
-                values = [value]
-                while not values[-1].endswith('"'):
-                    i += 1
-                    values.append(lines[i][20:].strip())
-                value = ''.join(values)
-            i += 1
-            if value.startswith('"'):
-                value = value[1:-1]
-            elif value.isdigit():
-                value = int(value)
-            qualifiers[key] = value
-        return qualifiers
-
-    def format(self, interval: NestedGenomicInterval, index=1) -> str:
-        raise NotImplementedError()
+import string
+
+from .locus_file import LocusFile
+from lhc.entities.genomic_coordinate import GenomicPosition, NestedGenomicInterval
+from lhc.misc.tokeniser import Tokeniser, Token
+from typing import List, Optional
+
+
+class EmblFile(LocusFile):
+
+    EXTENSION = ('.embl', '.embl.gz')
+    FORMAT = 'embl'
+
+    def __init__(self, filename: Optional[str] = None, mode: str = 'r', encoding: str = 'utf-8', index=1):
+        super().__init__(filename, mode, encoding, index)
+        self.tokeniser = Tokeniser(
+            {
+                'digit': string.digits,
+                'word': string.ascii_letters + '_.^',
+                'bracket': '()',
+                'separator': ',:',
+                'unknown': '<>',
+            },
+            individual={'(', ')'}
+        )
+        self.id = None
+
+    def iter(self):
+        line = next(self.file)
+        while not line.startswith(';ID'):
+            line = next(self.file)
+        self.id = line.split()[1]
+        while not line.startswith(';FT'):
+            line = next(self.file)
+        while line.startswith(';FT'):
+            raw_entry = [line]
+            while True:
+                line = next(self.file)
+                if len(line) < 7 or not line[6] == ' ':
+                    break
+                raw_entry.append(line)
+            yield raw_entry
+
+    def parse(self, lines: List[str], index=1) -> NestedGenomicInterval:
+        interval = self.parse_location(lines[0][20:].strip())
+        interval.data = self.parse_qualifiers(lines)
+        return interval
+
+    def parse_location(self, location_definition: str) -> NestedGenomicInterval:
+        tokens = list(self.tokeniser.tokenise(location_definition))
+        return self.parse_nested_interval(tokens)
+
+    def parse_nested_interval(self, tokens: List[Token]) -> NestedGenomicInterval:
+        """ Parses a super range.
+         SuperRange ::= Interval | Join | Complement
+        """
+        if tokens[0].type in {'digit', 'unknown'}:
+            return self.parse_interval(tokens)
+        elif tokens[0].value in ['join', 'order']:
+            return self.parse_join(tokens)
+        elif tokens[0].value == 'complement':
+            return self.parse_complement(tokens)
+        elif tokens[1].value == ':':
+            chromosome = tokens.pop(0).value
+            tokens.pop(0)  # pop ':'
+            return self.parse_interval(tokens, chromosome=chromosome)
+        raise ValueError('interval {} does not fit pattern.'.format(tokens))
+
+    def parse_interval(self, tokens: List[Token], chromosome=None) -> NestedGenomicInterval:
+        """ Parses an interval
+         Range ::= <num> | <num> ('..' | '^' | '.') <num>
+        """
+        fr = self.parse_digit(tokens) - 1
+        if len(tokens) > 1 and tokens[0].value in {'..', '^', '.'}:
+            tokens.pop(0)  # Pop '..' | '^' | '.'
+            to = self.parse_digit(tokens)
+            return NestedGenomicInterval(fr, to, chromosome=chromosome if chromosome else self.id)
+        return NestedGenomicInterval(fr, fr + 1, chromosome=chromosome if chromosome else self.id)
+
+    def parse_digit(self, tokens: List[Token]) -> GenomicPosition:
+        token = tokens.pop(0)
+        if token.value in '<>':
+            token = tokens.pop(0)
+        return GenomicPosition(int(token.value), chromosome=self.id)
+
+    def parse_join(self, tokens: List[Token]) -> NestedGenomicInterval:
+        """ Parses a join.
+         Join ::= 'join' '(' NestedInterval [',' NestedInterval] ')'
+        """
+        tokens.pop(0)  # Pop 'join'
+        tokens.pop(0)  # Pop '('
+        child = self.parse_nested_interval(tokens)
+        parent = NestedGenomicInterval(child.start.position, child.stop.position, chromosome=self.id)
+        parent.add_child(child)
+        while tokens[0].value == ',':
+            tokens.pop(0)
+            parent.add_child(self.parse_nested_interval(tokens))
+        tokens.pop(0)  # Pop ')'
+        return parent
+
+    def parse_complement(self, tokens: List[Token]) -> NestedGenomicInterval:
+        """ Parses a complement
+         Complement ::= 'complement' '(' NestedInterval ')'
+        """
+        tokens.pop(0)  # Pop 'complement'
+        tokens.pop(0)  # Pop '('
+        res = self.parse_nested_interval(tokens)
+        res.switch_strand()
+        tokens.pop(0)  # Pop ')'
+        return res
+
+    def parse_qualifiers(self, lines):
+        qualifiers = {'feature': lines[0][3:20].strip()}
+        i = 1
+        while i < len(lines) and lines[i][20] == '/':
+            key, value = lines[i][21:].strip().split('=')
+            if value.startswith('"') and not value.endswith('"'):
+                values = [value]
+                while not values[-1].endswith('"'):
+                    i += 1
+                    values.append(lines[i][20:].strip())
+                value = ''.join(values)
+            i += 1
+            if value.startswith('"'):
+                value = value[1:-1]
+            elif value.isdigit():
+                value = int(value)
+            qualifiers[key] = value
+        return qualifiers
+
+    def format(self, interval: NestedGenomicInterval, index=1) -> str:
+        raise NotImplementedError()
```

### Comparing `lhc-python-2.5.0/lhc/io/locus/gff.py` & `lhc_python-2.5.1/src/lhc/io/locus/gtf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,45 @@
-from .locus_file import GenomicInterval, LocusFile
-
-
-class GffFile(LocusFile):
-
-    EXTENSION = ('.gff', '.gff.gz')
-    FORMAT = 'gff'
-
-    def parse(self, line: str, index=1) -> GenomicInterval:
-        parts = line.rstrip('\r\n').split('\t')
-        attributes = self.parse_attributes(parts[8])
-        attributes['source'] = parts[1],
-        attributes['feature'] = parts[2]
-        attributes['score'] = parts[5]
-        attributes['frame'] = parts[7]
-        return GenomicInterval(int(parts[3]) - index, int(parts[4]),
-                              chromosome=parts[0],
-                              strand=parts[6],
-                              data=attributes)
-
-    def format(self, interval: GenomicInterval, index=1) -> str:
-        attrs = {key: value for key, value in interval.data.items() if key not in {'source', 'feature', 'score', 'frame'}}
-        return '{chr}\t{data[source]}\t{data[feature]}\t{start}\t{stop}\t{data[score]}\t{strand}\t{data[frame]}\t{attrs}'.format(
-            chr=interval.chromosome,
-            start=interval.start.position + index,
-            stop=interval.stop.position,
-            strand=interval.strand,
-            data=interval.data,
-            attrs=';'.join('{}={}'.format(key, value) for key, value in attrs.items()))
-
-    @staticmethod
-    def parse_attributes(line):
-        attributes = {}
-        for part in line.split(';'):
-            if part:
-                key, value = part.split('=', 1) if '=' in part else part
-                attributes[key] = value.split(',')
-        return attributes
+from .locus_file import GenomicInterval, LocusFile
+
+
+class GtfFile(LocusFile):
+
+    EXTENSION = ('.gtf', '.gtf.gz')
+    FORMAT = 'gtf'
+
+    def parse(self, line: str, index=1) -> GenomicInterval:
+        parts = line.rstrip('\r\n').split('\t')
+        attributes = self.parse_attributes(parts[8])
+        attributes['source'] = parts[1]
+        attributes['feature'] = parts[2]
+        attributes['score'] = parts[5]
+        attributes['frame'] = parts[7]
+        return GenomicInterval(int(parts[3]) - index, int(parts[4]),
+                               chromosome=parts[0],
+                               strand=parts[6],
+                               data=attributes)
+
+    def format(self, interval: GenomicInterval, index=1) -> str:
+        attrs = {key: value for key, value in interval.data.items() if key not in {'source', 'feature', 'score', 'frame'}}
+        source = interval.data.get('source', 'unknown')
+        feature = interval.data.get('feature', 'exon')
+        score = interval.data.get('score', 0)
+        frame = interval.data.get('frame', 0)
+        return '{chr}\t{source}\t{feature}\t{start}\t{stop}\t{score}\t{strand}\t{frame}\t{attrs}'.format(
+            chr=interval.chromosome,
+            source=source,
+            feature=feature,
+            start=interval.start.position + index,
+            stop=interval.stop.position,
+            score=score,
+            strand=interval.strand,
+            frame=frame,
+            data=interval.data,
+            attrs='; '.join(key if value is None else '{} "{}"'.format(key, value) if isinstance(value, str) else '{} {}'.format(key, value) for key, value in attrs.items()))
+
+    @staticmethod
+    def parse_attributes(line):
+        parts = (part.strip() for part in line.split(';'))
+        parts = [part.split(' ', 1) for part in parts if part != '']
+        for part in parts:
+            part[1] = part[1][1:-1] if part[1].startswith('"') else int(part[1])
+        return dict(parts)
```

### Comparing `lhc-python-2.5.0/lhc/io/locus/gtf.py` & `lhc_python-2.5.1/src/lhc/io/locus/gff.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,38 @@
-from .locus_file import GenomicInterval, LocusFile
-
-
-class GtfFile(LocusFile):
-
-    EXTENSION = ('.gtf', '.gtf.gz')
-    FORMAT = 'gtf'
-
-    def parse(self, line: str, index=1) -> GenomicInterval:
-        parts = line.rstrip('\r\n').split('\t')
-        attributes = self.parse_attributes(parts[8])
-        attributes['source'] = parts[1]
-        attributes['feature'] = parts[2]
-        attributes['score'] = parts[5]
-        attributes['frame'] = parts[7]
-        return GenomicInterval(int(parts[3]) - index, int(parts[4]),
-                               chromosome=parts[0],
-                               strand=parts[6],
-                               data=attributes)
-
-    def format(self, interval: GenomicInterval, index=1) -> str:
-        attrs = {key: value for key, value in interval.data.items() if key not in {'source', 'feature', 'score', 'frame'}}
-        source = interval.data.get('source', 'unknown')
-        feature = interval.data.get('feature', 'exon')
-        score = interval.data.get('score', 0)
-        frame = interval.data.get('frame', 0)
-        return '{chr}\t{source}\t{feature}\t{start}\t{stop}\t{score}\t{strand}\t{frame}\t{attrs}'.format(
-            chr=interval.chromosome,
-            source=source,
-            feature=feature,
-            start=interval.start.position + index,
-            stop=interval.stop.position,
-            score=score,
-            strand=interval.strand,
-            frame=frame,
-            data=interval.data,
-            attrs='; '.join(key if value is None else '{} "{}"'.format(key, value) if isinstance(value, str) else '{} {}'.format(key, value) for key, value in attrs.items()))
-
-    @staticmethod
-    def parse_attributes(line):
-        parts = (part.strip() for part in line.split(';'))
-        parts = [part.split(' ', 1) for part in parts if part != '']
-        for part in parts:
-            part[1] = part[1][1:-1] if part[1].startswith('"') else int(part[1])
-        return dict(parts)
+from .locus_file import GenomicInterval, LocusFile
+
+
+class GffFile(LocusFile):
+
+    EXTENSION = ('.gff', '.gff.gz')
+    FORMAT = 'gff'
+
+    def parse(self, line: str, index=1) -> GenomicInterval:
+        parts = line.rstrip('\r\n').split('\t')
+        attributes = self.parse_attributes(parts[8])
+        attributes['source'] = parts[1],
+        attributes['feature'] = parts[2]
+        attributes['score'] = parts[5]
+        attributes['frame'] = parts[7]
+        return GenomicInterval(int(parts[3]) - index, int(parts[4]),
+                              chromosome=parts[0],
+                              strand=parts[6],
+                              data=attributes)
+
+    def format(self, interval: GenomicInterval, index=1) -> str:
+        attrs = {key: value for key, value in interval.data.items() if key not in {'source', 'feature', 'score', 'frame'}}
+        return '{chr}\t{data[source]}\t{data[feature]}\t{start}\t{stop}\t{data[score]}\t{strand}\t{data[frame]}\t{attrs}'.format(
+            chr=interval.chromosome,
+            start=interval.start.position + index,
+            stop=interval.stop.position,
+            strand=interval.strand,
+            data=interval.data,
+            attrs=';'.join('{}={}'.format(key, value) for key, value in attrs.items()))
+
+    @staticmethod
+    def parse_attributes(line):
+        attributes = {}
+        for part in line.split(';'):
+            if part:
+                key, value = part.split('=', 1) if '=' in part else part
+                attributes[key] = value.split(',')
+        return attributes
```

### Comparing `lhc-python-2.5.0/lhc/io/locus/locus_file.py` & `lhc_python-2.5.1/src/lhc/io/sequence/sequence_file.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,96 @@
-from typing import ClassVar, Dict, Iterator, Optional
-from lhc.binf.genomic_coordinate import GenomicInterval
-from lhc.io import open_file
-
-
-class LocusFile:
-
-    REGISTERED_EXTENSIONS = {}
-    REGISTERED_FORMATS = {}  # type: Dict[str, ClassVar['LocusFile']]
-
-    def __init__(self, filename: Optional[str] = None, mode: str = 'r', encoding: str = 'utf-8', index=1):
-        self.generator = None
-        if 'r' in mode or 'w' in mode:
-            self.generator = open_file(filename, mode, encoding)
-            self.file = self.generator.__enter__()
-        elif mode == 'q':
-            import pysam
-            self.file = pysam.TabixFile(filename)
-        else:
-            raise ValueError('Unrecognised open mode: {}'.format(mode))
-        self.mode = mode
-        self.encoding = encoding
-        self.index = index
-
-    def __iter__(self) -> Iterator[GenomicInterval]:
-        if self.mode == 'w':
-            raise ValueError('Locus file opened for writing, not reading.')
-        for raw_entry in self.iter():
-            yield self.parse(raw_entry, self.index)
-
-    def iter(self) -> Iterator[str]:
-        for line in self.file:
-            if line and not line.startswith('#'):
-                yield line
-
-    def fetch(self, locus: GenomicInterval) -> Iterator[GenomicInterval]:
-        if self.mode in 'rw':
-            raise ValueError('Loci file opened for reading or writing, not querying.')
-        return (self.parse(raw_entry, self.index) for raw_entry in
-                self.file.fetch(str(locus.chromosome), locus.start.position, locus.stop.position))
-
-    def write(self, locus: GenomicInterval):
-        if self.mode in 'rq':
-            raise ValueError('Locus file opened for reading or querying, not writing.')
-        self.file.write(self.format(locus, self.index))
-        self.file.write('\n')
-
-    def close(self):
-        if self.mode in 'rw':
-            self.file.close()
-
-    def parse(self, raw_entry: str, index=1) -> GenomicInterval:
-        raise NotImplementedError('This function must be implemented by the subclass.')
-
-    def format(self, locus: GenomicInterval) -> str:
-        raise NotImplementedError('This function must be implemented by the subclass.')
-
-    @classmethod
-    def register_locus_file(cls, loci_file: ClassVar['LocusFile']):
-        for extension in loci_file.EXTENSION:
-            cls.REGISTERED_EXTENSIONS[extension] = loci_file.FORMAT
-        cls.REGISTERED_FORMATS[loci_file.FORMAT] = loci_file
-
-    @classmethod
-    def open_locus_file(cls, filename: Optional[str], mode='r', *,
-                        encoding='utf-8', format: Optional[str] = None, index=1) -> 'LocusFile':
-        if filename is None and format is None:
-            raise ValueError('When reading from stdin or writing to stdout, the file format must be specified.'
-                             ' Valid formats are {}'.format(', '.join(cls.REGISTERED_FORMATS)))
-        if not format:
-            for extension, format in cls.REGISTERED_EXTENSIONS.items():
-                if filename.endswith(extension):
-                    break
-        if format not in cls.REGISTERED_FORMATS:
-            raise ValueError('Unknown loci file format: {}.'.format(format))
-        return cls.REGISTERED_FORMATS[format](filename, mode, encoding, index)
+import sys
+
+from typing import ClassVar, Dict, Iterator, Optional
+from lhc.cli.sequences import Sequence
+from lhc.io import open_file
+
+
+class SequenceFile:
+
+    REGISTERED_EXTENSIONS = {}
+    REGISTERED_FORMATS = {}  # type: Dict[str, ClassVar['SequenceFile']]
+
+    def __init__(self, filename: Optional[str] = None, mode: str = 'r', encoding: str = 'utf-8', *, fr: float = 0, to: float = 1):
+        if fr < 0 or fr > 1 or to < 0 or to > 1:
+            raise ValueError('fr and to must be between 0 and 1.')
+        elif fr >= to:
+            raise ValueError('fr must be less than to.')
+
+        if 'r' in mode or 'w' in mode:
+            import os
+            self.generator = open_file(filename, mode, encoding)
+            self.file = self.generator.__enter__()
+
+            if filename:
+                statinfo = os.stat(filename)
+                self.pos = self.seek(int(fr * statinfo.st_size))
+                self.to = int(to * statinfo.st_size)
+            else:
+                self.pos = 0
+                self.to = sys.maxsize
+        elif mode == 'q':
+            import pysam
+            self.file = pysam.FastaFile(filename)
+            self.fr = None
+            self.to = None
+        else:
+            raise ValueError('Unrecognised open mode: {}'.format(mode))
+        self.mode = mode
+        self.encoding = encoding
+
+    def __del__(self):
+        self.generator.__exit__(None, None, None)
+
+    def __iter__(self) -> Iterator[Sequence]:
+        if self.mode == 'w':
+            raise ValueError('Sequence file opened for writing not reading.')
+
+        return self.iter()
+
+    def write(self, sequence: Sequence):
+        if self.mode in 'rq':
+            raise ValueError('Sequence file opened for reading or querying, not writing.')
+        self.file.write(self.format(sequence))
+        self.file.write('\n')
+
+    def iter(self) -> Iterator[Sequence]:
+        raise NotImplementedError('This function must be implemented by the subclass.')
+
+    def format(self, sequence: Sequence) -> str:
+        raise NotImplementedError('This function must be implemented by the subclass.')
+
+    def fetch(self, chromosome, start=None, end=None):
+        if self.mode != 'q':
+            raise ValueError('sequences file not opened for querying')
+        return self.file.fetch(chromosome, start, end)
+
+    def seek(self, pos: int):
+        raise NotImplementedError('This function must be implemented by the subclass')
+
+    @classmethod
+    def register_sequence_file(cls, loci_file: ClassVar['SequenceFile']):
+        for extension in loci_file.EXTENSION:
+            cls.REGISTERED_EXTENSIONS[extension] = loci_file.FORMAT
+        cls.REGISTERED_FORMATS[loci_file.FORMAT] = loci_file
+
+    @classmethod
+    def open_sequence_file(
+        cls,
+        filename: Optional[str] = None,
+        mode='r',
+        *,
+        encoding='utf-8',
+        format: Optional[str] = None,
+        fr: float = 0,
+        to: float = 1,
+    ) -> 'SequenceFile':
+        if filename is None and format is None:
+            raise ValueError('When reading from stdin or writing to stdout, the file format must be specified.'
+                             ' Valid formats are {}'.format(', '.join(cls.REGISTERED_FORMATS)))
+        if not format:
+            for extension, format in cls.REGISTERED_EXTENSIONS.items():
+                if filename.endswith(extension):
+                    break
+        if format not in cls.REGISTERED_FORMATS:
+            raise ValueError('Unknown loci file format: {}.'.format(format))
+        return cls.REGISTERED_FORMATS[format](filename, mode, encoding, fr=fr, to=to)
```

### Comparing `lhc-python-2.5.0/lhc/io/locus/region.py` & `lhc_python-2.5.1/src/lhc/io/locus/region.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .locus_file import GenomicInterval, LocusFile
-
-
-class RegionFile(LocusFile):
-
-    EXTENSION = ('.txt', '.txt.gz')
-    FORMAT = 'region'
-
-    def parse(self, line: str, index=1) -> GenomicInterval:
-        chromosome, interval = line.split(':', 1)
-        start, stop = interval.split('-')
-        return GenomicInterval(int(start) - index, int(stop), chromosome=chromosome)
-
-    def format(self, interval: GenomicInterval, index=1) -> str:
-        return '{chr}:{start}-{stop}'.format(
-            chr=interval.chromosome,
-            start=interval.start.position + index,
-            stop=interval.stop.position)
+from .locus_file import GenomicInterval, LocusFile
+
+
+class RegionFile(LocusFile):
+
+    EXTENSION = ('.txt', '.txt.gz')
+    FORMAT = 'region'
+
+    def parse(self, line: str, index=1) -> GenomicInterval:
+        chromosome, interval = line.split(':', 1)
+        start, stop = interval.split('-')
+        return GenomicInterval(int(start) - index, int(stop), chromosome=chromosome)
+
+    def format(self, interval: GenomicInterval, index=1) -> str:
+        return '{chr}:{start}-{stop}'.format(
+            chr=interval.chromosome,
+            start=interval.start.position + index,
+            stop=interval.stop.position)
```

### Comparing `lhc-python-2.5.0/lhc/io/locus/repeat_masker.py` & `lhc_python-2.5.1/src/lhc/io/locus/repeat_masker.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from abc import ABC
-from collections import Counter
-from .locus_file import GenomicInterval, LocusFile
-
-
-class RepeatMaskerFile(LocusFile):
-
-    EXTENSION = ('.out', '.out.gz')
-    FORMAT = 'repeat_masker'
-
-    def __init__(self, filename: str, mode: str = 'r', encoding: str = 'utf-8', index=1):
-        super().__init__(filename, mode, encoding, index)
-        self.transcript_ids = Counter()
-        self.unknown_genes = 0
-        next(self.file)
-        next(self.file)
-        next(self.file)
-
-    def parse(self, line: str, index=1) -> GenomicInterval:
-        parts = line.rstrip('\r\n').split()
-        class_, *family = parts[10].split('/', 1)
-        try:
-            gene_id = parts[14]
-        except IndexError:
-            self.unknown_genes += 1
-            gene_id = 'unknown_{}'.format(self.unknown_genes)
-        transcript_id = '{}.1'.format(gene_id)
-        self.transcript_ids[transcript_id] += 1
-        exon_number = self.transcript_ids[transcript_id]
-        exon_id = '{}.{}'.format(transcript_id, exon_number)
-        return GenomicInterval(
-            int(parts[5]) - index,
-            int(parts[6]),
-            chromosome=parts[4],
-            strand='+' if parts[8] == '+' else '-',
-            data={'score': parts[0], 'divergence': parts[1], 'deletion': parts[2], 'insertion': parts[3],
-                  'subfamily_id': parts[9], 'class_id': class_, 'family_id': ''.join(family), 'gene_id': gene_id,
-                  'transcript_id': transcript_id, 'source': 'RepeatMasker', 'feature': 'repeat_element', 'frame': '0',
-                  'exon_id': exon_id, 'exon_number': exon_number})
+from abc import ABC
+from collections import Counter
+from .locus_file import GenomicInterval, LocusFile
+
+
+class RepeatMaskerFile(LocusFile):
+
+    EXTENSION = ('.out', '.out.gz')
+    FORMAT = 'repeat_masker'
+
+    def __init__(self, filename: str, mode: str = 'r', encoding: str = 'utf-8', index=1):
+        super().__init__(filename, mode, encoding, index)
+        self.transcript_ids = Counter()
+        self.unknown_genes = 0
+        next(self.file)
+        next(self.file)
+        next(self.file)
+
+    def parse(self, line: str, index=1) -> GenomicInterval:
+        parts = line.rstrip('\r\n').split()
+        class_, *family = parts[10].split('/', 1)
+        try:
+            gene_id = parts[14]
+        except IndexError:
+            self.unknown_genes += 1
+            gene_id = 'unknown_{}'.format(self.unknown_genes)
+        transcript_id = '{}.1'.format(gene_id)
+        self.transcript_ids[transcript_id] += 1
+        exon_number = self.transcript_ids[transcript_id]
+        exon_id = '{}.{}'.format(transcript_id, exon_number)
+        return GenomicInterval(
+            int(parts[5]) - index,
+            int(parts[6]),
+            chromosome=parts[4],
+            strand='+' if parts[8] == '+' else '-',
+            data={'score': parts[0], 'divergence': parts[1], 'deletion': parts[2], 'insertion': parts[3],
+                  'subfamily_id': parts[9], 'class_id': class_, 'family_id': ''.join(family), 'gene_id': gene_id,
+                  'transcript_id': transcript_id, 'source': 'RepeatMasker', 'feature': 'repeat_element', 'frame': '0',
+                  'exon_id': exon_id, 'exon_number': exon_number})
```

### Comparing `lhc-python-2.5.0/lhc/io/locus/sam.py` & `lhc_python-2.5.1/src/lhc/io/locus/sam.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from .locus_file import GenomicInterval, LocusFile
-
-
-class SamFile(LocusFile):
-
-    EXTENSION = ('.sam', '.sam.gz')
-    FORMAT = 'sam'
-
-    def parse(self, line: str, index=1) -> GenomicInterval:
-        query_name, flag, rname, pos, mapq, cigar, rnext, pnext, tlen, seq, qual, *parts = line.rstrip('\r\n').split('\t')
-        print(cigar)
-        return GenomicInterval(int(pos) - index, int(pos),
-                               chromosome=rname,
-                               strand=strand,
-                               data={'query_name': query_name,
-                                     'query_length': int(query_length),
-                                     'query_start': int(query_start) - index,
-                                     'query_end': int(query_end),
-                                     'target_length': int(target_length),
-                                     'matches': matches,
-                                     'block_length': block_length,
-                                     'mapping_quality': mapping_quality})
-
-    def format(self, interval: GenomicInterval, index=1) -> str:
-        return '{query_name}\t{query_length}\t{query_start}\t{query_end}\t{strand}\t{target_name}\t{target_length}\t{target_start}\t{target_end}\t{matches}\t{block_length}\t{mapping_quality}'.format(
-            query_name=interval.data['query_name'],
-            query_length=interval.data['query_length'],
-            query_start=interval.data['query_start'] + index,
-            query_end=interval.data['query_end'],
-            strand=interval.strand,
-            target_name=interval.chromosome,
-            target_length=interval.data['target_length'],
-            target_start=interval.start + index,
-            target_end=interval.stop,
-            matches=interval.data['matches'],
-            block_length=interval.data['block_length'],
-            mapping_quality=interval.data['mapping_quality'])
+from .locus_file import GenomicInterval, LocusFile
+
+
+class SamFile(LocusFile):
+
+    EXTENSION = ('.sam', '.sam.gz')
+    FORMAT = 'sam'
+
+    def parse(self, line: str, index=1) -> GenomicInterval:
+        query_name, flag, rname, pos, mapq, cigar, rnext, pnext, tlen, seq, qual, *parts = line.rstrip('\r\n').split('\t')
+        print(cigar)
+        return GenomicInterval(int(pos) - index, int(pos),
+                               chromosome=rname,
+                               strand=strand,
+                               data={'query_name': query_name,
+                                     'query_length': int(query_length),
+                                     'query_start': int(query_start) - index,
+                                     'query_end': int(query_end),
+                                     'target_length': int(tlen),
+                                     'matches': matches,
+                                     'block_length': block_length,
+                                     'mapping_quality': mapq})
+
+    def format(self, interval: GenomicInterval, index=1) -> str:
+        return '{query_name}\t{query_length}\t{query_start}\t{query_end}\t{strand}\t{target_name}\t{target_length}\t{target_start}\t{target_end}\t{matches}\t{block_length}\t{mapping_quality}'.format(
+            query_name=interval.data['query_name'],
+            query_length=interval.data['query_length'],
+            query_start=interval.data['query_start'] + index,
+            query_end=interval.data['query_end'],
+            strand=interval.strand,
+            target_name=interval.chromosome,
+            target_length=interval.data['target_length'],
+            target_start=interval.start + index,
+            target_end=interval.stop,
+            matches=interval.data['matches'],
+            block_length=interval.data['block_length'],
+            mapping_quality=interval.data['mapping_quality'])
```

### Comparing `lhc-python-2.5.0/lhc/io/maf/iterator.py` & `lhc_python-2.5.1/src/lhc/io/variant/maf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,29 @@
-import bz2
-import gzip
-
-from collections import namedtuple
-
-MafLine = namedtuple('MafLine', ('hugo_symbol', 'entrez_gene_id', 'center', 'ncbi_build', 'chromosome', 'start_position',
-                                 'end_position', 'strand', 'variant_classification', 'variant_type', 'reference_allele',
-                                 'tumour_seq_allele1', 'tumour_seq_allele2', 'dnsnp_rs', 'dbsnp_val_status',
-                                 'tumour_sample_barcode', 'matched_norm_sample_barcode', 'match_norm_seq_allele1',
-                                 'match_norm_seq_allele2', 'tumour_validation_allele1', 'tumour_validation_allele2',
-                                 'match_norm_validation_allele1', 'match_norm_validation_allele2',
-                                 'verification_status', 'validation_status', 'mutation_status', 'sequencing_phase',
-                                 'sequence_source', 'validation_method', 'score', 'bam_file', 'sequencer',
-                                 'tumour_sample_uuid', 'matched_norm_sample_uuid', 'cosmic_codon', 'cosmic_gene',
-                                 'transcript_id', 'exon', 'chrom_change', 'aa_change', 'genome_plus_minus_10_bp',
-                                 'drug_target', 'ttot_cov', 'tvar_cov', 'ntot_cov', 'nvar_cov', 'dbSNPPopFreq'))
-
-
-class MafIterator(object):
-    def __init__(self, fname):
-        self.line_no = 0
-        self.fname = fname
-        self.fhndl =\
-            gzip.open(fname) if fname.endswith('.gz') else\
-            bz2.BZ2File(fname) if fname.endswith('.bz2') else\
-            open(fname, encoding='utf-8')
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        line = self.fhndl.readline()
-        if line == '':
-            return()
-        self.line_no += 1
-        return MafLine(*line.rstrip('\r\n').split('\t'))
+from lhc.entities.variant import Variant
+from lhc.io.variant import VariantFile
+
+
+class MafFile(VariantFile):
+
+    EXTENSION = ('.maf',)
+    FORMAT = 'maf'
+
+    COLUMNS = ('hugo_symbol', 'entrez_gene_id', 'center', 'ncbi_build', 'chromosome', 'start_position',
+               'end_position', 'strand', 'variant_classification', 'variant_type', 'reference_allele',
+               'tumour_seq_allele1', 'tumour_seq_allele2', 'dnsnp_rs', 'dbsnp_val_status',
+               'tumour_sample_barcode', 'matched_norm_sample_barcode', 'match_norm_seq_allele1',
+               'match_norm_seq_allele2', 'tumour_validation_allele1', 'tumour_validation_allele2',
+               'match_norm_validation_allele1', 'match_norm_validation_allele2',
+               'verification_status', 'validation_status', 'mutation_status', 'sequencing_phase',
+               'sequence_source', 'validation_method', 'score', 'bam_file', 'sequencer',
+               'tumour_sample_uuid', 'matched_norm_sample_uuid', 'cosmic_codon', 'cosmic_gene',
+               'transcript_id', 'exon', 'chrom_change', 'aa_change', 'genome_plus_minus_10_bp',
+               'drug_target', 'ttot_cov', 'tvar_cov', 'ntot_cov', 'nvar_cov', 'dbSNPPopFreq')
+
+    FORMAT_STRING = '\t'.join('{{{}}}'.format(column) for column in COLUMNS)
+
+    def parse(self, line: str, index=1) -> Variant:
+        parts = line.rstrip('\r\n').split('\t')
+        return Variant(parts[4], int(parts[5]), parts[10], parts[11], info=dict(zip(self.COLUMNS, parts)))
+
+    def format(self, variant: Variant, index=1):
+        return ''.format(**variant.info)
```

### Comparing `lhc-python-2.5.0/lhc/io/sequence/__init__.py` & `lhc_python-2.5.1/src/lhc/io/sequence/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from contextlib import contextmanager
-from typing import Optional
-from .sequence_file import Sequence, SequenceFile
-from .embl import EmblFile
-from .fasta import FastaFile
-from .fastq import FastqFile
-
-
-def iter_sequences(filename, *, encoding='utf-8', format: Optional[str] = None):
-    with open_sequence_file(filename, encoding=encoding, format=format) as sequences:
-        yield from sequences
-
-
-@contextmanager
-def open_sequence_file(filename: Optional[str], mode='r', *, encoding='utf-8', format: Optional[str] = None):
-    file = SequenceFile.open_sequence_file(filename, mode, encoding=encoding, format=format)
-    yield file
-    file.close()
-
-
-SequenceFile.register_sequence_file(EmblFile)
-SequenceFile.register_sequence_file(FastaFile)
-SequenceFile.register_sequence_file(FastqFile)
+from contextlib import contextmanager
+from typing import Optional
+from .sequence_file import Sequence, SequenceFile
+from .embl import EmblFile
+from .fasta import FastaFile
+from .fastq import FastqFile
+
+
+def iter_sequences(filename, *, encoding='utf-8', format: Optional[str] = None):
+    with open_sequence_file(filename, encoding=encoding, format=format) as sequences:
+        yield from sequences
+
+
+@contextmanager
+def open_sequence_file(filename: Optional[str] = None, mode='r', *, encoding='utf-8', format: Optional[str] = None, fr: float = 0, to: float = 1):
+    file = SequenceFile.open_sequence_file(filename, mode, encoding=encoding, format=format, fr=fr, to=to)
+    yield file
+
+
+SequenceFile.register_sequence_file(EmblFile)
+SequenceFile.register_sequence_file(FastaFile)
+SequenceFile.register_sequence_file(FastqFile)
```

### Comparing `lhc-python-2.5.0/lhc/io/txt/tools/check_format.py` & `lhc_python-2.5.1/src/lhc/cli/variants/shift.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,47 @@
-import argparse
-import sys
-
-from ..entity_parser import EntityParser
-
-
-def check_format(input, format):
-    parser = EntityParser()
-    entity = parser.parse(format)
-
-    for i, line in enumerate(input):
-        parts = line.rstrip('\r\n').split('\t')
-        try:
-            entity(parts)
-        except Exception as e:
-            sys.stderr.write('Error parsing line number {}: {}\n'.format(i, e))
-            sys.exit(1)
-    sys.stdout.write('Check complete.\n')
-
-
-# CLI
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser():
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser):
-    add_arg = parser.add_argument
-
-    add_arg('input', nargs='?',
-            help='input file (default: stdin)')
-    add_arg('-f', '--format', default='s1',
-            help='format to check (default: s1)')
-    parser.set_defaults(func=init_check_format)
-
-    return parser
-
-
-def init_check_format(args):
-    with sys.stdin if args.input is None else open(args.input, encoding='utf-8') as input:
-        check_format(input, args.format)
-
-
-if __name__ == '__main__':
-    sys.exit(main())
+import argparse
+import sys
+
+from typing import Iterable
+from lhc.entities.variant import Variant
+from lhc.io.variant import open_variant_file, VariantFile
+
+
+def shift(variants: VariantFile, amount=0) -> Iterable[Variant]:
+    for variant in variants:
+        variant.pos += amount
+        yield variant
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser():
+    return define_parser(argparse.ArgumentParser(get_description()))
+
+
+def get_description() -> str:
+    return 'Shift the position of a set of variants.'
+
+
+def define_parser(parser):
+    parser.add_argument('input', nargs='?',
+                        help='name of the vcf_ file to be filtered (default: stdin).')
+    parser.add_argument('output', nargs='?',
+                        help='name of the filtered vcf_ file (default: stdout).')
+    parser.add_argument('-a', '--amount', type=int, default=0,
+                        help='amount to shift position by (default: none).')
+    parser.set_defaults(func=init_shift)
+    return parser
+
+
+def init_shift(args):
+    with open_variant_file(args.input) as input, open_variant_file(args.output, 'w') as output:
+        output.set_headers(input.headers, input.samples)
+        for line in shift(input, args.amount):
+            output.write(line)
+
+
+if __name__ == '__main__':
+    sys.exit(main())
```

### Comparing `lhc-python-2.5.0/lhc/io/variant/vcf.py` & `lhc_python-2.5.1/src/lhc/io/variant/vcf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,92 @@
-from collections import OrderedDict
-from typing import Any, Dict, Iterator
-from .variant_file import Variant, VariantFile
-
-
-class VcfFile(VariantFile):
-
-    EXTENSION = ('.vcf', '.vcf.gz')
-    FORMAT = 'vcf'
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.header = []
-        self.sample_names = []
-
-    def iter(self) -> Iterator[str]:
-        line = next(self.file)
-        while line.startswith('##'):
-            self.header.append(line)
-            line = next(self.file)
-        self.sample_names = line.strip().split('\t')[9:]
-        for line in self.file:
-            yield line
-
-    def parse(self, line: str, index=1) -> Variant:
-        parts = line.rstrip('\r\n').split('\t')
-        info = dict(i.split('=', 1) if '=' in i else (i, i) for i in parts[7].split(';'))
-        format = None if len(parts) < 9 else parts[8].split(':')
-        return Variant(
-            parts[0],
-            int(parts[1]) - 1,
-            parts[3],
-            parts[4].split(',')[0],
-            parts[2],
-            get_float(parts[5]),
-            parts[6].split(',')[0],
-            info,
-            format,
-            self.get_samples(parts[9:], format))
-
-    def format(self, variant: Variant, index=1) -> str:
-        return '{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\n'.format(
-            str(variant.chr),
-            variant.pos + index,
-            variant.id,
-            variant.ref,
-            ','.join(variant.alt),
-            '.' if variant.qual is None else variant.qual,
-            ','.join(variant.filter),
-            ':'.join('{}={}'.format(k, v) for k, v in variant.info.items()),
-            ':'.join(variant.format),
-            '\t'.join(self.format_sample(variant.samples[sample], variant.format)
-                      if sample in variant.samples
-                      else '.' for sample in variant.samples)
-        )
-
-    def get_samples(self, parts, format) -> Dict[str, Any]:
-        samples = {}
-        for name, part in zip(self.sample_names, parts):
-            samples[name] = {} if part == '.' else dict(zip(format, part.split(':')))
-        return samples
-
-    @staticmethod
-    def format_sample(sample, format):
-        return ':'.join(sample[key] for key in format)
-
-
-def get_header(iterator):
-    header = OrderedDict()
-    line = next(iterator)
-    while line.startswith('##'):
-        key, value = line[2:].strip().split('=', 1)
-        if key not in header:
-            header[key] = set()
-        header[key].add(value)
-        line = next(iterator)
-    samples = line.rstrip('\r\n').split('\t')[9:]
-    return header, samples
-
-
-def get_float(string):
-    try:
-        return float(string)
-    except:
-        pass
+from collections import OrderedDict
+from typing import Any, Dict
+from lhc.entities.variant import Variant
+from .variant_file import VariantFile
+
+
+class VcfFile(VariantFile):
+
+    EXTENSION = ('.vcf', '.vcf.gz')
+    FORMAT = 'vcf'
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if self.mode == 'r':
+            self.header, self.samples = self.get_header()
+        elif self.mode == 'w':
+            self.header, self.samples = None, None
+
+    def set_header(self, header, samples):
+        self.header = header
+        self.samples = samples
+        self.write_header()
+
+    def get_header(self):
+        header = OrderedDict()
+        line = next(self.file)
+        while line.startswith('##'):
+            key, value = line[2:].strip().split('=', 1)
+            if key not in header:
+                header[key] = set()
+            header[key].add(value)
+            line = next(self.file)
+        samples = line.rstrip('\r\n').split('\t')[9:]
+        return header, samples
+
+    def write_header(self):
+        for key, value in self.header.items():
+            self.file.write('##{}={}\n'.format(key, value))
+        self.file.write('#CHROM\tPOS\tID\tREF\tALT\tQUAL\tFILTER\tINFO')
+        if len(self.samples) > 0:
+            self.file.write('FORMAT\t{}'.format('\t'.join(self.samples)))
+        self.file.write('\n')
+
+    def parse(self, line: str, index=1) -> Variant:
+        parts = line.rstrip('\r\n').split('\t')
+        info = dict(i.split('=', 1) if '=' in i else (i, i) for i in parts[7].split(';'))
+        format_ = None if len(parts) < 9 else parts[8].split(':')
+        return Variant(
+            parts[0],
+            int(parts[1]) - 1,
+            parts[3],
+            parts[4].split(',')[0],
+            parts[2],
+            self.get_float(parts[5]),
+            parts[6].split(',')[0],
+            info,
+            format_,
+            self.get_samples(parts[9:], format_))
+
+    def format(self, variant: Variant, index=1) -> str:
+        return '{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}\n'.format(
+            str(variant.chr),
+            variant.pos + index,
+            variant.id,
+            variant.ref,
+            ','.join(variant.alt),
+            '.' if variant.qual is None else variant.qual,
+            ','.join(variant.filter),
+            ':'.join('{}={}'.format(k, v) for k, v in variant.info.items()),
+            ':'.join(variant.format),
+            '\t'.join(self.format_sample(variant.samples[sample], variant.format)
+                      if sample in variant.samples
+                      else '.' for sample in variant.samples)
+        )
+
+    def get_samples(self, parts, format_) -> Dict[str, Any]:
+        samples = {}
+        for name, part in zip(self.samples, parts):
+            samples[name] = {} if part == '.' else dict(zip(format_, part.split(':')))
+        return samples
+
+    @staticmethod
+    def format_sample(sample, format_):
+        return ':'.join(sample[key] for key in format_)
+
+    @staticmethod
+    def get_float(string):
+        try:
+            return float(string)
+        except ValueError:
+            pass
+        return None
```

### Comparing `lhc-python-2.5.0/lhc/io/vcf/merger.py` & `lhc_python-2.5.1/src/lhc/entities/variant/merger.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-import re
-
-from collections import OrderedDict, defaultdict, Counter
-from functools import reduce
-from operator import add, or_
-from typing import List
-from sortedcontainers import SortedDict
-from lhc.binf.genomic_coordinate import GenomicPosition as Position
-from lhc.io.vcf import VcfIterator
-
-
-class VcfMerger(object):
-    
-    CHR_REGX = re.compile('\d+$|X$|Y$|M$')
-
-    def __init__(self, iterators: List[VcfIterator], bams=None, variant_fields=None):
-        for i, iterator in enumerate(iterators):
-            if len(iterator.samples) == 0:
-                raise ValueError('Iterator #{} has no samples.'.format(i))
-        bams = bams if bams else []
-        self.iterators = iterators
-        hdrs = [it.header for it in self.iterators]
-        self.hdrs = self._merge_headers(hdrs)
-        self.samples = reduce(add, (it.samples for it in iterators))
-        self.iterator_samples = [it.samples for it in iterators]
-        if bams is None or len(bams) == 0:
-            self.bams = []
-            self.sample_to_bam = {}
-        else:
-            import pysam
-            self.bams = []
-            self.sample_to_bam = {}
-            for bam_name in bams:
-                bam = pysam.Samfile(bam_name)
-                sample = bam.header['RG'][0]['SM'].strip()
-                self.bams.append(bam)
-                self.sample_to_bam[sample] = bam
-        self.variant_fields = [] if variant_fields is None else variant_fields
-
-    def __iter__(self):
-        """ Iterate through merged vcf_ lines.
-
-        TODO: phased genotypes aren't handled
-        """
-        tops = [next(iterator) for iterator in self.iterators]
-        sorted_tops = self._init_sorting(tops)
-
-        while len(sorted_tops) > 0:
-            key, idxs = sorted_tops.popitem(last=False)
-
-            # REF
-            ref = sorted((tops[idx].data['ref'] for idx in idxs), key=lambda x: len(x))[-1]
-
-            # ALT
-            alt = set()
-            for idx in idxs:
-                top = tops[idx]
-                top_alt = [a + ref[len(top.data['ref']):] for a in top.data['alt']]
-                alt.update(top_alt)
-            alt = sorted(alt)
-
-            # QUAL
-            qual = None if any(tops[idx].data['qual'] is None for idx in idxs) else\
-                min(tops[idx].data['qual'] for idx in idxs)
-
-            # FILTER
-            filter = reduce(or_, (tops[idx].data['filter'] for idx in idxs))
-
-            # INFO
-            info = defaultdict(set)
-            for idx in idxs:
-                top = tops[idx]
-                for key, value in top.data['info'].items():
-                    info[key].add(value)
-            move_to_sample = set(key for key in info if len(info[key]) > 1)
-            move_to_sample.update(self.variant_fields)
-            format_ = {key: '' for key in move_to_sample}
-            for key, value in info.items():
-                if key in move_to_sample:
-                    for idx in idxs:
-                        for sample in self.iterator_samples[idx]:
-                            tops[idx].data['samples'].setdefault(sample, {})[key] = tops[idx].data['info'].get(key, '')
-                else:
-                    info[key] = list(value)[0]
-            for key in move_to_sample:
-                if key in info:
-                    del info[key]
-
-            samples = {}
-            for idx in idxs:
-                chromosome = str(tops[idxs[0]].chromosome)
-                samples.update(tops[idx].data['samples'])
-                for sample_name in self.iterator_samples[idx]:
-                    if sample_name in self.sample_to_bam:
-                        if 'GT' not in format_:
-                            format_['GT'] = '0/0'
-                        if 'RO' not in format_:
-                            format_['RO'] = '0'
-                        if 'AO' not in format_:
-                            format_['AO'] = ','.join('0' * len(alt))
-                        if 'AF' not in format_:
-                            format_['AF'] = '0'
-                        ro, aos = self._get_depth(sample_name, chromosome, tops[idxs[0]].position, ref, alt)
-                        samples[sample_name] = {'.': '.'} if ro is None else {
-                            'RO': ro,
-                            'AO': aos,
-                        }
-                        if ro is None or aos is None:
-                            continue
-                        ro = float(ro)
-                        aos = [float(ao) for ao in aos.split(',')]
-                        afs = [ao / (ro + ao) if ro + ao > 0 else 0 for ao in aos]
-                        samples[sample_name]['AF'] = ','.join('{:.3f}'.format(af) for af in afs)
-
-            for fmt, default in format_.items():
-                for sample in samples.values():
-                    if fmt not in sample:
-                        sample[fmt] = default
-
-            yield Position(tops[idxs[0]].position, chromosome=tops[idxs[0]].chromosome, data={
-                'id': tops[idxs[0]].data['id'],
-                'ref': ref,
-                'alt': alt,
-                'qual': qual,
-                'filter': filter,
-                'info': info,
-                'format': sorted(format_),
-                'samples': samples
-            })
-
-            for idx in idxs:
-                try:
-                    tops[idx] = next(self.iterators[idx])
-                    self._update_sorting(sorted_tops, tops[idx], idx)
-                except StopIteration:
-                    pass
-    
-    def _init_sorting(self, tops):
-        sorted_tops = SortedDict()
-        for idx, entry in enumerate(tops):
-            self._update_sorting(sorted_tops, entry, idx)
-        return sorted_tops
-    
-    def _update_sorting(self, sorted_tops, entry, idx):
-        if entry not in sorted_tops:
-            sorted_tops[entry] = []
-        sorted_tops[entry].append(idx)
-    
-    def _merge_headers(self, hdrs):
-        all_keys = defaultdict(list)
-        for hdr in hdrs:
-            for i, key in enumerate(hdr):
-                all_keys[key].append(i)
-        res = OrderedDict()
-        for k, v in sorted(iter(all_keys.items()), key=lambda item: sum(item[1])):
-            values = OrderedDict()
-            for hdr in hdrs:
-                if k in hdr:
-                    values.update((value, None) for value in hdr[k])
-            res[k] = list(values)
-        return res
-    
-    def _get_gt(self, gt, old_alt, new_alt):
-        try:
-            a1, a2 = list(map(int, gt.split('/')))
-        except ValueError:
-            return './.'
-        a1 = new_alt.index(old_alt[a1 - 1]) + 1 if 0 < a1 <= len(old_alt) else 0
-        a2 = new_alt.index(old_alt[a2 - 1]) + 1 if 0 < a2 <= len(old_alt) else 0
-        return '{}/{}'.format(a1, a2)
-    
-    def _get_ao(self, ao, old_alt, new_alt):
-        res = {k: v for k, v in zip(old_alt, ao.split(','))}
-        return ','.join(res[a] if a in res else '0' for a in new_alt)
-    
-    def _get_depth(self, sample, chr, pos, ref, alt):
-        bam = self.sample_to_bam[sample]
-        ref_start = pos
-        ref_stop = pos + len(ref)
-        cnt = Counter()
-        for read in bam.fetch(chr, ref_start, ref_stop):
-            read_start, read_stop, truncated =\
-                self._get_read_interval(read, ref_start, ref_stop)
-            alt_seq = read.seq[read_start:read_stop]
-            if truncated:  # assume reference
-                alt_seq += ref[len(alt_seq):]
-            cnt[alt_seq] += 1
-        if cnt[ref] == 0 and all(cnt[a] == 0 for a in alt):
-            return None, None
-        return str(cnt[ref]), ','.join(str(cnt[a]) for a in alt)
-    
-    def _get_read_interval(self, read, ref_start, ref_stop):
-        read_start = 0
-        ref_pos = 0
-        truncated = True
-        read_pos = read.qstart
-        for op, length in read.cigar:
-            read_ext = [1, 1, 0, 1, 1, 1, 1, 1, 1][op] * length
-            ref_ext = [1, 0, 1, 1, 1, 1, 1, 1, 1][op] * length
-            if read.pos + ref_pos + ref_ext > ref_start and read_start == 0:
-                read_start = read_pos + (ref_start - ref_pos - read.pos)
-            if read.pos + ref_pos + ref_ext > ref_stop:
-                truncated = False
-                break
-            read_pos += read_ext
-            ref_pos += ref_ext
-        read_stop = read_pos + (ref_stop - ref_pos - read.pos)
-        return read_start, read_stop, truncated
+import re
+
+from collections import OrderedDict, defaultdict, Counter
+from functools import reduce
+from operator import add, or_
+from typing import List
+from sortedcontainers import SortedDict
+from lhc.entities.genomic_coordinate import GenomicPosition as Position
+from lhc.io.variant import VariantFile
+
+
+class VariantMerger(object):
+    
+    CHR_REGX = re.compile('\d+$|X$|Y$|M$')
+
+    def __init__(self, iterators: List[VariantFile], bams=None, variant_fields=None):
+        for i, iterator in enumerate(iterators):
+            if len(iterator.samples) == 0:
+                raise ValueError('Iterator #{} has no samples.'.format(i))
+        bams = bams if bams else []
+        self.iterators = iterators
+        hdrs = [it.header for it in self.iterators]
+        self.hdrs = self._merge_headers(hdrs)
+        self.samples = reduce(add, (it.samples for it in iterators))
+        self.iterator_samples = [it.samples for it in iterators]
+        if bams is None or len(bams) == 0:
+            self.bams = []
+            self.sample_to_bam = {}
+        else:
+            import pysam
+            self.bams = []
+            self.sample_to_bam = {}
+            for bam_name in bams:
+                bam = pysam.Samfile(bam_name)
+                sample = bam.header['RG'][0]['SM'].strip()
+                self.bams.append(bam)
+                self.sample_to_bam[sample] = bam
+        self.variant_fields = [] if variant_fields is None else variant_fields
+
+    def __iter__(self):
+        """ Iterate through merged vcf_ lines.
+
+        TODO: phased genotypes aren't handled
+        """
+        tops = [next(iterator) for iterator in self.iterators]
+        sorted_tops = self._init_sorting(tops)
+
+        while len(sorted_tops) > 0:
+            key, idxs = sorted_tops.popitem(last=False)
+
+            # REF
+            ref = sorted((tops[idx].data['ref'] for idx in idxs), key=lambda x: len(x))[-1]
+
+            # ALT
+            alt = set()
+            for idx in idxs:
+                top = tops[idx]
+                top_alt = [a + ref[len(top.data['ref']):] for a in top.data['alt']]
+                alt.update(top_alt)
+            alt = sorted(alt)
+
+            # QUAL
+            qual = None if any(tops[idx].data['qual'] is None for idx in idxs) else\
+                min(tops[idx].data['qual'] for idx in idxs)
+
+            # FILTER
+            filter = reduce(or_, (tops[idx].data['filter'] for idx in idxs))
+
+            # INFO
+            info = defaultdict(set)
+            for idx in idxs:
+                top = tops[idx]
+                for key, value in top.data['info'].items():
+                    info[key].add(value)
+            move_to_sample = set(key for key in info if len(info[key]) > 1)
+            move_to_sample.update(self.variant_fields)
+            format_ = {key: '' for key in move_to_sample}
+            for key, value in info.items():
+                if key in move_to_sample:
+                    for idx in idxs:
+                        for sample in self.iterator_samples[idx]:
+                            tops[idx].data['samples'].setdefault(sample, {})[key] = tops[idx].data['info'].get(key, '')
+                else:
+                    info[key] = list(value)[0]
+            for key in move_to_sample:
+                if key in info:
+                    del info[key]
+
+            samples = {}
+            for idx in idxs:
+                chromosome = str(tops[idxs[0]].chromosome)
+                samples.update(tops[idx].data['samples'])
+                for sample_name in self.iterator_samples[idx]:
+                    if sample_name in self.sample_to_bam:
+                        if 'GT' not in format_:
+                            format_['GT'] = '0/0'
+                        if 'RO' not in format_:
+                            format_['RO'] = '0'
+                        if 'AO' not in format_:
+                            format_['AO'] = ','.join('0' * len(alt))
+                        if 'AF' not in format_:
+                            format_['AF'] = '0'
+                        ro, aos = self._get_depth(sample_name, chromosome, tops[idxs[0]].position, ref, alt)
+                        samples[sample_name] = {'.': '.'} if ro is None else {
+                            'RO': ro,
+                            'AO': aos,
+                        }
+                        if ro is None or aos is None:
+                            continue
+                        ro = float(ro)
+                        aos = [float(ao) for ao in aos.split(',')]
+                        afs = [ao / (ro + ao) if ro + ao > 0 else 0 for ao in aos]
+                        samples[sample_name]['AF'] = ','.join('{:.3f}'.format(af) for af in afs)
+
+            for fmt, default in format_.items():
+                for sample in samples.values():
+                    if fmt not in sample:
+                        sample[fmt] = default
+
+            yield Position(tops[idxs[0]].position, chromosome=tops[idxs[0]].chromosome, data={
+                'id': tops[idxs[0]].data['id'],
+                'ref': ref,
+                'alt': alt,
+                'qual': qual,
+                'filter': filter,
+                'info': info,
+                'format': sorted(format_),
+                'samples': samples
+            })
+
+            for idx in idxs:
+                try:
+                    tops[idx] = next(self.iterators[idx])
+                    self._update_sorting(sorted_tops, tops[idx], idx)
+                except StopIteration:
+                    pass
+    
+    def _init_sorting(self, tops):
+        sorted_tops = SortedDict()
+        for idx, entry in enumerate(tops):
+            self._update_sorting(sorted_tops, entry, idx)
+        return sorted_tops
+    
+    def _update_sorting(self, sorted_tops, entry, idx):
+        if entry not in sorted_tops:
+            sorted_tops[entry] = []
+        sorted_tops[entry].append(idx)
+    
+    def _merge_headers(self, hdrs):
+        all_keys = defaultdict(list)
+        for hdr in hdrs:
+            for i, key in enumerate(hdr):
+                all_keys[key].append(i)
+        res = OrderedDict()
+        for k, v in sorted(iter(all_keys.items()), key=lambda item: sum(item[1])):
+            values = OrderedDict()
+            for hdr in hdrs:
+                if k in hdr:
+                    values.update((value, None) for value in hdr[k])
+            res[k] = list(values)
+        return res
+    
+    def _get_gt(self, gt, old_alt, new_alt):
+        try:
+            a1, a2 = list(map(int, gt.split('/')))
+        except ValueError:
+            return './.'
+        a1 = new_alt.index(old_alt[a1 - 1]) + 1 if 0 < a1 <= len(old_alt) else 0
+        a2 = new_alt.index(old_alt[a2 - 1]) + 1 if 0 < a2 <= len(old_alt) else 0
+        return '{}/{}'.format(a1, a2)
+    
+    def _get_ao(self, ao, old_alt, new_alt):
+        res = {k: v for k, v in zip(old_alt, ao.split(','))}
+        return ','.join(res[a] if a in res else '0' for a in new_alt)
+    
+    def _get_depth(self, sample, chr, pos, ref, alt):
+        bam = self.sample_to_bam[sample]
+        ref_start = pos
+        ref_stop = pos + len(ref)
+        cnt = Counter()
+        for read in bam.fetch(chr, ref_start, ref_stop):
+            read_start, read_stop, truncated =\
+                self._get_read_interval(read, ref_start, ref_stop)
+            alt_seq = read.seq[read_start:read_stop]
+            if truncated:  # assume reference
+                alt_seq += ref[len(alt_seq):]
+            cnt[alt_seq] += 1
+        if cnt[ref] == 0 and all(cnt[a] == 0 for a in alt):
+            return None, None
+        return str(cnt[ref]), ','.join(str(cnt[a]) for a in alt)
+    
+    def _get_read_interval(self, read, ref_start, ref_stop):
+        read_start = 0
+        ref_pos = 0
+        truncated = True
+        read_pos = read.qstart
+        for op, length in read.cigar:
+            read_ext = [1, 1, 0, 1, 1, 1, 1, 1, 1][op] * length
+            ref_ext = [1, 0, 1, 1, 1, 1, 1, 1, 1][op] * length
+            if read.pos + ref_pos + ref_ext > ref_start and read_start == 0:
+                read_start = read_pos + (ref_start - ref_pos - read.pos)
+            if read.pos + ref_pos + ref_ext > ref_stop:
+                truncated = False
+                break
+            read_pos += read_ext
+            ref_pos += ref_ext
+        read_stop = read_pos + (ref_stop - ref_pos - read.pos)
+        return read_start, read_stop, truncated
```

### Comparing `lhc-python-2.5.0/lhc/itertools/sorted_iterator_merger.py` & `lhc_python-2.5.1/src/lhc/itertools/sorted_iterator_merger.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from sortedcontainers import SortedDict
-from typing import List, Iterator, TypeVar
-
-T = TypeVar('T')
-
-
-class SortedIteratorMerger(object):
-    """ Merges several sorted iterators into one sorted iterator.
-    """
-
-    def __init__(self, iterators : List[Iterator[T]], key=None):
-        """ Initialise the SortedIteratorMerger.
-
-        :param iterators: The iterators to merge.
-        :param key: A function that converts the iterator entries into comparable keys.
-        :return: A SortedIteratorMerger
-        """
-        n_iterators = len(iterators)
-        self.iterators = iterators
-        self.sorted_tops = SortedDict()
-        self.tops = n_iterators * [None]
-        self.idxs = list(range(n_iterators))
-        self.c_idx = 0
-        self.key = (lambda x: x) if key is None else key
-
-        self._update_sorting()
-
-    def __iter__(self):
-        return self
-
-    def __next__(self) -> List[T]:
-        if self.c_idx == len(self.idxs):
-            self._update_sorting()
-        res = self.tops[self.idxs[self.c_idx]]
-        self.c_idx += 1
-        return res
-
-    def close(self):
-        """
-        Closes all the iterators.
-
-        This is particularly important if the iterators are files.
-        """
-        if hasattr(self, 'iterators'):
-            for it in self.iterators:
-                if hasattr(it, 'close'):
-                    it.close()
-
-    def _update_sorting(self):
-        """ Insert new entries into the merged iterator.
-
-        :param sorted_tops: A SortedDict.
-        :param tops: The most recent entry from each iterator.
-        :param idxs: The indices to update.
-        """
-        key = self.key
-        sorted_tops = self.sorted_tops
-        tops = self.tops
-        iterators = self.iterators
-        for idx in self.idxs:
-            try:
-                tops[idx] = next(iterators[idx])
-                top_key = key(tops[idx])
-                if top_key not in sorted_tops:
-                    sorted_tops[top_key] = []
-                sorted_tops[top_key].append(idx)
-            except StopIteration:
-                pass
-        if len(sorted_tops) == 0:
-            raise StopIteration
-        key, self.idxs = sorted_tops.popitem(0)
-        self.c_idx = 0
+from sortedcontainers import SortedDict
+from typing import List, Iterator, TypeVar
+
+T = TypeVar('T')
+
+
+class SortedIteratorMerger(object):
+    """ Merges several sorted iterators into one sorted iterator.
+    """
+
+    def __init__(self, iterators : List[Iterator[T]], key=None):
+        """ Initialise the SortedIteratorMerger.
+
+        :param iterators: The iterators to merge.
+        :param key: A function that converts the iterator entries into comparable keys.
+        :return: A SortedIteratorMerger
+        """
+        n_iterators = len(iterators)
+        self.iterators = iterators
+        self.sorted_tops = SortedDict()
+        self.tops = n_iterators * [None]
+        self.idxs = list(range(n_iterators))
+        self.c_idx = 0
+        self.key = (lambda x: x) if key is None else key
+
+        self._update_sorting()
+
+    def __iter__(self):
+        return self
+
+    def __next__(self) -> List[T]:
+        if self.c_idx == len(self.idxs):
+            self._update_sorting()
+        res = self.tops[self.idxs[self.c_idx]]
+        self.c_idx += 1
+        return res
+
+    def close(self):
+        """
+        Closes all the iterators.
+
+        This is particularly important if the iterators are files.
+        """
+        if hasattr(self, 'iterators'):
+            for it in self.iterators:
+                if hasattr(it, 'close'):
+                    it.close()
+
+    def _update_sorting(self):
+        """ Insert new entries into the merged iterator.
+
+        :param sorted_tops: A SortedDict.
+        :param tops: The most recent entry from each iterator.
+        :param idxs: The indices to update.
+        """
+        key = self.key
+        sorted_tops = self.sorted_tops
+        tops = self.tops
+        iterators = self.iterators
+        for idx in self.idxs:
+            try:
+                tops[idx] = next(iterators[idx])
+                top_key = key(tops[idx])
+                if top_key not in sorted_tops:
+                    sorted_tops[top_key] = []
+                sorted_tops[top_key].append(idx)
+            except StopIteration:
+                pass
+        if len(sorted_tops) == 0:
+            raise StopIteration
+        key, self.idxs = sorted_tops.popitem(0)
+        self.c_idx = 0
```

### Comparing `lhc-python-2.5.0/lhc/misc/performance_measures.py` & `lhc_python-2.5.1/src/lhc/misc/performance_measures.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-import math
-import numpy
-
-from collections import Counter
-
-
-TP = (1, 1)
-TN = (0, 0)
-FP = (0, 1)
-FN = (1, 0)
-
-X = 0  # True positives
-Y = 1  # False positives
-A = 2  # Area under curve
-T = 3  # Threshold
-M = 4  # Matthews correlation coefficient
-B = 5  # Balanced error rate
-
-
-def specificity(tp=None, tn=None, fp=None, fn=None):
-    """Specificity [0, 1]
-    
-    This function is designed to be used with the confusion performance
-    function below. If you only want to specify tp and fn, please use keyword
-    arguments when calling.
-    
-    :param int tp: number of true positives
-    :param int tn: number of true negatives
-    :param int fp: number of false positives
-    :param int fn: number of false negatives
-    :rtype: float 
-    """
-    return tp / float(tp + fn)
-
-
-def sensitivity(tp=None, tn=None, fp=None, fn=None):
-    """Sensitivity [0, 1]
-    
-    This function is designed to be used with the confusion performance
-    function below. If you only want to specify tp and fn, please use keyword
-    arguments when calling.
-    
-    :param int tp: number of true positives
-    :param int tn: number of true negatives
-    :param int fp: number of false positives
-    :param int fn: number of false negatives
-    :rtype: float
-    """
-    return tn / float(tn + fp)
-
-
-def ber(tp, tn, fp, fn):
-    """Balanced Error Rate [0, 1]
-    
-    :param int tp: number of true positives
-    :param int tn: number of true negatives
-    :param int fp: number of false positives
-    :param int fn: number of false negatives
-    :rtype: float 
-    """
-    return (fp / float(tn + fp) + fn / float(fn + tp)) / 2
-
-
-def mcc(tp, tn, fp, fn):
-    """ Matthew's Correlation Coefficient [-1, 1]
-    
-    0 = you're just guessing
-    
-    :param int tp: number of true positives
-    :param int tn: number of true negatives
-    :param int fp: number of false positives
-    :param int fn: number of false negatives
-    :rtype: float 
-    """
-    if tp + fp == 0 or tp + fn == 0 or tn + fp == 0 or tn + fn == 0:
-        den = 1.0
-    else:
-        den = math.sqrt((tp + fp) * (tp + fn) * (tn + fp) * (tn + fn))
-    return (tp * tn - fp * fn) / den
-
-
-def mse(exp, obs):
-    """Mean Squared Error
-    
-    :param exp: expected values
-    :type exp: list of float
-    :param obs: observed values
-    :type obs: list of float
-    """
-    assert len(exp) == len(obs)
-    return numpy.mean((numpy.array(exp) - numpy.array(obs)) ** 2)
-
-
-def mui(x, y):
-    """MUtial Information"""
-    assert len(x) == len(y)
-    l = len(x)
-    p_x = Counter(x)
-    p_y = Counter(y)
-    p_xy = Counter(zip(x, y))
-    return sum(p_xy[(x, y)] * math.log((p_xy[(x, y)] * l) / float(p_x[x] * p_y[y]), 2) / l
-               for x, y in p_xy)
-
-
-def roc(clss, vals, reverse=False):
-    """ Reciever Operator Characteristic
-    :param clss: known classes. 1 if positive case, -1 if the negative case
-    :type class: list of boolean
-    :param vals: classification probabilites etc...
-    :type vals: list of real numbers
-    :param bool reverse: whether the values should be sorted in reverse order
-    """
-    assert len(clss) == len(vals)
-    global X, Y, A, T, M, B
-    
-    order = numpy.argsort(vals)
-    if reverse:
-        order = order[::-1]
-    clss = numpy.array(clss)[order]
-    vals = numpy.array(vals)[order]
-    
-    length = len(clss) + 1
-    data = numpy.empty((length, 6), dtype=numpy.float32)
-    data[0, X], data[0, Y], data[0, A] = 0
-    data[0, T] = vals[0]
-    
-    for i in range(length-1):
-        if clss[i] == 1:
-            data[i+1, X] = data[i, X]
-            data[i+1, Y] = data[i, Y] + 1
-            data[i+1, A] = data[i, A]
-        else:
-            data[i+1, X] = data[i, X] + 1
-            data[i+1, Y] = data[i, Y]
-            data[i+1, A] = data[i, A] + data[i+1, Y]
-        
-        data[i+1, T] = vals[i]
-    
-    # Incorporate accuracy scores
-    data[0, M] = 0
-    for i in range(1, length-1):
-        fp = data[i, X]
-        tp = data[i, Y]
-        tn = data[-1, X] - fp
-        fn = data[-1, Y] - tp
-        data[i, M] = mcc(tp, tn, fp, fn)
-        data[i, B] = ber(tp, tn, fp, fn)
-    data[-1, M] = 0
-    return data
-
-
-def confusion_matrix(exp, obs):
-    """Create a confusion matrix
-    
-    In each axis of the resulting confusion matrix the negative case is
-    0-index and the positive case 1-index. The labels get sorted, in a
-    True/False scenario true positives will occur at (1,1). The first dimension
-    (rows) of the resulting matrix is the expected class and the second
-    dimension (columns) is the observed class.
-    
-    :param exp: expected values
-    :type exp: list of float
-    :param obs: observed values
-    :type obs: list of float
-    :rtype: tuple of square matrix and sorted labels
-    """
-    assert len(exp) == len(obs)
-    # Expected in the first dimension (0;rows), observed in the second (1;cols)
-    lbls = sorted(set(exp))
-    res = numpy.zeros(shape=(len(lbls), len(lbls)))
-    for i in range(len(exp)):
-        res[lbls.index(exp[i]), lbls.index(obs[i])] += 1
-    return res, lbls
-
-
-def confusion_performance(mat, fn):
-    """Apply a performance function to a confusion matrix
-    
-    :param mat: confusion matrix
-    :type mat: square matrix
-    :param function fn: performance function
-    """
-    if mat.shape[0] != mat.shape[1] or mat.shape < (2, 2):
-        raise TypeError('{} is not a confusion matrix'.format(mat))
-    elif mat.shape == (2, 2):
-        return fn(mat[TP], mat[TN], mat[FP], mat[FN])
-    res = numpy.empty(mat.shape[0])
-    for i in range(len(res)):
-        res[i] = fn(mat[i, i],                                   # TP
-                    sum(mat) - sum(mat[:, i]) - sum(mat[i, :]),  # TN
-                    sum(mat[:, i]) - mat[i, i],                  # FP
-                    sum(mat[i, :]) - mat[i, i])                  # FN
-    return res
+import math
+import numpy
+
+from collections import Counter
+
+
+TP = (1, 1)
+TN = (0, 0)
+FP = (0, 1)
+FN = (1, 0)
+
+X = 0  # True positives
+Y = 1  # False positives
+A = 2  # Area under curve
+T = 3  # Threshold
+M = 4  # Matthews correlation coefficient
+B = 5  # Balanced error rate
+
+
+def specificity(tp=None, tn=None, fp=None, fn=None):
+    """Specificity [0, 1]
+    
+    This function is designed to be used with the confusion performance
+    function below. If you only want to specify tp and fn, please use keyword
+    arguments when calling.
+    
+    :param int tp: number of true positives
+    :param int tn: number of true negatives
+    :param int fp: number of false positives
+    :param int fn: number of false negatives
+    :rtype: float 
+    """
+    return tp / float(tp + fn)
+
+
+def sensitivity(tp=None, tn=None, fp=None, fn=None):
+    """Sensitivity [0, 1]
+    
+    This function is designed to be used with the confusion performance
+    function below. If you only want to specify tp and fn, please use keyword
+    arguments when calling.
+    
+    :param int tp: number of true positives
+    :param int tn: number of true negatives
+    :param int fp: number of false positives
+    :param int fn: number of false negatives
+    :rtype: float
+    """
+    return tn / float(tn + fp)
+
+
+def ber(tp, tn, fp, fn):
+    """Balanced Error Rate [0, 1]
+    
+    :param int tp: number of true positives
+    :param int tn: number of true negatives
+    :param int fp: number of false positives
+    :param int fn: number of false negatives
+    :rtype: float 
+    """
+    return (fp / float(tn + fp) + fn / float(fn + tp)) / 2
+
+
+def mcc(tp, tn, fp, fn):
+    """ Matthew's Correlation Coefficient [-1, 1]
+    
+    0 = you're just guessing
+    
+    :param int tp: number of true positives
+    :param int tn: number of true negatives
+    :param int fp: number of false positives
+    :param int fn: number of false negatives
+    :rtype: float 
+    """
+    if tp + fp == 0 or tp + fn == 0 or tn + fp == 0 or tn + fn == 0:
+        den = 1.0
+    else:
+        den = math.sqrt((tp + fp) * (tp + fn) * (tn + fp) * (tn + fn))
+    return (tp * tn - fp * fn) / den
+
+
+def mse(exp, obs):
+    """Mean Squared Error
+    
+    :param exp: expected values
+    :type exp: list of float
+    :param obs: observed values
+    :type obs: list of float
+    """
+    assert len(exp) == len(obs)
+    return numpy.mean((numpy.array(exp) - numpy.array(obs)) ** 2)
+
+
+def mui(x, y):
+    """MUtial Information"""
+    assert len(x) == len(y)
+    l = len(x)
+    p_x = Counter(x)
+    p_y = Counter(y)
+    p_xy = Counter(zip(x, y))
+    return sum(p_xy[(x, y)] * math.log((p_xy[(x, y)] * l) / float(p_x[x] * p_y[y]), 2) / l
+               for x, y in p_xy)
+
+
+def roc(clss, vals, reverse=False):
+    """ Reciever Operator Characteristic
+    :param clss: known classes. 1 if positive case, -1 if the negative case
+    :type class: list of boolean
+    :param vals: classification probabilites etc...
+    :type vals: list of real numbers
+    :param bool reverse: whether the values should be sorted in reverse order
+    """
+    assert len(clss) == len(vals)
+    global X, Y, A, T, M, B
+    
+    order = numpy.argsort(vals)
+    if reverse:
+        order = order[::-1]
+    clss = numpy.array(clss)[order]
+    vals = numpy.array(vals)[order]
+    
+    length = len(clss) + 1
+    data = numpy.empty((length, 6), dtype=numpy.float32)
+    data[0, X], data[0, Y], data[0, A] = 0
+    data[0, T] = vals[0]
+    
+    for i in range(length-1):
+        if clss[i] == 1:
+            data[i+1, X] = data[i, X]
+            data[i+1, Y] = data[i, Y] + 1
+            data[i+1, A] = data[i, A]
+        else:
+            data[i+1, X] = data[i, X] + 1
+            data[i+1, Y] = data[i, Y]
+            data[i+1, A] = data[i, A] + data[i+1, Y]
+        
+        data[i+1, T] = vals[i]
+    
+    # Incorporate accuracy scores
+    data[0, M] = 0
+    for i in range(1, length-1):
+        fp = data[i, X]
+        tp = data[i, Y]
+        tn = data[-1, X] - fp
+        fn = data[-1, Y] - tp
+        data[i, M] = mcc(tp, tn, fp, fn)
+        data[i, B] = ber(tp, tn, fp, fn)
+    data[-1, M] = 0
+    return data
+
+
+def confusion_matrix(exp, obs):
+    """Create a confusion matrix
+    
+    In each axis of the resulting confusion matrix the negative case is
+    0-index and the positive case 1-index. The labels get sorted, in a
+    True/False scenario true positives will occur at (1,1). The first dimension
+    (rows) of the resulting matrix is the expected class and the second
+    dimension (columns) is the observed class.
+    
+    :param exp: expected values
+    :type exp: list of float
+    :param obs: observed values
+    :type obs: list of float
+    :rtype: tuple of square matrix and sorted labels
+    """
+    assert len(exp) == len(obs)
+    # Expected in the first dimension (0;rows), observed in the second (1;cols)
+    lbls = sorted(set(exp))
+    res = numpy.zeros(shape=(len(lbls), len(lbls)))
+    for i in range(len(exp)):
+        res[lbls.index(exp[i]), lbls.index(obs[i])] += 1
+    return res, lbls
+
+
+def confusion_performance(mat, fn):
+    """Apply a performance function to a confusion matrix
+    
+    :param mat: confusion matrix
+    :type mat: square matrix
+    :param function fn: performance function
+    """
+    if mat.shape[0] != mat.shape[1] or mat.shape < (2, 2):
+        raise TypeError('{} is not a confusion matrix'.format(mat))
+    elif mat.shape == (2, 2):
+        return fn(mat[TP], mat[TN], mat[FP], mat[FN])
+    res = numpy.empty(mat.shape[0])
+    for i in range(len(res)):
+        res[i] = fn(mat[i, i],                                   # TP
+                    sum(mat) - sum(mat[:, i]) - sum(mat[i, :]),  # TN
+                    sum(mat[:, i]) - mat[i, i],                  # FP
+                    sum(mat[i, :]) - mat[i, i])                  # FN
+    return res
```

### Comparing `lhc-python-2.5.0/lhc/misc/string.py` & `lhc_python-2.5.1/src/lhc/misc/string.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from itertools import repeat
-from typing import Optional
-
-
-def levenshtein(s, t):
-    """
-    Calculate the Levenshtein distance between two strings. From Wikipedia article: Iterative with two matrix rows.
-
-    :param s: string 1
-    :type s: str
-    :param t: string 2
-    :type s: str
-    :return: Levenshtein distance
-    :rtype: float
-    """
-
-    if s == t:
-        return 0
-    elif len(s) == 0:
-        return len(t)
-    elif len(t) == 0:
-        return len(s)
-
-    v0 = list(repeat(0, len(t) + 1))
-    v1 = list(repeat(0, len(t) + 1))
-    for i in range(len(v0)):
-        v0[i] = i
-    for i in range(len(s)):
-        v1[0] = i + 1
-        for j in range(len(t)):
-            cost = 0 if s[i] == t[j] else 1
-            v1[j + 1] = min(v1[j] + 1, v0[j + 1] + 1, v0[j] + cost)
-        for j in range(len(v0)):
-            v0[j] = v1[j]
-
-    return v1[len(t)]
-
-
-def hamming(s, t):
-    """
-    Calculate the Hamming distance between two strings. From Wikipedia article: Iterative with two matrix rows.
-
-    :param s: string 1
-    :type s: str
-    :param t: string 2
-    :type s: str
-    :return: Hamming distance
-    :rtype: float
-    """
-    if len(s) != len(t):
-        raise ValueError('Hamming distance needs strings of equal length.')
-    return sum(s_ != t_ for s_, t_ in zip(s, t))
-
-
-def get_index_of_approximate_match(query: str, template: str, allowed_mismatches=1) -> Optional[int]:
-    """ Find the index of a substring with mismatches. """
-    # TODO: Change this to bitap algorithm (https://en.wikipedia.org/wiki/Bitap_algorithm)
-    for index in range(-allowed_mismatches, len(template) - len(query) + allowed_mismatches + 1):
-        mismatches = max(0, -index)
-        for i in range(mismatches, min(len(query), len(template) - index)):
-            if query[i] != template[index + i]:
-                mismatches += 1
-                if mismatches > allowed_mismatches:
-                    break
-        if mismatches <= allowed_mismatches:
-            return index
-    return None
+from itertools import repeat
+from typing import Optional
+
+
+def levenshtein(s, t):
+    """
+    Calculate the Levenshtein distance between two strings. From Wikipedia article: Iterative with two matrix rows.
+
+    :param s: string 1
+    :type s: str
+    :param t: string 2
+    :type s: str
+    :return: Levenshtein distance
+    :rtype: float
+    """
+
+    if s == t:
+        return 0
+    elif len(s) == 0:
+        return len(t)
+    elif len(t) == 0:
+        return len(s)
+
+    v0 = list(repeat(0, len(t) + 1))
+    v1 = list(repeat(0, len(t) + 1))
+    for i in range(len(v0)):
+        v0[i] = i
+    for i in range(len(s)):
+        v1[0] = i + 1
+        for j in range(len(t)):
+            cost = 0 if s[i] == t[j] else 1
+            v1[j + 1] = min(v1[j] + 1, v0[j + 1] + 1, v0[j] + cost)
+        for j in range(len(v0)):
+            v0[j] = v1[j]
+
+    return v1[len(t)]
+
+
+def hamming(s, t):
+    """
+    Calculate the Hamming distance between two strings. From Wikipedia article: Iterative with two matrix rows.
+
+    :param s: string 1
+    :type s: str
+    :param t: string 2
+    :type s: str
+    :return: Hamming distance
+    :rtype: float
+    """
+    if len(s) != len(t):
+        raise ValueError('Hamming distance needs strings of equal length.')
+    return sum(s_ != t_ for s_, t_ in zip(s, t))
+
+
+def get_index_of_approximate_match(query: str, template: str, allowed_mismatches=1) -> Optional[int]:
+    """ Find the index of a substring with mismatches. """
+    # TODO: Change this to bitap algorithm (https://en.wikipedia.org/wiki/Bitap_algorithm)
+    for index in range(-allowed_mismatches, len(template) - len(query) + allowed_mismatches + 1):
+        mismatches = max(0, -index)
+        for i in range(mismatches, min(len(query), len(template) - index)):
+            if query[i] != template[index + i]:
+                mismatches += 1
+                if mismatches > allowed_mismatches:
+                    break
+        if mismatches <= allowed_mismatches:
+            return index
+    return None
```

### Comparing `lhc-python-2.5.0/lhc/random/reservoir.py` & `lhc_python-2.5.1/src/lhc/misc/reservoir.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-#!/usr/bin/env python3
-import argparse
-import gzip
-import itertools
-import sys
-import time
-import random
-
-
-def reservoir(iterator, k):
-    """ Performs reservoir sampling of k items in iterator. Make sure that the iterator is a once-only iterator
-    (ie. not created using the "range" function).
-
-    :param iterator: set of items to sample from
-    :param k: sample k items
-    :return: list of sampled items
-    """
-    sample = list(itertools.islice(iterator, 0, k))
-    for i, item in enumerate(iterator):
-        replace = random.randint(0, i + k)
-        if replace < k:
-            sample[replace] = item
-    return sample
-
-
-def main():
-    args = get_parser().parse_args()
-    args.func(args)
-
-
-def get_parser():
-    return define_parser(argparse.ArgumentParser())
-
-
-def define_parser(parser):
-    parser.add_argument('input', nargs='?')
-    parser.add_argument('k', type=int)
-    parser.add_argument('-c', '--comment')
-    parser.add_argument('-o', '--output')
-    parser.add_argument('-s', '--seed')
-    parser.set_defaults(func=reservoir_init)
-    return parser
-
-
-def reservoir_init(args):
-    with sys.stdin if args.input is None else\
-            gzip.open(args.input) if args.input.endswith('.gz') else\
-                    open(args.input, encoding='utf-8') as input:
-        random.seed(args.seed if args.seed else time.time())
-
-        comments = []
-        line = next(input)
-        if args.comment is not None:
-            while True:
-                if not line.startswith(args.comment):
-                    break
-                comments.append(line)
-                line = next(input)
-
-        sample = reservoir(itertools.chain([line], input), args.k)
-
-    with sys.stdout if args.output is None else open(args.output, 'w') as output:
-        for line in itertools.chain(comments, sample):
-            output.write(line)
-
-if __name__ == '__main__':
-    sys.exit(main())
+#!/usr/bin/env python3
+import argparse
+import gzip
+import itertools
+import sys
+import time
+import random
+
+
+def reservoir(iterator, k):
+    """ Performs reservoir sampling of k items in iterator. Make sure that the iterator is a once-only iterator
+    (ie. not created using the "range" function).
+
+    :param iterator: set of items to sample from
+    :param k: sample k items
+    :return: list of sampled items
+    """
+    sample = list(itertools.islice(iterator, 0, k))
+    for i, item in enumerate(iterator):
+        replace = random.randint(0, i + k)
+        if replace < k:
+            sample[replace] = item
+    return sample
+
+
+def main():
+    args = get_parser().parse_args()
+    args.func(args)
+
+
+def get_parser():
+    return define_parser(argparse.ArgumentParser())
+
+
+def define_parser(parser):
+    parser.add_argument('input', nargs='?')
+    parser.add_argument('k', type=int)
+    parser.add_argument('-c', '--comment')
+    parser.add_argument('-o', '--output')
+    parser.add_argument('-s', '--seed')
+    parser.set_defaults(func=reservoir_init)
+    return parser
+
+
+def reservoir_init(args):
+    with sys.stdin if args.input is None else\
+            gzip.open(args.input) if args.input.endswith('.gz') else\
+                    open(args.input, encoding='utf-8') as input:
+        random.seed(args.seed if args.seed else time.time())
+
+        comments = []
+        line = next(input)
+        if args.comment is not None:
+            while True:
+                if not line.startswith(args.comment):
+                    break
+                comments.append(line)
+                line = next(input)
+
+        sample = reservoir(itertools.chain([line], input), args.k)
+
+    with sys.stdout if args.output is None else open(args.output, 'w') as output:
+        for line in itertools.chain(comments, sample):
+            output.write(line)
+
+if __name__ == '__main__':
+    sys.exit(main())
```

### Comparing `lhc-python-2.5.0/lhc/tools/tokeniser.py` & `lhc_python-2.5.1/src/lhc/misc/tokeniser.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from collections import namedtuple
-
-Token = namedtuple('Token', ('type', 'value'))
-
-
-class Tokeniser(object):
-    def __init__(self, types, individual=None):
-        self._type_map = {}
-        for type, characters in types.items():
-            for character in characters:
-                self._type_map[character] = type
-        self.individual = set() if individual is None else individual
-
-    def tokenise(self, string):
-        type_map = self._type_map
-        individual = self.individual
-
-        fr = 0
-        while fr < len(string):
-            type = type_map[string[fr]]
-            to = fr + 1
-            while to < len(string) and type == type_map[string[to]] and string[to] not in individual:
-                to += 1
-            yield Token(type=type, value=string[fr:to])
-            fr = to
+from collections import namedtuple
+
+Token = namedtuple('Token', ('type', 'value'))
+
+
+class Tokeniser(object):
+    def __init__(self, types, individual=None):
+        self._type_map = {}
+        for type, characters in types.items():
+            for character in characters:
+                self._type_map[character] = type
+        self.individual = set() if individual is None else individual
+
+    def tokenise(self, string):
+        type_map = self._type_map
+        individual = self.individual
+
+        fr = 0
+        while fr < len(string):
+            type = type_map[string[fr]]
+            to = fr + 1
+            while to < len(string) and type == type_map[string[to]] and string[to] not in individual:
+                to += 1
+            yield Token(type=type, value=string[fr:to])
+            fr = to
```

### Comparing `lhc-python-2.5.0/lib/bitap/bitapmodule.cpp` & `lhc_python-2.5.1/src/lib/bitap/bitapmodule.cpp`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-#include <Python.h>
-#include "bitap.h"
-
-
-static PyObject *
-bitap_wrapper(PyObject *self, PyObject *args) {
-  const char *text;
-  const char *pattern;
-  int index;
-
-  if (!PyArg_ParseTuple(args, "ss", &pattern, &text))
-    return NULL;
-  index = bitap(text, pattern);
-
-  return PyLong_FromLong(index);
-}
-
-static PyObject *
-fuzzy_bitap_wrapper(PyObject *self, PyObject *args) {
-  const char *text;
-  const char *pattern;
-  int k;
-  int index;
-
-  if (!PyArg_ParseTuple(args, "ssi", &pattern, &text, &k))
-    return NULL;
-  index = fuzzy_bitap(text, pattern, k);
-
-  return PyLong_FromLong(index);
-}
-
-
-static PyMethodDef BitapMethods[] = {
-  { "bitap", bitap_wrapper, METH_VARARGS, "Exact bitap search" },
-  { "bitap_fuzzy", fuzzy_bitap_wrapper, METH_VARARGS, "Fuzzy bitap search" },
-  { NULL, NULL, 0, NULL }
-};
-
-static struct PyModuleDef bitapmodule = {
-    PyModuleDef_HEAD_INIT,
-    "bitap",   /* name of module */
-    NULL, /*bitap_doc, /* module documentation, may be NULL */
-    -1,       /* size of per-interpreter state of the module,
-                 or -1 if the module keeps state in global variables. */
-    BitapMethods
-};
-
-PyMODINIT_FUNC
-PyInit_bitap(void)
-{
-    return PyModule_Create(&bitapmodule);
-}
+#include <Python.h>
+#include "bitap.h"
+
+
+static PyObject *
+bitap_wrapper(PyObject *self, PyObject *args) {
+  const char *text;
+  const char *pattern;
+  int index;
+
+  if (!PyArg_ParseTuple(args, "ss", &pattern, &text))
+    return NULL;
+  index = bitap(text, pattern);
+
+  return PyLong_FromLong(index);
+}
+
+static PyObject *
+fuzzy_bitap_wrapper(PyObject *self, PyObject *args) {
+  const char *text;
+  const char *pattern;
+  int k;
+  int index;
+
+  if (!PyArg_ParseTuple(args, "ssi", &pattern, &text, &k))
+    return NULL;
+  index = fuzzy_bitap(text, pattern, k);
+
+  return PyLong_FromLong(index);
+}
+
+
+static PyMethodDef BitapMethods[] = {
+  { "bitap", bitap_wrapper, METH_VARARGS, "Exact bitap search" },
+  { "bitap_fuzzy", fuzzy_bitap_wrapper, METH_VARARGS, "Fuzzy bitap search" },
+  { NULL, NULL, 0, NULL }
+};
+
+static struct PyModuleDef bitapmodule = {
+    PyModuleDef_HEAD_INIT,
+    "bitap",   /* name of module */
+    NULL, /*bitap_doc, /* module documentation, may be NULL */
+    -1,       /* size of per-interpreter state of the module,
+                 or -1 if the module keeps state in global variables. */
+    BitapMethods
+};
+
+PyMODINIT_FUNC
+PyInit_bitap(void)
+{
+    return PyModule_Create(&bitapmodule);
+}
```

