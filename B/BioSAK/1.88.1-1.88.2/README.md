# Comparing `tmp/BioSAK-1.88.1.tar.gz` & `tmp/BioSAK-1.88.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BioSAK-1.88.1.tar", last modified: Sat May  4 12:52:08 2024, max compression
+gzip compressed data, was "BioSAK-1.88.2.tar", last modified: Mon May  6 06:08:22 2024, max compression
```

## Comparing `BioSAK-1.88.1.tar` & `BioSAK-1.88.2.tar`

### file list

```diff
@@ -1,167 +1,168 @@
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-04 12:52:08.164491 BioSAK-1.88.1/
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-04 12:52:08.161866 BioSAK-1.88.1/BioSAK/
--rw-r--r--   0 songweizhi   (501) staff       (20)     3653 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/BLCA_op_parser.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2031 2023-05-31 05:26:00.000000 BioSAK-1.88.1/BioSAK/BioSAK_config.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    39300 2024-03-22 00:45:31.000000 BioSAK-1.88.1/BioSAK/COG2020.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3615 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/COG_boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     6974 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/COG_boxplot_last2row.R
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     6067 2024-01-16 05:00:13.000000 BioSAK-1.88.1/BioSAK/CheckM.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5891 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/ConvertMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    16671 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/DnaFeaturesViewer.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2292 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/FastaSplitler_by_num.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2485 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/FastaSplitler_by_size.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2190 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/GTDB_for_BLCA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1321 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/Gene2Ctg.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    45147 2024-03-23 14:54:03.000000 BioSAK-1.88.1/BioSAK/KEGG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3484 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/KEGG_boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)      269 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/KEGG_get_eukaryotic_kos.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3077 2023-08-22 09:31:28.000000 BioSAK-1.88.1/BioSAK/KeepRemovingTmp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2620 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/MeanMappingDepth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-01-16 12:39:58.000000 BioSAK-1.88.1/BioSAK/MetaBiosample.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  3297822 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/MetaCHIP_phylo.hmm
--rw-r--r--   0 songweizhi   (501) staff       (20)  1206805 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/MetaCyc_reactions_with_ec.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)    16960 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/NetEnzymes.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3713 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/Newick_tree_plotter.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1659 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/OneLineAln.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    10448 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/Prodigal.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6048 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/Reads_simulator.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3573 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/RunGraphMB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3833 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/SILVA_for_BLCA.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     6255 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/SankeyTaxon.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5678 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/SliceMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3173 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/SubsampleLongReads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     1696 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/Tax4Fun2IndOTU.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3700 2024-05-04 12:52:07.000000 BioSAK-1.88.1/BioSAK/VERSION
--rw-r--r--   0 songweizhi   (501) staff       (20)      467 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/VisBlastOp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     9944 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/VisGeneFlk.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/__init__.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2526 2024-03-25 14:00:14.000000 BioSAK-1.88.1/BioSAK/add_desc.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    38577 2024-03-22 00:45:31.000000 BioSAK-1.88.1/BioSAK/arCOG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6985 2024-01-16 05:00:13.000000 BioSAK-1.88.1/BioSAK/bam2reads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2630 2024-03-22 13:23:45.000000 BioSAK-1.88.1/BioSAK/boxplot.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3312 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     6104 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/boxplot_matrix_COG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5403 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/boxplot_matrix_COG_backup.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6984 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/boxplot_matrix_KEGG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5747 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/boxplot_matrix_dbCAN.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1695 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/cat_fa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    13440 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/cdd2cog.pl
--rw-r--r--   0 songweizhi   (501) staff       (20)     1186 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/checkm_marker.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1485 2024-05-02 15:52:56.000000 BioSAK-1.88.1/BioSAK/compare_sets.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/compare_trees.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     9745 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/compare_trees.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      814 2024-05-04 12:52:07.000000 BioSAK-1.88.1/BioSAK/count_num.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6592 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/cross_link_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    24033 2024-03-22 00:45:31.000000 BioSAK-1.88.1/BioSAK/dbCAN.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1936 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      767 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/dwnld_sra_reads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    13250 2024-03-22 08:01:22.000000 BioSAK-1.88.1/BioSAK/enrich.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      929 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/exe_cmds.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1508 2023-12-05 01:06:39.000000 BioSAK-1.88.1/BioSAK/ezaai2mat.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1396 2023-12-05 01:02:55.000000 BioSAK-1.88.1/BioSAK/fa2id.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1195 2023-05-17 06:14:50.000000 BioSAK-1.88.1/BioSAK/fa2phy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1363 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/fa2tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6280 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/format_converter.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2861 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/format_leaf_name.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      639 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/fq2fa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3204 2024-04-19 15:04:59.000000 BioSAK-1.88.1/BioSAK/gapseq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2846 2023-06-14 10:08:30.000000 BioSAK-1.88.1/BioSAK/gbk2faa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3342 2023-06-14 10:14:13.000000 BioSAK-1.88.1/BioSAK/gbk2ffn.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2528 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/gbk2fna.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6886 2024-04-29 03:23:48.000000 BioSAK-1.88.1/BioSAK/gbk2gff.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3726 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/gbk_to_ffn_faa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1887 2024-04-15 02:59:40.000000 BioSAK-1.88.1/BioSAK/gc.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      813 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_EC_from_ko_stats_D.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7477 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_GTDB_taxon_gnm.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5428 2023-06-15 03:03:02.000000 BioSAK-1.88.1/BioSAK/get_MAG_reads_long.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3991 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_Pfam_hmms.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    29246 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_SCG_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1784 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_TopHits_taxonomy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2247 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_aa_composition.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12066 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_bin_abundance copy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2139 2024-01-23 11:57:14.000000 BioSAK-1.88.1/BioSAK/get_data_matrix.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5523 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_gene_depth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3591 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/get_genome_GTDB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6070 2024-01-16 04:57:23.000000 BioSAK-1.88.1/BioSAK/get_genome_NCBI.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    11209 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_genome_NCBI_v1.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12620 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_genome_NCBI_v2.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3048 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_gnm_size.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4834 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_ko_gene_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1192 2023-09-21 08:44:42.000000 BioSAK-1.88.1/BioSAK/get_krona_plot.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1559 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_reads_from_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      792 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_reads_id_in_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2386 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_sankey_plot.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     4242 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_top_hit.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      820 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/get_total_length.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1834 2024-04-29 04:11:58.000000 BioSAK-1.88.1/BioSAK/gff2chrom.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4643 2023-05-18 01:37:58.000000 BioSAK-1.88.1/BioSAK/global_functions.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2910 2024-03-11 00:57:02.000000 BioSAK-1.88.1/BioSAK/hpc3.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    26872 2024-04-12 00:51:29.000000 BioSAK-1.88.1/BioSAK/iTOL.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3337 2024-03-07 03:01:35.000000 BioSAK-1.88.1/BioSAK/js_cmds.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3281 2024-04-08 09:48:49.000000 BioSAK-1.88.1/BioSAK/js_hpc3.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1643 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/keep_best_hit.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  3361029 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/ko00001.keg
--rw-r--r--   0 songweizhi   (501) staff       (20)     1848 2024-03-10 15:18:30.000000 BioSAK-1.88.1/BioSAK/koala.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2772 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/label_tree.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     4788 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/label_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    35857 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/link_16S_MAG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12349 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/magabund.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    19855 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/magabund2.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1224 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/manipulator_fasta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/manipulator_msa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3659 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/manipulator_newick.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/manipulator_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      903 2024-04-17 08:12:49.000000 BioSAK-1.88.1/BioSAK/mannwhitneyu.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2433 2023-05-30 01:59:44.000000 BioSAK-1.88.1/BioSAK/mean_MAG_cov.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1880 2024-03-25 06:45:20.000000 BioSAK-1.88.1/BioSAK/merge_df.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2405 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/merge_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6742 2024-01-23 07:37:01.000000 BioSAK-1.88.1/BioSAK/metaAssembly.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1327 2023-06-11 13:56:21.000000 BioSAK-1.88.1/BioSAK/metabat2concoct.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1612 2023-06-11 16:00:51.000000 BioSAK-1.88.1/BioSAK/metabat2maxbin.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/msa_to_distance_matrix.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1759 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/ncbi_dataset.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2024-03-03 11:00:02.000000 BioSAK-1.88.1/BioSAK/odp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2820 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/parse_MetaCyc_RxnDB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1460 2023-09-18 14:42:31.000000 BioSAK-1.88.1/BioSAK/parse_mmseqs_tsv.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     8633 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/plot_mag.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7332 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/plot_sam_depth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1638 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/plot_tree.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     2256 2023-07-22 00:36:16.000000 BioSAK-1.88.1/BioSAK/prefix_file.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4221 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/prokka.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5057 2023-08-03 02:58:56.000000 BioSAK-1.88.1/BioSAK/reads2bam.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2534 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/rename_leaves.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2005 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/rename_reads_for_Reago.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6801 2023-10-26 11:55:44.000000 BioSAK-1.88.1/BioSAK/rename_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2210 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/rename_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    15703 2024-04-29 07:37:26.000000 BioSAK-1.88.1/BioSAK/ribbon.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1996 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/sam2bam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6877 2023-05-13 11:01:19.000000 BioSAK-1.88.1/BioSAK/sampling_GTDB_gnms.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3603 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/select_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3167 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/sep_reads_by_barcode.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2671 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/slice_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3788 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/split_fasta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1998 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/split_folder.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4561 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/split_sam.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     1204 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/submitHPC.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2011 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/subset_GTDB_meta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4585 2024-04-09 03:15:33.000000 BioSAK-1.88.1/BioSAK/subset_df.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7296 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/subset_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7844 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/top_16S_hits.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2106 2023-05-09 01:09:35.000000 BioSAK-1.88.1/BioSAK/top_hits_in_a_group.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      831 2024-04-09 06:05:51.000000 BioSAK-1.88.1/BioSAK/transpose.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2252 2024-01-16 05:10:59.000000 BioSAK-1.88.1/BioSAK/usearch_uc.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      962 2024-04-17 08:12:49.000000 BioSAK-1.88.1/BioSAK/wilcox.py
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-04 12:52:08.164045 BioSAK-1.88.1/BioSAK.egg-info/
--rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-04 12:52:08.000000 BioSAK-1.88.1/BioSAK.egg-info/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     3747 2024-05-04 12:52:08.000000 BioSAK-1.88.1/BioSAK.egg-info/SOURCES.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        1 2024-05-04 12:52:08.000000 BioSAK-1.88.1/BioSAK.egg-info/dependency_links.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)       95 2024-05-04 12:52:08.000000 BioSAK-1.88.1/BioSAK.egg-info/requires.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        7 2024-05-04 12:52:08.000000 BioSAK-1.88.1/BioSAK.egg-info/top_level.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2023-05-09 01:09:36.000000 BioSAK-1.88.1/LICENSE
--rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2023-05-09 01:09:36.000000 BioSAK-1.88.1/MANIFEST.in
--rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-04 12:52:08.164287 BioSAK-1.88.1/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     1533 2024-01-23 07:37:01.000000 BioSAK-1.88.1/README.md
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-04 12:52:08.162883 BioSAK-1.88.1/bin/
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    78394 2024-05-04 12:29:48.000000 BioSAK-1.88.1/bin/BioSAK
--rw-r--r--   0 songweizhi   (501) staff       (20)       38 2024-05-04 12:52:08.164532 BioSAK-1.88.1/setup.cfg
--rw-r--r--   0 songweizhi   (501) staff       (20)      915 2024-01-15 11:41:11.000000 BioSAK-1.88.1/setup.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-06 06:08:22.432919 BioSAK-1.88.2/
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-06 06:08:22.430542 BioSAK-1.88.2/BioSAK/
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3653 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/BLCA_op_parser.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2031 2023-05-31 05:26:00.000000 BioSAK-1.88.2/BioSAK/BioSAK_config.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    39300 2024-03-22 00:45:31.000000 BioSAK-1.88.2/BioSAK/COG2020.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3615 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/COG_boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6974 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/COG_boxplot_last2row.R
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     6067 2024-01-16 05:00:13.000000 BioSAK-1.88.2/BioSAK/CheckM.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5891 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/ConvertMSA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    16671 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/DnaFeaturesViewer.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2292 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/FastaSplitler_by_num.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2485 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/FastaSplitler_by_size.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2190 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/GTDB_for_BLCA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1321 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/Gene2Ctg.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    45147 2024-03-23 14:54:03.000000 BioSAK-1.88.2/BioSAK/KEGG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3484 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/KEGG_boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)      269 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/KEGG_get_eukaryotic_kos.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3077 2023-08-22 09:31:28.000000 BioSAK-1.88.2/BioSAK/KeepRemovingTmp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2620 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/MeanMappingDepth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-01-16 12:39:58.000000 BioSAK-1.88.2/BioSAK/MetaBiosample.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  3297822 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/MetaCHIP_phylo.hmm
+-rw-r--r--   0 songweizhi   (501) staff       (20)  1206805 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/MetaCyc_reactions_with_ec.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)    16960 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/NetEnzymes.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3713 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/Newick_tree_plotter.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1659 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/OneLineAln.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    10448 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/Prodigal.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6048 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/Reads_simulator.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3573 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/RunGraphMB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3833 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/SILVA_for_BLCA.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     6255 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/SankeyTaxon.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5678 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/SliceMSA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3173 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/SubsampleLongReads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     1696 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/Tax4Fun2IndOTU.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3700 2024-05-06 06:08:20.000000 BioSAK-1.88.2/BioSAK/VERSION
+-rw-r--r--   0 songweizhi   (501) staff       (20)      467 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/VisBlastOp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     9944 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/VisGeneFlk.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/__init__.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2526 2024-03-25 14:00:14.000000 BioSAK-1.88.2/BioSAK/add_desc.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    38577 2024-03-22 00:45:31.000000 BioSAK-1.88.2/BioSAK/arCOG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6985 2024-01-16 05:00:13.000000 BioSAK-1.88.2/BioSAK/bam2reads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2630 2024-03-22 13:23:45.000000 BioSAK-1.88.2/BioSAK/boxplot.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3312 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6104 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/boxplot_matrix_COG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5403 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/boxplot_matrix_COG_backup.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6984 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/boxplot_matrix_KEGG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5747 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/boxplot_matrix_dbCAN.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1695 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/cat_fa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    13440 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/cdd2cog.pl
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1186 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/checkm_marker.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1485 2024-05-02 15:52:56.000000 BioSAK-1.88.2/BioSAK/compare_sets.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/compare_trees.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     9745 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/compare_trees.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      814 2024-05-04 12:52:07.000000 BioSAK-1.88.2/BioSAK/count_num.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6592 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/cross_link_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    24033 2024-03-22 00:45:31.000000 BioSAK-1.88.2/BioSAK/dbCAN.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1936 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      767 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/dwnld_sra_reads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    13250 2024-03-22 08:01:22.000000 BioSAK-1.88.2/BioSAK/enrich.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      929 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/exe_cmds.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1508 2023-12-05 01:06:39.000000 BioSAK-1.88.2/BioSAK/ezaai2mat.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1396 2023-12-05 01:02:55.000000 BioSAK-1.88.2/BioSAK/fa2id.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1195 2023-05-17 06:14:50.000000 BioSAK-1.88.2/BioSAK/fa2phy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1363 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/fa2tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6280 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/format_converter.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2861 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/format_leaf_name.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      639 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/fq2fa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3204 2024-04-19 15:04:59.000000 BioSAK-1.88.2/BioSAK/gapseq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2846 2023-06-14 10:08:30.000000 BioSAK-1.88.2/BioSAK/gbk2faa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3342 2023-06-14 10:14:13.000000 BioSAK-1.88.2/BioSAK/gbk2ffn.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2528 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/gbk2fna.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6886 2024-04-29 03:23:48.000000 BioSAK-1.88.2/BioSAK/gbk2gff.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3726 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/gbk_to_ffn_faa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1887 2024-04-15 02:59:40.000000 BioSAK-1.88.2/BioSAK/gc.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      813 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_EC_from_ko_stats_D.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7477 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_GTDB_taxon_gnm.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5428 2023-06-15 03:03:02.000000 BioSAK-1.88.2/BioSAK/get_MAG_reads_long.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3991 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_Pfam_hmms.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    29246 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_SCG_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1784 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_TopHits_taxonomy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2247 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_aa_composition.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12066 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_bin_abundance copy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2139 2024-01-23 11:57:14.000000 BioSAK-1.88.2/BioSAK/get_data_matrix.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5523 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_gene_depth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3591 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/get_genome_GTDB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6070 2024-01-16 04:57:23.000000 BioSAK-1.88.2/BioSAK/get_genome_NCBI.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    11209 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_genome_NCBI_v1.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12620 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_genome_NCBI_v2.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3048 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_gnm_size.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4834 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_ko_gene_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1192 2023-09-21 08:44:42.000000 BioSAK-1.88.2/BioSAK/get_krona_plot.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1559 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_reads_from_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      792 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_reads_id_in_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2386 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_sankey_plot.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4242 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_top_hit.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      820 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/get_total_length.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1834 2024-04-29 04:11:58.000000 BioSAK-1.88.2/BioSAK/gff2chrom.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4643 2023-05-18 01:37:58.000000 BioSAK-1.88.2/BioSAK/global_functions.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2910 2024-03-11 00:57:02.000000 BioSAK-1.88.2/BioSAK/hpc3.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    26872 2024-04-12 00:51:29.000000 BioSAK-1.88.2/BioSAK/iTOL.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3337 2024-03-07 03:01:35.000000 BioSAK-1.88.2/BioSAK/js_cmds.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3281 2024-04-08 09:48:49.000000 BioSAK-1.88.2/BioSAK/js_hpc3.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1643 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/keep_best_hit.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  3361029 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/ko00001.keg
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1848 2024-03-10 15:18:30.000000 BioSAK-1.88.2/BioSAK/koala.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2772 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/label_tree.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4788 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/label_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    35857 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/link_16S_MAG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12349 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/magabund.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    19855 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/magabund2.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1224 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/manipulator_fasta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/manipulator_msa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3659 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/manipulator_newick.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/manipulator_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      903 2024-04-17 08:12:49.000000 BioSAK-1.88.2/BioSAK/mannwhitneyu.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2433 2023-05-30 01:59:44.000000 BioSAK-1.88.2/BioSAK/mean_MAG_cov.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1880 2024-03-25 06:45:20.000000 BioSAK-1.88.2/BioSAK/merge_df.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2405 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/merge_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     8812 2024-05-06 06:07:04.000000 BioSAK-1.88.2/BioSAK/metaAssembly.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1327 2023-06-11 13:56:21.000000 BioSAK-1.88.2/BioSAK/metabat2concoct.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1612 2023-06-11 16:00:51.000000 BioSAK-1.88.2/BioSAK/metabat2maxbin.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/msa_to_distance_matrix.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1759 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/ncbi_dataset.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2024-03-03 11:00:02.000000 BioSAK-1.88.2/BioSAK/odp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2820 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/parse_MetaCyc_RxnDB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1460 2023-09-18 14:42:31.000000 BioSAK-1.88.2/BioSAK/parse_mmseqs_tsv.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     8633 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/plot_mag.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7332 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/plot_sam_depth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1638 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/plot_tree.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2256 2023-07-22 00:36:16.000000 BioSAK-1.88.2/BioSAK/prefix_file.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4221 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/prokka.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5057 2023-08-03 02:58:56.000000 BioSAK-1.88.2/BioSAK/reads2bam.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2534 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/rename_leaves.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2005 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/rename_reads_for_Reago.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6801 2023-10-26 11:55:44.000000 BioSAK-1.88.2/BioSAK/rename_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2210 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/rename_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    15703 2024-04-29 07:37:26.000000 BioSAK-1.88.2/BioSAK/ribbon.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1996 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/sam2bam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6877 2023-05-13 11:01:19.000000 BioSAK-1.88.2/BioSAK/sampling_GTDB_gnms.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3603 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/select_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3167 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/sep_reads_by_barcode.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2671 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/slice_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3788 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/split_fasta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1998 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/split_folder.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4561 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/split_sam.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     1204 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/submitHPC.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2011 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/subset_GTDB_meta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4585 2024-04-09 03:15:33.000000 BioSAK-1.88.2/BioSAK/subset_df.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7296 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/subset_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1912 2024-05-06 05:46:35.000000 BioSAK-1.88.2/BioSAK/tmp_1.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7844 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/top_16S_hits.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2106 2023-05-09 01:09:35.000000 BioSAK-1.88.2/BioSAK/top_hits_in_a_group.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      831 2024-04-09 06:05:51.000000 BioSAK-1.88.2/BioSAK/transpose.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2252 2024-01-16 05:10:59.000000 BioSAK-1.88.2/BioSAK/usearch_uc.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      962 2024-04-17 08:12:49.000000 BioSAK-1.88.2/BioSAK/wilcox.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-06 06:08:22.432384 BioSAK-1.88.2/BioSAK.egg-info/
+-rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-06 06:08:22.000000 BioSAK-1.88.2/BioSAK.egg-info/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3763 2024-05-06 06:08:22.000000 BioSAK-1.88.2/BioSAK.egg-info/SOURCES.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        1 2024-05-06 06:08:22.000000 BioSAK-1.88.2/BioSAK.egg-info/dependency_links.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)       95 2024-05-06 06:08:22.000000 BioSAK-1.88.2/BioSAK.egg-info/requires.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        7 2024-05-06 06:08:22.000000 BioSAK-1.88.2/BioSAK.egg-info/top_level.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2023-05-09 01:09:36.000000 BioSAK-1.88.2/LICENSE
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2023-05-09 01:09:36.000000 BioSAK-1.88.2/MANIFEST.in
+-rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-06 06:08:22.432688 BioSAK-1.88.2/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1533 2024-01-23 07:37:01.000000 BioSAK-1.88.2/README.md
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-06 06:08:22.431641 BioSAK-1.88.2/bin/
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    78394 2024-05-04 12:29:48.000000 BioSAK-1.88.2/bin/BioSAK
+-rw-r--r--   0 songweizhi   (501) staff       (20)       38 2024-05-06 06:08:22.432967 BioSAK-1.88.2/setup.cfg
+-rw-r--r--   0 songweizhi   (501) staff       (20)      915 2024-01-15 11:41:11.000000 BioSAK-1.88.2/setup.py
```

### Comparing `BioSAK-1.88.1/BioSAK/BLCA_op_parser.py` & `BioSAK-1.88.2/BioSAK/BLCA_op_parser.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/BioSAK_config.py` & `BioSAK-1.88.2/BioSAK/BioSAK_config.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/COG2020.py` & `BioSAK-1.88.2/BioSAK/COG2020.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/COG_boxplot_last1row.R` & `BioSAK-1.88.2/BioSAK/COG_boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/COG_boxplot_last2row.R` & `BioSAK-1.88.2/BioSAK/COG_boxplot_last2row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/CheckM.py` & `BioSAK-1.88.2/BioSAK/CheckM.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/ConvertMSA.py` & `BioSAK-1.88.2/BioSAK/ConvertMSA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/DnaFeaturesViewer.py` & `BioSAK-1.88.2/BioSAK/DnaFeaturesViewer.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/FastaSplitler_by_num.py` & `BioSAK-1.88.2/BioSAK/FastaSplitler_by_num.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/FastaSplitler_by_size.py` & `BioSAK-1.88.2/BioSAK/FastaSplitler_by_size.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/GTDB_for_BLCA.py` & `BioSAK-1.88.2/BioSAK/GTDB_for_BLCA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/Gene2Ctg.py` & `BioSAK-1.88.2/BioSAK/Gene2Ctg.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/KEGG.py` & `BioSAK-1.88.2/BioSAK/KEGG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/KEGG_boxplot_last1row.R` & `BioSAK-1.88.2/BioSAK/KEGG_boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/KeepRemovingTmp.py` & `BioSAK-1.88.2/BioSAK/KeepRemovingTmp.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/MeanMappingDepth.py` & `BioSAK-1.88.2/BioSAK/MeanMappingDepth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/MetaBiosample.py` & `BioSAK-1.88.2/BioSAK/MetaBiosample.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/MetaCHIP_phylo.hmm` & `BioSAK-1.88.2/BioSAK/MetaCHIP_phylo.hmm`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/MetaCyc_reactions_with_ec.txt` & `BioSAK-1.88.2/BioSAK/MetaCyc_reactions_with_ec.txt`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/NetEnzymes.py` & `BioSAK-1.88.2/BioSAK/NetEnzymes.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/Newick_tree_plotter.py` & `BioSAK-1.88.2/BioSAK/Newick_tree_plotter.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/OneLineAln.py` & `BioSAK-1.88.2/BioSAK/OneLineAln.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/Prodigal.py` & `BioSAK-1.88.2/BioSAK/Prodigal.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/Reads_simulator.py` & `BioSAK-1.88.2/BioSAK/Reads_simulator.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/RunGraphMB.py` & `BioSAK-1.88.2/BioSAK/RunGraphMB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/SILVA_for_BLCA.py` & `BioSAK-1.88.2/BioSAK/SILVA_for_BLCA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/SankeyTaxon.py` & `BioSAK-1.88.2/BioSAK/SankeyTaxon.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/SliceMSA.py` & `BioSAK-1.88.2/BioSAK/SliceMSA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/SubsampleLongReads.py` & `BioSAK-1.88.2/BioSAK/SubsampleLongReads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/Tax4Fun2IndOTU.py` & `BioSAK-1.88.2/BioSAK/Tax4Fun2IndOTU.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/VERSION` & `BioSAK-1.88.2/BioSAK/VERSION`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-1.88.1
+1.88.2
 - fixed bugs
 
 1.88.0
 - new modules added: count_num
 
 1.87.0
 - new modules added: compare_sets
```

### Comparing `BioSAK-1.88.1/BioSAK/VisGeneFlk.py` & `BioSAK-1.88.2/BioSAK/VisGeneFlk.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/add_desc.py` & `BioSAK-1.88.2/BioSAK/add_desc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/arCOG.py` & `BioSAK-1.88.2/BioSAK/arCOG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/bam2reads.py` & `BioSAK-1.88.2/BioSAK/bam2reads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/boxplot.py` & `BioSAK-1.88.2/BioSAK/boxplot.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/boxplot_last1row.R` & `BioSAK-1.88.2/BioSAK/boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/boxplot_matrix_COG.py` & `BioSAK-1.88.2/BioSAK/boxplot_matrix_COG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/boxplot_matrix_COG_backup.py` & `BioSAK-1.88.2/BioSAK/boxplot_matrix_COG_backup.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/boxplot_matrix_KEGG.py` & `BioSAK-1.88.2/BioSAK/boxplot_matrix_KEGG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/boxplot_matrix_dbCAN.py` & `BioSAK-1.88.2/BioSAK/boxplot_matrix_dbCAN.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/cat_fa.py` & `BioSAK-1.88.2/BioSAK/cat_fa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/cdd2cog.pl` & `BioSAK-1.88.2/BioSAK/cdd2cog.pl`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/checkm_marker.py` & `BioSAK-1.88.2/BioSAK/checkm_marker.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/compare_sets.py` & `BioSAK-1.88.2/BioSAK/compare_sets.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/compare_trees.R` & `BioSAK-1.88.2/BioSAK/compare_trees.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/compare_trees.py` & `BioSAK-1.88.2/BioSAK/compare_trees.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/count_num.py` & `BioSAK-1.88.2/BioSAK/count_num.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/cross_link_seqs.py` & `BioSAK-1.88.2/BioSAK/cross_link_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/dbCAN.py` & `BioSAK-1.88.2/BioSAK/dbCAN.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py` & `BioSAK-1.88.2/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/dwnld_sra_reads.py` & `BioSAK-1.88.2/BioSAK/dwnld_sra_reads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/enrich.py` & `BioSAK-1.88.2/BioSAK/enrich.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/exe_cmds.py` & `BioSAK-1.88.2/BioSAK/exe_cmds.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/ezaai2mat.py` & `BioSAK-1.88.2/BioSAK/ezaai2mat.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/fa2id.py` & `BioSAK-1.88.2/BioSAK/fa2id.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/fa2phy.py` & `BioSAK-1.88.2/BioSAK/fa2phy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/fa2tree.py` & `BioSAK-1.88.2/BioSAK/fa2tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/format_converter.py` & `BioSAK-1.88.2/BioSAK/format_converter.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/format_leaf_name.py` & `BioSAK-1.88.2/BioSAK/format_leaf_name.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/fq2fa.py` & `BioSAK-1.88.2/BioSAK/fq2fa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/gapseq.py` & `BioSAK-1.88.2/BioSAK/gapseq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/gbk2faa.py` & `BioSAK-1.88.2/BioSAK/gbk2faa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/gbk2ffn.py` & `BioSAK-1.88.2/BioSAK/gbk2ffn.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/gbk2fna.py` & `BioSAK-1.88.2/BioSAK/gbk2fna.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/gbk2gff.py` & `BioSAK-1.88.2/BioSAK/gbk2gff.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/gbk_to_ffn_faa.py` & `BioSAK-1.88.2/BioSAK/gbk_to_ffn_faa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/gc.py` & `BioSAK-1.88.2/BioSAK/gc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_EC_from_ko_stats_D.py` & `BioSAK-1.88.2/BioSAK/get_EC_from_ko_stats_D.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_GTDB_taxon_gnm.py` & `BioSAK-1.88.2/BioSAK/get_GTDB_taxon_gnm.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_MAG_reads_long.py` & `BioSAK-1.88.2/BioSAK/get_MAG_reads_long.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_Pfam_hmms.py` & `BioSAK-1.88.2/BioSAK/get_Pfam_hmms.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_SCG_tree.py` & `BioSAK-1.88.2/BioSAK/get_SCG_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_TopHits_taxonomy.py` & `BioSAK-1.88.2/BioSAK/get_TopHits_taxonomy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_aa_composition.py` & `BioSAK-1.88.2/BioSAK/get_aa_composition.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_bin_abundance copy.py` & `BioSAK-1.88.2/BioSAK/get_bin_abundance copy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_data_matrix.py` & `BioSAK-1.88.2/BioSAK/get_data_matrix.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_gene_depth.py` & `BioSAK-1.88.2/BioSAK/get_gene_depth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_genome_GTDB.py` & `BioSAK-1.88.2/BioSAK/get_genome_GTDB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_genome_NCBI.py` & `BioSAK-1.88.2/BioSAK/get_genome_NCBI.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_genome_NCBI_v1.py` & `BioSAK-1.88.2/BioSAK/get_genome_NCBI_v1.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_genome_NCBI_v2.py` & `BioSAK-1.88.2/BioSAK/get_genome_NCBI_v2.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_gnm_size.py` & `BioSAK-1.88.2/BioSAK/get_gnm_size.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_ko_gene_seqs.py` & `BioSAK-1.88.2/BioSAK/get_ko_gene_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_krona_plot.py` & `BioSAK-1.88.2/BioSAK/get_krona_plot.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_reads_from_sam.py` & `BioSAK-1.88.2/BioSAK/get_reads_from_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_reads_id_in_sam.py` & `BioSAK-1.88.2/BioSAK/get_reads_id_in_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_sankey_plot.R` & `BioSAK-1.88.2/BioSAK/get_sankey_plot.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_top_hit.py` & `BioSAK-1.88.2/BioSAK/get_top_hit.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/get_total_length.py` & `BioSAK-1.88.2/BioSAK/get_total_length.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/gff2chrom.py` & `BioSAK-1.88.2/BioSAK/gff2chrom.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/global_functions.py` & `BioSAK-1.88.2/BioSAK/global_functions.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/hpc3.py` & `BioSAK-1.88.2/BioSAK/hpc3.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/iTOL.py` & `BioSAK-1.88.2/BioSAK/iTOL.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/js_cmds.py` & `BioSAK-1.88.2/BioSAK/js_cmds.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/js_hpc3.py` & `BioSAK-1.88.2/BioSAK/js_hpc3.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/keep_best_hit.py` & `BioSAK-1.88.2/BioSAK/keep_best_hit.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/ko00001.keg` & `BioSAK-1.88.2/BioSAK/ko00001.keg`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/koala.py` & `BioSAK-1.88.2/BioSAK/koala.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/label_tree.R` & `BioSAK-1.88.2/BioSAK/label_tree.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/label_tree.py` & `BioSAK-1.88.2/BioSAK/label_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/link_16S_MAG.py` & `BioSAK-1.88.2/BioSAK/link_16S_MAG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/magabund.py` & `BioSAK-1.88.2/BioSAK/magabund.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/magabund2.py` & `BioSAK-1.88.2/BioSAK/magabund2.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/manipulator_fasta.py` & `BioSAK-1.88.2/BioSAK/manipulator_fasta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/manipulator_newick.py` & `BioSAK-1.88.2/BioSAK/manipulator_newick.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/mannwhitneyu.py` & `BioSAK-1.88.2/BioSAK/mannwhitneyu.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/mean_MAG_cov.py` & `BioSAK-1.88.2/BioSAK/mean_MAG_cov.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/merge_df.py` & `BioSAK-1.88.2/BioSAK/merge_df.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/merge_seq.py` & `BioSAK-1.88.2/BioSAK/merge_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/metaAssembly.py` & `BioSAK-1.88.2/BioSAK/metaAssembly.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,14 +31,54 @@
             not_detected_programs.append(needed_program)
 
     if not_detected_programs != []:
         print('%s not detected, program exited!' % ','.join(not_detected_programs))
         exit()
 
 
+def get_nonredundant_table(file_in, file_out, ignore_na):
+    col_dict = dict()
+    col_list = []
+    col_index_dict = dict()
+    line_num_index = 0
+    for each_line in open(file_in):
+        line_num_index += 1
+        line_split = each_line.strip().split('\t')
+        if line_num_index == 1:
+            col_list = line_split
+            col_index_dict = {key: i for i, key in enumerate(line_split)}
+        else:
+            for col in col_list:
+                if col not in col_dict:
+                    col_dict[col] = [line_split[col_index_dict[col]]]
+                else:
+                    col_dict[col].append(line_split[col_index_dict[col]])
+
+    # write out
+    file_out_handle = open(file_out, 'w')
+    for col in col_list:
+
+        value_list_uniq = list(set(col_dict[col]))
+        if value_list_uniq == ['']:
+            value_list_uniq = ['na']
+
+        if col not in ['Assembly BioSample Attribute Name', 'Assembly BioSample Attribute Value']:
+            if ignore_na is True:
+                if value_list_uniq != ['na']:
+                    file_out_handle.write('%s:\t%s\n' % (col, ','.join(value_list_uniq)))
+            else:
+                file_out_handle.write('%s:\t%s\n' % (col, ','.join(value_list_uniq)))
+        else:
+            biosample_attribute_name_list = col_dict.get('Assembly BioSample Attribute Name', [])
+            biosample_attribute_value_list = col_dict.get('Assembly BioSample Attribute Value', [])
+            for (name, value) in zip(biosample_attribute_name_list, biosample_attribute_value_list):
+                file_out_handle.write('Assembly BioSample Attribute %s:\t%s\n' % (name, value))
+    file_out_handle.close()
+
+
 def metaAssembly(args):
 
     assembly_id_txt = args['i']
     op_dir          = args['o']
     num_threads     = args['t']
     force_overwrite = args['f']
 
@@ -47,17 +87,18 @@
     if os.path.isdir(op_dir) is True:
         if force_overwrite is True:
             os.system('rm -r %s' % op_dir)
         else:
             print('Output folder detected, program exited!')
             exit()
 
-    tmp_dir = '%s/tmp'        % op_dir
-    op_txt  = '%s/output.txt' % op_dir
-    cmd_txt = '%s/cmds.txt'   % op_dir
+    tmp_dir             = '%s/tmp'          % op_dir
+    tmp_dir_reformatted = '%s/report'       % op_dir
+    op_txt              = '%s/summary.txt'  % op_dir
+    cmd_txt             = '%s/cmds.txt'     % op_dir
 
     os.mkdir(op_dir)
     os.mkdir(tmp_dir)
 
     assembly_id_set = set()
     if os.path.isfile(assembly_id_txt):
         for assembly_id in open(assembly_id_txt):
@@ -68,15 +109,15 @@
     else:
         assembly_id_set.add(assembly_id_txt)
 
     # prepare cmds for datasets and dataformat
     cmd_list = []
     cmd_txt_handle = open(cmd_txt, 'w')
     for assembly_id in assembly_id_set:
-        op_metadata_tsv   = '%s/%s_data_report.tsv' % (tmp_dir, assembly_id)
+        op_metadata_tsv   = '%s/%s.txt' % (tmp_dir, assembly_id)
         ncbi_datasets_cmd = 'datasets summary genome accession %s --as-json-lines | dataformat tsv genome > %s' % (assembly_id, op_metadata_tsv)
         cmd_list.append(ncbi_datasets_cmd)
         cmd_txt_handle.write(ncbi_datasets_cmd + '\n')
     cmd_txt_handle.close()
 
     # run datasets and dataformat with mp
     print('Running %s commands with %s cores' % (len(cmd_list), num_threads))
@@ -85,18 +126,21 @@
     pool.close()
     pool.join()
 
     # parse outputs from datasets and dataformat
     with open(op_txt, 'w') as op_txt_handle:
         op_txt_handle.write('Assembly\tBioSample\tDescription\tModel\tIsolation_Source\tMetagenome_Source\tHost\tLocation\tComment\n')
 
+    #os.mkdir(tmp_dir_reformatted)
+
     print('Parsing outputs from datasets and dataformat')
     missing_output_id_set = set()
     for assembly_id in assembly_id_set:
-        op_metadata_tsv = '%s/%s_data_report.tsv' % (tmp_dir, assembly_id)
+        op_metadata_tsv             = '%s/%s.txt' % (tmp_dir, assembly_id)
+        op_metadata_tsv_reformatted = '%s/%s.txt' % (tmp_dir_reformatted, assembly_id)
         if os.path.isfile(op_metadata_tsv) is False:
             missing_output_id_set.add(assembly_id)
         else:
             host = 'na'
             geo_loc_name = 'na'
             biosample_model = 'na'
             isolation_source = 'na'
@@ -136,14 +180,18 @@
                         missing_output_id_set.add(assembly_id)
 
             str_to_write = '%s\t%s\t%s\t%s\t%s\t%s\t%s\t%s\t%s' % (assembly_id, biosample_accession, biosample_description_title, biosample_model, isolation_source, metagenome_source, host, geo_loc_name, biosample_description_comment)
 
             with open(op_txt, 'a') as op_txt_handle:
                 op_txt_handle.write(str_to_write + '\n')
 
+        # reformat report file
+        # if os.path.isfile(op_metadata_tsv) is True:
+        #     get_nonredundant_table(op_metadata_tsv, op_metadata_tsv_reformatted, ignore_na=True)
+
     if len(missing_output_id_set) > 0:
         print('datasets and dataformat failed on the following IDs:')
         print(','.join(missing_output_id_set))
 
     print('Done!')
```

### Comparing `BioSAK-1.88.1/BioSAK/metabat2concoct.py` & `BioSAK-1.88.2/BioSAK/metabat2concoct.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/metabat2maxbin.py` & `BioSAK-1.88.2/BioSAK/metabat2maxbin.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/ncbi_dataset.py` & `BioSAK-1.88.2/BioSAK/ncbi_dataset.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/parse_MetaCyc_RxnDB.py` & `BioSAK-1.88.2/BioSAK/parse_MetaCyc_RxnDB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/parse_mmseqs_tsv.py` & `BioSAK-1.88.2/BioSAK/parse_mmseqs_tsv.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/plot_mag.py` & `BioSAK-1.88.2/BioSAK/plot_mag.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/plot_sam_depth.py` & `BioSAK-1.88.2/BioSAK/plot_sam_depth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/plot_tree.R` & `BioSAK-1.88.2/BioSAK/plot_tree.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/prefix_file.py` & `BioSAK-1.88.2/BioSAK/prefix_file.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/prokka.py` & `BioSAK-1.88.2/BioSAK/prokka.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/reads2bam.py` & `BioSAK-1.88.2/BioSAK/reads2bam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/rename_leaves.py` & `BioSAK-1.88.2/BioSAK/rename_leaves.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/rename_reads_for_Reago.py` & `BioSAK-1.88.2/BioSAK/rename_reads_for_Reago.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/rename_seq.py` & `BioSAK-1.88.2/BioSAK/rename_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/rename_seqs.py` & `BioSAK-1.88.2/BioSAK/rename_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/ribbon.py` & `BioSAK-1.88.2/BioSAK/ribbon.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/sam2bam.py` & `BioSAK-1.88.2/BioSAK/sam2bam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/sampling_GTDB_gnms.py` & `BioSAK-1.88.2/BioSAK/sampling_GTDB_gnms.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/select_seq.py` & `BioSAK-1.88.2/BioSAK/select_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/sep_reads_by_barcode.py` & `BioSAK-1.88.2/BioSAK/sep_reads_by_barcode.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/slice_seq.py` & `BioSAK-1.88.2/BioSAK/slice_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/split_fasta.py` & `BioSAK-1.88.2/BioSAK/split_fasta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/split_folder.py` & `BioSAK-1.88.2/BioSAK/split_folder.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/split_sam.py` & `BioSAK-1.88.2/BioSAK/split_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/submitHPC.py` & `BioSAK-1.88.2/BioSAK/submitHPC.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/subset_GTDB_meta.py` & `BioSAK-1.88.2/BioSAK/subset_GTDB_meta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/subset_df.py` & `BioSAK-1.88.2/BioSAK/subset_df.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/subset_tree.py` & `BioSAK-1.88.2/BioSAK/subset_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/top_16S_hits.py` & `BioSAK-1.88.2/BioSAK/top_16S_hits.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/top_hits_in_a_group.py` & `BioSAK-1.88.2/BioSAK/top_hits_in_a_group.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/transpose.py` & `BioSAK-1.88.2/BioSAK/transpose.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/usearch_uc.py` & `BioSAK-1.88.2/BioSAK/usearch_uc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK/wilcox.py` & `BioSAK-1.88.2/BioSAK/wilcox.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/BioSAK.egg-info/SOURCES.txt` & `BioSAK-1.88.2/BioSAK.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,15 @@
 BioSAK/split_fasta.py
 BioSAK/split_folder.py
 BioSAK/split_sam.py
 BioSAK/submitHPC.py
 BioSAK/subset_GTDB_meta.py
 BioSAK/subset_df.py
 BioSAK/subset_tree.py
+BioSAK/tmp_1.py
 BioSAK/top_16S_hits.py
 BioSAK/top_hits_in_a_group.py
 BioSAK/transpose.py
 BioSAK/usearch_uc.py
 BioSAK/wilcox.py
 BioSAK.egg-info/PKG-INFO
 BioSAK.egg-info/SOURCES.txt
```

### Comparing `BioSAK-1.88.1/LICENSE` & `BioSAK-1.88.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/README.md` & `BioSAK-1.88.2/README.md`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/bin/BioSAK` & `BioSAK-1.88.2/bin/BioSAK`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.1/setup.py` & `BioSAK-1.88.2/setup.py`

 * *Files identical despite different names*

