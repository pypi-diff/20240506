# Comparing `tmp/mavedb-2023.3.0.tar.gz` & `tmp/mavedb-2024.0.0.tar.gz`

## Comparing `mavedb-2023.3.0.tar` & `mavedb-2024.0.0.tar`

### file list

```diff
@@ -1,177 +1,232 @@
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mavedb-2023.3.0/.flake8
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 mavedb-2023.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 mavedb-2023.3.0/Dockerfile
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 mavedb-2023.3.0/alembic.ini
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mavedb-2023.3.0/requirements.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mavedb-2023.3.0/alembic/README
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 mavedb-2023.3.0/alembic/alembic_helpers.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 mavedb-2023.3.0/alembic/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 mavedb-2023.3.0/alembic/script.py.mako
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 mavedb-2023.3.0/alembic/versions/22e2d92d602e_add_publication_identifier_metadata_.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 mavedb-2023.3.0/alembic/versions/33e99d4b90cc_add_mapped_variants_table.py
--rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 mavedb-2023.3.0/alembic/versions/5cad62af3705_rename_pubmed_identifiers_table_to_publication_identifiers.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 mavedb-2023.3.0/alembic/versions/988ca84c701b_.py
--rw-r--r--   0        0        0    24200 2020-02-02 00:00:00.000000 mavedb-2023.3.0/alembic/versions/9d566d915a2c_.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mavedb-2023.3.0/alembic/versions/da9ba478647d_add_primary_publication.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 mavedb-2023.3.0/alembic/versions/f11fd758436e_.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 mavedb-2023.3.0/settings/.env.template
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/deps.py
--rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/server_main.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/db/base.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/db/session.py
--rw-r--r--   0        0        0    83435 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/array_comparison.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/authentication.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/authorization.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/exceptions.py
--rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/experiments.py
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/experiments.py.orig
--rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/identifiers.py
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/permissions.py
--rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/rxiv.py
--rw-r--r--   0        0        0    13267 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/score_sets.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/temp_urns.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/urns.py
--rw-r--r--   0        0        0     8201 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/worker.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/mave/constants.py
--rw-r--r--   0        0        0    21586 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/mave/dataset.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/mave/hgvs.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/mave/utils.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/mave/variant.py
--rw-r--r--   0        0        0    19654 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/dataframe.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/exceptions.py
--rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/identifier.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/keywords.py
--rw-r--r--   0        0        0     6662 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/publication.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/target.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/urn_re.py
--rw-r--r--   0        0        0    11673 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/utilities.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/variant.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/constants/conversion.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/constants/general.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/constants/identifier.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/constants/keywords.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/constants/publication.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/lib/validation/constants/target.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/__init__.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/access_key.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/doi_identifier.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/ensembl_identifier.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/ensembl_offset.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/experiment.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/experiment_publication_identifier.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/experiment_set.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/failed_task.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/genome_identifier.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/keyword.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/license.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/mapped_variant.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/publication_identifier.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/raw_read_identifier.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/reference_genome.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/reference_map.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/refseq_identifier.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/refseq_offset.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/role.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/score_set.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/score_set_publication_identifier.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/target_gene.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/uniprot_identifier.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/uniprot_offset.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/user.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/variant.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/wild_type_sequence.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/enums/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/enums/processing_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/legacy/__init__.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/legacy/auth_association.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/legacy/auth_code.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/legacy/auth_nonce.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/legacy/auth_partial.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/legacy/django_reversion_revision.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/models/legacy/django_reversion_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/__init__.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/access_keys.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/api_information.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/doi_identifiers.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/experiment_sets.py
--rw-r--r--   0        0        0    11562 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/experiments.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/licenses.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/mapped_variant.py
--rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/publication_identifiers.py
--rw-r--r--   0        0        0     9835 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/publication_identifiers.py.orig
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/raw_read_identifiers.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/reference_genomes.py
--rw-r--r--   0        0        0    30527 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/score_sets.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/target_gene_identifiers.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/target_genes.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/routers/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/tasks/__init__.py
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/tasks/scoreset_tasks.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/access_key.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/api_version.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/doi_identifier.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/experiment.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/experiment_set.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/external_gene_identifier.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/external_gene_identifier_offset.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/license.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/mapped_variant.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/publication_identifier.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/raw_read_identifier.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/reference_genome.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/reference_map.py
--rw-r--r--   0        0        0     8149 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/score_set.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/search.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/search.py.orig
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/target_gene.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/user.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/variant.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/wild_type_sequence.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/base/__init__.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 mavedb-2023.3.0/src/mavedb/view_models/base/base.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/helpers/__init__.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/helpers/constants.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/helpers/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/__init__.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/conftest.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/counts.csv
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/counts_with_different_variants.csv
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/counts_with_hgvs_nt_and_pro.csv
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/counts_with_score.csv
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/scores.csv
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/scores_hgvs_nt_not_match_pro.csv
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/scores_hgvs_pro_has_same_values.csv
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/scores_with_duplicate_columns.csv
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/scores_with_hgvs_nt_and_pro.csv
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/scores_with_invalid_hgvs_nt_prefix.csv
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/scores_with_invalid_hgvs_pro_prefix.csv
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/scores_with_nan_column_name.csv
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/scores_with_string.csv
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/scores_without_hgvs_column.csv
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/scores_without_score_column.csv
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/test_experiments.py
--rw-r--r--   0        0        0    18525 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/test_score_set.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/data/counts.csv
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/routers/data/scores.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/validation/__init__.py
--rw-r--r--   0        0        0    22359 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/validation/test_dataframe.py
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/validation/test_identifier.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/validation/test_keywords.py
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/validation/test_publication.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/validation/test_target.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/validation/test_urn_re.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/validation/test_utilities.py
--rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/validation/test_variant.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/view_models/__init__.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/view_models/test_external_gene_identifiers.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/view_models/test_publication_identifier.py
--rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/view_models/test_target_gene.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 mavedb-2023.3.0/tests/view_models/test_wild_type_sequence.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 mavedb-2023.3.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 mavedb-2023.3.0/LICENSE
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 mavedb-2023.3.0/README.md
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 mavedb-2023.3.0/pyproject.toml
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 mavedb-2023.3.0/PKG-INFO
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mavedb-2024.0.0/.flake8
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 mavedb-2024.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 mavedb-2024.0.0/Dockerfile
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 mavedb-2024.0.0/Dockerfile.test
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 mavedb-2024.0.0/Dockerfile.worker
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic.ini
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mavedb-2024.0.0/docker-compose-local.yml
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 mavedb-2024.0.0/requirements.txt
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 mavedb-2024.0.0/.github/workflows/run-tests-on-push.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/README
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/alembic_helpers.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/script.py.mako
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/manual_migrations/README
+-rw-r--r--   0        0        0   489011 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/manual_migrations/migrate_target_organism_to_taxonomy.py
+-rw-r--r--   0        0        0    37583 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/manual_migrations/populate_taxonomy_table.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/194cfebabe32_rename_wild_type_sequence.py
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/22e2d92d602e_add_publication_identifier_metadata_.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/33e99d4b90cc_add_mapped_variants_table.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/44d5c568f64b_simplify_reference_genome_target_.py
+-rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/5cad62af3705_rename_pubmed_identifiers_table_to_publication_identifiers.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/60103ad1cb5b_add_target_sequence_label.py
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/6fae83d65ee4_taxonomy.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/886e059ad1a8_score_set_processing_errors.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/90e7860964a2_add_target_accession.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/988ca84c701b_.py
+-rw-r--r--   0        0        0    24200 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/9d566d915a2c_.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/b3767156e04a_merge_6fae83d65ee4_and_886e059ad1a8.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/c6154dd7d9b9_add_gene_name_column_to_target_.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/da9ba478647d_add_primary_publication.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/f11fd758436e_.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 mavedb-2024.0.0/alembic/versions/fecb3e0d181d_make_urns_unique.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/README.md
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/bioutils/assemblies.pyi
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/cdot/assembly_helper.pyi
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/cdot/hgvs/dataproviders/__init__.pyi
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/cdot/hgvs/dataproviders/fasta_seqfetcher.pyi
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/cdot/hgvs/dataproviders/json_data_provider.pyi
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/exceptions.pyi
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/parser.pyi
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/sequencevariant.pyi
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/validator.pyi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/dataproviders/interface.pyi
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/dataproviders/seqfetcher.pyi
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/hgvs/dataproviders/uta.pyi
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/idutils/README.md
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/idutils/__init__.pyi
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/mavehgvs/README.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/mavehgvs/__init__.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/mavehgvs/exceptions.pyi
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/mavehgvs/position.pyi
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mavedb-2024.0.0/mypy_stubs/mavehgvs/variant.pyi
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 mavedb-2024.0.0/settings/.env.dev
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 mavedb-2024.0.0/settings/.env.template
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/__init__.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/deps.py
+-rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/server_main.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/data_providers/services.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/db/base.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/db/session.py
+-rw-r--r--   0        0        0     5554 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/authentication.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/authorization.py
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/exceptions.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/experiments.py
+-rw-r--r--   0        0        0    17221 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/identifiers.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/permissions.py
+-rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/rxiv.py
+-rw-r--r--   0        0        0    20708 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/score_sets.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/slack.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/taxonomies.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/temp_urns.py
+-rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/urns.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/mave/constants.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/mave/hgvs.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/mave/utils.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/mave/variant.py
+-rw-r--r--   0        0        0    28991 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/dataframe.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/exceptions.py
+-rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/identifier.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/keywords.py
+-rw-r--r--   0        0        0     6662 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/publication.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/target.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/urn_re.py
+-rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/utilities.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/variant.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/constants/conversion.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/constants/general.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/constants/identifier.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/constants/keywords.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/constants/publication.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/lib/validation/constants/target.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/__init__.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/access_key.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/doi_identifier.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/ensembl_identifier.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/ensembl_offset.py
+-rw-r--r--   0        0        0     6486 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/experiment.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/experiment_publication_identifier.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/experiment_set.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/genome_identifier.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/keyword.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/license.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/mapped_variant.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/publication_identifier.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/raw_read_identifier.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/refseq_identifier.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/refseq_offset.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/role.py
+-rw-r--r--   0        0        0     7981 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/score_set.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/score_set_publication_identifier.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/target_accession.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/target_gene.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/target_sequence.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/taxonomy.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/uniprot_identifier.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/uniprot_offset.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/user.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/variant.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/enums/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/enums/processing_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/__init__.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/auth_association.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/auth_code.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/auth_nonce.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/auth_partial.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/django_reversion_revision.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/models/legacy/django_reversion_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/__init__.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/access_keys.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/api_information.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/doi_identifiers.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/experiment_sets.py
+-rw-r--r--   0        0        0    11314 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/experiments.py
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/hgvs.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/licenses.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/mapped_variant.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/publication_identifiers.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/raw_read_identifiers.py
+-rw-r--r--   0        0        0    33666 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/score_sets.py
+-rw-r--r--   0        0        0    14702 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/statistics.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/target_gene_identifiers.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/target_genes.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/taxonomies.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/routers/users.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/access_key.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/api_version.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/doi_identifier.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/experiment.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/experiment_set.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/external_gene_identifier.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/external_gene_identifier_offset.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/license.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/mapped_variant.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/publication_identifier.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/raw_read_identifier.py
+-rw-r--r--   0        0        0    10086 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/score_set.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/search.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/target_accession.py
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/target_gene.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/target_sequence.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/taxonomy.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/user.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/variant.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/base/__init__.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/view_models/base/base.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/worker/__init__.py
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/worker/jobs.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 mavedb-2024.0.0/src/mavedb/worker/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/dump_rels.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/helpers/constants.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/helpers/util.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/helpers/data/refseq.NM_001637.3.fasta
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/helpers/data/refseq.NM_001637.3.fasta.fai
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/lib/__init__.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/lib/conftest.py
+-rw-r--r--   0        0        0     8460 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/lib/test_score_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/__init__.py
+-rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/conftest.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/counts.csv
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/counts_with_different_variants.csv
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/counts_with_hgvs_nt_and_pro.csv
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/counts_with_score.csv
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores.csv
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_hgvs_nt_not_match_pro.csv
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_hgvs_pro_has_same_values.csv
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_with_duplicate_columns.csv
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_with_hgvs_nt_and_pro.csv
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_with_invalid_hgvs_nt_prefix.csv
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_with_invalid_hgvs_pro_prefix.csv
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_with_nan_column_name.csv
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_with_string.csv
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_without_hgvs_column.csv
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/scores_without_score_column.csv
+-rw-r--r--   0        0        0    18066 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/test_experiments.py
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/test_hgvs.py
+-rw-r--r--   0        0        0    22111 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/test_score_set.py
+-rw-r--r--   0        0        0    16645 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/test_statistics.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/data/counts.csv
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/data/counts_acc.csv
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/data/scores.csv
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/routers/data/scores_acc.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/__init__.py
+-rw-r--r--   0        0        0    47206 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_dataframe.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_identifier.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_keywords.py
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_publication.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_target.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_urn_re.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_utilities.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/validation/test_variant.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/view_models/__init__.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/view_models/test_external_gene_identifiers.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/view_models/test_publication_identifier.py
+-rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/view_models/test_target_gene.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/view_models/test_wild_type_sequence.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/__init__.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/conftest.py
+-rw-r--r--   0        0        0    12486 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/test_jobs.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/data/counts.csv
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/data/counts_acc.csv
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/data/scores.csv
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 mavedb-2024.0.0/tests/worker/data/scores_acc.csv
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 mavedb-2024.0.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 mavedb-2024.0.0/LICENSE
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 mavedb-2024.0.0/README.md
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 mavedb-2024.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7720 2020-02-02 00:00:00.000000 mavedb-2024.0.0/PKG-INFO
```

### Comparing `mavedb-2023.3.0/alembic.ini` & `mavedb-2024.0.0/alembic.ini`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/alembic/alembic_helpers.py` & `mavedb-2024.0.0/alembic/alembic_helpers.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/alembic/env.py` & `mavedb-2024.0.0/alembic/env.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/alembic/versions/22e2d92d602e_add_publication_identifier_metadata_.py` & `mavedb-2024.0.0/alembic/versions/22e2d92d602e_add_publication_identifier_metadata_.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/alembic/versions/33e99d4b90cc_add_mapped_variants_table.py` & `mavedb-2024.0.0/alembic/versions/33e99d4b90cc_add_mapped_variants_table.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/alembic/versions/5cad62af3705_rename_pubmed_identifiers_table_to_publication_identifiers.py` & `mavedb-2024.0.0/alembic/versions/5cad62af3705_rename_pubmed_identifiers_table_to_publication_identifiers.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/alembic/versions/988ca84c701b_.py` & `mavedb-2024.0.0/alembic/versions/988ca84c701b_.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/alembic/versions/9d566d915a2c_.py` & `mavedb-2024.0.0/alembic/versions/9d566d915a2c_.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/alembic/versions/da9ba478647d_add_primary_publication.py` & `mavedb-2024.0.0/alembic/versions/da9ba478647d_add_primary_publication.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/alembic/versions/f11fd758436e_.py` & `mavedb-2024.0.0/alembic/versions/f11fd758436e_.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/settings/.env.template` & `mavedb-2024.0.0/settings/.env.dev`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/server_main.py` & `mavedb-2024.0.0/src/mavedb/server_main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-import json
 import logging
-import os
 
 import uvicorn
 from fastapi import FastAPI
 from fastapi.encoders import jsonable_encoder
 from fastapi.exceptions import RequestValidationError
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.openapi.utils import get_openapi
 from requests import Request
-from slack_sdk.webhook import WebhookClient
 from sqlalchemy.orm import configure_mappers
 from starlette import status
 from starlette.responses import JSONResponse
-from eutils._internal.exceptions import EutilsRequestError
+from eutils._internal.exceptions import EutilsRequestError  # type: ignore
 
 from mavedb.models import *
 
 from mavedb import __version__
 from mavedb.routers import (
     access_keys,
     api_information,
     doi_identifiers,
     experiment_sets,
     experiments,
+    hgvs,
     licenses,
     mapped_variant,
     publication_identifiers,
     target_gene_identifiers,
+    taxonomies,
     raw_read_identifiers,
-    reference_genomes,
     score_sets,
+    statistics,
     target_genes,
     users,
 )
-from mavedb.lib.exceptions import AmbiguousIdentifierError, NonexistentIdentifierError
+from mavedb.lib.exceptions import AmbiguousIdentifierError, NonexistentIdentifierError, MixedTargetError
+from mavedb.lib.permissions import PermissionException
+from mavedb.lib.slack import send_slack_message
 
 logging.basicConfig()
 # Un-comment this line to log all database queries:
 # logging.getLogger("sqlalchemy.engine").setLevel(logging.INFO)
 logger = logging.getLogger(__name__)
 
 
@@ -55,25 +56,35 @@
     allow_headers=["*"],
 )
 app.include_router(access_keys.router)
 app.include_router(api_information.router)
 app.include_router(doi_identifiers.router)
 app.include_router(experiment_sets.router)
 app.include_router(experiments.router)
+app.include_router(hgvs.router)
 app.include_router(licenses.router)
 app.include_router(mapped_variant.router)
 app.include_router(publication_identifiers.router)
 app.include_router(raw_read_identifiers.router)
-app.include_router(reference_genomes.router)
 app.include_router(score_sets.router)
+app.include_router(statistics.router)
 app.include_router(target_gene_identifiers.router)
 app.include_router(target_genes.router)
+app.include_router(taxonomies.router)
 app.include_router(users.router)
 
 
+@app.exception_handler(PermissionException)
+async def permission_exception_handler(request: Request, exc: PermissionException):
+    return JSONResponse(
+        {"detail": exc.message},
+        status_code=exc.http_code,
+    )
+
+
 @app.exception_handler(RequestValidationError)
 async def validation_exception_handler(request: Request, exc: RequestValidationError):
     return JSONResponse(
         status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
         content=jsonable_encoder({"detail": list(map(lambda error: customize_validation_error(error), exc.errors()))}),
     )
 
@@ -98,45 +109,37 @@
 async def nonexistent_pmid_error_exception_handler(request: Request, exc: EutilsRequestError):
     return JSONResponse(
         status_code=404,
         content={"message": str(exc)},
     )
 
 
+@app.exception_handler(MixedTargetError)
+async def mixed_target_exception_handler(request: Request, exc: MixedTargetError):
+    return JSONResponse(
+        status_code=400,
+        content={"message": str(exc)},
+    )
+
+
 def customize_validation_error(error):
+    # surface custom validation loc context
+    if error.get("ctx", {}).get("custom_loc"):
+        error = {"loc": error["ctx"]["custom_loc"], "msg": error["msg"], "type": error["type"]}
+
     if error["type"] == "type_error.none.not_allowed":
         return {"loc": error["loc"], "msg": "Required", "type": error["type"]}
     return error
 
 
-def exception_as_dict(ex):
-    return dict(
-        type=ex.__class__.__name__,
-        exception=str(ex),
-    )
-
-
 @app.exception_handler(Exception)
 async def exception_handler(request, err):
     logger.error("Uncaught exception", exc_info=err)
-    slack_webhook_url = os.getenv("SLACK_WEBHOOK_URL")
-    if slack_webhook_url is not None and len(slack_webhook_url) > 0:
-        client = WebhookClient(url=slack_webhook_url)
-        response = client.send(
-            text=json.dumps(exception_as_dict(err)),
-            blocks=[
-                {
-                    "type": "section",
-                    "text": {
-                        "type": "plain_text",
-                        "text": json.dumps(exception_as_dict(err)),
-                    },
-                }
-            ],
-        )
+    send_slack_message(err=err, request=request)
+
     return JSONResponse(status_code=500, content={"message": "Internal server error"})
 
 
 def customize_openapi_schema():
     title = "MaveDB API"
     version = __version__
     openapi_schema = get_openapi(title=title, version=version, routes=app.routes)
```

### Comparing `mavedb-2023.3.0/src/mavedb/db/session.py` & `mavedb-2024.0.0/src/mavedb/db/session.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/lib/authentication.py` & `mavedb-2024.0.0/src/mavedb/lib/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,25 +41,26 @@
             ORCID_JWT_SIGNING_PUBLIC_KEY,
             algorithms=["RS256"],
             audience=ORCID_JWT_AUDIENCE,
             # ORCID sends an at_hash when using the OpenID Connect implicit flow, even though there is no auth_token.
             options={"verify_at_hash": False},
         )
         return decoded_token
+    # TODO: should catch specific exceptions, and should log them more usefully.
     except Exception as ex:
         print(ex)
         return {}
 
 
 class JWTBearer(HTTPBearer):
     def __init__(self, auto_error: bool = True):
         super(JWTBearer, self).__init__(auto_error=auto_error)
 
     async def __call__(self, request: Request):
-        credentials: HTTPAuthorizationCredentials
+        credentials: Optional[HTTPAuthorizationCredentials]
         try:
             credentials = await super(JWTBearer, self).__call__(request)
         except HTTPException:
             credentials = None
         if credentials:
             if not credentials.scheme == "Bearer":
                 raise HTTPException(status_code=403, detail="Invalid authentication scheme.")
@@ -67,20 +68,16 @@
             if not token_payload:
                 raise HTTPException(status_code=403, detail="Invalid token or expired token.")
             return token_payload
         else:
             return None
 
     @staticmethod
-    def verify_jwt(token: str) -> bool:
-        try:
-            payload = decode_jwt(token)
-        except:
-            payload = None
-        return payload
+    def verify_jwt(token: str) -> dict:
+        return decode_jwt(token)
 
 
 ####################################################################################################
 # API key authentication
 ####################################################################################################
 
 access_token_query = APIKeyQuery(name=ACCESS_TOKEN_NAME, auto_error=False)
```

### Comparing `mavedb-2023.3.0/src/mavedb/lib/authorization.py` & `mavedb-2024.0.0/src/mavedb/lib/authorization.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/lib/exceptions.py` & `mavedb-2024.0.0/src/mavedb/lib/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,7 +144,13 @@
     pass
 
 
 class NonexistentIdentifierError(ValueError):
     """Raised when a user tries to create a publication with a non-existent identifier"""
 
     pass
+
+
+class MixedTargetError(ValueError):
+    """Raised when a user tries to create a score-set against a set of mixed targets"""
+
+    pass
```

### Comparing `mavedb-2023.3.0/src/mavedb/lib/experiments.py` & `mavedb-2024.0.0/src/mavedb/lib/experiments.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
-from operator import or_
 from typing import Optional
 
-from sqlalchemy import func
+from sqlalchemy import func, or_
 from sqlalchemy.orm import Session
 
 from mavedb.models.experiment import Experiment
 from mavedb.models.score_set import ScoreSet
 from mavedb.models.user import User
 from mavedb.view_models.search import ExperimentsSearch
 from mavedb.models.publication_identifier import PublicationIdentifier
@@ -19,42 +18,40 @@
     # .filter(ScoreSet.private.is_(False))
 
     if owner is not None:
         query = query.filter(Experiment.created_by_id == owner.id)
 
     if search.published is not None:
         if search.published:
-            query = query.filter(Experiment.published_date is not None)
+            query = query.filter(Experiment.published_date.isnot(None))
         else:
-            query = query.filter(Experiment.published_date is None)
+            query = query.filter(Experiment.published_date.is_(None))
 
     if search.text:
         lower_search_text = search.text.lower()
         query = query.filter(
             or_(
-                Experiment.urn.contains(lower_search_text),
-                Experiment.title.contains(lower_search_text),
-                Experiment.short_description.contains(lower_search_text),
-                Experiment.abstract_text.contains(lower_search_text),
+                Experiment.urn.icontains(lower_search_text),
+                Experiment.title.icontains(lower_search_text),
+                Experiment.short_description.icontains(lower_search_text),
+                Experiment.abstract_text.icontains(lower_search_text),
                 Experiment.publication_identifiers.any(
-                    func.lower(PublicationIdentifier.identifier).contains(lower_search_text)
+                    func.lower(PublicationIdentifier.identifier).icontains(lower_search_text)
                 ),
                 Experiment.publication_identifiers.any(
-                    func.lower(PublicationIdentifier.abstract).contains(lower_search_text)
+                    func.lower(PublicationIdentifier.abstract).icontains(lower_search_text)
                 ),
                 Experiment.publication_identifiers.any(
-                    func.lower(PublicationIdentifier.title).contains(lower_search_text)
+                    func.lower(PublicationIdentifier.title).icontains(lower_search_text)
                 ),
                 Experiment.publication_identifiers.any(
-                    func.lower(PublicationIdentifier.publication_journal).contains(lower_search_text)
+                    func.lower(PublicationIdentifier.publication_journal).icontains(lower_search_text)
                 ),
                 Experiment.publication_identifiers.any(
-                    func.jsonb_path_exists(
-                        PublicationIdentifier.authors, f"""$[*].name ? (@ like_regex "{lower_search_text}" flag "i")"""
-                    )
+                    func.jsonb_path_exists(PublicationIdentifier.authors, f"""$[*].name ? (@ like_regex "{lower_search_text}" flag "i")""")
                 ),
             )
         )
 
     if search.publication_identifiers:
         query = query.filter(
             ScoreSet.publication_identifiers.any(PublicationIdentifier.identifier.in_(search.publication_identifiers))
```

### Comparing `mavedb-2023.3.0/src/mavedb/lib/identifiers.py` & `mavedb-2024.0.0/src/mavedb/lib/identifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from datetime import date
-from typing import Optional, Union
+from typing import Optional, Union, Mapping
 
-import eutils
-from eutils import EutilsNCBIError
-from eutils._internal.xmlfacades.pubmedarticle import PubmedArticle
-from eutils._internal.xmlfacades.pubmedarticleset import PubmedArticleSet
+import eutils  # type: ignore
+from eutils import EutilsNCBIError  # type: ignore
+from eutils._internal.xmlfacades.pubmedarticle import PubmedArticle  # type: ignore
+from eutils._internal.xmlfacades.pubmedarticleset import PubmedArticleSet  # type: ignore
 from sqlalchemy.orm import Session
 
 from mavedb.lib.exceptions import AmbiguousIdentifierError, NonexistentIdentifierError
 from mavedb.lib.rxiv import Rxiv, RxivContentDetail
 from mavedb.lib.validation.publication import identifier_valid_for, validate_db_name
 from mavedb.models.doi_identifier import DoiIdentifier
 from mavedb.models.ensembl_identifier import EnsemblIdentifier
@@ -18,14 +18,17 @@
 from mavedb.models.raw_read_identifier import RawReadIdentifier
 from mavedb.models.refseq_identifier import RefseqIdentifier
 from mavedb.models.refseq_offset import RefseqOffset
 from mavedb.models.target_gene import TargetGene
 from mavedb.models.uniprot_identifier import UniprotIdentifier
 from mavedb.models.uniprot_offset import UniprotOffset
 
+# XXX these classes all have an "identifier" attribute but there's no superclass
+# to unify them ...
+
 EXTERNAL_GENE_IDENTIFIER_CLASSES = {
     "Ensembl": EnsemblIdentifier,
     "RefSeq": RefseqIdentifier,
     "UniProt": UniprotIdentifier,
 }
 
 EXTERNAL_GENE_IDENTIFIER_OFFSET_CLASSES = {"Ensembl": EnsemblOffset, "RefSeq": RefseqOffset, "UniProt": UniprotOffset}
@@ -145,15 +148,15 @@
             journal = "(None)" if not self.publication_journal else self.publication_journal.strip(".")
             year = "(Unknown year)" if not self.publication_year else self.publication_year
             volume = "(Unknown volume)" if not self.publication_volume else self.publication_volume
             pages = "(Unknown pages)" if not self.publication_pages else self.publication_pages
         else:
             doi_str = "" if not self.preprint_doi else self.preprint_doi
             title = "(None)" if not self.title else self.title.strip(".")
-            journal = "(None)" if not self.publication_journal else self.publication_journal.strip(".")
+            journal = "(None)" if not (hasattr(self, "publication_journal") and self.publication_journal) else self.publication_journal.strip(".")
             year = "(Unknown year)" if not self.preprint_date else self.preprint_date.year
 
             # We don't receive these fields from rxiv platforms
             volume = "(Unknown volume)"
             pages = "(Unknown pages)"
 
         return self._article_cit_fmt.format(
@@ -205,50 +208,53 @@
 #       content detail list.
 async def fetch_biorxiv_article(identifier: str) -> Optional[ExternalPublication]:
     """
     Fetch an existing bioRxiv article from Rxiv
     """
     fetch = Rxiv("https://api.biorxiv.org", "biorxiv")
     try:
-        article = fetch.content_detail(identifier=identifier)
-        article = ExternalPublication(identifier=identifier, db_name="bioRxiv", external_publication=article[-1])
+        articles = fetch.content_detail(identifier=identifier)
+        article = ExternalPublication(identifier=identifier, db_name="bioRxiv", external_publication=articles[-1])
     except IndexError:
         return None
     else:
         return article
 
 
 async def fetch_medrxiv_article(identifier: str) -> Optional[ExternalPublication]:
     """
     Fetch an existing medRxiv article from Rxiv
     """
     fetch = Rxiv("https://api.biorxiv.org", "medrxiv")
     try:
-        article = fetch.content_detail(identifier=identifier)
-        article = ExternalPublication(identifier=identifier, db_name="medRxiv", external_publication=article[-1])
+        articles = fetch.content_detail(identifier=identifier)
+        article = ExternalPublication(identifier=identifier, db_name="medRxiv", external_publication=articles[-1])
     except IndexError:
         return None
     else:
         return article
 
 
 async def find_generic_article(
     db: Session, identifier: str
-) -> dict[str, Union[ExternalPublication, PublicationIdentifier]]:
+) -> Mapping[str, Union[ExternalPublication, PublicationIdentifier]]:
     """
     Check if a provided publication identifier ambiguously identifies a publication,
     ie the same identifier is identifies publications in multiple publication databases
     that we accept.
 
     :param db: An active database session
     :param identifier: A valid publication identifier
     :return: A list of databases where this identifier exists.
     """
     valid_databases = identifier_valid_for(identifier)
     matching_articles = {}
+    pubmed_pub: Union[PublicationIdentifier, ExternalPublication, None]
+    biorxiv_pub: Union[PublicationIdentifier, ExternalPublication, None]
+    medrxiv_pub: Union[PublicationIdentifier, ExternalPublication, None]
 
     if valid_databases["PubMed"]:
         pubmed_pub = (
             db.query(PublicationIdentifier)
             .filter(PublicationIdentifier.identifier == identifier, PublicationIdentifier.db_name == "PubMed")
             .one_or_none()
         )
@@ -325,14 +331,16 @@
     """
     Find an existing publication identifier record with the specified identifier string, or create a new one.
 
     :param db: An active database session
     :param identifier: A valid publication identifier
     :return: An existing PublicationIdentifier containing the specified identifier string, or a new, unsaved PublicationIdentifier
     """
+    article: Union[PublicationIdentifier, ExternalPublication, None]
+
     matching_articles = await find_generic_article(db, identifier)
 
     if not matching_articles:
         raise NonexistentIdentifierError(
             f"No matching articles found for identifier {identifier} across all accepted publication databases."
         )
 
@@ -379,17 +387,16 @@
     :param db: An active database session
     :param identifier: A valid identifier
     :return: An existing EnsemblIdentifier, RefseqIdentifier, or UniprotIdentifier containing the specified identifier
       string, or a new, unsaved instance of one of these classes
     """
 
     # TODO Handle key errors.
-    identifier_class: Union[EnsemblIdentifier, RefseqIdentifier, UniprotIdentifier] = EXTERNAL_GENE_IDENTIFIER_CLASSES[
-        db_name
-    ]
+    identifier_class = EXTERNAL_GENE_IDENTIFIER_CLASSES[db_name]
+    assert hasattr(identifier_class, "identifier")
 
     external_gene_identifier = (
         db.query(identifier_class).filter(identifier_class.identifier == identifier).one_or_none()
     )
 
     if not external_gene_identifier:
         external_gene_identifier = identifier_class(
```

### Comparing `mavedb-2023.3.0/src/mavedb/lib/permissions.py` & `mavedb-2024.0.0/src/mavedb/lib/permissions.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,19 +20,27 @@
 class PermissionResponse:
     def __init__(self, permitted: bool, http_code: int = 403, message: Optional[str] = None):
         self.permitted = permitted
         self.http_code = http_code if not permitted else None
         self.message = message if not permitted else None
 
 
+class PermissionException(Exception):
+    def __init__(self, http_code: int, message: str):
+        self.http_code = http_code
+        self.message = message
+
+
 def has_permission(user: User, item: Base, action: Action) -> PermissionResponse:
     private = False
     user_is_owner = False
     if isinstance(item, ExperimentSet) or isinstance(item, Experiment) or isinstance(item, ScoreSet):
+        assert item.private is not None
         private = item.private
+
         user_is_owner = user is not None and item.created_by_id == user.id
 
     if isinstance(item, ExperimentSet):
         if action == Action.READ:
             if user_is_owner or not private:
                 return PermissionResponse(True)
             elif private:
@@ -52,14 +60,16 @@
             return PermissionResponse(
                 user_is_owner,
                 404 if private else 403,
                 f"experiment set with URN '{item.urn}' not found"
                 if private
                 else f"insufficient permissions for URN '{item.urn}'",
             )
+        else:
+            raise NotImplementedError(f"has_permission(User, ExperimentSet, {action})")
     elif isinstance(item, Experiment):
         if action == Action.READ:
             if user_is_owner or not private:
                 return PermissionResponse(True)
             elif private:
                 # Do not acknowledge the existence of a private entity.
                 return PermissionResponse(False, 404, f"experiment with URN '{item.urn}' not found")
@@ -77,14 +87,17 @@
             return PermissionResponse(
                 user_is_owner,
                 404 if private else 403,
                 f"experiment with URN '{item.urn}' not found"
                 if private
                 else f"insufficient permissions for URN '{item.urn}'",
             )
+        else:
+            raise NotImplementedError(f"has_permission(User, Experiment, {action})")
+
     elif isinstance(item, ScoreSet):
         if action == Action.READ:
             if user_is_owner or not private:
                 return PermissionResponse(True)
             elif private:
                 # Do not acknowledge the existence of a private entity.
                 return PermissionResponse(False, 404, f"score set with URN '{item.urn}' not found")
@@ -102,7 +115,19 @@
             return PermissionResponse(
                 user_is_owner,
                 404 if private else 403,
                 f"score set with URN '{item.urn}' not found"
                 if private
                 else f"insufficient permissions for URN '{item.urn}'",
             )
+        else:
+            raise NotImplementedError(f"has_permission(User, ScoreSet, {action})")
+    else:
+        raise NotImplementedError(f"has_permission(User, {item.__class__}, {action}")
+
+
+def assert_permission(user: User, item: Base, action: Action) -> PermissionResponse:
+    permission = has_permission(user, item, action)
+    if not permission.permitted:
+        assert permission.http_code and permission.message
+        raise PermissionException(http_code=permission.http_code, message=permission.message)
+    return permission
```

### Comparing `mavedb-2023.3.0/src/mavedb/lib/rxiv.py` & `mavedb-2024.0.0/src/mavedb/lib/rxiv.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/lib/urns.py` & `mavedb-2024.0.0/src/mavedb/lib/urns.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,24 +24,23 @@
     :param db: An active database session
     :return: The next available experiment set URN
     """
 
     # TODO We can't use func.max if an experiment set URN's numeric part will ever have anything other than 8 digits,
     # because we rely on the order guaranteed by zero-padding. This assumption is valid until we have 99999999
     # experiment sets.
-    if db.get_bind().engine.driver == "pysqlite":  # running unit tests
-        row = db.query(func.max(ExperimentSet.urn)).filter(ExperimentSet.urn.like("urn:mavedb:%")).one_or_none()
-    else:  # use PostgreSQL-specific regex operator: ~
-        row = (
-            db.query(func.max(ExperimentSet.urn)).filter(ExperimentSet.urn.op("~")("^urn:mavedb:[0-9]+$")).one_or_none()
-        )
+    row = (
+        db.query(func.max(ExperimentSet.urn)).filter(ExperimentSet.urn.op("~")("^urn:mavedb:[0-9]+$")).one_or_none()
+    )
     max_urn_number = 0
     if row and row[0]:
         max_urn = row[0]
-        max_urn_number = int(re.search("^urn:mavedb:([0-9]+)$", max_urn).groups(1)[0])
+        match = re.search("^urn:mavedb:([0-9]+)$", max_urn)
+        assert match is not None
+        max_urn_number = int(match.groups(1)[0])
     next_urn_number = max_urn_number + 1
     return f"urn:mavedb:{next_urn_number:08}"
 
 
 def generate_experiment_urn(db: Session, experiment_set: ExperimentSet, experiment_is_meta_analysis: bool):
     """
     Generate a new URN for an experiment.
@@ -60,36 +59,33 @@
     :param db: An active database session
     :param experiment_set: The experiment set to which this experiment belongs
     :param experiment_is_meta_analysis: Whether the experiment is a meta-analysis
     :return: The next available experiment URN
     """
 
     experiment_set_urn = experiment_set.urn
+    assert experiment_set_urn is not None
 
     if experiment_is_meta_analysis:
         # Do not increment for meta-analysis, since this is a singleton
         next_suffix = "0"
     else:
-        if db.get_bind().engine.driver == "pysqlite":  # running unit tests
-            published_experiments_query = (
-                db.query(Experiment)
-                .filter(Experiment.experiment_set_id == experiment_set.id)
-                .filter(Experiment.urn.like(f"{experiment_set_urn}-%"))
-            )
-        else:  # use PostgreSQL-specific regex operator: ~
-            published_experiments_query = (
-                db.query(Experiment)
-                .filter(Experiment.experiment_set_id == experiment_set.id)
-                .filter(Experiment.urn.op("~")(f"^{re.escape(experiment_set_urn)}-[a-z]+$"))
-            )
+        published_experiments_query = (
+            db.query(Experiment)
+            .filter(Experiment.experiment_set_id == experiment_set.id)
+            .filter(Experiment.urn.op("~")(f"^{re.escape(experiment_set_urn)}-[a-z]+$"))
+        )
         max_suffix = None
         for experiment in published_experiments_query:
-            suffix = re.search(f"^{re.escape(experiment_set.urn)}-([a-z]+)$", experiment.urn).group(1)
-            if suffix and (max_suffix is None or len(max_suffix) < len(experiment.urn) or max_suffix < suffix):
-                max_suffix = suffix
+            assert experiment.urn is not None
+            match = re.search(f"^{re.escape(experiment_set_urn)}-([a-z]+)$", experiment.urn)
+            if match is not None:
+                suffix = match.group(1)
+                if suffix and (max_suffix is None or len(max_suffix) < len(suffix) or max_suffix < suffix):
+                    max_suffix = suffix
         if max_suffix is None:
             next_suffix = "a"
         else:
             max_suffix_number = 0
             while len(max_suffix) > 0:
                 max_suffix_number *= 26
                 max_suffix_number += string.ascii_lowercase.index(max_suffix[0]) + 1
@@ -116,27 +112,24 @@
 
     :param db: An active database session
     :param experiment: The experiment to which this score set belongs
     :return: The next available score set URN
     """
 
     experiment_urn = experiment.urn
+    assert experiment_urn is not None
 
-    if db.get_bind().engine.driver == "pysqlite":  # running unit tests
-        published_score_sets_query = (
-            db.query(ScoreSet)
-            .filter(ScoreSet.experiment_id == experiment.id)
-            .filter(ScoreSet.urn.like(f"{experiment_urn}-%"))
-        )
-    else:  # use PostgreSQL-specific regex operator: ~
-        published_score_sets_query = (
-            db.query(ScoreSet)
-            .filter(ScoreSet.experiment_id == experiment.id)
-            .filter(ScoreSet.urn.op("~")(f"^{re.escape(experiment_urn)}-[0-9]+$"))
-        )
+    published_score_sets_query = (
+        db.query(ScoreSet)
+        .filter(ScoreSet.experiment_id == experiment.id)
+        .filter(ScoreSet.urn.op("~")(f"^{re.escape(experiment_urn)}-[0-9]+$"))
+    )
     max_suffix_number = 0
     for score_set in published_score_sets_query:
-        suffix_number = int(re.search(f"^{re.escape(experiment.urn)}-([0-9]+)$", score_set.urn).group(1))
-        if suffix_number > max_suffix_number:
-            max_suffix_number = suffix_number
+        assert score_set.urn is not None
+        match = re.search(f"^{re.escape(experiment_urn)}-([0-9]+)$", score_set.urn)
+        if match is not None:
+            suffix_number = int(match.group(1))
+            if suffix_number > max_suffix_number:
+                max_suffix_number = suffix_number
     next_suffix_number = max_suffix_number + 1
     return f"{experiment_urn}-{next_suffix_number}"
```

### Comparing `mavedb-2023.3.0/src/mavedb/lib/mave/hgvs.py` & `mavedb-2024.0.0/src/mavedb/lib/mave/hgvs.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/lib/mave/utils.py` & `mavedb-2024.0.0/src/mavedb/lib/mave/utils.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/lib/mave/variant.py` & `mavedb-2024.0.0/src/mavedb/lib/mave/variant.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/lib/validation/dataframe.py` & `mavedb-2024.0.0/src/mavedb/lib/validation/dataframe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+from typing import Optional, Tuple, Union
+
+import hgvs.exceptions
+import hgvs.parser
+import hgvs.validator
+from cdot.hgvs.dataproviders import RESTDataProvider
+import numpy as np
 import pandas as pd
-from mavehgvs.variant import Variant
+
+from fqfa.util.translate import translate_dna
 from mavehgvs.exceptions import MaveHgvsParseError
-import numpy as np
-from typing import Optional, Tuple
+from mavehgvs.variant import Variant
 
+from mavedb.lib.exceptions import MixedTargetError
 from mavedb.lib.validation.constants.general import (
     hgvs_nt_column,
-    hgvs_splice_column,
     hgvs_pro_column,
+    hgvs_splice_column,
     required_score_column,
 )
 from mavedb.lib.validation.exceptions import ValidationError
-from fqfa.util.translate import translate_dna
+from mavedb.models.target_accession import TargetAccession
+from mavedb.models.target_gene import TargetGene
+from mavedb.models.target_sequence import TargetSequence
 
 # handle with pandas all null strings
 # provide a csv or a pandas dataframe
 # take dataframe, output as csv to temp directory, use standard library
 
 
 STANDARD_COLUMNS = (hgvs_nt_column, hgvs_splice_column, hgvs_pro_column, required_score_column)
@@ -100,158 +110,132 @@
         The dataframe to standardize
 
     Returns
     -------
     pandas.DataFrame
         The standardized dataframe
     """
-    new_columns = [x.lower() if x.lower() in STANDARD_COLUMNS else x for x in df.columns]
-    df.columns = new_columns
-
-    return sort_dataframe_columns(df)
+    column_mapper = {x: x.lower() for x in df.columns if x.lower() in STANDARD_COLUMNS}
 
+    df.rename(columns=column_mapper, inplace=True)
 
-def validate_dataframe(df: pd.DataFrame, kind: str, target_seq: str, target_seq_type: str) -> None:
-    """
-    Validate that a given dataframe passes all checks.
-
-    Parameters
-    ----------
-    df : pandas.DataFrame
-        The dataframe to validate
-    kind : str
-        The kind of dataframe "counts" or "scores"
-    target_seq : str
-        The target sequence to validate variants against
-    target_seq_type : str
-        The kind of target sequence, one of "infer" "dna" or "protein"
-
-    Returns
-    -------
-    None
-
-    Raises
-    ------
-    ValidationError
-        If one of the validators called raises an exception
-    """
-    # basic checks
-    validate_column_names(df, kind)
-    validate_no_null_rows(df)
-
-    # validate individual columns
-    column_mapping = {c.lower(): c for c in df.columns}
-    index_column = choose_dataframe_index_column(df)
-    for c in column_mapping:
-        if c in (hgvs_nt_column, hgvs_splice_column, hgvs_pro_column):
-            is_index = column_mapping[c] == index_column
-            if is_index or not df[column_mapping[c]].isna().all():  # ignore null non-index HGVS columns
-                validate_hgvs_column(df[column_mapping[c]], is_index, target_seq, target_seq_type)
-        else:
-            force_numeric = (c == required_score_column) or (kind == "counts")
-            validate_data_column(df[column_mapping[c]], force_numeric)
-
-    # validate hgvs agreement
-    prefixes = dict()
-    for c in (hgvs_nt_column, hgvs_splice_column, hgvs_pro_column):
-        prefixes[c] = None
-        if c in column_mapping:
-            if not df[column_mapping[c]].isna().all():
-                prefixes[c] = df[column_mapping[c]].dropna()[0][0]
-    validate_hgvs_prefix_combinations(
-        hgvs_nt=prefixes[hgvs_nt_column], hgvs_splice=prefixes[hgvs_splice_column], hgvs_pro=prefixes[hgvs_pro_column]
-    )
+    return sort_dataframe_columns(df)
 
 
 def validate_and_standardize_dataframe_pair(
-    scores_df: pd.DataFrame, counts_df: Optional[pd.DataFrame], target_seq: str, target_seq_type: str
+    scores_df: pd.DataFrame, counts_df: Optional[pd.DataFrame], targets: list[TargetGene], hdp: RESTDataProvider
 ) -> Tuple[pd.DataFrame, Optional[pd.DataFrame]]:
     """
     Perform validation and standardization on a pair of score and count dataframes.
 
     Parameters
     ----------
     scores_df : pandas.DataFrame
         The scores dataframe
     counts_df : Optional[pandas.DataFrame]
         The counts dataframe, can be None if not present
-    target_seq : str
-        The target sequence for the dataset
-    target_seq_type : str
-        The target sequence type, can be "infer" "dna" or "protein"
+    targets : str
+        The target genes on which to validate dataframes
+    hdp : RESTDataProvider
+        The biocommons.hgvs compatible data provider. Used to fetch sequences for hgvs validation.
 
     Returns
     -------
     Tuple[pd.DataFrame, Optional[pd.DataFrame]]
         The standardized score and count dataframes, or score and None if no count dataframe was provided
 
     Raises
     ------
     ValidationError
         If one of the validation functions raises an exception
     """
-    # validate the dataframes
-    validate_dataframe(scores_df, "scores", target_seq, target_seq_type)
+    if not targets:
+        raise ValueError("Can't validate provided file with no targets.")
+
+    validate_dataframe(scores_df, "scores", targets, hdp)
     if counts_df is not None:
-        validate_dataframe(counts_df, "counts", target_seq, target_seq_type)
+        validate_dataframe(counts_df, "counts", targets, hdp)
         validate_variant_columns_match(scores_df, counts_df)
 
     new_scores_df = standardize_dataframe(scores_df)
-    if counts_df is not None:
-        new_counts_df = standardize_dataframe(counts_df)
-    else:
-        new_counts_df = None
+    new_counts_df = standardize_dataframe(counts_df) if counts_df is not None else None
     return new_scores_df, new_counts_df
 
 
-def choose_dataframe_index_column(df: pd.DataFrame) -> str:
+def validate_dataframe(df: pd.DataFrame, kind: str, targets: list["TargetGene"], hdp: RESTDataProvider) -> None:
     """
-    Identify the HGVS variant column that should be used as the index column in this dataframe.
+    Validate that a given dataframe passes all checks.
 
     Parameters
     ----------
     df : pandas.DataFrame
-        The dataframe to check
+        The dataframe to validate
+    kind : str
+        The kind of dataframe "counts" or "scores"
+    target_seq : str
+        The target sequence to validate variants against
+    target_seq_type : str
+        The kind of target sequence, one of "infer" "dna" or "protein"
 
     Returns
     -------
-    str
-        The column name of the index column
+    None
 
     Raises
     ------
     ValidationError
-        If no valid HGVS variant column is found
+        If one of the validators called raises an exception
     """
-    column_mapping = {c.lower(): c for c in df.columns if not df[c].isna().all()}
+    # basic checks
+    validate_column_names(df, kind)
+    validate_no_null_rows(df)
 
-    if hgvs_nt_column in column_mapping:
-        return column_mapping[hgvs_nt_column]
-    elif hgvs_pro_column in column_mapping:
-        return column_mapping[hgvs_pro_column]
-    else:
-        raise ValidationError("failed to find valid HGVS variant column")
+    column_mapping = {c.lower(): c for c in df.columns}
+    index_column = choose_dataframe_index_column(df)
 
+    prefixes: dict[str, Optional[str]] = dict()
+    for c in column_mapping:
+        if c in (hgvs_nt_column, hgvs_splice_column, hgvs_pro_column):
+            is_index = column_mapping[c] == index_column
+            prefixes[c] = None
 
-def validate_no_null_rows(df: pd.DataFrame) -> None:
-    """Check that there are no fully null rows in the dataframe.
+            # Ignore validation for null non-index hgvs columns
+            if df[column_mapping[c]].isna().all() and not is_index:
+                continue
+
+            # This is typesafe, despite Pylance's claims otherwise
+            if all(target.target_accession for target in targets):
+                validate_hgvs_genomic_column(
+                    df[column_mapping[c]], is_index, [target.target_accession for target in targets], hdp  # type: ignore
+                )
+            elif all(target.target_sequence for target in targets):
+                validate_hgvs_transgenic_column(
+                    df[column_mapping[c]], is_index, {target.target_sequence.label: target.target_sequence for target in targets}  # type: ignore
+                )
+            else:
+                raise MixedTargetError("Could not validate dataframe against provided mixed target types.")
+
+            # post validation, handle prefixes. We've already established these columns are non-null
+            if len(targets) > 1:
+                prefixes[c] = (
+                    df[column_mapping[c]].dropna()[0].split(" ")[0].split(":")[1][0]
+                )  # Just take the first prefix, we validate consistency elsewhere
+            else:
+                prefixes[c] = df[column_mapping[c]].dropna()[0][0]
 
-    Parameters
-    __________
-    df : pandas.DataFrame
-        The scores or counts dataframe being validated
+        else:
+            force_numeric = (c == required_score_column) or (kind == "counts")
+            validate_data_column(df[column_mapping[c]], force_numeric)
 
-    Raises
-    ______
-    ValidationError
-        If there are null rows in the dataframe
-    """
-    null_rows = df.apply(lambda row: np.all(row.isna()), axis=1)
-    if sum(null_rows) > 0:
-        raise ValidationError(f"found {sum(null_rows)} null rows in the data frame")
+    validate_hgvs_prefix_combinations(
+        hgvs_nt=prefixes[hgvs_nt_column],
+        hgvs_splice=prefixes[hgvs_splice_column],
+        hgvs_pro=prefixes[hgvs_pro_column],
+        transgenic=all(target.target_sequence for target in targets),
+    )
 
 
 def validate_column_names(df: pd.DataFrame, kind: str) -> None:
     """Validate the column names in a dataframe.
 
     This function validates the column names in the given dataframe.
     It can be run for either a "scores" dataframe or a "counts" dataframe.
@@ -304,112 +288,356 @@
     if set(columns).isdisjoint({hgvs_nt_column, hgvs_splice_column, hgvs_pro_column}):
         raise ValidationError("dataframe does not define any variant columns")
 
     if set(columns).issubset({hgvs_nt_column, hgvs_splice_column, hgvs_pro_column}):
         raise ValidationError("dataframe does not define any data columns")
 
 
-def validate_hgvs_column(column: pd.Series, is_index: bool, target_seq: str, target_seq_type) -> None:
+def validate_no_null_rows(df: pd.DataFrame) -> None:
+    """Check that there are no fully null rows in the dataframe.
+
+    Parameters
+    __________
+    df : pandas.DataFrame
+        The scores or counts dataframe being validated
+
+    Raises
+    ______
+    ValidationError
+        If there are null rows in the dataframe
+    """
+    if any(df.isnull().all(axis=1)):
+        raise ValidationError(f"found {len(df[df.isnull().all(axis=1)])} null rows in the data frame")
+
+
+def choose_dataframe_index_column(df: pd.DataFrame) -> str:
+    """
+    Identify the HGVS variant column that should be used as the index column in this dataframe.
+
+    Parameters
+    ----------
+    df : pandas.DataFrame
+        The dataframe to check
+
+    Returns
+    -------
+    str
+        The column name of the index column
+
+    Raises
+    ------
+    ValidationError
+        If no valid HGVS variant column is found
+    """
+    column_mapping = {c.lower(): c for c in df.columns if not df[c].isna().all()}
+
+    if hgvs_nt_column in column_mapping:
+        return column_mapping[hgvs_nt_column]
+    elif hgvs_pro_column in column_mapping:
+        return column_mapping[hgvs_pro_column]
+    else:
+        raise ValidationError("failed to find valid HGVS variant column")
+
+
+def validate_hgvs_transgenic_column(column: pd.Series, is_index: bool, targets: dict[str, "TargetSequence"]) -> None:
     """
     Validate the variants in an HGVS column from a dataframe.
 
     Tests whether the column has a correct and consistent prefix.
     This function also validates all individual variants in the column and checks for agreement against the target
     sequence (for non-splice variants).
 
+    Implementation NOTE: We assume variants will only be presented as fully qualified (accession:variant)
+    if this column is being validated against multiple targets.
+
     Parameters
     ----------
     column : pd.Series
         The column from the dataframe to validate
     is_index : bool
         True if this is the index column for the dataframe and therefore cannot have missing values; else False
-    target_seq : str
-        The target sequence to validate against
-    target_seq_type : str
-        The type of target sequence, which can be one of "dna", "protein", or "infer"
+    targets : dict
+        Dictionary containing a mapping of target gene names to their sequences.
 
     Returns
     -------
     None
 
     Raises
     ------
     ValueError
         If the target sequence does is not dna or protein (or inferred as dna or protein)
     ValueError
         If the target sequence is not valid for the variants (e.g. protein sequence for nucleotide variants)
-    ValueError
-        If the column name is not recognized
-    ValidationError
-        If the column contains multiple prefixes or the wrong prefix for that column name
-    ValidationError
-        If an index column contains missing values
     ValidationError
         If one of the variants fails validation
     """
-    if target_seq_type not in ("dna", "protein"):
-        raise ValueError("invalid target sequence type")
+    valid_sequence_types = ("dna", "protein")
+    validate_variant_column(column, is_index)
+    prefixes = generate_variant_prefixes(column)
+    validate_variant_formatting(column, prefixes, list(targets.keys()))
+
+    observed_sequence_types = [target.sequence_type for target in targets.values()]
+    invalid_sequence_types = set(observed_sequence_types) - set(valid_sequence_types)
+    if invalid_sequence_types:
+        raise ValueError(
+            f"Some targets are invalid sequence types: {invalid_sequence_types}. Sequence types shoud be one of: {valid_sequence_types}"
+        )
 
-    if infer_column_type(column) not in ("string", "empty"):
-        raise ValidationError(f"variant column '{column.name}' cannot contain numeric data")
+    # If this is the `hgvs_nt` column, at least one target should be of type `dna`.
+    if str(column.name).lower() == hgvs_nt_column:
+        if "dna" not in observed_sequence_types:
+            raise ValueError(
+                f"invalid target sequence type(s) for '{column.name}'. At least one target should be of type `dna`. Observed types: {observed_sequence_types}"
+            )
 
-    if is_index:
-        if column.isna().any():
-            raise ValidationError(f"primary variant column '{column.name}' cannot contain null values")
-        if not column.is_unique:
-            raise ValidationError(f"primary variant column '{column.name}' must contain unique values")
-
-    # check the variant prefixes
-    if column.name.lower() == hgvs_nt_column:
-        prefixes = [f"{a}." for a in "cngmo"]
-    elif column.name.lower() == hgvs_splice_column:
-        prefixes = [f"{a}." for a in "cn"]
-    elif column.name.lower() == hgvs_pro_column:
-        prefixes = ["p."]
-    else:
+    # Make sure this column is either the splice column or protein column.
+    elif str(column.name).lower() != hgvs_splice_column and str(column.name).lower() != hgvs_pro_column:
         raise ValueError(f"unrecognized hgvs column name '{column.name}'")
-    if len(set(s[:2] for s in column.dropna())) > 1:
-        raise ValidationError(f"variant column '{column.name}' has inconsistent variant prefixes")
-    if not all(s[:2] in prefixes for s in column.dropna()):
-        raise ValidationError(f"variant column '{column.name}' has invalid variant prefixes")
 
-    # validate the individual variant strings
-    # prepare the target sequence for validation
-    if column.name.lower() == hgvs_nt_column:
-        if target_seq_type != "dna":
-            raise ValueError(f"invalid target sequence type for '{column.name}'")
-    elif column.name.lower() == hgvs_splice_column:
-        target_seq = None  # don't validate splice variants against the target sequence
-    elif column.name.lower() == hgvs_pro_column:
-        if target_seq_type == "dna":
-            target_seq = translate_dna(target_seq)[0]  # translate the target sequence if needed
-    else:
-        raise ValueError(f"unrecognized hgvs column name '{column.name}'")
+    # Build dictionary of target sequences based on the column we are validating.
+    target_seqs: dict[str, Union[str, None]] = {}
+    for name, target in targets.items():
+        if str(column.name).lower() == hgvs_nt_column:
+            target_seqs[name] = target.sequence
+
+        # don't validate splice columns against provided sequences.
+        elif str(column.name).lower() == hgvs_splice_column:
+            target_seqs[name] = None
+
+        # translate the target sequence if needed.
+        elif str(column.name).lower() == hgvs_pro_column:
+            if target.sequence_type == "dna" and target.sequence is not None:
+                target_seqs[name] = translate_dna(target.sequence)[0]
+            else:
+                target_seqs[name] = target.sequence
+
     # get a list of all invalid variants
     invalid_variants = list()
     for i, s in column.items():
-        if s is not None:
-            try:
-                Variant(s, targetseq=target_seq)
-            except MaveHgvsParseError:
+        if not s:
+            continue
+
+        # variants can exist on the same line separated by a space
+        for variant in s.split(" "):
+            # When there are multiple targets, treat provided variants as fully qualified.
+            if len(targets) > 1:
+                name, variant = str(variant).split(":")
+            else:
+                name = list(targets.keys())[0]
+            if variant is not None:
                 try:
-                    Variant(s)  # note this will get called a second time for splice variants
+                    Variant(variant, targetseq=target_seqs[name])
                 except MaveHgvsParseError:
-                    invalid_variants.append(f"invalid variant string '{s}' at row {i}")
-                else:
-                    invalid_variants.append(f"target sequence mismatch for '{s}' at row {i}")
+                    try:
+                        Variant(variant)  # note this will get called a second time for splice variants
+                    except MaveHgvsParseError:
+                        invalid_variants.append(f"invalid variant string '{variant}' at row {i} for sequence {name}")
+                    else:
+                        invalid_variants.append(
+                            f"target sequence mismatch for '{variant}' at row {i} for sequence {name}"
+                        )
+
     # format and raise an error message that contains all invalid variants
     if len(invalid_variants) > 0:
         raise ValidationError(
-            f"encountered {len(invalid_variants)} invalid variant strings: {(', '.join(invalid_variants))}"
+            f"encountered {len(invalid_variants)} invalid variant strings.", triggers=invalid_variants
         )
 
 
+def validate_hgvs_genomic_column(
+    column: pd.Series, is_index: bool, targets: list["TargetAccession"], hdp: RESTDataProvider
+) -> None:
+    """
+    Validate the variants in an HGVS column from a dataframe.
+
+    Tests whether the column has a correct and consistent prefix.
+    This function also validates all individual variants in the column and checks for agreement against the target
+    sequence (for non-splice variants).
+
+    Implementation NOTE: We assume variants will only be presented as fully qualified (accession:variant)
+    if this column is being validated against multiple targets.
+
+    Parameters
+    ----------
+    column : pd.Series
+        The column from the dataframe to validate
+    is_index : bool
+        True if this is the index column for the dataframe and therefore cannot have missing values; else False
+    targets : list
+        Dictionary containing a list of target accessions.
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValueError
+        If the target sequence does is not dna or protein (or inferred as dna or protein)
+    ValueError
+        If the target sequence is not valid for the variants (e.g. protein sequence for nucleotide variants)
+    ValidationError
+        If one of the variants fails validation
+    """
+    validate_variant_column(column, is_index)
+    prefixes = generate_variant_prefixes(column)
+    validate_variant_formatting(
+        column, prefixes, [target.accession for target in targets if target.accession is not None]
+    )
+
+    # validate the individual variant strings
+    # prepare the target sequences for validation
+    target_seqs: dict[str, Union[str, None]] = {}
+    for target in targets:
+        assert target.accession is not None
+        # We shouldn't have to worry about translating protein sequences when we deal with accession based variants
+        if str(column.name).lower() == hgvs_nt_column or str(column.name).lower() == hgvs_pro_column:
+            target_seqs[target.accession] = target.accession
+
+        # TODO: no splice col for genomic coordinate variants?
+        elif str(column.name).lower() == hgvs_splice_column:
+            target_seqs[target.accession] = None  # don't validate splice variants against a target sequence
+
+        else:
+            raise ValueError(f"unrecognized hgvs column name '{column.name}'")
+
+    hp = hgvs.parser.Parser()
+    vr = hgvs.validator.Validator(hdp=hdp)
+
+    invalid_variants = list()
+    for i, s in column.items():
+        if s is not None:
+            for variant in s.split(" "):
+                # Add accession info when we only have one target
+                if len(targets) == 1:
+                    s = f"{targets[0].accession}:{variant}"
+                try:
+                    # We set strict to `False` to suppress validation warnings about intronic variants.
+                    vr.validate(hp.parse(s), strict=False)
+                except hgvs.exceptions.HGVSError as e:
+                    invalid_variants.append(f"Failed to parse row {i} with HGVS exception: {e}")
+
+    # format and raise an error message that contains all invalid variants
+    if len(invalid_variants) > 0:
+        raise ValidationError(
+            f"encountered {len(invalid_variants)} invalid variant strings.", triggers=invalid_variants
+        )
+
+
+def validate_variant_formatting(column: pd.Series, prefixes: list[str], targets: list[str]):
+    """
+    Validate the formatting of HGVS variants present in the passed column against
+    lists of prefixes and targets
+
+    Parameters
+    ----------
+    column : pd.Series
+        A pandas column containing HGVS variants
+    prefixes : list[str]
+        A list of prefixes we can expect to occur within the passed column
+    targets : list[str]
+        A list of targets we can expect to occur within the passed column
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValidationError
+        If any of the variants in the column are not fully qualified with respect to multiple possible targets
+    ValidationError
+        If the column contains multiple prefixes or the wrong prefix for that column name
+    ValidationError
+        If the column contains target accessions not present in the list of possible targets
+    """
+    variants = [variant for s in column.dropna() for variant in s.split(" ")]
+
+    # if there is more than one target, we expect variants to be fully qualified
+    if len(targets) > 1:
+        if not all(len(str(v).split(":")) == 2 for v in variants):
+            raise ValidationError(
+                f"variant column '{column.name}' needs fully qualified coordinates when validating against multiple targets"
+            )
+        if len(set(str(v).split(":")[1][:2] for v in variants)) > 1:
+            raise ValidationError(f"variant column '{column.name}' has inconsistent variant prefixes")
+        if not all(str(v).split(":")[1][:2] in prefixes for v in variants):
+            raise ValidationError(f"variant column '{column.name}' has invalid variant prefixes")
+        if not all(str(v).split(":")[0] in targets for v in variants):
+            raise ValidationError(f"variant column '{column.name}' has invalid accession identifiers")
+
+    else:
+        if len(set(v[:2] for v in variants)) > 1:
+            raise ValidationError(f"variant column '{column.name}' has inconsistent variant prefixes")
+        if not all(v[:2] in prefixes for v in variants):
+            raise ValidationError(f"variant column '{column.name}' has invalid variant prefixes")
+
+
+def generate_variant_prefixes(column: pd.Series):
+    """
+    Generate variant prefixes for the provided column
+
+    Parameters
+    ----------
+    column : pd.Series
+        The pandas column from which to generate variant prefixes
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValueError
+        If the provided pandas column has an unrecognized variant column name
+    """
+    if str(column.name).lower() == hgvs_nt_column:
+        return [f"{a}." for a in "cngmo"]
+    if str(column.name).lower() == hgvs_splice_column:
+        return [f"{a}." for a in "cn"]
+    if str(column.name).lower() == hgvs_pro_column:
+        return ["p."]
+
+    raise ValueError(f"unrecognized hgvs column name '{column.name}'")
+
+
+def validate_variant_column(column: pd.Series, is_index: bool):
+    """
+    Validate critical column properties of an HGVS variant column, with special
+    attention to certain properties expected on index columns
+
+    Parameters
+    ----------
+    column : pd.Series
+        The pandas column containing HGVS variant information
+    id_index : bool
+        Whether the provided column is the index column
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValidationError
+        If an index column contains missing or non-unique values
+    ValidationError
+        If a column contains any numeric data
+    """
+    if infer_column_type(column) not in ("string", "empty"):
+        raise ValidationError(f"variant column '{column.name}' cannot contain numeric data")
+    if column.isna().any() and is_index:
+        raise ValidationError(f"primary variant column '{column.name}' cannot contain null values")
+    if not column.is_unique and is_index:
+        raise ValidationError(f"primary variant column '{column.name}' must contain unique values")
+
+
 def validate_hgvs_prefix_combinations(
-    hgvs_nt: Optional[str], hgvs_splice: Optional[str], hgvs_pro: Optional[str]
+    hgvs_nt: Optional[str], hgvs_splice: Optional[str], hgvs_pro: Optional[str], transgenic: bool
 ) -> None:
     """
     Validate the combination of HGVS variant prefixes.
 
     This function assumes that other validation, such as checking that all variants in the column have the same prefix,
     has already been performed.
 
@@ -417,14 +645,16 @@
     ----------
     hgvs_nt : Optional[str]
         The first character (prefix) of the HGVS nucleotide variant strings, or None if not used.
     hgvs_splice : Optional[str]
         The first character (prefix) of the HGVS splice variant strings, or None if not used.
     hgvs_pro : Optional[str]
         The first character (prefix) of the HGVS protein variant strings, or None if not used.
+    transgenic : bool
+        Whether we should validate these prefix combinations as transgenic variants
 
     Returns
     -------
     None
 
     Raises
     ------
@@ -453,16 +683,17 @@
                 raise ValidationError("splice variants must use 'n.' prefix when protein variants are not present")
     elif hgvs_pro is not None and hgvs_nt is not None:
         if hgvs_nt != "c":
             raise ValidationError(
                 "nucleotide variants must use 'c.' prefix when protein variants are present and splicing variants are"
                 " not present"
             )
+    # Only raise if this data will not be validated by biocommons.hgvs
     elif hgvs_nt is not None:  # just hgvs_nt
-        if hgvs_nt != "n":
+        if hgvs_nt != "n" and transgenic:
             raise ValidationError("nucleotide variants must use 'n.' prefix when only nucleotide variants are defined")
 
 
 def validate_variant_consistency(df: pd.DataFrame) -> None:
     """
     Ensure that variants defined in a single row describe the same variant.
```

### Comparing `mavedb-2023.3.0/src/mavedb/lib/validation/identifier.py` & `mavedb-2024.0.0/src/mavedb/lib/validation/identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/lib/validation/keywords.py` & `mavedb-2024.0.0/src/mavedb/lib/validation/keywords.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/lib/validation/publication.py` & `mavedb-2024.0.0/src/mavedb/lib/validation/publication.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/lib/validation/target.py` & `mavedb-2024.0.0/src/mavedb/lib/validation/target.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/lib/validation/urn_re.py` & `mavedb-2024.0.0/src/mavedb/lib/validation/urn_re.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/lib/validation/utilities.py` & `mavedb-2024.0.0/src/mavedb/lib/validation/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from random import choice
-from typing import Optional
+from typing import Optional, SupportsIndex
 
 from mavedb.lib.validation.constants.conversion import codon_dict_DNA
 from mavedb.lib.validation.constants.conversion import aa_dict_key_1
 from mavedb.lib.validation.constants.general import null_values_re
 from mavehgvs.variant import Variant
 
 
@@ -148,17 +148,17 @@
     if _is_wild_type(hgvs_nt):  # variant_codon is wild-type
         codon_number = None
         target_codon = None
     else:  # any other variant change
         # instantiate Variant object
         variant = Variant(hgvs_nt)
         # get variant position and convert to int
-        if type(variant.positions) == list:  # multiple positions values exist
+        if type(variant.positions) is list:  # multiple positions values exist
             variant_position = int(str(variant.positions[0]))
-        elif type(variant.positions) == tuple:
+        elif type(variant.positions) is tuple:
             variant_position = int(str(variant.positions[0]))
         else:  # only one value for positions
             variant_position = int(str(variant.positions))
         # now that we have the variant_position, get codon_number
         codon_number = round((variant_position / 3) + 0.5)
         # use codon_number to get target_codon from target_seq
         target_codon = target_seq[(codon_number - 1) * 3 : codon_number * 3]
@@ -180,37 +180,42 @@
     if _is_wild_type(hgvs_nt):  # variant_codon is wild-type
         variant_codon = target_codon
         sub_one = None  # no nucleotide substitutions
     elif _is_deletion(hgvs_nt):  # target_codon was deleted
         variant_codon = None
         sub_one = None  # no nucleotide substitutions
     elif _is_substitution_one_base(hgvs_nt):  # variant_codon has one nucleotide substitution
+        assert isinstance(variant.sequence, SupportsIndex)
         # instantiate Variant object
         variant = Variant(hgvs_nt)
         # get index of nucleotide substitution
         sub_one = int(str(variant.positions)) % 3 - 1
         # get nucleotide of substitution
         sub_one_nuc = variant.sequence[1]
         # set other possible indices for codon substitution to None
         sub_two = None
         sub_three = None
     elif _is_substitution_two_bases_nonadjacent(hgvs_nt):  # variant has two nucleotide substitutions, non-adjacent
         # instantiate Variant object
         variant = Variant(hgvs_nt)
+        assert isinstance(variant.sequence, SupportsIndex)
+        assert isinstance(variant.positions, SupportsIndex)
         # get indices of nucleotide substitutions
         sub_one = int(str(variant.positions[0])) % 3 - 1
         sub_two = int(str(variant.positions[1])) % 3 - 1
         # get nucleotides of substitutions
         sub_one_nuc = variant.sequence[0][1]
         sub_two_nuc = variant.sequence[1][1]
         # set other possible indices for codon substitution to None
         sub_three = None
     else:  # variant_codon has two or three adjacent nucleotide substitutions
         # instantiate Variant object
         variant = Variant(hgvs_nt)
+        assert isinstance(variant.sequence, str)
+        assert isinstance(variant.positions, SupportsIndex)
         variant_codon = variant.sequence
         # get index of first codon substitution
         sub_one = int(str(variant.positions[0])) % 3 - 1
         # get string of substituted nucleotides
         sub_nucs = variant.sequence
         if len(sub_nucs) == 2:  # variant codon has two adjacent nucleotide substitutions
             # assign additional nucleotide substitution indices
@@ -254,20 +259,22 @@
             variant_codon = variant_codon + sub_two_nuc
         elif sub_three == -1 or sub_three == 2:
             variant_codon = variant_codon + sub_three_nuc
         else:
             variant_codon = variant_codon + target_codon[2]
 
     # convert to 3 letter amino acid code
+    assert target_codon is not None
     target_aa = codon_dict_DNA[target_codon]
-    if variant_codon:
-        variant_aa = codon_dict_DNA[variant_codon]
-    else:
-        variant_aa = None
+    if not variant_codon:
+        return "p.="
+
+    variant_aa = codon_dict_DNA[variant_codon]
 
+    assert codon_number is not None
     return construct_hgvs_pro(wt=target_aa, mutant=variant_aa, position=codon_number, target_seq=target_seq)
 
 
 def _is_wild_type(hgvs: str):
     # TODO this is no longer valid
     """
     This function takes an hgvs formatted string and returns True if the hgvs string indicates
```

### Comparing `mavedb-2023.3.0/src/mavedb/lib/validation/variant.py` & `mavedb-2024.0.0/src/mavedb/lib/validation/variant.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/lib/validation/constants/conversion.py` & `mavedb-2024.0.0/src/mavedb/lib/validation/constants/conversion.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/lib/validation/constants/general.py` & `mavedb-2024.0.0/src/mavedb/lib/validation/constants/general.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import re
 
 """
 Null Constant definitions
 """
 NA_STRING = "NA"
-null_values_list = (
+null_values_list = [
     "nan",
     "na",
     "none",
     "",
     "undefined",
     "n/a",
     "null",
     "nil",
     "-",
-    None,
-)
+]
 # enforce the assumption that these are all lowercase values
-null_values_list = [s.lower() for s in null_values_list if s is not None]
+assert all(s.lower() == s for s in null_values_list)
+
 # add the NA_STRING only if it's not already in the list
 if NA_STRING.lower() not in null_values_list:
     null_values_list.append(NA_STRING.lower())
 null_values_list.sort()
 
 null_values_re = re.compile(
     r"^\s+$|" + "|".join(f"^{s}$" for s in null_values_list if len(s)),
```

### Comparing `mavedb-2023.3.0/src/mavedb/models/access_key.py` & `mavedb-2024.0.0/src/mavedb/models/access_key.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from datetime import datetime
 
 from sqlalchemy import Column, Date, DateTime, Integer, String, ForeignKey
-from sqlalchemy.orm import backref, relationship
+from sqlalchemy.orm import backref, relationship, Mapped
 
 from mavedb.db.base import Base
+from mavedb.models.user import User
 
 
 class AccessKey(Base):
     __tablename__ = "access_keys"
 
     id = Column(Integer, primary_key=True)
     user_id = Column(Integer, ForeignKey("users.id"), nullable=False)
-    user = relationship("User", backref=backref("access_keys", cascade="all,delete-orphan"))
+    user : Mapped[User] = relationship(back_populates="access_keys")
     key_id = Column(String, unique=True, index=True, nullable=False)
     public_key = Column(String, nullable=False)
     name = Column(String, nullable=True)
     expiration_date = Column(Date, nullable=True)
     creation_time = Column(DateTime, nullable=True, default=datetime.now)
```

### Comparing `mavedb-2023.3.0/src/mavedb/models/doi_identifier.py` & `mavedb-2024.0.0/src/mavedb/models/doi_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/models/ensembl_identifier.py` & `mavedb-2024.0.0/src/mavedb/models/ensembl_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/models/ensembl_offset.py` & `mavedb-2024.0.0/src/mavedb/models/uniprot_offset.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from sqlalchemy import Column, Integer, ForeignKey
-from sqlalchemy.orm import relationship, backref
+from sqlalchemy.orm import relationship, backref, Mapped
 
 from mavedb.db.base import Base
-from mavedb.models.ensembl_identifier import EnsemblIdentifier
+from mavedb.models.uniprot_identifier import UniprotIdentifier
 from mavedb.models.target_gene import TargetGene
 
 
-class EnsemblOffset(Base):
-    __tablename__ = "ensembl_offsets"
+class UniprotOffset(Base):
+    __tablename__ = "uniprot_offsets"
 
-    identifier_id = Column(Integer, ForeignKey("ensembl_identifiers.id"), nullable=False, primary_key=True)
-    identifier = relationship("EnsemblIdentifier", backref=backref("target_gene_offsets", uselist=True))
-    target_gene_id = Column(Integer, ForeignKey("target_genes.id"), nullable=False, primary_key=True)
-    target_gene = relationship(
-        "TargetGene",
-        backref=backref("ensembl_offset", cascade="all,delete-orphan", single_parent=True, uselist=False),
-        single_parent=True,
+    identifier_id = Column(Integer, ForeignKey("uniprot_identifiers.id"), nullable=False, primary_key=True)
+    identifier : Mapped[UniprotIdentifier] = relationship(
+        "UniprotIdentifier",
+        backref=backref("target_gene_offsets", uselist=True)
     )
+    target_gene_id = Column(Integer, ForeignKey("target_genes.id"), nullable=False, primary_key=True)
+    target_gene : Mapped[TargetGene] = relationship(back_populates="uniprot_offset", single_parent=True)
+
     offset = Column(Integer, nullable=False)
```

### Comparing `mavedb-2023.3.0/src/mavedb/models/experiment.py` & `mavedb-2024.0.0/src/mavedb/models/experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 from datetime import date
 
-from typing import Optional
+from typing import Optional, List, TYPE_CHECKING
+
 from sqlalchemy import Boolean, Column, Date, ForeignKey, Integer, String
 from sqlalchemy.event import listens_for
-from sqlalchemy.ext.associationproxy import association_proxy
-from sqlalchemy.orm import relationship, backref
+from sqlalchemy.ext.associationproxy import association_proxy, AssociationProxy
+from sqlalchemy.orm import relationship, Mapped
 from sqlalchemy.schema import Table
+from sqlalchemy.dialects.postgresql import JSONB
 
 from mavedb.db.base import Base
-from mavedb.deps import JSONB
 from mavedb.lib.temp_urns import generate_temp_urn
 from mavedb.models.experiment_set import ExperimentSet
 from mavedb.models.keyword import Keyword
+from mavedb.models.doi_identifier import DoiIdentifier
+from mavedb.models.raw_read_identifier import RawReadIdentifier
 from mavedb.models.experiment_publication_identifier import ExperimentPublicationIdentifierAssociation
+from mavedb.models.user import User
+from mavedb.models.publication_identifier import PublicationIdentifier
+
+if TYPE_CHECKING:
+    from mavedb.models.score_set import ScoreSet
 
 experiments_doi_identifiers_association_table = Table(
     "experiment_doi_identifiers",
     Base.metadata,
     Column("experiment_id", ForeignKey("experiments.id"), primary_key=True),
     Column("doi_identifier_id", ForeignKey("doi_identifiers.id"), primary_key=True),
 )
@@ -40,54 +48,57 @@
 
 
 class Experiment(Base):
     __tablename__ = "experiments"
 
     id = Column(Integer, primary_key=True, index=True)
 
-    urn = Column(String(64), nullable=True, default=generate_temp_urn)  # index=True, nullable=True
+    urn = Column(String(64), nullable=True, default=generate_temp_urn, unique=True, index=True)
     title = Column(String, nullable=False)
     short_description = Column(String, nullable=False)
     abstract_text = Column(String, nullable=False)
     method_text = Column(String, nullable=False)
     extra_metadata = Column(JSONB, nullable=False)
 
     private = Column(Boolean, nullable=False, default=True)
     approved = Column(Boolean, nullable=False, default=False)
     published_date = Column(Date, nullable=True)
     processing_state = Column(String, nullable=True)
 
     # TODO Remove this obsolete column.
     num_score_sets = Column("num_scoresets", Integer, nullable=False, default=0)
+    score_sets: Mapped[List["ScoreSet"]] = relationship(back_populates="experiment", cascade="all, delete-orphan")
 
     experiment_set_id = Column(Integer, ForeignKey("experiment_sets.id"), nullable=True)
-    experiment_set = relationship("ExperimentSet", backref=backref("experiments", cascade="all,delete-orphan"))
+    experiment_set: Mapped[Optional[ExperimentSet]] = relationship(back_populates="experiments")
 
     created_by_id = Column(Integer, ForeignKey("users.id"), nullable=True)
-    created_by = relationship("User", foreign_keys="Experiment.created_by_id")
+    created_by: Mapped[User] = relationship("User", foreign_keys="Experiment.created_by_id")
     modified_by_id = Column(Integer, ForeignKey("users.id"), nullable=True)
-    modified_by = relationship("User", foreign_keys="Experiment.modified_by_id")
+    modified_by: Mapped[User] = relationship("User", foreign_keys="Experiment.modified_by_id")
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
 
-    keyword_objs = relationship("Keyword", secondary=experiments_keywords_association_table, backref="experiments")
-    doi_identifiers = relationship(
+    keyword_objs: Mapped[list[Keyword]] = relationship(
+        "Keyword", secondary=experiments_keywords_association_table, backref="experiments"
+    )
+    doi_identifiers: Mapped[list[DoiIdentifier]] = relationship(
         "DoiIdentifier", secondary=experiments_doi_identifiers_association_table, backref="experiments"
     )
-    publication_identifier_associations = relationship(
+    publication_identifier_associations: Mapped[list[ExperimentPublicationIdentifierAssociation]] = relationship(
         "ExperimentPublicationIdentifierAssociation", back_populates="experiment", cascade="all, delete-orphan"
     )
-    publication_identifiers = association_proxy(
+    publication_identifiers: AssociationProxy[List[PublicationIdentifier]] = association_proxy(
         "publication_identifier_associations",
         "publication",
         creator=lambda p: ExperimentPublicationIdentifierAssociation(publication=p, primary=p.primary),
     )
 
     # sra_identifiers = relationship('SraIdentifier', secondary=experiments_sra_identifiers_association_table, backref='experiments')
-    raw_read_identifiers = relationship(
+    raw_read_identifiers: Mapped[list[RawReadIdentifier]] = relationship(
         "RawReadIdentifier", secondary=experiments_raw_read_identifiers_association_table, backref="experiments"
     )
 
     # Unfortunately, we can't use association_proxy here, because in spite of what the documentation seems to imply, it
     # doesn't check for a pre-existing keyword with the same text.
     # keywords = association_proxy('keyword_objs', 'text', creator=lambda text: Keyword(text=text))
 
@@ -96,15 +107,15 @@
 
     @property
     def keywords(self) -> list[str]:
         # if self._updated_keywords:
         #     return self._updated_keywords
         # else:
         keyword_objs = self.keyword_objs or []  # getattr(self, 'keyword_objs', [])
-        return list(map(lambda keyword_obj: keyword_obj.text, keyword_objs))
+        return [keyword_obj.text for keyword_obj in keyword_objs if keyword_obj.text is not None]
 
     async def set_keywords(self, db, keywords: Optional[list[str]]):
         if keywords is None:
             self.keyword_objs = []
         else:
             self.keyword_objs = [await self._find_or_create_keyword(db, text) for text in keywords]
```

### Comparing `mavedb-2023.3.0/src/mavedb/models/experiment_publication_identifier.py` & `mavedb-2024.0.0/src/mavedb/models/experiment_publication_identifier.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from sqlalchemy import Column, Integer, Boolean, ForeignKey
-from sqlalchemy.orm import relationship
+from sqlalchemy.orm import relationship, Mapped
 
 from mavedb.db.base import Base
 
+# Prevent circular imports
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from mavedb.models.experiment import Experiment
+    from mavedb.models.publication_identifier import PublicationIdentifier
+
 
 class ExperimentPublicationIdentifierAssociation(Base):
     __tablename__ = "experiment_publication_identifiers"
 
     experiment_id = Column(Integer, ForeignKey("experiments.id"), primary_key=True)
     publication_identifier_id = Column(Integer, ForeignKey("publication_identifiers.id"), primary_key=True)
     primary = Column(Boolean, nullable=True, default=False)
 
-    experiment = relationship("Experiment", back_populates="publication_identifier_associations")
-    publication = relationship("PublicationIdentifier")
+    experiment : Mapped["Experiment"] = relationship("Experiment", back_populates="publication_identifier_associations")
+    publication : Mapped["PublicationIdentifier"] = relationship("PublicationIdentifier")
```

### Comparing `mavedb-2023.3.0/src/mavedb/models/experiment_set.py` & `mavedb-2024.0.0/src/mavedb/models/experiment_set.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 from datetime import date
+from typing import List, TYPE_CHECKING
 
 from sqlalchemy import Boolean, Column, Date, ForeignKey, Integer, String
-from sqlalchemy.orm import relationship
+from sqlalchemy.orm import relationship, Mapped
 from sqlalchemy.schema import Table
+from sqlalchemy.dialects.postgresql import JSONB
 
 from mavedb.db.base import Base
-from mavedb.deps import JSONB
 from mavedb.lib.temp_urns import generate_temp_urn
+from .user import User
+from .keyword import Keyword
+from .doi_identifier import DoiIdentifier
+from .publication_identifier import PublicationIdentifier
+from .raw_read_identifier import RawReadIdentifier
+
+if TYPE_CHECKING:
+    from mavedb.models.experiment import Experiment
 
 experiment_sets_doi_identifiers_association_table = Table(
     "experiment_set_doi_identifiers",
     Base.metadata,
     Column("experiment_set_id", ForeignKey("experiment_sets.id"), primary_key=True),
     Column("doi_identifier_id", ForeignKey("doi_identifiers.id"), primary_key=True),
 )
@@ -39,40 +48,43 @@
 
 
 class ExperimentSet(Base):
     __tablename__ = "experiment_sets"
 
     id = Column(Integer, primary_key=True, index=True)
 
-    urn = Column(String(64), nullable=True, default=generate_temp_urn)  # index=True, nullable=True
+    urn = Column(String(64), nullable=True, default=generate_temp_urn, unique=True, index=True)
     extra_metadata = Column(JSONB, nullable=False)
 
     private = Column(Boolean, nullable=False, default=True)
     approved = Column(Boolean, nullable=False, default=False)
     published_date = Column(Date, nullable=True)
     processing_state = Column(String, nullable=True)
 
     # TODO Refactor the way we handle child collections?
     num_experiments = Column(Integer, nullable=False, default=0)
+    experiments: Mapped[List["Experiment"]] = relationship(
+        back_populates="experiment_set", cascade="all, delete-orphan"
+    )
 
     created_by_id = Column(Integer, ForeignKey("users.id"), nullable=True)
-    created_by = relationship("User", foreign_keys="ExperimentSet.created_by_id")
+    created_by: Mapped[User] = relationship("User", foreign_keys="ExperimentSet.created_by_id")
     modified_by_id = Column(Integer, ForeignKey("users.id"), nullable=True)
-    modified_by = relationship("User", foreign_keys="ExperimentSet.modified_by_id")
+    modified_by: Mapped[User] = relationship("User", foreign_keys="ExperimentSet.modified_by_id")
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
 
-    keyword_objs = relationship(
+    keyword_objs: Mapped[list[Keyword]] = relationship(
         "Keyword", secondary=experiment_sets_keywords_association_table, backref="experiment_sets"
     )
-    doi_identifiers = relationship(
+    doi_identifiers: Mapped[list[DoiIdentifier]] = relationship(
         "DoiIdentifier", secondary=experiment_sets_doi_identifiers_association_table, backref="experiment_sets"
     )
-    publication_identifiers = relationship(
+    publication_identifiers: Mapped[list[PublicationIdentifier]] = relationship(
         "PublicationIdentifier",
         secondary=experiment_sets_publication_identifiers_association_table,
         backref="experiment_sets",
     )
     # sra_identifiers = relationship('SraIdentifier', secondary=experiment_sets_sra_identifiers_association_table, backref='experiment_sets')
-    raw_read_identifiers = relationship(
+    raw_read_identifiers: Mapped[list[RawReadIdentifier]] = relationship(
         "RawReadIdentifier", secondary=experiment_sets_raw_read_identifiers_association_table, backref="experiment_sets"
     )
```

### Comparing `mavedb-2023.3.0/src/mavedb/models/genome_identifier.py` & `mavedb-2024.0.0/src/mavedb/models/genome_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/models/license.py` & `mavedb-2024.0.0/src/mavedb/models/license.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/models/publication_identifier.py` & `mavedb-2024.0.0/src/mavedb/models/publication_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/models/raw_read_identifier.py` & `mavedb-2024.0.0/src/mavedb/models/raw_read_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/models/reference_map.py` & `mavedb-2024.0.0/src/mavedb/models/ensembl_offset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from datetime import date
-
-from sqlalchemy import Boolean, Column, Date, ForeignKey, Integer
-from sqlalchemy.orm import relationship, backref
+from sqlalchemy import Column, Integer, ForeignKey
+from sqlalchemy.orm import relationship, backref, Mapped
 
 from mavedb.db.base import Base
+from mavedb.models.ensembl_identifier import EnsemblIdentifier
+from mavedb.models.target_gene import TargetGene
 
 
-class ReferenceMap(Base):
-    __tablename__ = "reference_maps"
+class EnsemblOffset(Base):
+    __tablename__ = "ensembl_offsets"
 
-    id = Column(Integer, primary_key=True, index=True)
-    is_primary = Column(Boolean, nullable=False, default=False)
-    genome_id = Column(Integer, ForeignKey("reference_genomes.id"), nullable=False)
-    genome = relationship("ReferenceGenome", backref="reference_maps")
-    target_id = Column(Integer, ForeignKey("target_genes.id"), nullable=False)
-    target = relationship("TargetGene", backref=backref("reference_maps", cascade="all,delete-orphan"))
-    creation_date = Column(Date, nullable=False, default=date.today)
-    modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
+    identifier_id = Column(Integer, ForeignKey("ensembl_identifiers.id"), nullable=False, primary_key=True)
+    identifier : Mapped[EnsemblIdentifier] = relationship("EnsemblIdentifier", backref=backref("target_gene_offsets", uselist=True))
+    target_gene_id = Column(Integer, ForeignKey("target_genes.id"), nullable=False, primary_key=True)
+    target_gene : Mapped[TargetGene] = relationship(back_populates="ensembl_offset")
+   
+    offset = Column(Integer, nullable=False)
```

### Comparing `mavedb-2023.3.0/src/mavedb/models/refseq_identifier.py` & `mavedb-2024.0.0/src/mavedb/models/refseq_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/models/score_set.py` & `mavedb-2024.0.0/src/mavedb/models/score_set.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 from datetime import date
 from sqlalchemy import Boolean, Column, Date, Enum, ForeignKey, Integer, String
-from sqlalchemy.orm import relationship, backref
-from sqlalchemy.ext.associationproxy import association_proxy
+from sqlalchemy.orm import relationship, backref, Mapped
+from sqlalchemy.ext.associationproxy import association_proxy, AssociationProxy
 from sqlalchemy.schema import Table
+from sqlalchemy.dialects.postgresql import JSONB
+
+from typing import List, TYPE_CHECKING, Optional
 
 from mavedb.db.base import Base
-from mavedb.deps import JSONB
 from mavedb.models.enums.processing_state import ProcessingState
-from mavedb.models.score_set_publication_identifier import ScoreSetPublicationIdentifierAssociation
-from .keyword import Keyword
+import mavedb.models.score_set_publication_identifier
+
+from mavedb.models.experiment import Experiment
+from mavedb.models.user import User
+from mavedb.models.license import License
+from mavedb.models.keyword import Keyword
+from mavedb.models.doi_identifier import DoiIdentifier
+from mavedb.models.publication_identifier import PublicationIdentifier
+
+if TYPE_CHECKING:
+    from mavedb.models.variant import Variant
+    from mavedb.models.target_gene import TargetGene
 
 # from .raw_read_identifier import SraIdentifier
 from mavedb.lib.temp_urns import generate_temp_urn
 
 # TODO Reformat code without removing dependencies whose use is not detected.
 
 score_sets_doi_identifiers_association_table = Table(
@@ -49,15 +61,15 @@
 
 
 class ScoreSet(Base):
     __tablename__ = "scoresets"
 
     id = Column(Integer, primary_key=True, index=True)
 
-    urn = Column(String(64), nullable=True, default=generate_temp_urn)  # index=True, nullable=True
+    urn = Column(String(64), nullable=True, default=generate_temp_urn, unique=True, index=True)
     title = Column(String, nullable=False)
     method_text = Column(String, nullable=False)
     abstract_text = Column(String, nullable=False)
     short_description = Column(String, nullable=False)
     extra_metadata = Column(JSONB, nullable=False)
     dataset_columns = Column(JSONB, nullable=False, default={})
 
@@ -65,72 +77,83 @@
     private = Column(Boolean, nullable=False, default=True)
     approved = Column(Boolean, nullable=False, default=False)
     published_date = Column(Date, nullable=True)
     processing_state = Column(
         Enum(ProcessingState, create_constraint=True, length=32, native_enum=False, validate_strings=True),
         nullable=True,
     )
+    processing_errors = Column(JSONB, nullable=True)
     data_usage_policy = Column(String, nullable=True)
 
     # TODO Refactor the way we track the number of variants?
     num_variants = Column(Integer, nullable=False, default=0)
+    variants: Mapped[list["Variant"]] = relationship(back_populates="score_set", cascade="all, delete-orphan")
 
     experiment_id = Column(Integer, ForeignKey("experiments.id"), nullable=False)
-    experiment = relationship("Experiment", backref=backref("score_sets", cascade="all,delete-orphan"))
+    experiment: Mapped["Experiment"] = relationship(back_populates="score_sets")
+
     # TODO Standardize on US or GB spelling for licenc/se.
     licence_id = Column(Integer, ForeignKey("licenses.id"), nullable=False)
-    license = relationship("License")
+    license: Mapped["License"] = relationship("License")
     superseded_score_set_id = Column("replaces_id", Integer, ForeignKey("scoresets.id"), nullable=True)  # TODO
-    superseded_score_set = relationship(
+    superseded_score_set: Mapped[Optional["ScoreSet"]] = relationship(
         "ScoreSet", uselist=False, remote_side=[id], backref=backref("superseding_score_set", uselist=False)
     )
 
     created_by_id = Column(Integer, ForeignKey("users.id"), nullable=True)
-    created_by = relationship("User", foreign_keys="ScoreSet.created_by_id")
+    created_by: Mapped["User"] = relationship("User", foreign_keys="ScoreSet.created_by_id")
     modified_by_id = Column(Integer, ForeignKey("users.id"), nullable=True)
-    modified_by = relationship("User", foreign_keys="ScoreSet.modified_by_id")
+    modified_by: Mapped["User"] = relationship("User", foreign_keys="ScoreSet.modified_by_id")
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
 
-    keyword_objs = relationship("Keyword", secondary=score_sets_keywords_association_table, backref="score_sets")
-    doi_identifiers = relationship(
+    keyword_objs: Mapped[list["Keyword"]] = relationship(
+        "Keyword", secondary=score_sets_keywords_association_table, backref="score_sets"
+    )
+    doi_identifiers: Mapped[list["DoiIdentifier"]] = relationship(
         "DoiIdentifier", secondary=score_sets_doi_identifiers_association_table, backref="score_sets"
     )
-    publication_identifier_associations = relationship(
+    publication_identifier_associations: Mapped[
+        list[mavedb.models.score_set_publication_identifier.ScoreSetPublicationIdentifierAssociation]
+    ] = relationship(
         "ScoreSetPublicationIdentifierAssociation", back_populates="score_set", cascade="all, delete-orphan"
     )
-    publication_identifiers = association_proxy(
+    publication_identifiers: AssociationProxy[List[PublicationIdentifier]] = association_proxy(
         "publication_identifier_associations",
         "publication",
-        creator=lambda p: ScoreSetPublicationIdentifierAssociation(publication=p, primary=p.primary),
+        creator=lambda p: mavedb.models.score_set_publication_identifier.ScoreSetPublicationIdentifierAssociation(
+            publication=p, primary=p.primary
+        ),
     )
     # sra_identifiers = relationship('SraIdentifier', secondary=score_sets_sra_identifiers_association_table, backref='score_sets')
     # raw_read_identifiers = relationship('RawReadIdentifier', secondary=score_sets_raw_read_identifiers_association_table,backref='score_sets')
-    meta_analyzes_score_sets = relationship(
+    meta_analyzes_score_sets: Mapped[list["ScoreSet"]] = relationship(
         "ScoreSet",
         secondary=score_sets_meta_analysis_score_sets_association_table,
         primaryjoin=(score_sets_meta_analysis_score_sets_association_table.c.meta_analysis_scoreset_id == id),
         secondaryjoin=(score_sets_meta_analysis_score_sets_association_table.c.source_scoreset_id == id),
         backref="meta_analyzed_by_score_sets",
     )
 
+    target_genes: Mapped[List["TargetGene"]] = relationship(back_populates="score_set", cascade="all, delete-orphan")
+
     # Unfortunately, we can't use association_proxy here, because in spite of what the documentation seems to imply, it
     # doesn't check for a pre-existing keyword with the same text.
     # keywords = association_proxy('keyword_objs', 'text', creator=lambda text: Keyword(text=text))
 
     # _updated_keywords: list[str] = None
     # _updated_doi_identifiers: list[str] = None
 
     @property
     def keywords(self) -> list[str]:
         # if self._updated_keywords:
         #     return self._updated_keywords
         # else:
         keyword_objs = self.keyword_objs or []  # getattr(self, 'keyword_objs', [])
-        return list(map(lambda keyword_obj: keyword_obj.text, keyword_objs))
+        return [keyword_obj.text for keyword_obj in keyword_objs if keyword_obj.text is not None]
 
     async def set_keywords(self, db, keywords: list[str]):
         if keywords is None:
             self.keyword_objs = []
         else:
             self.keyword_objs = [await self._find_or_create_keyword(db, text) for text in keywords]
```

### Comparing `mavedb-2023.3.0/src/mavedb/models/target_gene.py` & `mavedb-2024.0.0/src/mavedb/models/target_gene.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 from datetime import date
 from sqlalchemy import Column, Date, ForeignKey, Integer, String
-from sqlalchemy.orm import backref, relationship
+from sqlalchemy.orm import backref, relationship, Mapped
+
+from typing import TYPE_CHECKING
 
 from mavedb.db.base import Base
-from .ensembl_identifier import EnsemblIdentifier
-from .reference_map import ReferenceMap
-from .refseq_identifier import RefseqIdentifier
-from .uniprot_identifier import UniprotIdentifier
-from .wild_type_sequence import WildTypeSequence
+from mavedb.models.target_sequence import TargetSequence
+from mavedb.models.target_accession import TargetAccession
+from mavedb.models.score_set import ScoreSet
+
+if TYPE_CHECKING:
+    from mavedb.models.ensembl_offset import EnsemblOffset
+    from mavedb.models.refseq_offset import RefseqOffset
+    from mavedb.models.uniprot_offset import UniprotOffset
 
 # TODO Reformat code without removing dependencies whose use is not detected.
 
 
 class TargetGene(Base):
     __tablename__ = "target_genes"
 
     id = Column(Integer, primary_key=True, index=True)
 
     name = Column(String, nullable=False)
     category = Column(String, nullable=False)
 
-    # ensembl_id_id = Column(Integer, ForeignKey('metadata_ensemblidentifier.id'), nullable=True)
-    # ensembl_id_id = Column(Integer, ForeignKey('ensembl_identifiers.id'), nullable=True)
-    # ensembl_id = relationship('EnsemblIdentifier', backref='target_genes')
-    # refseq_id_id = Column(Integer, nullable=True)  # , ForeignKey('dataset_scoreset.id'), nullable=False)
     score_set_id = Column("scoreset_id", Integer, ForeignKey("scoresets.id"), nullable=False)
-    score_set = relationship(
-        "ScoreSet",
-        backref=backref("target_gene", cascade="all,delete-orphan", single_parent=True, uselist=False),
-        single_parent=True,
+    score_set : Mapped[ScoreSet] = relationship(
+        back_populates="target_genes", single_parent=True, uselist=True
     )
-    # uniprot_id_id = Column(Integer, nullable=True)  # , ForeignKey('dataset_scoreset.id'), nullable=False)
-    wt_sequence_id = Column(Integer, ForeignKey("wild_type_sequences.id"), nullable=False)
-    wt_sequence = relationship(
-        "WildTypeSequence",
-        backref=backref("target_gene", single_parent=True, uselist=False),
+
+    target_sequence_id = Column(Integer, ForeignKey("target_sequences.id"), nullable=True)
+    accession_id = Column(Integer, ForeignKey("target_accessions.id"), nullable=True)
+    target_sequence : Mapped[TargetSequence] = relationship(
+        back_populates="target_genes", cascade="all,delete-orphan", single_parent=True
+    )
+    target_accession : Mapped[TargetAccession] = relationship(
+        "TargetAccession",
+        backref=backref("target_genes", single_parent=True, uselist=True),
         cascade="all,delete-orphan",
         single_parent=True,
     )
 
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
+
+    ensembl_offset : Mapped["EnsemblOffset"] = relationship(back_populates="target_gene", cascade="all, delete-orphan")
+    refseq_offset : Mapped["RefseqOffset"] = relationship(back_populates="target_gene", cascade="all, delete-orphan")
+    uniprot_offset : Mapped["UniprotOffset"] = relationship(back_populates="target_gene", cascade="all, delete-orphan")
```

### Comparing `mavedb-2023.3.0/src/mavedb/models/uniprot_identifier.py` & `mavedb-2024.0.0/src/mavedb/models/uniprot_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/models/user.py` & `mavedb-2024.0.0/src/mavedb/models/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 from sqlalchemy import Boolean, Column, DateTime, ForeignKey, Integer, String, Table
-from sqlalchemy.orm import relationship
-
+from sqlalchemy.orm import relationship, Mapped
+from typing import List, TYPE_CHECKING
 from mavedb.db.base import Base
 from mavedb.models.role import Role
 
 users_roles_association_table = Table(
     "users_roles",
     Base.metadata,
     Column("user_id", ForeignKey("users.id"), primary_key=True),
     Column("role_id", ForeignKey("roles.id"), primary_key=True),
 )
 
+if TYPE_CHECKING:
+    from mavedb.models.access_key import AccessKey
+
 
 class User(Base):
     __tablename__ = "users"
 
     id = Column(Integer, primary_key=True)
     username = Column(String, index=True, nullable=False)
     first_name = Column(String, nullable=True)
     last_name = Column(String, nullable=True)
     email = Column(String, nullable=True)
     is_superuser = Column(Boolean, nullable=False, default=False)
     is_staff = Column(Boolean, nullable=False, default=False)
     is_active = Column(Boolean, nullable=False)
     date_joined = Column(DateTime, nullable=True)
     email = Column(String, nullable=True)
-    role_objs = relationship("Role", secondary=users_roles_association_table, backref="users")
+    role_objs : Mapped[List[Role]] = relationship("Role", secondary=users_roles_association_table, backref="users")
     last_login = Column(DateTime, nullable=True)
 
+    access_keys : Mapped[List["AccessKey"]] = relationship(back_populates="user", cascade="all, delete-orphan")
+
     @property
     def roles(self) -> list[str]:
         role_objs = self.role_objs or []
-        return list(map(lambda role_obj: role_obj.name, role_objs))
+        return [role_obj.name for role_obj in role_objs if role_obj.name is not None]
 
     async def set_roles(self, db, roles: list[str]):
         self.role_objs = [await self._find_or_create_role(db, name) for name in roles]
 
     @staticmethod
     async def _find_or_create_role(db, role_name):
         role_obj = db.query(Role).filter(Role.name == role_name).one_or_none()
```

### Comparing `mavedb-2023.3.0/src/mavedb/models/variant.py` & `mavedb-2024.0.0/src/mavedb/models/variant.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from datetime import date
 
 from sqlalchemy import Column, Date, ForeignKey, Integer, String
-from sqlalchemy.orm import relationship, backref
+from sqlalchemy.orm import relationship, backref, Mapped
+from sqlalchemy.dialects.postgresql import JSONB
 
 from mavedb.db.base import Base
-from mavedb.deps import JSONB
+from .score_set import ScoreSet
 
 
 class Variant(Base):
     __tablename__ = "variants"
 
     id = Column(Integer, primary_key=True, index=True)
 
-    urn = Column(String(64), nullable=True)  # index=True, nullable=True
+    urn = Column(String(64), nullable=True, unique=True, index=True)
     data = Column(JSONB, nullable=False)
 
     score_set_id = Column("scoreset_id", Integer, ForeignKey("scoresets.id"), nullable=False)
     # TODO examine if delete-orphan is necessary, explore cascade
-    score_set = relationship("ScoreSet", backref=backref("variants", cascade="all,delete-orphan"))
+    score_set: Mapped[ScoreSet] = relationship(back_populates="variants")
 
     hgvs_nt = Column(String, nullable=True)
     hgvs_pro = Column(String, nullable=True)
     hgvs_splice = Column(String, nullable=True)
 
     creation_date = Column(Date, nullable=False, default=date.today)
     modification_date = Column(Date, nullable=False, default=date.today, onupdate=date.today)
```

### Comparing `mavedb-2023.3.0/src/mavedb/models/legacy/django_reversion_version.py` & `mavedb-2024.0.0/src/mavedb/models/legacy/django_reversion_version.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/routers/access_keys.py` & `mavedb-2024.0.0/src/mavedb/routers/access_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,10 +64,10 @@
 def delete_my_access_key(
     *, key_id: str, db: Session = Depends(deps.get_db), user: User = Depends(require_current_user)
 ) -> Any:
     """
     Delete one of the current user's access keys.
     """
     item = db.query(AccessKey).filter(AccessKey.key_id == key_id).one_or_none()
-    if item.user.id == user.id:
+    if item and item.user.id == user.id:
         db.delete(item)
     db.commit()
```

### Comparing `mavedb-2023.3.0/src/mavedb/routers/api_information.py` & `mavedb-2024.0.0/src/mavedb/routers/api_information.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/routers/doi_identifiers.py` & `mavedb-2024.0.0/src/mavedb/routers/doi_identifiers.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/routers/experiment_sets.py` & `mavedb-2024.0.0/src/mavedb/routers/experiment_sets.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/routers/experiments.py` & `mavedb-2024.0.0/src/mavedb/routers/experiments.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import logging
 from operator import attrgetter
 from typing import Any, Optional
 
-from fastapi import APIRouter, Depends, HTTPException, status
+from fastapi import APIRouter, Depends, HTTPException
 from fastapi.encoders import jsonable_encoder
+from sqlalchemy import or_, and_
 from sqlalchemy.orm import Session
 
 from mavedb import deps
 from mavedb.lib.authentication import get_current_user
 from mavedb.lib.authorization import require_current_user
 from mavedb.lib.experiments import search_experiments as _search_experiments
 from mavedb.lib.identifiers import (
     find_or_create_doi_identifier,
     find_or_create_publication_identifier,
     find_or_create_raw_read_identifier,
 )
-from mavedb.lib.permissions import has_permission, Action
+from mavedb.lib.permissions import assert_permission, Action
 from mavedb.models.experiment import Experiment
 from mavedb.models.experiment_set import ExperimentSet
 from mavedb.models.score_set import ScoreSet
 from mavedb.models.user import User
 from mavedb.view_models import experiment, score_set
 from mavedb.view_models.search import ExperimentsSearch
 
+import requests
+
 logger = logging.getLogger(__name__)
 
 router = APIRouter(prefix="/api/v1", tags=["experiments"], responses={404: {"description": "Not found"}})
 
 
 @router.get(
     "/experiments/", status_code=200, response_model=list[experiment.Experiment], response_model_exclude_none=True
@@ -87,17 +90,15 @@
     """
     Fetch a single experiment by URN.
     """
     # item = db.query(Experiment).filter(Experiment.urn == urn).filter(Experiment.private.is_(False)).first()
     item = db.query(Experiment).filter(Experiment.urn == urn).first()
     if not item:
         raise HTTPException(status_code=404, detail=f"Experiment with URN {urn} not found")
-    permission = has_permission(user, item, Action.READ)
-    if not permission.permitted:
-        raise HTTPException(status_code=permission.http_code, detail=permission.message)
+    assert_permission(user, item, Action.READ)
     return item
 
 
 @router.get(
     "/experiments/{urn}/score-sets",
     status_code=200,
     response_model=list[score_set.ScoreSet],
@@ -112,20 +113,23 @@
 ) -> Any:
     """
     Get all score sets belonging to an experiment.
     """
     experiment = db.query(Experiment).filter(Experiment.urn == urn).first()
     if not experiment:
         raise HTTPException(status_code=404, detail=f"experiment with URN '{urn}' not found")
-    permission = has_permission(user, experiment, Action.READ)
-    if not permission.permitted:
-        raise HTTPException(status_code=permission.http_code, detail=permission.message)
-    # Only get published score sets. Unpublished score sets won't be shown on experiment page.
-    # score_sets = db.query(ScoreSet).filter(ScoreSet.experiment_id == experiment.id).filter(not ScoreSet.private).all()
-    score_sets = db.query(ScoreSet).filter(ScoreSet.experiment_id == experiment.id).filter(ScoreSet.private.is_(False)).all()
+    assert_permission(user, experiment, Action.READ)
+    # If there is a current user with score sets associated with this experiment, return all of them. Otherwise, only show
+    # the public / published score sets.
+    score_sets = (
+        db.query(ScoreSet)
+        .filter(ScoreSet.experiment_id == experiment.id)
+        .filter(or_(ScoreSet.private.is_(False), and_(ScoreSet.private.is_(True), ScoreSet.created_by == user)))
+        .all()
+    )
     if not score_sets:
         raise HTTPException(status_code=404, detail="no associated score sets")
     else:
         score_sets.sort(key=attrgetter("urn"))
     return score_sets
 
 
@@ -148,34 +152,37 @@
         experiment_set = (
             db.query(ExperimentSet).filter(ExperimentSet.urn == item_create.experiment_set_urn).one_or_none()
         )
         if not experiment_set:
             raise HTTPException(
                 status_code=404, detail=f"experiment set with URN '{item_create.experiment_set_urn}' not found."
             )
-        permission = has_permission(user, experiment_set, Action.ADD_EXPERIMENT)
-        if not permission.permitted:
-            raise HTTPException(status_code=permission.http_code, detail=permission.message)
-    doi_identifiers = [
-        await find_or_create_doi_identifier(db, identifier.identifier)
-        for identifier in item_create.doi_identifiers or []
-    ]
-    raw_read_identifiers = [
-        await find_or_create_raw_read_identifier(db, identifier.identifier)
-        for identifier in item_create.raw_read_identifiers or []
-    ]
+        assert_permission(user, experiment_set, Action.ADD_EXPERIMENT)
+    try:
+        doi_identifiers = [
+            await find_or_create_doi_identifier(db, identifier.identifier)
+            for identifier in item_create.doi_identifiers or []
+        ]
+        raw_read_identifiers = [
+            await find_or_create_raw_read_identifier(db, identifier.identifier)
+            for identifier in item_create.raw_read_identifiers or []
+        ]
+        primary_publication_identifiers = [
+            await find_or_create_publication_identifier(db, identifier.identifier, identifier.db_name)
+            for identifier in item_create.primary_publication_identifiers or []
+        ]
+        publication_identifiers = [
+            await find_or_create_publication_identifier(db, identifier.identifier, identifier.db_name)
+            for identifier in item_create.secondary_publication_identifiers or []
+        ] + primary_publication_identifiers
+    except requests.exceptions.ConnectTimeout:
+        raise HTTPException(status_code=504, detail="Gateway Timeout")
+    except requests.exceptions.HTTPError:
+        raise HTTPException(status_code=502, detail="Bad Gateway")
 
-    primary_publication_identifiers = [
-        await find_or_create_publication_identifier(db, identifier.identifier, identifier.db_name)
-        for identifier in item_create.primary_publication_identifiers or []
-    ]
-    publication_identifiers = [
-        await find_or_create_publication_identifier(db, identifier.identifier, identifier.db_name)
-        for identifier in item_create.secondary_publication_identifiers or []
-    ] + primary_publication_identifiers
     # create a temporary `primary` attribute on each of our publications that indicates
     # to our association proxy whether it is a primary publication or not
     primary_identifiers = [pub.identifier for pub in primary_publication_identifiers]
     for publication in publication_identifiers:
         setattr(publication, "primary", publication.identifier in primary_identifiers)
 
     item = Experiment(
@@ -193,15 +200,15 @@
         ),
         experiment_set=experiment_set,
         doi_identifiers=doi_identifiers,
         publication_identifiers=publication_identifiers,  # an internal association proxy representation
         raw_read_identifiers=raw_read_identifiers,
         created_by=user,
         modified_by=user,
-    )
+    )  # type: ignore
     await item.set_keywords(db, item_create.keywords)
     db.add(item)
     db.commit()
     db.refresh(item)
     return item
 
 
@@ -220,17 +227,15 @@
     """
     if item_update is None:
         return None
     # item = db.query(Experiment).filter(Experiment.urn == urn).filter(Experiment.private.is_(False)).one_or_none()
     item = db.query(Experiment).filter(Experiment.urn == urn).one_or_none()
     if item is None:
         raise HTTPException(status_code=404, detail=f"experiment with URN {urn} not found")
-    permission = has_permission(user, item, Action.UPDATE)
-    if not permission.permitted:
-        raise HTTPException(status_code=permission.http_code, detail=permission.message)
+    assert_permission(user, item, Action.UPDATE)
 
     pairs = {
         k: v
         for k, v in vars(item_update).items()
         if k
         not in [
             "doi_identifiers",
@@ -297,13 +302,11 @@
     or
     communitcate to client whether the operation succeeded
     204 if successful but not returning content - likely going with this
     """
     item = db.query(Experiment).filter(Experiment.urn == urn).one_or_none()
     if not item:
         raise HTTPException(status_code=404, detail=f"experiment with URN '{urn}' not found.")
-    permission = has_permission(user, item, Action.DELETE)
-    if not permission.permitted:
-        raise HTTPException(status_code=permission.http_code, detail=permission.message)
+    assert_permission(user, item, Action.DELETE)
 
     db.delete(item)
     db.commit()
```

### Comparing `mavedb-2023.3.0/src/mavedb/routers/licenses.py` & `mavedb-2024.0.0/src/mavedb/routers/licenses.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/routers/mapped_variant.py` & `mavedb-2024.0.0/src/mavedb/routers/mapped_variant.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/routers/publication_identifiers.py` & `mavedb-2024.0.0/src/mavedb/routers/publication_identifiers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,144 +1,36 @@
 from typing import Any, List, Optional
 
 from fastapi import APIRouter, Depends, HTTPException
 from sqlalchemy import func
 from sqlalchemy.exc import MultipleResultsFound
 from sqlalchemy.orm import Session
-from sqlalchemy.exc import MultipleResultsFound
 
 from mavedb import deps
 from mavedb.lib.authentication import get_current_user
 from mavedb.lib.identifiers import find_generic_article
 from mavedb.models.publication_identifier import PublicationIdentifier
 from mavedb.models.user import User
 from mavedb.view_models import publication_identifier
-from mavedb.view_models import author
 from mavedb.view_models.search import TextSearch
 
 router = APIRouter(
     prefix="/api/v1/publication-identifiers",
     tags=["publication identifiers"],
     responses={404: {"description": "Not found"}},
 )
 
 
 @router.get("/", status_code=200, response_model=list[publication_identifier.PublicationIdentifier])
-def list_publications(*, db: Session = Depends(deps.get_db)) -> Any:
-    """
-    List stored publications
-    """
-    items = db.query(PublicationIdentifier).all()
-    return items
-
-
-@router.get(
-    "/{db_name}/{identifier}",
-    status_code=200,
-    response_model=publication_identifier.PublicationIdentifier,
-    responses={404: {}},
-)
-def fetch_experiment(*, db_name: str, identifier: str, db: Session = Depends(deps.get_db)) -> PublicationIdentifier:
-    """
-    Fetch a single publication by db name and identifier.
-    """
-    item = (
-        db.query(PublicationIdentifier)
-        .filter(PublicationIdentifier.identifier == identifier and PublicationIdentifier.db_name == db_name)
-        .first()
-    )
-    if not item:
-        raise HTTPException(
-            status_code=404, detail=f"Publication with identifier {identifier} in database {db_name} not found"
-        )
-    return item
-
-
-@router.get("/journals", status_code=200, response_model=list[str], responses={404: {}})
-def list_publication_journal_names(
-    *,
-    db: Session = Depends(deps.get_db),
-) -> Any:
-    """
-    List distinct journal names, in alphabetical order.
-    """
-
-    items = db.query(PublicationIdentifier).all()
-    journals = map(lambda item: item.publication_journal, items)
-    return sorted(list(set(journals)))
-
-
-@router.get("/databases", status_code=200, response_model=list[str], responses={404: {}})
-def list_publication_database_names(
+def list_publications(
     *,
     db: Session = Depends(deps.get_db),
+    user: User = Depends(get_current_user),
 ) -> Any:
     """
-    List distinct database names, in alphabetical order.
-    """
-
-    items = db.query(PublicationIdentifier).all()
-    databases = map(lambda item: item.db_name, items)
-    return sorted(list(set(databases)))
-
-
-@router.get(
-    "/publications/{identifier}",
-    status_code=200,
-    response_model=publication_identifier.PublicationIdentifier,
-    responses={404: {}, 500: {}},
-)
-async def search_publications_by_identifier(*, identifier: str, db: Session = Depends(deps.get_db)) -> Any:
-    """
-    Fetch a single scoreset by URN.
-    """
-    try:
-        item = db.query(PublicationIdentifier).filter(PublicationIdentifier.identifier == identifier).one_or_none()
-    except MultipleResultsFound:
-        raise HTTPException(status_code=500, detail=f"Multiple publications with identifier {identifier} were found.")
-
-    if not item:
-        raise HTTPException(status_code=404, detail=f"Publication with identifier {identifier} not found")
-    return item
-
-
-@router.get(
-    "/publications/{db_name}/{identifier}",
-    status_code=200,
-    response_model=publication_identifier.PublicationIdentifier,
-    responses={404: {}, 500: {}},
-)
-async def search_publications_by_identifier_and_db(
-    *, identifier: str, db_name: str, db: Session = Depends(deps.get_db)
-) -> Any:
-    """
-    Fetch a single scoreset by URN.
-    """
-    try:
-        item = (
-            db.query(PublicationIdentifier)
-            .filter(PublicationIdentifier.identifier == identifier and PublicationIdentifier.db_name == db_name)
-            .one_or_none()
-        )
-    except MultipleResultsFound:
-        raise HTTPException(
-            status_code=500,
-            detail=f"Multiple publications with identifier {identifier} and db_name {db_name} were found.",
-        )
-
-    if not item:
-        raise HTTPException(
-            status_code=404, detail=f"Publication with identifier {identifier} and db_name {db_name} not found"
-        )
-    return item
-
-
-@router.post("/search", status_code=200, response_model=list[publication_identifier.PublicationIdentifier])
-def search_publication_identifiers(search: TextSearch, db: Session = Depends(deps.get_db)) -> Any:
-    """
     List stored all stored publications.
     """
     items = db.query(PublicationIdentifier).all()
     return items
 
 
 @router.get(
```

### Comparing `mavedb-2023.3.0/src/mavedb/routers/raw_read_identifiers.py` & `mavedb-2024.0.0/src/mavedb/routers/raw_read_identifiers.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/routers/score_sets.py` & `mavedb-2024.0.0/src/mavedb/routers/score_sets.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,50 +3,52 @@
 import logging
 import re
 from datetime import date
 from typing import Any, List, Optional
 
 import numpy as np
 import pandas as pd
-from fastapi import APIRouter, Depends, File, status, UploadFile
+from arq import ArqRedis
+from cdot.hgvs.dataproviders import RESTDataProvider
+from fastapi import APIRouter, Depends, File, status, UploadFile, Query
 from fastapi.encoders import jsonable_encoder
 from fastapi.exceptions import HTTPException
 from fastapi.responses import StreamingResponse
 from sqlalchemy import or_
 from sqlalchemy.orm import Session
 from sqlalchemy.exc import MultipleResultsFound
 
 from mavedb import deps
 from mavedb.lib.authorization import get_current_user, require_current_user
 from mavedb.lib.identifiers import (
     create_external_gene_identifier_offset,
     find_or_create_doi_identifier,
     find_or_create_publication_identifier,
 )
-from mavedb.lib.permissions import Action, has_permission
+from mavedb.lib.permissions import Action, assert_permission
 from mavedb.lib.score_sets import (
-    create_variants_data,
     find_meta_analyses_for_experiment_sets,
     search_score_sets as _search_score_sets,
-    VariantData,
+    HGVSColumns,
+    csv_data_to_df,
 )
+from mavedb.lib.taxonomies import find_or_create_taxonomy
 from mavedb.lib.urns import generate_experiment_set_urn, generate_experiment_urn, generate_score_set_urn
-from mavedb.lib.validation import exceptions
-from mavedb.lib.validation.constants.general import null_values_list
-from mavedb.lib.validation.dataframe import validate_and_standardize_dataframe_pair
+from mavedb.lib.exceptions import MixedTargetError
 from mavedb.models.enums.processing_state import ProcessingState
 from mavedb.models.experiment import Experiment
 from mavedb.models.license import License
 from mavedb.models.mapped_variant import MappedVariant
-from mavedb.models.reference_map import ReferenceMap
 from mavedb.models.score_set import ScoreSet
 from mavedb.models.target_gene import TargetGene
+from mavedb.models.target_accession import TargetAccession
+from mavedb.models.taxonomy import Taxonomy
 from mavedb.models.user import User
 from mavedb.models.variant import Variant
-from mavedb.models.wild_type_sequence import WildTypeSequence
+from mavedb.models.target_sequence import TargetSequence
 from mavedb.view_models import mapped_variant
 from mavedb.view_models import score_set
 from mavedb.view_models.search import ScoreSetsSearch
 
 logger = logging.getLogger(__name__)
 
 null_values_re = re.compile(r"\s+|none|nan|na|undefined|n/a|null|nil", flags=re.IGNORECASE)
@@ -60,20 +62,21 @@
     :param urn: The score set URN.
     :param owner: A user whose private score sets may be included in the search. If None, then the score set will only
         be returned if it is public.
     :return: The score set, or None if the URL was not found or refers to a private score set not owned by the specified
         user.
     """
     try:
-        permission_filter = ScoreSet.private.is_(False)
         if owner is not None:
             permission_filter = or_(
-                permission_filter,
+                ScoreSet.private.is_(False),
                 ScoreSet.created_by_id == owner.id,
             )
+        else:
+            permission_filter = ScoreSet.private.is_(False)
         item = db.query(ScoreSet).filter(ScoreSet.urn == urn).filter(permission_filter).one_or_none()
     except MultipleResultsFound:
         raise HTTPException(status_code=500, detail=f"multiple score sets with URN '{urn}' were found")
     if not item:
         raise HTTPException(status_code=404, detail=f"score set with URN '{urn}' not found")
     return item
 
@@ -134,30 +137,49 @@
             """ and hgvs_splice), plus score columns defined by the score set.""",
         }
     },
 )
 def get_score_set_scores_csv(
     *,
     urn: str,
+    start: int = Query(default=None, description="Start index for pagination"),
+    limit: int = Query(default=None, description="Number of variants to return"),
     db: Session = Depends(deps.get_db),
     user: User = Depends(get_current_user),
 ) -> Any:
     """
     Return scores from a score set, identified by URN, in CSV format.
-    """
+    If no start and limit, all of variants of this score set will be returned.
+    Example path:
+    /score-sets/{urn}/scores
+    /score-sets/{urn}/scores?start=0&limit=100
+    /score-sets/{urn}/scores?start=100
+    """
+    if start and start < 0:
+        raise HTTPException(status_code=400, detail="Start index must be non-negative")
+    if limit != None and limit <= 0:
+        raise HTTPException(status_code=400, detail="Limit must be positive")
+
     score_set = db.query(ScoreSet).filter(ScoreSet.urn == urn).first()
     if not score_set:
         raise HTTPException(status_code=404, detail=f"score set with URN '{urn}' not found")
-    permission = has_permission(user, score_set, Action.READ)
-    if not permission.permitted:
-        raise HTTPException(status_code=permission.http_code, detail=permission.message)
+    assert_permission(user, score_set, Action.READ)
 
-    columns = ["accession", "hgvs_nt", "hgvs_splice", "hgvs_pro"] + score_set.dataset_columns["score_columns"]
+    assert type(score_set.dataset_columns) is dict
+    score_columns = [str(x) for x in list(score_set.dataset_columns.get("score_columns", []))]
+    columns = ["accession", "hgvs_nt", "hgvs_splice", "hgvs_pro"] + score_columns
     type_column = "score_data"
-    rows_data = get_csv_rows_data(score_set.variants, columns=columns, dtype=type_column)
+    variants = score_set.variants
+
+    if start:
+        variants = variants[start:]
+    if limit:
+        variants = variants[:limit]
+
+    rows_data = get_csv_rows_data(variants, columns=columns, dtype=type_column)
     stream = io.StringIO()
     writer = csv.DictWriter(stream, fieldnames=columns, quoting=csv.QUOTE_MINIMAL)
     writer.writeheader()
     writer.writerows(rows_data)
     return StreamingResponse(iter([stream.getvalue()]), media_type="text/csv")
 
 
@@ -171,30 +193,49 @@
             """ and hgvs_splice), plus score columns defined by the score set.""",
         }
     },
 )
 async def get_score_set_counts_csv(
     *,
     urn: str,
+    start: int = Query(default=None, description="Start index for pagination"),
+    limit: int = Query(default=None, description="Number of variants to return"),
     db: Session = Depends(deps.get_db),
     user: User = Depends(get_current_user),
 ) -> Any:
     """
     Return counts from a score set, identified by URN, in CSV format.
-    """
+    If no start and limit, all of variants of this score set will be returned.
+    Example path:
+    /score-sets/{urn}/counts
+    /score-sets/{urn}/counts?start=0&limit=100
+    /score-sets/{urn}/counts?start=100
+    """
+    if start and start < 0:
+        raise HTTPException(status_code=400, detail="Start index must be non-negative")
+    if limit != None and limit <= 0:
+        raise HTTPException(status_code=400, detail="Limit must be positive")
+
     score_set = db.query(ScoreSet).filter(ScoreSet.urn == urn).first()
     if not score_set:
         raise HTTPException(status_code=404, detail=f"score set with URN {urn} not found")
-    permission = has_permission(user, score_set, Action.READ)
-    if not permission.permitted:
-        raise HTTPException(status_code=permission.http_code, detail=permission.message)
+    assert_permission(user, score_set, Action.READ)
 
-    columns = ["accession", "hgvs_nt", "hgvs_splice", "hgvs_pro"] + score_set.dataset_columns["count_columns"]
+    assert type(score_set.dataset_columns) is dict
+    count_columns = [str(x) for x in list(score_set.dataset_columns.get("count_columns", []))]
+    columns = ["accession", "hgvs_nt", "hgvs_splice", "hgvs_pro"] + count_columns
     type_column = "count_data"
-    rows_data = get_csv_rows_data(score_set.variants, columns=columns, dtype=type_column)
+    variants = score_set.variants
+
+    if start:
+        variants = variants[start:]
+    if limit:
+        variants = variants[:limit]
+
+    rows_data = get_csv_rows_data(variants, columns=columns, dtype=type_column)
     stream = io.StringIO()
     writer = csv.DictWriter(stream, fieldnames=columns, quoting=csv.QUOTE_MINIMAL)
     writer.writeheader()
     writer.writerows(rows_data)
     return StreamingResponse(iter([stream.getvalue()]), media_type="text/csv")
 
 
@@ -207,17 +248,15 @@
 ) -> Any:
     """
     Return mapped variants from a score set, identified by URN.
     """
     score_set = db.query(ScoreSet).filter(ScoreSet.urn == urn).first()
     if not score_set:
         raise HTTPException(status_code=404, detail=f"score set with URN {urn} not found")
-    permission = has_permission(user, score_set, Action.READ)
-    if not permission.permitted:
-        raise HTTPException(status_code=permission.http_code, detail=permission.message)
+    assert_permission(user, score_set, Action.READ)
 
     mapped_variants = (
         db.query(MappedVariant)
         .filter(ScoreSet.urn == urn)
         .filter(ScoreSet.id == Variant.score_set_id)
         .filter(Variant.id == MappedVariant.variant_id)
         .all()
@@ -225,24 +264,14 @@
 
     if not mapped_variants:
         raise HTTPException(status_code=404, detail=f"No mapped variant associated with score set URN {urn} was found")
 
     return mapped_variants
 
 
-class HGVSColumns:
-    NUCLEOTIDE: str = "hgvs_nt"  # dataset.constants.hgvs_nt_column
-    TRANSCRIPT: str = "hgvs_splice"  # dataset.constants.hgvs_splice_column
-    PROTEIN: str = "hgvs_pro"  # dataset.constants.hgvs_pro_column
-
-    @classmethod
-    def options(cls) -> List[str]:
-        return [cls.NUCLEOTIDE, cls.TRANSCRIPT, cls.PROTEIN]
-
-
 @router.post("/score-sets/", response_model=score_set.ScoreSet, responses={422: {}}, response_model_exclude_none=True)
 async def create_score_set(
     *,
     item_create: score_set.ScoreSetCreate,
     db: Session = Depends(deps.get_db),
     user: User = Depends(require_current_user),
 ) -> Any:
@@ -251,54 +280,59 @@
     """
 
     # TODO Confirm that the experiment is editable by this user.
 
     if item_create is None:
         return None
 
-    experiment: Experiment = None
+    experiment: Optional[Experiment] = None
     if item_create.experiment_urn is not None:
         experiment = db.query(Experiment).filter(Experiment.urn == item_create.experiment_urn).one_or_none()
         if not experiment:
             raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Unknown experiment")
-        permission = has_permission(user, experiment, Action.ADD_SCORE_SET)
-        if not permission.permitted:
-            raise HTTPException(status_code=permission.http_code, detail=permission.message)
+        assert_permission(user, experiment, Action.ADD_SCORE_SET)
 
     license_ = db.query(License).filter(License.id == item_create.license_id).one_or_none()
     if not license_:
         raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Unknown license")
 
     if item_create.superseded_score_set_urn is not None:
         superseded_score_set = await fetch_score_set_by_urn(db, item_create.superseded_score_set_urn, user)
         if superseded_score_set is None:
             raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Unknown superseded score set")
     else:
         superseded_score_set = None
 
     distinct_meta_analyzes_score_set_urns = list(set(item_create.meta_analyzes_score_set_urns or []))
     meta_analyzes_score_sets = [
-        await fetch_score_set_by_urn(db, urn, None) for urn in distinct_meta_analyzes_score_set_urns
+        ss
+        for ss in [await fetch_score_set_by_urn(db, urn, None) for urn in distinct_meta_analyzes_score_set_urns]
+        if ss is not None
     ]
+
     for i, meta_analyzes_score_set in enumerate(meta_analyzes_score_sets):
         if meta_analyzes_score_set is None:
             raise HTTPException(
                 status_code=status.HTTP_400_BAD_REQUEST,
                 detail=f"Unknown meta-analyzed score set {distinct_meta_analyzes_score_set_urns[i]}",
             )
 
     if len(meta_analyzes_score_sets) > 0:
         # If any existing score set is a meta-analysis for score sets in the same collection of exepriment sets, use its
         # experiment as the parent of our new meta-analysis. Otherwise, create a new experiment.
         meta_analyzes_experiment_sets = list(
-            set(map(lambda ss: ss.experiment.experiment_set, meta_analyzes_score_sets))
-        )
-        meta_analyzes_experiment_set_urns = list(
-            set(map(lambda ss: ss.experiment.experiment_set.urn, meta_analyzes_score_sets))
+            set(
+                (
+                    ss.experiment.experiment_set
+                    for ss in meta_analyzes_score_sets
+                    if ss.experiment.experiment_set is not None
+                )
+            )
         )
+        meta_analyzes_experiment_set_urns = [es.urn for es in meta_analyzes_experiment_sets if es.urn is not None]
         existing_meta_analyses = find_meta_analyses_for_experiment_sets(db, meta_analyzes_experiment_set_urns)
 
         if len(existing_meta_analyses) > 0:
             experiment = existing_meta_analyses[0].experiment
         elif len(meta_analyzes_experiment_sets) == 1:
             # The analyzed score sets all belong to one experiment set, so the meta-analysis should go in that
             # experiment set's meta-analysis experiment. But there is no meta-analysis experiment (or else we would
@@ -339,58 +373,104 @@
     ] + primary_publication_identifiers
     # create a temporary `primary` attribute on each of our publications that indicates
     # to our association proxy whether it is a primary publication or not
     primary_identifiers = [pub.identifier for pub in primary_publication_identifiers]
     for publication in publication_identifiers:
         setattr(publication, "primary", publication.identifier in primary_identifiers)
 
-    wt_sequence = WildTypeSequence(**jsonable_encoder(item_create.target_gene.wt_sequence, by_alias=False))
-    target_gene = TargetGene(
-        **jsonable_encoder(
-            item_create.target_gene,
-            by_alias=False,
-            exclude={"external_identifiers", "reference_maps", "wt_sequence"},
-        ),
-        wt_sequence=wt_sequence,
-    )
-    for external_gene_identifier_offset_create in item_create.target_gene.external_identifiers:
-        offset = external_gene_identifier_offset_create.offset
-        identifier_create = external_gene_identifier_offset_create.identifier
-        await create_external_gene_identifier_offset(
-            db, target_gene, identifier_create.db_name, identifier_create.identifier, offset
-        )
-    reference_map = ReferenceMap(genome_id=item_create.target_gene.reference_maps[0].genome_id, target=target_gene)
+    targets: list[TargetGene] = []
+    accessions = False
+    for gene in item_create.target_genes:
+        if gene.target_sequence:
+            if accessions and len(targets) > 0:
+                raise MixedTargetError(
+                    "MaveDB does not support score-sets with both sequence and accession based targets. Please re-submit this scoreset using only one type of target."
+                )
+            upload_taxonomy = gene.target_sequence.taxonomy
+            taxonomy = await find_or_create_taxonomy(db, upload_taxonomy)
+
+            if not taxonomy:
+                raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Unknown taxonomy")
+
+            # If the target sequence has a label, use it. Otherwise, use the name from the target gene as the label.
+            # View model validation rules enforce that sequences must have a label defined if there are more than one
+            # targets defined on a score set.
+            seq_label = gene.target_sequence.label if gene.target_sequence.label is not None else gene.name
+            target_sequence = TargetSequence(
+                **jsonable_encoder(gene.target_sequence, by_alias=False, exclude={"taxonomy", "label"}),
+                taxonomy=taxonomy,
+                label=seq_label,
+            )
+            target_gene = TargetGene(
+                **jsonable_encoder(
+                    gene,
+                    by_alias=False,
+                    exclude={"external_identifiers", "target_sequence", "target_accession"},
+                ),
+                target_sequence=target_sequence,
+            )
+
+        elif gene.target_accession:
+            if not accessions and len(targets) > 0:
+                raise MixedTargetError(
+                    "MaveDB does not support score-sets with both sequence and accession based targets. Please re-submit this scoreset using only one type of target."
+                )
+            accessions = True
+            target_accession = TargetAccession(**jsonable_encoder(gene.target_accession, by_alias=False))
+            target_gene = TargetGene(
+                **jsonable_encoder(
+                    gene,
+                    by_alias=False,
+                    exclude={"external_identifiers", "target_sequence", "target_accession"},
+                ),
+                target_accession=target_accession,
+            )
+        else:
+            raise ValueError("One of either `target_accession` or `target_gene` should be present")
+
+        for external_gene_identifier_offset_create in gene.external_identifiers:
+            offset = external_gene_identifier_offset_create.offset
+            identifier_create = external_gene_identifier_offset_create.identifier
+            await create_external_gene_identifier_offset(
+                db, target_gene, identifier_create.db_name, identifier_create.identifier, offset
+            )
+
+        targets.append(target_gene)
+
+    assert experiment is not None
+
     item = ScoreSet(
         **jsonable_encoder(
             item_create,
             by_alias=False,
             exclude={
                 "doi_identifiers",
                 "experiment_urn",
                 "keywords",
                 "license_id",
                 "meta_analyzes_score_set_urns",
                 "primary_publication_identifiers",
                 "secondary_publication_identifiers",
                 "superseded_score_set_urn",
-                "target_gene",
+                "target_genes",
             },
         ),
         experiment=experiment,
         license=license_,
         superseded_score_set=superseded_score_set,
         meta_analyzes_score_sets=meta_analyzes_score_sets,
-        target_gene=target_gene,
+        target_genes=targets,
         doi_identifiers=doi_identifiers,
         publication_identifiers=publication_identifiers,
         processing_state=ProcessingState.incomplete,
         created_by=user,
         modified_by=user,
-    )
-    await item.set_keywords(db, item_create.keywords)
+    )  # type: ignore
+    if item_create.keywords is not None:
+        await item.set_keywords(db, item_create.keywords)
     db.add(item)
     db.commit()
     db.refresh(item)
     return item
 
 
 @router.post(
@@ -402,153 +482,69 @@
 async def upload_score_set_variant_data(
     *,
     urn: str,
     counts_file: Optional[UploadFile] = File(None),
     scores_file: UploadFile = File(...),
     db: Session = Depends(deps.get_db),
     user: User = Depends(require_current_user),
+    worker: ArqRedis = Depends(deps.get_worker),
 ) -> Any:
     """
     Upload scores and variant count files for a score set, and initiate processing these files to
     create variants.
     """
 
     # TODO Confirm access.
 
     # item = db.query(ScoreSet).filter(ScoreSet.urn == urn).filter(ScoreSet.private.is_(False)).one_or_none()
     item = db.query(ScoreSet).filter(ScoreSet.urn == urn).one_or_none()
-    if not item.urn or not scores_file:
+    if not item or not item.urn or not scores_file:
         return None
-    permission = has_permission(user, item, Action.SET_SCORES)
-    if not permission.permitted:
-        raise HTTPException(status_code=permission.http_code, detail=permission.message)
+    assert_permission(user, item, Action.SET_SCORES)
 
-    # Delete the old variants so that uploading new scores and counts won't accumulate the old ones.
+    # Mark the score set as being processed and delete the old variants so that uploading new scores and counts won't accumulate the old ones.
+    item.processing_state = ProcessingState.processing
     db.query(Variant).filter(Variant.score_set_id == item.id).delete()
-
-    extra_na_values = set(
-        list(null_values_list)
-        + [str(x).lower() for x in null_values_list]
-        + [str(x).upper() for x in null_values_list]
-        + [str(x).capitalize() for x in null_values_list]
-    )
-    scores_df = pd.read_csv(
-        filepath_or_buffer=scores_file.file,
-        sep=",",
-        encoding="utf-8",
-        quotechar="'",
-        comment="#",
-        na_values=extra_na_values,
-        keep_default_na=True,
-        dtype={**{col: str for col in HGVSColumns.options()}, "scores": float},
-    )  # .replace(null_values_re, np.NaN) String will be replaced to NaN value
-    for c in HGVSColumns.options():
-        if c not in scores_df.columns:
-            scores_df[c] = np.NaN
-    score_columns = [col for col in scores_df.columns if col not in HGVSColumns.options()]
-    counts_df = None
-    count_columns = []
-    if counts_file and counts_file.filename:
-        counts_df = pd.read_csv(
-            filepath_or_buffer=counts_file.file,
-            sep=",",
-            encoding="utf-8",
-            quotechar="'",
-            comment="#",
-            na_values=extra_na_values,
-            keep_default_na=True,
-            dtype={**{col: str for col in HGVSColumns.options()}, "scores": float},
-        ).replace(null_values_re, np.NaN)
-        for c in HGVSColumns.options():
-            if c not in counts_df.columns:
-                counts_df[c] = np.NaN
-
-        count_columns = [col for col in counts_df.columns if col not in HGVSColumns.options()]
-    """
-    if counts_file:
-        try:
-            validate_column_names(counts_df)
-        except exceptions.ValidationError as e:
-            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=str(e))
-    """
-    if scores_file:
-        try:
-            validate_and_standardize_dataframe_pair(
-                scores_df, counts_df, item.target_gene.wt_sequence.sequence, item.target_gene.wt_sequence.sequence_type
-            )
-        except exceptions.ValidationError as e:
-            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=str(e))
-
-    variants_data = create_variants_data(scores_df, counts_df, None)  # , index_col)
-
-    item.num_variants = create_variants(db, item, variants_data)
-    logger.info(f"saving variants for {item.urn}")
-
-    item.dataset_columns = {"count_columns": list(count_columns), "score_columns": list(score_columns)}
-    item.modified_by = user
     db.add(item)
-
-    # create_variants_task.submit_task(kwargs={
-    #    'user_id': None,
-    #    'score_set_urn': item.urn,
-    #    'scores': None
-    #    # 'counts',
-    #    # 'index_col',
-    #    # 'dataset_columns'
-    # })
-
     db.commit()
     db.refresh(item)
-    return item
-
 
-# @classmethod
-# @transaction.atomic
-def create_variants(db, score_set: ScoreSet, variants_data: list[VariantData], batch_size=None) -> int:
-    num_variants = len(variants_data)
-    variant_urns = bulk_create_urns(num_variants, score_set, True)
-    variants = (
-        Variant(urn=urn, score_set_id=score_set.id, **kwargs) for urn, kwargs in zip(variant_urns, variants_data)
-    )
-    db.bulk_save_objects(variants)
-    db.add(score_set)
-    return len(score_set.variants)
+    scores_df = csv_data_to_df(scores_file.file)
+    counts_df = None
+    if counts_file and counts_file.filename:
+        counts_df = csv_data_to_df(counts_file.file)
 
+    if scores_file:
+        # await the insertion of this job into the worker queue, not the job itself.
+        await worker.enqueue_job("create_variants_for_score_set", item.urn, user.id, scores_df, counts_df)
 
-# @staticmethod
-def bulk_create_urns(n, score_set, reset_counter=False) -> List[str]:
-    start_value = 0 if reset_counter else score_set.num_variants
-    parent_urn = score_set.urn
-    child_urns = ["{}#{}".format(parent_urn, start_value + (i + 1)) for i in range(n)]
-    current_value = start_value + n
-    score_set.num_variants = current_value
-    return child_urns
+    return item
 
 
 @router.put("/score-sets/{urn}", response_model=score_set.ScoreSet, responses={422: {}})
 async def update_score_set(
     *,
     urn: str,
     item_update: score_set.ScoreSetUpdate,
     db: Session = Depends(deps.get_db),
     user: User = Depends(require_current_user),
+    hdp: RESTDataProvider = Depends(deps.hgvs_data_provider),  # TODO - remove.
+    worker: ArqRedis = Depends(deps.get_worker),
 ) -> Any:
     """
     Update a score set.
     """
 
     if not item_update:
         raise HTTPException(status_code=400, detail="The request contained no updated item.")
 
     item = db.query(ScoreSet).filter(ScoreSet.urn == urn).one_or_none()
     if not item:
         raise HTTPException(status_code=404, detail=f"score set with URN '{urn}' not found")
-    permission = has_permission(user, item, Action.UPDATE)
-    if not permission.permitted:
-        raise HTTPException(status_code=permission.http_code, detail=permission.message)
+    assert_permission(user, item, Action.UPDATE)
 
     # Editing unpublished score set
     if item.private is True:
         license_ = None
         if item_update.license_id is not None:
             license_ = db.query(License).filter(License.id == item_update.license_id).one_or_none()
             if not license_:
@@ -559,86 +555,148 @@
             if var not in [
                 "keywords",
                 "doi_identifiers",
                 "experiment_urn",
                 "license_id",
                 "secondary_publication_identifiers",
                 "primary_publication_identifiers",
-                "target_gene",
+                "target_genes",
             ]:
                 setattr(item, var, value) if value else None
 
         item.doi_identifiers = [
             await find_or_create_doi_identifier(db, identifier.identifier)
             for identifier in item_update.doi_identifiers or []
         ]
         primary_publication_identifiers = [
             await find_or_create_publication_identifier(db, identifier.identifier, identifier.db_name)
             for identifier in item_update.primary_publication_identifiers or []
         ]
         publication_identifiers = [
             await find_or_create_publication_identifier(db, identifier.identifier, identifier.db_name)
             for identifier in item_update.secondary_publication_identifiers or []
-        ]
+        ] + primary_publication_identifiers
         # create a temporary `primary` attribute on each of our publications that indicates
         # to our association proxy whether it is a primary publication or not
         primary_identifiers = [pub.identifier for pub in primary_publication_identifiers]
         for publication in publication_identifiers:
             setattr(publication, "primary", publication.identifier in primary_identifiers)
 
         item.publication_identifiers = publication_identifiers
-        await item.set_keywords(db, item_update.keywords)
+        if item_update.keywords is not None:
+            await item.set_keywords(db, item_update.keywords)
 
         # Delete the old target gene, WT sequence, and reference map. These will be deleted when we set the score set's
         # target_gene to None, because we have set cascade='all,delete-orphan' on ScoreSet.target_gene. (Since the
         # relationship is defined with the target gene as owner, this is actually set up in the backref attribute of
         # TargetGene.score_set.)
         #
         # We must flush our database queries now so that the old target gene will be deleted before inserting a new one
         # with the same score_set_id.
-        item.target_gene = None
+        item.target_genes = []
         db.flush()
 
-        wt_sequence = WildTypeSequence(**jsonable_encoder(item_update.target_gene.wt_sequence, by_alias=False))
+        targets: List[TargetGene] = []
+        accessions = False
+        for gene in item_update.target_genes:
+            if gene.target_sequence:
+                if accessions and len(targets) > 0:
+                    raise MixedTargetError(
+                        "MaveDB does not support score-sets with both sequence and accession based targets. Please re-submit this scoreset using only one type of target."
+                    )
+
+                upload_taxonomy = gene.target_sequence.taxonomy
+                taxonomy = await find_or_create_taxonomy(db, upload_taxonomy)
+
+                if not taxonomy:
+                    raise HTTPException(
+                        status_code=status.HTTP_400_BAD_REQUEST,
+                        detail=f"Unknown taxonomy {gene.target_sequence.taxonomy.tax_id}",
+                    )
+
+                # If the target sequence has a label, use it. Otherwise, use the name from the target gene as the label.
+                # View model validation rules enforce that sequences must have a label defined if there are more than one
+                # targets defined on a score set.
+                seq_label = gene.target_sequence.label if gene.target_sequence.label is not None else gene.name
+                target_sequence = TargetSequence(
+                    **jsonable_encoder(gene.target_sequence, by_alias=False, exclude={"taxonomy", "label"}),
+                    taxonomy=taxonomy,
+                    label=seq_label,
+                )
+                target_gene = TargetGene(
+                    **jsonable_encoder(
+                        gene,
+                        by_alias=False,
+                        exclude={"external_identifiers", "target_sequence", "target_accession"},
+                    ),
+                    target_sequence=target_sequence,
+                )
+
+            elif gene.target_accession:
+                if not accessions and len(targets) > 0:
+                    raise MixedTargetError(
+                        "MaveDB does not support score-sets with both sequence and accession based targets. Please re-submit this scoreset using only one type of target."
+                    )
+                accessions = True
+                target_accession = TargetAccession(**jsonable_encoder(gene.target_accession, by_alias=False))
+                target_gene = TargetGene(
+                    **jsonable_encoder(
+                        gene,
+                        by_alias=False,
+                        exclude={"external_identifiers", "target_sequence", "target_accession"},
+                    ),
+                    target_accession=target_accession,
+                )
+            else:
+                raise ValueError("One of either `target_accession` or `target_gene` should be present")
+
+            for external_gene_identifier_offset_create in gene.external_identifiers:
+                offset = external_gene_identifier_offset_create.offset
+                identifier_create = external_gene_identifier_offset_create.identifier
+                await create_external_gene_identifier_offset(
+                    db, target_gene, identifier_create.db_name, identifier_create.identifier, offset
+                )
+
+            targets.append(target_gene)
+
+        item.target_genes = targets
+
+        # re-validate existing variants and clear them if they do not pass validation
+        if item.variants:
+            assert item.dataset_columns is not None
+            score_columns = ["hgvs_nt", "hgvs_splice", "hgvs_pro"] + item.dataset_columns["score_columns"]
+            count_columns = ["hgvs_nt", "hgvs_splice", "hgvs_pro"] + item.dataset_columns["count_columns"]
+            scores_data = pd.DataFrame(
+                get_csv_rows_data(item.variants, columns=score_columns, dtype="score_data")
+            ).replace("NA", pd.NA)
+            count_data = pd.DataFrame(
+                get_csv_rows_data(item.variants, columns=count_columns, dtype="count_data")
+            ).replace("NA", pd.NA)
 
-        target_gene = TargetGene(
-            **jsonable_encoder(
-                item_update.target_gene,
-                by_alias=False,
-                exclude={"external_identifiers", "reference_maps", "wt_sequence"},
-            ),
-            wt_sequence=wt_sequence,
-        )
-        for external_gene_identifier_offset_create in item_update.target_gene.external_identifiers:
-            offset = external_gene_identifier_offset_create.offset
-            identifier_create = external_gene_identifier_offset_create.identifier
-            external_gene_identifier = await create_external_gene_identifier_offset(
-                db, target_gene, identifier_create.db_name, identifier_create.identifier, offset
-            )
-        item.target_gene = target_gene
+            # await the insertion of this job into the worker queue, not the job itself.
+            await worker.enqueue_job("create_variants_for_score_set", item.urn, user.id, scores_data, count_data)
 
-        reference_map = ReferenceMap(genome_id=item_update.target_gene.reference_maps[0].genome_id, target=target_gene)
         for var, value in vars(item_update).items():
             if var not in [
                 "keywords",
                 "doi_identifiers",
                 "experiment_urn",
                 "primary_publication_identifiers",
                 "secondary_publication_identifiers",
-                "target_gene",
+                "target_genes",
             ]:
                 setattr(item, var, value) if value else None
 
     # Editing published score set
     else:
         for var, value in vars(item_update).items():
             if var in ["title", "method_text", "abstract_text", "short_description"]:
                 setattr(item, var, value) if value else None
-    db.add(item)
 
+    db.add(item)
     db.commit()
     db.refresh(item)
     return item
 
 
 @router.delete("/score-sets/{urn}", responses={422: {}})
 async def delete_score_set(
@@ -656,36 +714,32 @@
     or
     communitcate to client whether the operation succeeded
     204 if successful but not returning content - likely going with this
     """
     item = db.query(ScoreSet).filter(ScoreSet.urn == urn).one_or_none()
     if not item:
         raise HTTPException(status_code=404, detail=f"score set with URN '{urn}' not found")
-    permission = has_permission(user, item, Action.DELETE)
-    if not permission.permitted:
-        raise HTTPException(status_code=permission.http_code, detail=permission.message)
+    assert_permission(user, item, Action.DELETE)
     db.delete(item)
     db.commit()
 
 
 @router.post(
     "/score-sets/{urn}/publish", status_code=200, response_model=score_set.ScoreSet, response_model_exclude_none=True
 )
 def publish_score_set(
     *, urn: str, db: Session = Depends(deps.get_db), user: User = Depends(require_current_user)
 ) -> Any:
     """
     Publish a score set.
     """
-    item: ScoreSet = db.query(ScoreSet).filter(ScoreSet.urn == urn).one_or_none()
+    item: Optional[ScoreSet] = db.query(ScoreSet).filter(ScoreSet.urn == urn).one_or_none()
     if not item:
         raise HTTPException(status_code=404, detail=f"score set with URN '{urn}' not found")
-    permission = has_permission(user, item, Action.UPDATE)
-    if not permission.permitted:
-        raise HTTPException(status_code=permission.http_code, detail=permission.message)
+    assert_permission(user, item, Action.UPDATE)
 
     if not item.experiment:
         raise HTTPException(
             status_code=500, detail="This score set does not belong to an experiment and cannot be published."
         )
     if not item.experiment.experiment_set:
         raise HTTPException(
```

### Comparing `mavedb-2023.3.0/src/mavedb/routers/target_gene_identifiers.py` & `mavedb-2024.0.0/src/mavedb/routers/target_gene_identifiers.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 @router.post("/search", status_code=200, response_model=List[external_gene_identifier.ExternalGeneIdentifier])
 def search_target_gene_identifiers(db_name: str, search: TextSearch, db: Session = Depends(deps.get_db)) -> Any:
     """
     Search target gene identifiers.
     """
 
     identifier_class = EXTERNAL_GENE_IDENTIFIER_CLASSES[db_name]
+    assert hasattr(identifier_class, "identifier")
+
     query = db.query(identifier_class)
 
     if search.text and len(search.text.strip()) > 0:
         lower_search_text = search.text.strip().lower()
         query = query.filter(func.lower(identifier_class.identifier).contains(lower_search_text))
     else:
         raise HTTPException(status_code=500, detail="Search text is required")
```

### Comparing `mavedb-2023.3.0/src/mavedb/routers/target_genes.py` & `mavedb-2024.0.0/src/mavedb/routers/target_genes.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,12 +76,11 @@
     query = db.query(TargetGene)
 
     if search.text and len(search.text.strip()) > 0:
         lower_search_text = search.text.strip().lower()
         query = query.filter(func.lower(TargetGene.name).contains(lower_search_text))
     else:
         raise HTTPException(status_code=500, detail="Search text is required")
-
     items = query.order_by(TargetGene.name).limit(50).all()
     if not items:
         items = []
     return items
```

### Comparing `mavedb-2023.3.0/src/mavedb/routers/users.py` & `mavedb-2024.0.0/src/mavedb/routers/users.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/__init__.py` & `mavedb-2024.0.0/src/mavedb/view_models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     Pydantic uses GetterDict objects to access source objects as dictionaries, which can
     then be turned into Pydantic view model objects. We need to remap the underlying
     SQLAlchemy model's AssociationList objects with information about whether a
     publication is primary or not into two separate lists with that same information.
     """
 
-    def get(self, key: str, default: Any) -> Any:
+    def get(self, key: Any, default: Any = ...) -> Any:
         if key == "secondary_publication_identifiers":
             pub_assc = getattr(self._obj, "publication_identifier_associations")
             return [assc.publication for assc in pub_assc if not assc.primary]
         elif key == "primary_publication_identifiers":
             pub_assc = getattr(self._obj, "publication_identifier_associations")
             return [assc.publication for assc in pub_assc if assc.primary]
         else:
```

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/access_key.py` & `mavedb-2024.0.0/src/mavedb/view_models/access_key.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/doi_identifier.py` & `mavedb-2024.0.0/src/mavedb/view_models/doi_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/experiment.py` & `mavedb-2024.0.0/src/mavedb/view_models/experiment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import date
-from typing import Any, Collection, Optional
+from typing import Any, Collection, Optional, Sequence
 
 from mavedb.lib.validation import keywords
 from mavedb.lib.validation.exceptions import ValidationError
 from mavedb.view_models import PublicationIdentifiersGetter
 from mavedb.view_models.base.base import BaseModel, validator
 from mavedb.view_models.doi_identifier import (
     DoiIdentifier,
@@ -20,15 +20,15 @@
     RawReadIdentifierCreate,
     SavedRawReadIdentifier,
 )
 from mavedb.view_models.user import SavedUser, User
 
 
 class ExperimentGetter(PublicationIdentifiersGetter):
-    def get(self, key: str, default: Any) -> Any:
+    def get(self, key: Any, default: Any = ...) -> Any:
         if key == "score_set_urns":
             score_sets = getattr(self._obj, "score_sets") or []
             return sorted([score_set.urn for score_set in score_sets])
         elif key == "experiment_set_urn":
             experiment_set = getattr(self._obj, "experiment_set")
             return experiment_set.urn if experiment_set is not None else None
         else:
@@ -87,18 +87,18 @@
     created_by: SavedUser
     modified_by: SavedUser
     creation_date: date
     modification_date: date
     published_date: Optional[date]
     experiment_set_urn: str
     score_set_urns: list[str]
-    doi_identifiers: list[SavedDoiIdentifier]
-    primary_publication_identifiers: list[SavedPublicationIdentifier]
-    secondary_publication_identifiers: list[SavedPublicationIdentifier]
-    raw_read_identifiers: list[SavedRawReadIdentifier]
+    doi_identifiers: Sequence[SavedDoiIdentifier]
+    primary_publication_identifiers: Sequence[SavedPublicationIdentifier]
+    secondary_publication_identifiers: Sequence[SavedPublicationIdentifier]
+    raw_read_identifiers: Sequence[SavedRawReadIdentifier]
     processing_state: Optional[str]
     keywords: list[str]
 
     class Config:
         orm_mode = True
         getter_dict = ExperimentGetter
 
@@ -108,18 +108,18 @@
     def publication_identifiers_validator(cls, value, values, field) -> list[PublicationIdentifier]:
         assert isinstance(value, Collection), f"{field.name} must be a collection, not {type(value)}"
         return list(value)  # Re-cast into proper list-like type
 
 
 # Properties to return to non-admin clients
 class Experiment(SavedExperiment):
-    doi_identifiers: list[DoiIdentifier]
-    primary_publication_identifiers: list[PublicationIdentifier]
-    secondary_publication_identifiers: list[PublicationIdentifier]
-    raw_read_identifiers: list[RawReadIdentifier]
+    doi_identifiers: Sequence[DoiIdentifier]
+    primary_publication_identifiers: Sequence[PublicationIdentifier]
+    secondary_publication_identifiers: Sequence[PublicationIdentifier]
+    raw_read_identifiers: Sequence[RawReadIdentifier]
     created_by: User
     modified_by: User
 
 
 class ShortExperiment(SavedExperiment):
     pass
```

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/experiment_set.py` & `mavedb-2024.0.0/src/mavedb/view_models/experiment_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import date
-from typing import Dict, List
+from typing import List, Sequence
 
 from pydantic.types import Optional
 
 from mavedb.view_models.base.base import BaseModel
 from mavedb.view_models.experiment import Experiment, SavedExperiment
 from mavedb.view_models.user import SavedUser, User
 
@@ -20,32 +20,32 @@
 class ExperimentSetUpdate(ExperimentSetBase):
     pass
 
 
 # Properties shared by models stored in DB
 class SavedExperimentSet(ExperimentSetBase):
     id: int
-    experiments: List[SavedExperiment]
+    experiments: Sequence[SavedExperiment]
     created_by: Optional[SavedUser]
     modified_by: Optional[SavedUser]
     creation_date: date
     modification_date: date
 
     class Config:
         orm_mode = True
 
 
 # Properties to return to non-admin clients
 class ExperimentSet(SavedExperimentSet):
     created_by: Optional[User]
     modified_by: Optional[User]
-    experiments: List[Experiment]
+    experiments: Sequence[Experiment]
 
 
 # Properties to return to admin clients
 class AdminExperimentSet(SavedExperimentSet):
     private: bool
     approved: bool
     processing_state: Optional[str]
     created_by: Optional[User]
     modified_by: Optional[User]
-    experiments: List[Experiment]
+    experiments: Sequence[Experiment]
```

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/external_gene_identifier.py` & `mavedb-2024.0.0/src/mavedb/view_models/external_gene_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/external_gene_identifier_offset.py` & `mavedb-2024.0.0/src/mavedb/view_models/external_gene_identifier_offset.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/license.py` & `mavedb-2024.0.0/src/mavedb/view_models/license.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/publication_identifier.py` & `mavedb-2024.0.0/src/mavedb/view_models/publication_identifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 # Properties of external publication identifiers
 class ExternalPublicationIdentifier(PublicationIdentifierBase):
     url: str
     reference_html: str
     title: str
-    abstract: str
+    abstract: Optional[str]
     authors: list[dict[str, str]]
     publication_doi: Optional[str]
     preprint_doi: Optional[str]
     publication_year: Optional[int]
     preprint_date: Optional[date]
     publication_journal: Optional[str]
```

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/search.py` & `mavedb-2024.0.0/src/mavedb/view_models/search.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 class ScoreSetsSearch(BaseModel):
     published: Optional[bool]
     targets: Optional[list[str]]
     target_organism_names: Optional[list[str]]
     target_types: Optional[list[str]]
+    target_accessions: Optional[list[str]]
     authors: Optional[list[str]]
     databases: Optional[list[str]]
     journals: Optional[list[str]]
     publication_identifiers: Optional[list[str]]
     text: Optional[str]
```

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/user.py` & `mavedb-2024.0.0/src/mavedb/view_models/user.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/variant.py` & `mavedb-2024.0.0/src/mavedb/view_models/variant.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/wild_type_sequence.py` & `mavedb-2024.0.0/src/mavedb/view_models/target_sequence.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from datetime import date
+from typing import Optional
 
 from mavedb.view_models.base.base import BaseModel, validator
+from mavedb.view_models.taxonomy import AdminTaxonomy, SavedTaxonomy, Taxonomy, TaxonomyCreate
 from mavedb.lib.validation import target
+from mavedb.lib.validation.exceptions import ValidationError
 
 from fqfa import infer_sequence_type
 
 
-class WildTypeSequenceBase(BaseModel):
+class TargetSequenceBase(BaseModel):
     sequence_type: str
     sequence: str
+    label: Optional[str]
 
 
-class WildTypeSequenceModify(WildTypeSequenceBase):
+class TargetSequenceModify(TargetSequenceBase):
     @validator("sequence_type")
     def validate_category(cls, field_value, values, field, config):
         field_value = field_value.lower()
         target.validate_sequence_category(field_value)
         if field_value == "infer":
             if "sequence" in values.keys():
                 field_value = infer_sequence_type(values["sequence"])
@@ -31,32 +35,45 @@
             sequence_type = values["sequence_type"]
             # field_value is sequence
             target.validate_target_sequence(field_value, sequence_type)
         else:
             raise ValueError("sequence_type is invalid")
         return field_value
 
+    @validator("label")
+    def check_alphanumeric(cls, field_value, values, field, config) -> str:
+        if isinstance(field_value, str):
+            is_alphanumeric = field_value.replace("_", "").isalnum()
+            if not is_alphanumeric:
+                raise ValidationError(
+                    f"Target sequence label `{field_value}` can contain only letters, numbers, and underscores."
+                )
+        return field_value
 
-class WildTypeSequenceCreate(WildTypeSequenceModify):
-    pass
+
+class TargetSequenceCreate(TargetSequenceModify):
+    taxonomy: TaxonomyCreate
 
 
-class WildTypeSequenceUpdate(WildTypeSequenceModify):
+class TargetSequenceUpdate(TargetSequenceModify):
     pass
 
 
 # Properties shared by models stored in DB
-class SavedWildTypeSequence(WildTypeSequenceBase):
+class SavedTargetSequence(TargetSequenceBase):
+    taxonomy: SavedTaxonomy
+
     class Config:
         orm_mode = True
         arbitrary_types_allowed = True
 
 
 # Properties to return to non-admin clients
-class WildTypeSequence(SavedWildTypeSequence):
-    pass
+class TargetSequence(SavedTargetSequence):
+    taxonomy: Taxonomy
 
 
 # Properties to return to admin clients
-class AdminWildTypeSequence(SavedWildTypeSequence):
+class AdminTargetSequence(SavedTargetSequence):
     creation_date: date
     modification_date: date
+    taxonomy: AdminTaxonomy
```

### Comparing `mavedb-2023.3.0/src/mavedb/view_models/base/base.py` & `mavedb-2024.0.0/src/mavedb/view_models/base/base.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/routers/counts.csv` & `mavedb-2024.0.0/tests/routers/counts.csv`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/routers/counts_with_different_variants.csv` & `mavedb-2024.0.0/tests/routers/counts_with_different_variants.csv`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/routers/counts_with_score.csv` & `mavedb-2024.0.0/tests/routers/counts_with_score.csv`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/routers/scores.csv` & `mavedb-2024.0.0/tests/routers/scores.csv`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/routers/scores_hgvs_pro_has_same_values.csv` & `mavedb-2024.0.0/tests/routers/scores_hgvs_pro_has_same_values.csv`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/routers/scores_with_duplicate_columns.csv` & `mavedb-2024.0.0/tests/routers/scores_with_duplicate_columns.csv`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/routers/scores_with_invalid_hgvs_nt_prefix.csv` & `mavedb-2024.0.0/tests/routers/scores_with_invalid_hgvs_nt_prefix.csv`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/routers/scores_with_invalid_hgvs_pro_prefix.csv` & `mavedb-2024.0.0/tests/routers/scores_with_invalid_hgvs_pro_prefix.csv`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/routers/scores_with_nan_column_name.csv` & `mavedb-2024.0.0/tests/routers/scores_with_nan_column_name.csv`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/routers/scores_with_string.csv` & `mavedb-2024.0.0/tests/routers/scores_with_string.csv`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/routers/test_score_set.py` & `mavedb-2024.0.0/tests/routers/test_score_set.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,51 @@
-from pathlib import Path
-import jsonschema
 import re
 from copy import deepcopy
 from datetime import date
+from unittest.mock import patch
+
+import jsonschema
 import pytest
-from mavedb.view_models.score_set import ScoreSet, ScoreSetCreate
-from mavedb.models.score_set import ScoreSet as ScoreSetDbModel
-from tests.helpers.constants import TEST_MINIMAL_SCORE_SET, TEST_MINIMAL_SCORE_SET_RESPONSE
-from tests.helpers.util import create_experiment, create_score_set, change_ownership, create_score_set_with_variants
+from arq import ArqRedis
 from mavedb.lib.validation.urn_re import MAVEDB_TMP_URN_RE
+from mavedb.models.enums.processing_state import ProcessingState
+from mavedb.models.score_set import ScoreSet as ScoreSetDbModel
+from mavedb.view_models.score_set import ScoreSet, ScoreSetCreate
+
+from tests.helpers.constants import (
+    TEST_MINIMAL_ACC_SCORESET,
+    TEST_MINIMAL_SEQ_SCORESET,
+    TEST_MINIMAL_SEQ_SCORESET_RESPONSE,
+)
+from tests.helpers.util import (
+    change_ownership,
+    create_experiment,
+    create_seq_score_set,
+    create_seq_score_set_with_variants,
+)
+
 
+def test_TEST_MINIMAL_SEQ_SCORESET_is_valid():
+    jsonschema.validate(instance=TEST_MINIMAL_SEQ_SCORESET, schema=ScoreSetCreate.schema())
 
-def test_test_minimal_score_set_is_valid():
-    jsonschema.validate(instance=TEST_MINIMAL_SCORE_SET, schema=ScoreSetCreate.schema())
+
+def test_TEST_MINIMAL_ACC_SCORESET_is_valid():
+    jsonschema.validate(instance=TEST_MINIMAL_ACC_SCORESET, schema=ScoreSetCreate.schema())
 
 
 def test_create_minimal_score_set(client, setup_router_db):
     experiment = create_experiment(client)
-    score_set_post_payload = deepcopy(TEST_MINIMAL_SCORE_SET)
+    score_set_post_payload = deepcopy(TEST_MINIMAL_SEQ_SCORESET)
     score_set_post_payload["experimentUrn"] = experiment["urn"]
     response = client.post("/api/v1/score-sets/", json=score_set_post_payload)
     assert response.status_code == 200
     response_data = response.json()
     jsonschema.validate(instance=response_data, schema=ScoreSet.schema())
     assert isinstance(MAVEDB_TMP_URN_RE.fullmatch(response_data["urn"]), re.Match)
-    expected_response = deepcopy(TEST_MINIMAL_SCORE_SET_RESPONSE)
+    expected_response = deepcopy(TEST_MINIMAL_SEQ_SCORESET_RESPONSE)
     expected_response.update({"urn": response_data["urn"]})
     expected_response["experiment"].update(
         {
             "urn": experiment["urn"],
             "experimentSetUrn": experiment["experimentSetUrn"],
             "scoreSetUrns": [response_data["urn"]],
         }
@@ -38,16 +55,16 @@
         assert (key, expected_response[key]) == (key, response_data[key])
     response = client.get(f"/api/v1/score-sets/{response_data['urn']}")
     assert response.status_code == 200
 
 
 def test_get_own_private_score_set(client, setup_router_db):
     experiment = create_experiment(client)
-    score_set = create_score_set(client, experiment["urn"])
-    expected_response = deepcopy(TEST_MINIMAL_SCORE_SET_RESPONSE)
+    score_set = create_seq_score_set(client, experiment["urn"])
+    expected_response = deepcopy(TEST_MINIMAL_SEQ_SCORESET_RESPONSE)
     expected_response.update({"urn": score_set["urn"]})
     expected_response["experiment"].update(
         {
             "urn": experiment["urn"],
             "experimentSetUrn": experiment["experimentSetUrn"],
             "scoreSetUrns": [score_set["urn"]],
         }
@@ -58,115 +75,141 @@
     assert sorted(expected_response.keys()) == sorted(response_data.keys())
     for key in expected_response:
         assert (key, expected_response[key]) == (key, response_data[key])
 
 
 def test_cannot_get_other_user_private_score_set(session, client, setup_router_db):
     experiment = create_experiment(client)
-    score_set = create_score_set(client, experiment["urn"])
+    score_set = create_seq_score_set(client, experiment["urn"])
     change_ownership(session, score_set["urn"], ScoreSetDbModel)
     response = client.get(f"/api/v1/score-sets/{score_set['urn']}")
     assert response.status_code == 404
     response_data = response.json()
     assert f"score set with URN '{score_set['urn']}' not found" in response_data["detail"]
 
 
-def test_add_score_set_variants_scores_only(client, setup_router_db, data_files):
+def test_add_score_set_variants_scores_only_endpoint(client, setup_router_db, data_files):
     experiment = create_experiment(client)
-    score_set = create_score_set(client, experiment["urn"])
+    score_set = create_seq_score_set(client, experiment["urn"])
     scores_csv_path = data_files / "scores.csv"
-    with open(scores_csv_path, "rb") as scores_file:
+    with (
+        open(scores_csv_path, "rb") as scores_file,
+        patch.object(ArqRedis, "enqueue_job", return_value=None) as queue,
+    ):
         response = client.post(
             f"/api/v1/score-sets/{score_set['urn']}/variants/data",
             files={"scores_file": (scores_csv_path.name, scores_file, "text/csv")},
         )
+        queue.assert_called_once()
+
     assert response.status_code == 200
     response_data = response.json()
     jsonschema.validate(instance=response_data, schema=ScoreSet.schema())
-    assert response_data["numVariants"] == 3
-    assert response_data["datasetColumns"] == {"countColumns": [], "scoreColumns": ["score"]}
 
+    # We test the worker process that actually adds the variant data separately. Here, we take it as
+    # fact that it would have succeeded.
+    score_set.update({"processingState": "processing"})
+    assert score_set == response_data
 
-def test_add_score_set_variants_scores_and_counts(client, setup_router_db, data_files):
+
+def test_add_score_set_variants_scores_and_counts_endpoint(session, client, setup_router_db, data_files):
     experiment = create_experiment(client)
-    score_set = create_score_set(client, experiment["urn"])
+    score_set = create_seq_score_set(client, experiment["urn"])
     scores_csv_path = data_files / "scores.csv"
     counts_csv_path = data_files / "counts.csv"
-    with open(scores_csv_path, "rb") as scores_file, open(counts_csv_path, "rb") as counts_file:
+    with (
+        open(scores_csv_path, "rb") as scores_file,
+        open(counts_csv_path, "rb") as counts_file,
+        patch.object(ArqRedis, "enqueue_job", return_value=None) as queue,
+    ):
         response = client.post(
             f"/api/v1/score-sets/{score_set['urn']}/variants/data",
             files={
                 "scores_file": (scores_csv_path.name, scores_file, "text/csv"),
                 "counts_file": (counts_csv_path.name, counts_file, "text/csv"),
             },
         )
+        queue.assert_called_once()
+
     assert response.status_code == 200
     response_data = response.json()
     jsonschema.validate(instance=response_data, schema=ScoreSet.schema())
-    assert response_data["numVariants"] == 3
-    assert response_data["datasetColumns"] == {"countColumns": ["c_0", "c_1"], "scoreColumns": ["score"]}
+
+    # We test the worker process that actually adds the variant data separately. Here, we take it as
+    # fact that it would have succeeded.
+    score_set.update({"processingState": "processing"})
+    assert score_set == response_data
 
 
 def test_cannot_add_scores_to_other_user_score_set(session, client, setup_router_db, data_files):
     experiment = create_experiment(client)
-    score_set = create_score_set(client, experiment["urn"])
+    score_set = create_seq_score_set(client, experiment["urn"])
     change_ownership(session, score_set["urn"], ScoreSetDbModel)
     scores_csv_path = data_files / "scores.csv"
     with open(scores_csv_path, "rb") as scores_file:
         response = client.post(
             f"/api/v1/score-sets/{score_set['urn']}/variants/data",
             files={"scores_file": (scores_csv_path.name, scores_file, "text/csv")},
         )
     assert response.status_code == 404
     response_data = response.json()
     assert f"score set with URN '{score_set['urn']}' not found" in response_data["detail"]
 
 
-def test_publish_score_set(client, setup_router_db, data_files):
+def test_publish_score_set(session, data_provider, client, setup_router_db, data_files):
     experiment = create_experiment(client)
-    score_set = create_score_set_with_variants(client, experiment["urn"], data_files / "scores.csv")
+    score_set = create_seq_score_set_with_variants(
+        client, session, data_provider, experiment["urn"], data_files / "scores.csv"
+    )
+
     response = client.post(f"/api/v1/score-sets/{score_set['urn']}/publish")
     assert response.status_code == 200
     response_data = response.json()
     assert response_data["urn"] == "urn:mavedb:00000001-a-1"
     assert response_data["experiment"]["urn"] == "urn:mavedb:00000001-a"
-    expected_response = deepcopy(TEST_MINIMAL_SCORE_SET_RESPONSE)
+
+    expected_response = deepcopy(TEST_MINIMAL_SEQ_SCORESET_RESPONSE)
     expected_response.update(
         {
             "urn": response_data["urn"],
             "publishedDate": date.today().isoformat(),
             "numVariants": 3,
             "private": False,
             "datasetColumns": {"countColumns": [], "scoreColumns": ["score"]},
+            "processingState": ProcessingState.success.name,
         }
     )
     expected_response["experiment"].update(
         {
             "urn": response_data["experiment"]["urn"],
             "experimentSetUrn": response_data["experiment"]["experimentSetUrn"],
             "scoreSetUrns": [response_data["urn"]],
             "publishedDate": date.today().isoformat(),
         }
     )
     assert sorted(expected_response.keys()) == sorted(response_data.keys())
+
+    # refresh score set to post worker state
+    score_set = (client.get(f"/api/v1/score-sets/{response_data['urn']}")).json()
     for key in expected_response:
-        assert (key, expected_response[key]) == (key, response_data[key])
+        assert (key, expected_response[key]) == (key, score_set[key])
 
 
-def test_publish_multiple_score_sets(client, setup_router_db, data_files):
+def test_publish_multiple_score_sets(session, data_provider, client, setup_router_db, data_files):
     experiment = create_experiment(client)
-    score_set_1 = create_score_set_with_variants(
-        client, experiment["urn"], data_files / "scores.csv", update={"title": "Score Set 1"}
+    score_set_1 = create_seq_score_set_with_variants(
+        client, session, data_provider, experiment["urn"], data_files / "scores.csv", update={"title": "Score Set 1"}
     )
-    score_set_2 = create_score_set_with_variants(
-        client, experiment["urn"], data_files / "scores.csv", update={"title": "Score Set 2"}
+    score_set_2 = create_seq_score_set_with_variants(
+        client, session, data_provider, experiment["urn"], data_files / "scores.csv", update={"title": "Score Set 2"}
     )
-    score_set_3 = create_score_set_with_variants(
-        client, experiment["urn"], data_files / "scores.csv", update={"title": "Score Set 3"}
+    score_set_3 = create_seq_score_set_with_variants(
+        client, session, data_provider, experiment["urn"], data_files / "scores.csv", update={"title": "Score Set 3"}
     )
+
     pub_score_set_1_response = client.post(f"/api/v1/score-sets/{score_set_1['urn']}/publish")
     assert pub_score_set_1_response.status_code == 200
     pub_score_set_2_response = client.post(f"/api/v1/score-sets/{score_set_2['urn']}/publish")
     assert pub_score_set_2_response.status_code == 200
     pub_score_set_3_response = client.post(f"/api/v1/score-sets/{score_set_3['urn']}/publish")
     assert pub_score_set_3_response.status_code == 200
     pub_score_set_1_data = pub_score_set_1_response.json()
@@ -181,184 +224,284 @@
     assert pub_score_set_3_data["urn"] == "urn:mavedb:00000001-a-3"
     assert pub_score_set_3_data["title"] == score_set_3["title"]
     assert pub_score_set_3_data["experiment"]["urn"] == "urn:mavedb:00000001-a"
 
 
 def test_cannot_publish_score_set_without_variants(client, setup_router_db):
     experiment = create_experiment(client)
-    score_set = create_score_set(client, experiment["urn"])
+    score_set = create_seq_score_set(client, experiment["urn"])
     response = client.post(f"/api/v1/score-sets/{score_set['urn']}/publish")
     assert response.status_code == 422
     response_data = response.json()
-    assert f"cannot publish score set without variant scores" in response_data["detail"]
+    assert "cannot publish score set without variant scores" in response_data["detail"]
 
 
-def test_cannot_publish_other_user_private_score_set(session, client, setup_router_db, data_files):
+def test_cannot_publish_other_user_private_score_set(session, data_provider, client, setup_router_db, data_files):
     experiment = create_experiment(client)
-    score_set = create_score_set_with_variants(client, experiment["urn"], data_files / "scores.csv")
+    score_set = create_seq_score_set_with_variants(
+        client, session, data_provider, experiment["urn"], data_files / "scores.csv"
+    )
+
     change_ownership(session, score_set["urn"], ScoreSetDbModel)
     response = client.post(f"/api/v1/score-sets/{score_set['urn']}/publish")
     assert response.status_code == 404
     response_data = response.json()
     assert f"score set with URN '{score_set['urn']}' not found" in response_data["detail"]
 
 
-def test_create_single_score_set_meta_analysis(client, setup_router_db, data_files):
+def test_create_single_score_set_meta_analysis(session, data_provider, client, setup_router_db, data_files):
     experiment = create_experiment(client)
-    score_set = create_score_set_with_variants(client, experiment["urn"], data_files / "scores.csv")
-    score_set = client.post(f"/api/v1/score-sets/{score_set['urn']}/publish").json()
-    meta_score_set = create_score_set_with_variants(
+    score_set = create_seq_score_set_with_variants(
+        client, session, data_provider, experiment["urn"], data_files / "scores.csv"
+    )
+
+    score_set = (client.post(f"/api/v1/score-sets/{score_set['urn']}/publish")).json()
+    meta_score_set = create_seq_score_set_with_variants(
         client,
+        session,
+        data_provider,
         None,
         data_files / "scores.csv",
         update={"title": "Test Meta Analysis", "metaAnalyzesScoreSetUrns": [score_set["urn"]]},
     )
-    score_set_refresh = client.get(f"/api/v1/score-sets/{score_set['urn']}").json()
+
+    score_set_refresh = (client.get(f"/api/v1/score-sets/{score_set['urn']}")).json()
     assert meta_score_set["metaAnalyzesScoreSetUrns"] == [score_set["urn"]]
     assert score_set_refresh["metaAnalyzedByScoreSetUrns"] == [meta_score_set["urn"]]
     assert isinstance(MAVEDB_TMP_URN_RE.fullmatch(meta_score_set["urn"]), re.Match)
 
 
-def test_publish_single_score_set_meta_analysis(client, setup_router_db, data_files):
+def test_publish_single_score_set_meta_analysis(session, data_provider, client, setup_router_db, data_files):
     experiment = create_experiment(client)
-    score_set = create_score_set_with_variants(client, experiment["urn"], data_files / "scores.csv")
-    score_set = client.post(f"/api/v1/score-sets/{score_set['urn']}/publish").json()
-    meta_score_set = create_score_set_with_variants(
+    score_set = create_seq_score_set_with_variants(
+        client, session, data_provider, experiment["urn"], data_files / "scores.csv"
+    )
+
+    score_set = (client.post(f"/api/v1/score-sets/{score_set['urn']}/publish")).json()
+    meta_score_set = create_seq_score_set_with_variants(
         client,
+        session,
+        data_provider,
         None,
         data_files / "scores.csv",
         update={"title": "Test Meta Analysis", "metaAnalyzesScoreSetUrns": [score_set["urn"]]},
     )
-    meta_score_set = client.post(f"/api/v1/score-sets/{meta_score_set['urn']}/publish").json()
-    assert meta_score_set["urn"] == f"urn:mavedb:00000001-0-1"
+
+    meta_score_set = (client.post(f"/api/v1/score-sets/{meta_score_set['urn']}/publish")).json()
+    assert meta_score_set["urn"] == "urn:mavedb:00000001-0-1"
 
 
-def test_multiple_score_set_meta_analysis_single_experiment(client, setup_router_db, data_files):
+def test_multiple_score_set_meta_analysis_single_experiment(
+    session, data_provider, client, setup_router_db, data_files
+):
     experiment = create_experiment(client)
-    score_set_1 = create_score_set_with_variants(
-        client, experiment["urn"], data_files / "scores.csv", update={"title": "Score Set 1"}
+    score_set_1 = create_seq_score_set_with_variants(
+        client, session, data_provider, experiment["urn"], data_files / "scores.csv", update={"title": "Score Set 1"}
     )
-    score_set_2 = create_score_set_with_variants(
-        client, experiment["urn"], data_files / "scores.csv", update={"title": "Score Set 2"}
+    score_set_2 = create_seq_score_set_with_variants(
+        client, session, data_provider, experiment["urn"], data_files / "scores.csv", update={"title": "Score Set 2"}
     )
-    score_set_1 = client.post(f"/api/v1/score-sets/{score_set_1['urn']}/publish").json()
-    score_set_2 = client.post(f"/api/v1/score-sets/{score_set_2['urn']}/publish").json()
-    meta_score_set = create_score_set_with_variants(
+
+    score_set_1 = (client.post(f"/api/v1/score-sets/{score_set_1['urn']}/publish")).json()
+    score_set_2 = (client.post(f"/api/v1/score-sets/{score_set_2['urn']}/publish")).json()
+
+    meta_score_set = create_seq_score_set_with_variants(
         client,
+        session,
+        data_provider,
         None,
         data_files / "scores.csv",
         update={"title": "Test Meta Analysis", "metaAnalyzesScoreSetUrns": [score_set_1["urn"], score_set_2["urn"]]},
     )
-    score_set_1_refresh = client.get(f"/api/v1/score-sets/{score_set_1['urn']}").json()
+    score_set_1_refresh = (client.get(f"/api/v1/score-sets/{score_set_1['urn']}")).json()
     assert meta_score_set["metaAnalyzesScoreSetUrns"] == sorted([score_set_1["urn"], score_set_2["urn"]])
     assert score_set_1_refresh["metaAnalyzedByScoreSetUrns"] == [meta_score_set["urn"]]
-    meta_score_set = client.post(f"/api/v1/score-sets/{meta_score_set['urn']}/publish").json()
-    assert meta_score_set["urn"] == f"urn:mavedb:00000001-0-1"
+
+    meta_score_set = (client.post(f"/api/v1/score-sets/{meta_score_set['urn']}/publish")).json()
+    assert meta_score_set["urn"] == "urn:mavedb:00000001-0-1"
 
 
-def test_multiple_score_set_meta_analysis_multiple_experiment_sets(client, setup_router_db, data_files):
+def test_multiple_score_set_meta_analysis_multiple_experiment_sets(
+    session, data_provider, client, setup_router_db, data_files
+):
     experiment_1 = create_experiment(client, {"title": "Experiment 1"})
     experiment_2 = create_experiment(client, {"title": "Experiment 2"})
-    score_set_1 = create_score_set_with_variants(
-        client, experiment_1["urn"], data_files / "scores.csv", update={"title": "Score Set 1"}
+    score_set_1 = create_seq_score_set_with_variants(
+        client, session, data_provider, experiment_1["urn"], data_files / "scores.csv", update={"title": "Score Set 1"}
     )
-    score_set_2 = create_score_set_with_variants(
-        client, experiment_2["urn"], data_files / "scores.csv", update={"title": "Score Set 2"}
+    score_set_2 = create_seq_score_set_with_variants(
+        client, session, data_provider, experiment_2["urn"], data_files / "scores.csv", update={"title": "Score Set 2"}
     )
-    score_set_1 = client.post(f"/api/v1/score-sets/{score_set_1['urn']}/publish").json()
-    score_set_2 = client.post(f"/api/v1/score-sets/{score_set_2['urn']}/publish").json()
-    meta_score_set = create_score_set_with_variants(
+
+    score_set_1 = (client.post(f"/api/v1/score-sets/{score_set_1['urn']}/publish")).json()
+    score_set_2 = (client.post(f"/api/v1/score-sets/{score_set_2['urn']}/publish")).json()
+
+    meta_score_set = create_seq_score_set_with_variants(
         client,
+        session,
+        data_provider,
         None,
         data_files / "scores.csv",
         update={"title": "Test Meta Analysis", "metaAnalyzesScoreSetUrns": [score_set_1["urn"], score_set_2["urn"]]},
     )
-    score_set_1_refresh = client.get(f"/api/v1/score-sets/{score_set_1['urn']}").json()
+    score_set_1_refresh = (client.get(f"/api/v1/score-sets/{score_set_1['urn']}")).json()
     assert meta_score_set["metaAnalyzesScoreSetUrns"] == sorted([score_set_1["urn"], score_set_2["urn"]])
     assert score_set_1_refresh["metaAnalyzedByScoreSetUrns"] == [meta_score_set["urn"]]
-    meta_score_set = client.post(f"/api/v1/score-sets/{meta_score_set['urn']}/publish").json()
-    assert meta_score_set["urn"] == f"urn:mavedb:00000003-0-1"
+
+    meta_score_set = (client.post(f"/api/v1/score-sets/{meta_score_set['urn']}/publish")).json()
+    assert meta_score_set["urn"] == "urn:mavedb:00000003-0-1"
 
 
-def test_multiple_score_set_meta_analysis_multiple_experiments(client, setup_router_db, data_files):
+def test_multiple_score_set_meta_analysis_multiple_experiments(
+    session, data_provider, client, setup_router_db, data_files
+):
     experiment_1 = create_experiment(client, {"title": "Experiment 1"})
     experiment_2 = create_experiment(
         client, {"title": "Experiment 2", "experimentSetUrn": experiment_1["experimentSetUrn"]}
     )
-    score_set_1 = create_score_set_with_variants(
-        client, experiment_1["urn"], data_files / "scores.csv", update={"title": "Score Set 1"}
+    score_set_1 = create_seq_score_set_with_variants(
+        client, session, data_provider, experiment_1["urn"], data_files / "scores.csv", update={"title": "Score Set 1"}
     )
-    score_set_2 = create_score_set_with_variants(
-        client, experiment_2["urn"], data_files / "scores.csv", update={"title": "Score Set 2"}
+    score_set_2 = create_seq_score_set_with_variants(
+        client, session, data_provider, experiment_2["urn"], data_files / "scores.csv", update={"title": "Score Set 2"}
     )
-    score_set_1 = client.post(f"/api/v1/score-sets/{score_set_1['urn']}/publish").json()
-    score_set_2 = client.post(f"/api/v1/score-sets/{score_set_2['urn']}/publish").json()
-    meta_score_set = create_score_set_with_variants(
+
+    score_set_1 = (client.post(f"/api/v1/score-sets/{score_set_1['urn']}/publish")).json()
+    score_set_2 = (client.post(f"/api/v1/score-sets/{score_set_2['urn']}/publish")).json()
+
+    meta_score_set = create_seq_score_set_with_variants(
         client,
+        session,
+        data_provider,
         None,
         data_files / "scores.csv",
         update={"title": "Test Meta Analysis", "metaAnalyzesScoreSetUrns": [score_set_1["urn"], score_set_2["urn"]]},
     )
-    score_set_1_refresh = client.get(f"/api/v1/score-sets/{score_set_1['urn']}").json()
+    score_set_1_refresh = (client.get(f"/api/v1/score-sets/{score_set_1['urn']}")).json()
     assert meta_score_set["metaAnalyzesScoreSetUrns"] == sorted([score_set_1["urn"], score_set_2["urn"]])
     assert score_set_1_refresh["metaAnalyzedByScoreSetUrns"] == [meta_score_set["urn"]]
-    meta_score_set = client.post(f"/api/v1/score-sets/{meta_score_set['urn']}/publish").json()
-    assert meta_score_set["urn"] == f"urn:mavedb:00000001-0-1"
+
+    meta_score_set = (client.post(f"/api/v1/score-sets/{meta_score_set['urn']}/publish")).json()
+    assert meta_score_set["urn"] == "urn:mavedb:00000001-0-1"
 
 
 def test_multiple_score_set_meta_analysis_multiple_experiment_sets_different_score_sets(
-    client, setup_router_db, data_files
+    session, data_provider, client, setup_router_db, data_files
 ):
     experiment_1 = create_experiment(client, {"title": "Experiment 1"})
     experiment_2 = create_experiment(client, {"title": "Experiment 2"})
-    score_set_1_1 = create_score_set_with_variants(
-        client, experiment_1["urn"], data_files / "scores.csv", update={"title": "Exp 1 Score Set 1"}
+    score_set_1_1 = create_seq_score_set_with_variants(
+        client,
+        session,
+        data_provider,
+        experiment_1["urn"],
+        data_files / "scores.csv",
+        update={"title": "Exp 1 Score Set 1"},
     )
-    score_set_1_2 = create_score_set_with_variants(
-        client, experiment_1["urn"], data_files / "scores.csv", update={"title": "Exp 1 Score Set 2"}
+    score_set_1_2 = create_seq_score_set_with_variants(
+        client,
+        session,
+        data_provider,
+        experiment_1["urn"],
+        data_files / "scores.csv",
+        update={"title": "Exp 1 Score Set 2"},
+    )
+    score_set_2_1 = create_seq_score_set_with_variants(
+        client,
+        session,
+        data_provider,
+        experiment_2["urn"],
+        data_files / "scores.csv",
+        update={"title": "Exp 2 Score Set 1"},
     )
-    score_set_2_1 = create_score_set_with_variants(
-        client, experiment_2["urn"], data_files / "scores.csv", update={"title": "Exp 2 Score Set 1"}
+    score_set_2_2 = create_seq_score_set_with_variants(
+        client,
+        session,
+        data_provider,
+        experiment_2["urn"],
+        data_files / "scores.csv",
+        update={"title": "Exp 2 Score Set 2"},
     )
-    score_set_2_2 = create_score_set_with_variants(
-        client, experiment_2["urn"], data_files / "scores.csv", update={"title": "Exp 2 Score Set 2"}
-    )
-    score_set_1_1 = client.post(f"/api/v1/score-sets/{score_set_1_1['urn']}/publish").json()
-    score_set_1_2 = client.post(f"/api/v1/score-sets/{score_set_1_2['urn']}/publish").json()
-    score_set_2_1 = client.post(f"/api/v1/score-sets/{score_set_2_1['urn']}/publish").json()
-    score_set_2_2 = client.post(f"/api/v1/score-sets/{score_set_2_2['urn']}/publish").json()
-    meta_score_set_1 = create_score_set_with_variants(
+
+    score_set_1_1 = (client.post(f"/api/v1/score-sets/{score_set_1_1['urn']}/publish")).json()
+    score_set_1_2 = (client.post(f"/api/v1/score-sets/{score_set_1_2['urn']}/publish")).json()
+    score_set_2_1 = (client.post(f"/api/v1/score-sets/{score_set_2_1['urn']}/publish")).json()
+    score_set_2_2 = (client.post(f"/api/v1/score-sets/{score_set_2_2['urn']}/publish")).json()
+    meta_score_set_1 = create_seq_score_set_with_variants(
         client,
+        session,
+        data_provider,
         None,
         data_files / "scores.csv",
         update={
             "title": "Test Meta Analysis 1-1 2-1",
             "metaAnalyzesScoreSetUrns": [score_set_1_1["urn"], score_set_2_1["urn"]],
         },
     )
-    score_set_1_1_refresh = client.get(f"/api/v1/score-sets/{score_set_1_1['urn']}").json()
+    score_set_1_1_refresh = (client.get(f"/api/v1/score-sets/{score_set_1_1['urn']}")).json()
     assert meta_score_set_1["metaAnalyzesScoreSetUrns"] == sorted([score_set_1_1["urn"], score_set_2_1["urn"]])
     assert score_set_1_1_refresh["metaAnalyzedByScoreSetUrns"] == [meta_score_set_1["urn"]]
-    meta_score_set_1 = client.post(f"/api/v1/score-sets/{meta_score_set_1['urn']}/publish").json()
-    assert meta_score_set_1["urn"] == f"urn:mavedb:00000003-0-1"
-    meta_score_set_2 = create_score_set_with_variants(
+    meta_score_set_2 = create_seq_score_set_with_variants(
         client,
+        session,
+        data_provider,
         None,
         data_files / "scores.csv",
         update={
             "title": "Test Meta Analysis 1-2 2-2",
             "metaAnalyzesScoreSetUrns": [score_set_1_2["urn"], score_set_2_2["urn"]],
         },
     )
-    meta_score_set_2 = client.post(f"/api/v1/score-sets/{meta_score_set_2['urn']}/publish").json()
-    assert meta_score_set_2["urn"] == f"urn:mavedb:00000003-0-2"
-    meta_score_set_3 = create_score_set_with_variants(
+
+    meta_score_set_3 = create_seq_score_set_with_variants(
         client,
+        session,
+        data_provider,
         None,
         data_files / "scores.csv",
         update={
             "title": "Test Meta Analysis 1-1 2-2",
             "metaAnalyzesScoreSetUrns": [score_set_1_1["urn"], score_set_2_2["urn"]],
         },
     )
-    meta_score_set_3 = client.post(f"/api/v1/score-sets/{meta_score_set_3['urn']}/publish").json()
-    assert meta_score_set_3["urn"] == f"urn:mavedb:00000003-0-3"
+
+    meta_score_set_1 = (client.post(f"/api/v1/score-sets/{meta_score_set_1['urn']}/publish")).json()
+    assert meta_score_set_1["urn"] == "urn:mavedb:00000003-0-1"
+    meta_score_set_2 = (client.post(f"/api/v1/score-sets/{meta_score_set_2['urn']}/publish")).json()
+    assert meta_score_set_2["urn"] == "urn:mavedb:00000003-0-2"
+    meta_score_set_3 = (client.post(f"/api/v1/score-sets/{meta_score_set_3['urn']}/publish")).json()
+    assert meta_score_set_3["urn"] == "urn:mavedb:00000003-0-3"
+
+
+def test_search_core_sets_no_match(session, data_provider, client, setup_router_db, data_files):
+    experiment_1 = create_experiment(client, {"title": "Experiment 1"})
+    create_seq_score_set_with_variants(
+        client,
+        session,
+        data_provider,
+        experiment_1["urn"],
+        data_files / "scores.csv",
+        update={"title": "Test Score Set"},
+    )
+
+    search_payload = {"text": "fnord"}
+    response = client.post("/api/v1/score-sets/search", json=search_payload)
+    assert response.status_code == 200
+    assert len(response.json()) == 0
+
+
+def test_search_core_sets_match(session, data_provider, client, setup_router_db, data_files):
+    experiment_1 = create_experiment(client, {"title": "Experiment 1"})
+    score_set_1_1 = create_seq_score_set_with_variants(
+        client,
+        session,
+        data_provider,
+        experiment_1["urn"],
+        data_files / "scores.csv",
+        update={"title": "Test Fnord Score Set"},
+    )
+
+    search_payload = {"text": "fnord"}
+    response = client.post("/api/v1/score-sets/search", json=search_payload)
+    assert response.status_code == 200
+    assert len(response.json()) == 1
+    assert response.json()[0]["title"] == score_set_1_1["title"]
```

### Comparing `mavedb-2023.3.0/tests/validation/test_identifier.py` & `mavedb-2024.0.0/tests/validation/test_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/validation/test_keywords.py` & `mavedb-2024.0.0/tests/validation/test_keywords.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/validation/test_publication.py` & `mavedb-2024.0.0/tests/validation/test_publication.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/validation/test_target.py` & `mavedb-2024.0.0/tests/validation/test_target.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/validation/test_urn_re.py` & `mavedb-2024.0.0/tests/validation/test_urn_re.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/validation/test_utilities.py` & `mavedb-2024.0.0/tests/validation/test_utilities.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/validation/test_variant.py` & `mavedb-2024.0.0/tests/validation/test_variant.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/view_models/test_external_gene_identifiers.py` & `mavedb-2024.0.0/tests/view_models/test_external_gene_identifiers.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/tests/view_models/test_publication_identifier.py` & `mavedb-2024.0.0/tests/view_models/test_publication_identifier.py`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/.gitignore` & `mavedb-2024.0.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -90,25 +90,22 @@
 #   having no cross-platform support, pipenv may install dependencies that don't work, or not
 #   install all needed dependencies.
 #Pipfile.lock
 
 # PEP 582; used by e.g. github.com/David-OConnor/pyflow
 __pypackages__/
 
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
 # SageMath parsed files
 *.sage.py
 
 # Environments
 .env
 .env.*
 !.env.template
+!.env.dev
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
```

### Comparing `mavedb-2023.3.0/LICENSE` & `mavedb-2024.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mavedb-2023.3.0/README.md` & `mavedb-2024.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # mavedb-api
 
-API for MaveDB, the database of the database of Multiplexed Assays of Variant Effect
+API for MaveDB. MaveDB is a biological database for Multiplex Assays of Variant Effect (MAVE) datasets.
+The API powers the MaveDB website at [mavedb.org](https://www.mavedb.org) and can also be called separately (see
+instructions [below](#using-mavedb-api)).
+
+
+For more information about MaveDB or to cite MaveDB please refer to the
+[MaveDB paper in Genome Biology](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1845-6).
 
 ## Using mavedb-api
 
 ### Using the library as an API client or validator for MaveDB data sets
 
 Simply install the package using PIP:
 
@@ -34,64 +40,53 @@
 The build utility will look at `pyproject.toml` and invoke Hatchling to build the distributions.
 
 The distribution can be uploaded to PyPI using [twine](https://twine.readthedocs.io/en/stable/).
 
 For use as a server, this distribution includes an optional set of dependencies, which are only invoked if the package
 is installed with `pip install mavedb[server]`.
 
-### Running the API server in Docker on production and test systems
+### Running a local version of the API server
 
 First build the application's Docker image:
 ```
 docker build --tag mavedb-api/mavedb-api .
 ```
 Then start the application and its database:
 ```
-docker-compose -f docker-compose-prod.yml up -d
+docker-compose -f docker-compose-local.yml up -d
 ```
 Omit `-d` (daemon) if you want to run the application in your terminal session, for instance to see startup errors without having
 to inspect the Docker container's log.
 
 To stop the application when it is running as a daemon, run
 ```
-docker-compose -f docker-compose-prod.yml down
+docker-compose -f docker-compose-local.yml down
 ```
 
-`docker-compose-prod.yml` configures two containers: one for the API server and one for the PostgreSQL database. The
-The database stores data in a Docker volume named `mavedb-data`, which will persist after running `docker-compose down`.
+`docker-compose-local.yml` configures four containers: one for the API server, one for the PostgreSQL database, one for the
+worker node and one for the Redis cache which acts as the job queue for the worker node. The worker node stores data in a Docker
+volume named `mavedb-redis` and the database stores data in a Docker volume named `mavedb-data`. Both these volumes will persist
+after running `docker-compose down`.
 
 **Notes**
 1. The `mavedb-api` container requires the following environment variables, which are configured in
-  `docker-compose-prod.yml`:
+  `docker-compose-local.yml`:
 
     - DB_HOST
     - DB_PORT
     - DB_DATABASE_NAME
     - DB_USERNAME
     - DB_PASSWORD
     - NCBI_API_KEY
+    - REDIS_IP
+    - REDIS_PORT
 
     The database username and password should be edited for production deployments. `NCBI_API_KEY` will be removed in
     the future. **TODO** Move these to an .env file.
 
-2. In the procedure given above, we do not push the Docker image to a repository like Docker Hub; we simply build the
-  image on the machine where it will be used. But to deploy the API server on the AWS-hosted test site, first tag the
-  image appropriately and push it to Elastic Container Repository. (These commands require )
-  ```
-  export ECRPASSWORD=$(aws ecr get-login-password --region us-west-2 --profile mavedb-test)
-  echo $ECRPASSWORD | docker login --username AWS --password-stdin {aws_account_id}.dkr.ecr.us-west-2.amazonaws.com
-  docker tag mavedb-api:latest {aws_account_id}.dkr.ecr.us-west-2.amazonaws.com/mavedb-api
-  docker push {aws_account_id}.dkr.ecr.us-west-2.amazonaws.com/mavedb-api
-  ```
-  These commands presuppose that you have the [AWS CLI](https://aws.amazon.com/cli/) installed and have created a named
-  profile, `mavedb-test`, with your AWS credentials.
-
-  With the Docker image pushed to ECR, you can now deploy the application. **TODO** Add instructions if we want to
-  document this.
-
 ### Running the API server in Docker for development
 
 A similar procedure can be followed to run the API server in development mode on your local machine. There are a couple
 of differences:
 
 - Your local source code directory is mounted to the Docker container, instead of copying it into the container.
 - The Uvicorn web server is started with a `--reload` option, so that code changes will cause the application to be
@@ -99,15 +94,15 @@
 - The API uses HTTP, whereas in production it uses encrypted communication via HTTPS.
 
 To start the Docker container for development, make sure that the mavedb-api directory is allowed to be shared with
 Docker.  In Docker Desktop, this can be configured under Settings > Resources > File sharing.
 
 To start the application, run
 ```
-docker-compose -f docker-compose-dev.yml up -d
+docker-compose -f docker-compose-dev.yml up --build -d
 ```
 
 Docker integration can also be configured in IDEs like PyCharm.
 
 ### Running the API server directly for development
 
 Sometimes you may want to run the API server outside of Docker. There are two ways to do this:
@@ -124,7 +119,14 @@
   ```
   export PYTHONPATH=${PYTHONPATH}:"`pwd`/src"
   uvicorn mavedb.server_main:app --reload
   ```
 
 If you use PyCharm, the first method can be used in a Python run configuration, but the second method supports PyCharm's
 FastAPI run configuration.
+
+### Running the API server for production
+
+We maintain deployment configuration options and steps within a [private repository](https://github.com/VariantEffect/mavedb-deployment) used for deploying this source code to
+the production MaveDB environment. The main difference between the production setup and these local setups is that
+the worker and api services are split into distinct environments, allowing them to scale up or down individually
+dependent on need.
```

### Comparing `mavedb-2023.3.0/pyproject.toml` & `mavedb-2024.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -14,47 +14,62 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 dependencies = [
-    "fqfa~=1.2.3",
+    "fqfa~=1.3.0",
     "pyhumps~=3.8.0",
     "IDUtils~=1.2.0",
     "mavehgvs~=0.6.0",
     "eutils~=0.6.0",
-    "numpy~=1.22.3",
+    "hgvs~=1.5.4",
+    "biocommons~=0.0.0",
+    "cdot~=0.2.21",
+    "httpx~=0.26.0",
+    "numpy~=1.22",
     "pandas~=1.4.1",
-    "pydantic~=1.9.1",
+    "pydantic~=1.10",
     "python-dotenv~=0.20.0",
-    "SQLAlchemy~=1.4.31",
+    "SQLAlchemy~=2.0.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black",
     "flake8",
+    "mypy",
     "pre-commit",
     "pytest~=7.0.1",
+    "pytest-postgresql~=5.0.0",
+    "pytest-asyncio==0.23.5",
+    "redis==5.0.2",
+    "fakeredis==2.21.1",
     "jsonschema",
+    "SQLAlchemy[mypy]~=2.0.0",
+    "requests-mock~=1.11.0",
+    "pytest-socket~=0.6.0",
+    "pandas-stubs~=2.1.4",
+    "types-requests~=2.31.0",
+    "types-python-jose~=3.3.4",
 ]
 server = [
     "alembic~=1.7.6",
+    "arq~=0.25.0",
     "authlib~=0.15.5",
-    "cryptography~=37.0.4",
-    "celery~=5.2.3",
-    "fastapi~=0.71.0",
+    "cryptography~=41.0.6",
+    "fastapi~=0.95.0",
     "orcid~=1.0.3",
     "psycopg2~=2.9.3",
     "python-jose[cryptography]~=3.3.0",
     "python-multipart~=0.0.5",
-    "requests~=2.28.1",
+    "requests~=2.31.0",
     "slack-sdk~=3.21.3",
-    "starlette~=0.17.1",
+    "starlette~=0.27.0",
     "uvicorn[standard]",
 ]
 
 [project.urls]
 repository = "https://github.com/VariantEffect/mavedb-api"
 documentation = "https://mavedb.org/docs/mavedb/"
 
@@ -74,15 +89,22 @@
     "docker-compose-prod.yml",
     "docs/",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/mavedb"]
 
-[tool.pytest.ini_options]
-addopts = [
-    "--import-mode=importlib",
+[tool.mypy]
+plugins = [
+    "sqlalchemy.ext.mypy.plugin",
+    "numpy.typing.mypy_plugin",
 ]
-norecursedirs = "tests/helpers"
+mypy_path = "mypy_stubs"
+
+[tool.pytest.ini_options]
+addopts = "-v -rP --import-mode=importlib --disable-socket --allow-hosts localhost,::1,127.0.0.1"
+asyncio_mode = 'strict'
+testpaths = "tests/"
+norecursedirs = "tests/helpers/"
 # Uncomment the following lines to include application log output in Pytest logs.
 # log_cli = true
 # log_cli_level = "DEBUG"
```

