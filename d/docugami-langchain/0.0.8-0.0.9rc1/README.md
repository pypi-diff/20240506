# Comparing `tmp/docugami_langchain-0.0.8.tar.gz` & `tmp/docugami_langchain-0.0.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugami_langchain-0.0.8.tar", max compression
+gzip compressed data, was "docugami_langchain-0.0.9rc1.tar", max compression
```

## Comparing `docugami_langchain-0.0.8.tar` & `docugami_langchain-0.0.9rc1.tar`

### file list

```diff
@@ -1,62 +1,64 @@
--rw-r--r--   0        0        0     1072 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/LICENSE
--rw-r--r--   0        0        0      361 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/README.md
--rw-r--r--   0        0        0      747 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/docugami_langchain/__init__.py
--rw-r--r--   0        0        0      487 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/docugami_langchain/agents/__init__.py
--rw-r--r--   0        0        0     8192 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/docugami_langchain/agents/base.py
--rw-r--r--   0        0        0     1760 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/docugami_langchain/agents/models.py
--rw-r--r--   0        0        0    10775 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/docugami_langchain/agents/re_act_agent.py
--rw-r--r--   0        0        0     8325 2024-05-04 06:11:45.826604 docugami_langchain-0.0.8/docugami_langchain/agents/tool_router_agent.py
--rw-r--r--   0        0        0    16628 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/base_runnable.py
--rw-r--r--   0        0        0     1396 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/__init__.py
--rw-r--r--   0        0        0     2210 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/answer_chain.py
--rw-r--r--   0        0        0     1415 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/base.py
--rw-r--r--   0        0        0      243 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/chunks/__init__.py
--rw-r--r--   0        0        0     3390 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
--rw-r--r--   0        0        0     3980 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/chunks/summarize_chunk_chain.py
--rw-r--r--   0        0        0      291 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/documents/__init__.py
--rw-r--r--   0        0        0     3838 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/documents/describe_document_set_chain.py
--rw-r--r--   0        0        0     3983 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/documents/summarize_document_chain.py
--rw-r--r--   0        0        0      647 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/querying/__init__.py
--rw-r--r--   0        0        0     2909 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
--rw-r--r--   0        0        0     3999 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_fixup_chain.py
--rw-r--r--   0        0        0     4360 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_query_explainer_chain.py
--rw-r--r--   0        0        0     8665 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_result_chain.py
--rw-r--r--   0        0        0     3522 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_result_explainer_chain.py
--rw-r--r--   0        0        0      498 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/rag/__init__.py
--rw-r--r--   0        0        0     3297 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/rag/simple_rag_chain.py
--rw-r--r--   0        0        0     4006 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/rag/standalone_question_chain.py
--rw-r--r--   0        0        0     4592 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/rag/suggested_questions_chain.py
--rw-r--r--   0        0        0     4193 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/rag/suggested_report_chain.py
--rw-r--r--   0        0        0     4832 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/rag/tool_final_answer_chain.py
--rw-r--r--   0        0        0      567 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/types/__init__.py
--rw-r--r--   0        0        0      999 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/types/common.py
--rw-r--r--   0        0        0     3147 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/types/data_type_detection_chain.py
--rw-r--r--   0        0        0     3243 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/types/date_add_chain.py
--rw-r--r--   0        0        0     2963 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/types/date_parse_chain.py
--rw-r--r--   0        0        0     2464 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/chains/types/timespan_parse_chain.py
--rw-r--r--   0        0        0     1515 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/config.py
--rw-r--r--   0        0        0      109 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/document_loaders/__init__.py
--rw-r--r--   0        0        0    13516 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/document_loaders/docugami.py
--rw-r--r--   0        0        0     2798 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/history.py
--rw-r--r--   0        0        0      797 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/__init__.py
--rw-r--r--   0        0        0     4206 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/custom_react_json_single_input.py
--rw-r--r--   0        0        0     2091 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/datetime.py
--rw-r--r--   0        0        0     1075 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/key_finding.py
--rw-r--r--   0        0        0     1242 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/line_separated_list.py
--rw-r--r--   0        0        0     2816 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/sql_finding.py
--rw-r--r--   0        0        0      735 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/text_cleaning.py
--rw-r--r--   0        0        0     4502 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/output_parsers/timespan.py
--rw-r--r--   0        0        0      833 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/params.py
--rw-r--r--   0        0        0      122 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/py.typed
--rw-r--r--   0        0        0      165 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/retrievers/__init__.py
--rw-r--r--   0        0        0     7829 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/retrievers/fused_summary.py
--rw-r--r--   0        0        0     5472 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/retrievers/mappings.py
--rw-r--r--   0        0        0      194 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/tools/__init__.py
--rw-r--r--   0        0        0     3657 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/tools/common.py
--rw-r--r--   0        0        0     7105 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/tools/reports.py
--rw-r--r--   0        0        0     6268 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/tools/retrieval.py
--rw-r--r--   0        0        0      708 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/utils/documents.py
--rw-r--r--   0        0        0     8975 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/utils/sql.py
--rw-r--r--   0        0        0     3389 2024-05-04 06:11:45.830605 docugami_langchain-0.0.8/docugami_langchain/utils/string_cleanup.py
--rw-r--r--   0        0        0     2826 2024-05-04 06:11:45.834605 docugami_langchain-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 docugami_langchain-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/LICENSE
+-rw-r--r--   0        0        0      361 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/README.md
+-rw-r--r--   0        0        0      747 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/agents/__init__.py
+-rw-r--r--   0        0        0     8459 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/agents/base.py
+-rw-r--r--   0        0        0     1805 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/agents/models.py
+-rw-r--r--   0        0        0    10928 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/agents/re_act_agent.py
+-rw-r--r--   0        0        0     8325 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/agents/tool_router_agent.py
+-rw-r--r--   0        0        0    16628 2024-05-06 21:38:16.563129 docugami_langchain-0.0.9rc1/docugami_langchain/base_runnable.py
+-rw-r--r--   0        0        0     1396 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/__init__.py
+-rw-r--r--   0        0        0     2210 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/answer_chain.py
+-rw-r--r--   0        0        0     1415 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/base.py
+-rw-r--r--   0        0        0      243 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/chunks/__init__.py
+-rw-r--r--   0        0        0     3390 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/chunks/elaborate_chunk_chain.py
+-rw-r--r--   0        0        0     3980 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/chunks/summarize_chunk_chain.py
+-rw-r--r--   0        0        0      291 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/documents/__init__.py
+-rw-r--r--   0        0        0     3838 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/documents/describe_document_set_chain.py
+-rw-r--r--   0        0        0     3983 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/documents/summarize_document_chain.py
+-rw-r--r--   0        0        0      647 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/__init__.py
+-rw-r--r--   0        0        0     3398 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py
+-rw-r--r--   0        0        0      262 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/models.py
+-rw-r--r--   0        0        0     3999 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_fixup_chain.py
+-rw-r--r--   0        0        0     4360 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_query_explainer_chain.py
+-rw-r--r--   0        0        0     8808 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_result_chain.py
+-rw-r--r--   0        0        0     3522 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_result_explainer_chain.py
+-rw-r--r--   0        0        0      498 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/__init__.py
+-rw-r--r--   0        0        0      124 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/models.py
+-rw-r--r--   0        0        0     4409 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/simple_rag_chain.py
+-rw-r--r--   0        0        0     4006 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/standalone_question_chain.py
+-rw-r--r--   0        0        0     4592 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/suggested_questions_chain.py
+-rw-r--r--   0        0        0     4193 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/suggested_report_chain.py
+-rw-r--r--   0        0        0     4832 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/tool_final_answer_chain.py
+-rw-r--r--   0        0        0      567 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/common.py
+-rw-r--r--   0        0        0     3147 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/data_type_detection_chain.py
+-rw-r--r--   0        0        0     3243 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/date_add_chain.py
+-rw-r--r--   0        0        0     2963 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/date_parse_chain.py
+-rw-r--r--   0        0        0     2464 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/timespan_parse_chain.py
+-rw-r--r--   0        0        0     1515 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/config.py
+-rw-r--r--   0        0        0      109 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/document_loaders/__init__.py
+-rw-r--r--   0        0        0    13516 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/document_loaders/docugami.py
+-rw-r--r--   0        0        0     2798 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/history.py
+-rw-r--r--   0        0        0      797 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     4206 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/custom_react_json_single_input.py
+-rw-r--r--   0        0        0     2091 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/datetime.py
+-rw-r--r--   0        0        0     1075 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/key_finding.py
+-rw-r--r--   0        0        0     1242 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/line_separated_list.py
+-rw-r--r--   0        0        0     2816 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/sql_finding.py
+-rw-r--r--   0        0        0      735 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/text_cleaning.py
+-rw-r--r--   0        0        0     4502 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/timespan.py
+-rw-r--r--   0        0        0      833 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/params.py
+-rw-r--r--   0        0        0      122 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/py.typed
+-rw-r--r--   0        0        0      165 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/retrievers/__init__.py
+-rw-r--r--   0        0        0     7894 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/retrievers/fused_summary.py
+-rw-r--r--   0        0        0     5472 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/retrievers/mappings.py
+-rw-r--r--   0        0        0      194 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/tools/__init__.py
+-rw-r--r--   0        0        0     3958 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/tools/common.py
+-rw-r--r--   0        0        0     8697 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/tools/reports.py
+-rw-r--r--   0        0        0     6830 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/tools/retrieval.py
+-rw-r--r--   0        0        0      708 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/utils/documents.py
+-rw-r--r--   0        0        0     8975 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/utils/sql.py
+-rw-r--r--   0        0        0     3389 2024-05-06 21:38:16.567129 docugami_langchain-0.0.9rc1/docugami_langchain/utils/string_cleanup.py
+-rw-r--r--   0        0        0     2829 2024-05-06 21:38:16.571129 docugami_langchain-0.0.9rc1/pyproject.toml
+-rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 docugami_langchain-0.0.9rc1/PKG-INFO
```

### Comparing `docugami_langchain-0.0.8/LICENSE` & `docugami_langchain-0.0.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/__init__.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/agents/base.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/agents/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,31 +41,35 @@
         if not inv_model:
             raise Exception(f"No tool invocation in model: {state}")
 
         previous_steps = state.get("intermediate_steps") or []
         if previous_steps and any(
             [s for s in previous_steps if s.invocation == inv_model]
         ):
-            output = (
-                "This tool has been invoked before with identical inputs. Please try different inputs or a different tool, after reconsidering previous thoughts and observations. "
-                + "Be careful you don't get stuck in a loop."
+            tool_output = CitedAnswer(
+                source=inv_model.tool_name,
+                answer="This tool has been invoked before with identical inputs. Please try different inputs or a different tool, after reconsidering previous thoughts and observations. "
+                + "Be careful you don't get stuck in a loop.",
             )
         else:
             tool_executor = ToolExecutor(self.tools)
-            output = tool_executor.invoke(
+            tool_output = tool_executor.invoke(
                 ToolInvocation(  # LangChain version of the Invocation object
                     tool=inv_model.tool_name,
                     tool_input=inv_model.tool_input,
                 ),
                 config,
             )
+            if not isinstance(tool_output, CitedAnswer):
+                raise Exception(f"Invalid output from tool executor: {tool_output}")
 
         step = StepState(
             invocation=inv_model,
-            output=str(output),
+            output=tool_output.answer,
+            citations=tool_output.citations,
         )
         return {"intermediate_steps": previous_steps + [step]}
 
     def invocation_answer(
         self,
         invocation: Invocation,
         answer_source: str,
```

### Comparing `docugami_langchain-0.0.8/docugami_langchain/agents/models.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/agents/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import Annotated, Sequence, TypedDict, Union
 
 from langchain_core.pydantic_v1 import BaseModel
 
 
 class Citation(BaseModel):
     label: str
-    details: str
-    link: str
+    details: str = ""
+    link: str = ""
 
 
 class CitedAnswer(BaseModel):
     source: str
     answer: str
     citations: list[Citation] = []
     is_final: bool = False
@@ -32,14 +32,15 @@
         # Compare tool_name and tool_input for equality
         return (self.tool_name, self.tool_input) == (other.tool_name, other.tool_input)
 
 
 class StepState(BaseModel):
     output: str
     invocation: Invocation
+    citations: list[Citation] = []
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, StepState):
             return NotImplemented
 
         # Compare invocation and output for equality
         return (self.invocation, self.output) == (other.invocation, other.output)
```

### Comparing `docugami_langchain-0.0.8/docugami_langchain/agents/re_act_agent.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/agents/re_act_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,29 +185,32 @@
 
         def generate_re_act(
             state: AgentState, config: Optional[RunnableConfig]
         ) -> AgentState:
             react_output = agent_runnable.invoke(state, config)
 
             answer_source = ReActAgent.__name__
+            citations = []
             if isinstance(react_output, Invocation):
                 # Agent wants to invoke a tool
                 return self.invocation_answer(react_output, answer_source)
             elif isinstance(react_output, str):
                 # Agent thinks it has a final answer.
 
-                # Source final answer from the last invocation, if any.
-                tool_invocation = state.get("tool_invocation")
-                if tool_invocation and tool_invocation.tool_name:
-                    answer_source = tool_invocation.tool_name
-
+                # Source the answer from the last step, if any
+                intermediate_steps = state.get("intermediate_steps")
+                if intermediate_steps:
+                    last_step = intermediate_steps[-1]
+                    answer_source = last_step.invocation.tool_name
+                    citations = last_step.citations
                 return {
                     "cited_answer": CitedAnswer(
                         source=answer_source,
                         is_final=True,
+                        citations=citations,
                         answer=react_output,  # This is the final answer.
                     ),
                 }
 
             raise Exception(f"Unrecognized agent output: {react_output}")
 
         def should_continue(state: AgentState) -> str:
```

### Comparing `docugami_langchain-0.0.8/docugami_langchain/agents/tool_router_agent.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/agents/tool_router_agent.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/base_runnable.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/base_runnable.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/__init__.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/answer_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/answer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/base.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/base.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/chunks/elaborate_chunk_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/chunks/elaborate_chunk_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/chunks/summarize_chunk_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/chunks/summarize_chunk_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/documents/describe_document_set_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/documents/describe_document_set_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/documents/summarize_document_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/documents/summarize_document_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/querying/__init__.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/docugami_explained_sql_query_chain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,101 @@
 from operator import itemgetter
 from typing import AsyncIterator, Optional
 
-from langchain_core.runnables import Runnable, RunnableConfig, RunnableMap
+from langchain_core.runnables import (
+    Runnable,
+    RunnableConfig,
+    RunnableLambda,
+    RunnableMap,
+)
 
 from docugami_langchain.base_runnable import TracedResponse
 from docugami_langchain.chains.base import BaseDocugamiChain
+from docugami_langchain.chains.querying.models import ExplainedSQLQuestionResult
 from docugami_langchain.chains.querying.sql_query_explainer_chain import (
     SQLQueryExplainerChain,
 )
 from docugami_langchain.chains.querying.sql_result_chain import SQLResultChain
 from docugami_langchain.chains.querying.sql_result_explainer_chain import (
     SQLResultExplainerChain,
 )
 from docugami_langchain.params import RunnableParameters
 
 
-class DocugamiExplainedSQLQueryChain(BaseDocugamiChain[dict]):
+class DocugamiExplainedSQLQueryChain(BaseDocugamiChain[ExplainedSQLQuestionResult]):
     sql_result_chain: SQLResultChain
-    sql_result_explainer_chain: SQLResultExplainerChain
-    sql_query_explainer_chain: Optional[SQLQueryExplainerChain]
+    sql_result_explainer_chain: Optional[SQLResultExplainerChain] = None
+    sql_query_explainer_chain: Optional[SQLQueryExplainerChain] = None
 
     def runnable(self) -> Runnable:
         """
         Custom runnable for this chain.
         """
 
+        def empty_string(inputs: dict) -> str:
+            return ""
+
         return RunnableMap(
             {
                 "question": itemgetter("question"),
                 "results": self.sql_result_chain.runnable()
                 | {
                     "question": itemgetter("question"),
                     "sql_query": itemgetter("sql_query"),
                     "sql_result": itemgetter("sql_result"),
                 }
                 | {
                     "sql_query": itemgetter("sql_query"),
                     "sql_result": itemgetter("sql_result"),
-                    "explained_sql_result": self.sql_result_explainer_chain.runnable(),
+                    "explained_sql_result": (
+                        self.sql_result_explainer_chain.runnable()
+                        if self.sql_result_explainer_chain
+                        else RunnableLambda(empty_string)
+                    ),
                     "explained_sql_query": (
                         self.sql_query_explainer_chain.runnable()
                         if self.sql_query_explainer_chain
-                        else None
+                        else RunnableLambda(empty_string)
                     ),
                 },
             }
         )
 
     def params(self) -> RunnableParameters:
         raise NotImplementedError()
 
     def run(  # type: ignore[override]
         self,
         question: str,
         config: Optional[RunnableConfig] = None,
-    ) -> TracedResponse[dict]:
+    ) -> TracedResponse[ExplainedSQLQuestionResult]:
         if not question:
             raise Exception("Input required: question")
 
         return super().run(
             question=question,
             config=config,
         )
 
     async def run_stream(  # type: ignore[override]
         self,
         question: str,
         config: Optional[RunnableConfig] = None,
-    ) -> AsyncIterator[TracedResponse[dict]]:
+    ) -> AsyncIterator[TracedResponse[ExplainedSQLQuestionResult]]:
         if not question:
             raise Exception("Input required: question")
 
         async for item in super().run_stream(
             question=question,
             config=config,
         ):
             yield item
 
     def run_batch(  # type: ignore[override]
         self,
         inputs: list[str],
         config: Optional[RunnableConfig] = None,
-    ) -> list[dict]:
+    ) -> list[ExplainedSQLQuestionResult]:
         return super().run_batch(
             inputs=[{"question": i} for i in inputs],
             config=config,
         )
```

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_fixup_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_fixup_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_query_explainer_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_query_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_result_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_result_chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 from langchain_community.utilities.sql_database import SQLDatabase
 from langchain_core.example_selectors import MaxMarginalRelevanceExampleSelector
 from langchain_core.runnables import Runnable, RunnableConfig, RunnableLambda
 from sqlglot import ParseError
 
 from docugami_langchain.base_runnable import TracedResponse
 from docugami_langchain.chains.base import BaseDocugamiChain
+from docugami_langchain.chains.querying.models import ExplainedSQLResult
 from docugami_langchain.chains.querying.sql_fixup_chain import SQLFixupChain
 from docugami_langchain.output_parsers.sql_finding import SQLFindingOutputParser
 from docugami_langchain.params import RunnableParameters, RunnableSingleParameter
 from docugami_langchain.utils.sql import (
     check_and_format_query,
     create_example_selector,
     get_table_info_as_create_table,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class SQLResultChain(BaseDocugamiChain[dict]):
+class SQLResultChain(BaseDocugamiChain[ExplainedSQLResult]):
     db: SQLDatabase
     """The underlying SQL database that is queried by this chain."""
 
     sql_fixup_chain: Optional[SQLFixupChain] = None
     """A chain used to fix SQL generated by this chain in case of issues."""
 
     _example_row_selector: Optional[MaxMarginalRelevanceExampleSelector] = None
@@ -53,15 +54,15 @@
             question = inputs.get("question")
             return get_table_info_as_create_table(
                 self.db,
                 question=question,
                 example_selector=self._example_row_selector,
             )
 
-        def run_sql_query(inputs: dict, config: Optional[RunnableConfig]) -> dict:
+        def run_sql_query(inputs: dict, config: Optional[RunnableConfig]) -> ExplainedSQLResult:
             """
             Runs the given SQL query against the database connection for this chain, and returns the result.
             """
 
             question = inputs.get("question")
             sql_query = inputs.get("sql_query")
             table_info = table_info_func({"question": question})
@@ -154,39 +155,39 @@
             stop_sequences=["\n", ";", "<|eot_id|>"],
         )
 
     def run(  # type: ignore[override]
         self,
         question: str,
         config: Optional[RunnableConfig] = None,
-    ) -> TracedResponse[dict]:
+    ) -> TracedResponse[ExplainedSQLResult]:
         if not question:
             raise Exception("Input required: question")
 
         return super().run(
             question=question,
             config=config,
         )
 
     async def run_stream(  # type: ignore[override]
         self,
         question: str,
         config: Optional[RunnableConfig] = None,
-    ) -> AsyncIterator[TracedResponse[dict]]:
+    ) -> AsyncIterator[TracedResponse[ExplainedSQLResult]]:
         if not question:
             raise Exception("Input required: question")
 
         async for item in super().run_stream(
             question=question,
             config=config,
         ):
             yield item
 
     def run_batch(  # type: ignore[override]
         self,
         inputs: list[str],
         config: Optional[RunnableConfig] = None,
-    ) -> list[dict]:
+    ) -> list[ExplainedSQLResult]:
         return super().run_batch(
             inputs=[{"question": i} for i in inputs],
             config=config,
         )
```

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/querying/sql_result_explainer_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/querying/sql_result_explainer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/rag/simple_rag_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/simple_rag_chain.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from operator import itemgetter
 from typing import AsyncIterator, Optional
 
 from langchain_core.documents import Document
-from langchain_core.retrievers import BaseRetriever
-from langchain_core.runnables import Runnable, RunnableConfig
+from langchain_core.runnables import Runnable, RunnableConfig, RunnableLambda
 
 from docugami_langchain.base_runnable import TracedResponse
 from docugami_langchain.chains.base import BaseDocugamiChain
+from docugami_langchain.chains.rag.models import ExtendedRAGResult
 from docugami_langchain.params import RunnableParameters, RunnableSingleParameter
+from docugami_langchain.retrievers.fused_summary import FusedSummaryRetriever
 
 
-class SimpleRAGChain(BaseDocugamiChain[str]):
+class SimpleRAGChain(BaseDocugamiChain[ExtendedRAGResult]):
 
-    retriever: BaseRetriever
+    retriever: FusedSummaryRetriever
 
     def params(self) -> RunnableParameters:
         return RunnableParameters(
             inputs=[
                 RunnableSingleParameter(
                     "context",
                     "CONTEXT",
@@ -27,72 +28,103 @@
                     "QUESTION",
                     "Question asked by the user.",
                 ),
             ],
             output=RunnableSingleParameter(
                 "answer",
                 "ANSWER",
-                "Human readable answer to the question.",
+                "Human readable answer to the question, based on the given context.",
             ),
             task_description="acts as an assistant for question-answering tasks",
             additional_instructions=[
                 "- Use only the given pieces of retrieved context to answer the question, don't make up answers.",
-                "- If you don't know the answer, just say that you don't know.",
+                "- If you cannot find the answer in the given context, just say that you don't know.",
                 "- Your answer should be concise, up to three sentences long.",
             ],
             stop_sequences=["<|eot_id|>"],
             key_finding_output_parse=False,  # set to False for streaming
             include_output_instruction_suffix=True,
         )
 
-    def runnable(self) -> Runnable:
+    def run_rag(
+        self, inputs: dict, config: Optional[RunnableConfig]
+    ) -> ExtendedRAGResult:
         """
-        Custom runnable for this agent.
+        Runs rag for the given question against the given context, and returns the result.
         """
 
         def format_retrieved_docs(docs: list[Document]) -> str:
             return "\n\n".join(doc.page_content for doc in docs)
 
+        def list_retrieved_docs(docs: list[Document]) -> list[str]:
+            return [doc.metadata[self.retriever.source_key] for doc in docs]
+
+        context = inputs.get("context")
+        question = inputs.get("question")
+
+        answer = (
+            super()
+            .runnable()
+            .invoke(
+                {
+                    "context": format_retrieved_docs(context),  # type: ignore
+                    "question": question,
+                },
+                config,
+            )
+        )
+
+        return {
+            "answer": answer,
+            "question": question,
+            "sources": list_retrieved_docs(context),  # type: ignore
+        }
+
+    def runnable(self) -> Runnable:
+        """
+        Custom runnable for this agent.
+        """
+
         return {
-            "context": itemgetter("question") | self.retriever | format_retrieved_docs,
+            "context": itemgetter("question") | self.retriever,
             "question": itemgetter("question"),
-        } | super().runnable()
+        } | RunnableLambda(self.run_rag)
 
     def run(  # type: ignore[override]
         self,
         question: str,
         config: Optional[RunnableConfig] = None,
-    ) -> TracedResponse[str]:
+    ) -> TracedResponse[ExtendedRAGResult]:
         if not question:
             raise Exception("Input required: question")
 
         return super().run(
             question=question,
             config=config,
         )
 
     async def run_stream(  # type: ignore[override]
         self,
         question: str,
         config: Optional[RunnableConfig] = None,
-    ) -> AsyncIterator[TracedResponse[str]]:
+    ) -> AsyncIterator[TracedResponse[ExtendedRAGResult]]:
         if not question:
             raise Exception("Input required: question")
 
         async for item in super().run_stream(
             question=question,
             config=config,
         ):
             yield item
 
     def run_batch(  # type: ignore[override]
         self,
         inputs: list[str],
         config: Optional[RunnableConfig] = None,
-    ) -> list[str]:
+    ) -> list[ExtendedRAGResult]:
         return super().run_batch(
             inputs=[
                 {
                     "question": i,
                 }
                 for i in inputs
             ],
```

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/rag/standalone_question_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/standalone_question_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/rag/suggested_questions_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/suggested_questions_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/rag/suggested_report_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/suggested_report_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/rag/tool_final_answer_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/rag/tool_final_answer_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/types/__init__.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/types/common.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/common.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/types/data_type_detection_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/data_type_detection_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/types/date_add_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/date_add_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/types/date_parse_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/date_parse_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/chains/types/timespan_parse_chain.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/chains/types/timespan_parse_chain.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/config.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/config.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/document_loaders/docugami.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/document_loaders/docugami.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/history.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/history.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/output_parsers/__init__.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/output_parsers/custom_react_json_single_input.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/custom_react_json_single_input.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/output_parsers/datetime.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/datetime.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/output_parsers/key_finding.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/key_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/output_parsers/line_separated_list.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/line_separated_list.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/output_parsers/sql_finding.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/sql_finding.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/output_parsers/text_cleaning.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/text_cleaning.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/output_parsers/timespan.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/output_parsers/timespan.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/params.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/params.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/retrievers/fused_summary.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/retrievers/fused_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,12 +206,13 @@
             fragments_str: str = "\n\n".join([d.strip() for d in element.fragments])
             fused_docs.append(
                 Document(
                     page_content=DOCUMENT_SUMMARY_TEMPLATE.format(
                         doc_name=element.source,
                         summary=element.summary,
                         fragments=fragments_str,
-                    )
+                    ),
+                    metadata={self.source_key: element.source},
                 )
             )
 
         return fused_docs
```

### Comparing `docugami_langchain-0.0.8/docugami_langchain/retrievers/mappings.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/retrievers/mappings.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/tools/common.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/tools/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from langchain_core.callbacks import CallbackManagerForToolRun
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.runnables import RunnableConfig
 from langchain_core.tools import BaseTool
 
-from docugami_langchain.agents.models import Invocation
+from docugami_langchain.agents.models import CitedAnswer, Invocation
 from docugami_langchain.base_runnable import TracedResponse
 from docugami_langchain.chains.answer_chain import AnswerChain
 
 NOT_FOUND = "Not found, please rephrase your question since this may improve your chances of finding results."
 
 
 def render_text_description(tools: list[BaseTool]) -> str:
@@ -65,14 +65,23 @@
     """Customized representation of tools with additional functionality."""
 
     @abstractmethod
     def to_human_readable(self, invocation: Invocation) -> str:
         """Converts tool invocation to human readable string."""
         ...
 
+    @abstractmethod
+    def _run(
+        self,
+        question: str,
+        run_manager: Optional[CallbackManagerForToolRun] = None,
+    ) -> CitedAnswer:  # type: ignore
+        """Use the tool."""
+        ...
+
 
 class ChatBotTool(BaseDocugamiTool):
     answer_chain: AnswerChain
     name: str = "chat_bot"
     description: str = (
         "Responds to greetings, small talk, or general knowledge questions."
     )
@@ -80,29 +89,32 @@
     def to_human_readable(self, invocation: Invocation) -> str:
         return f"Thinking: {invocation.tool_input}"
 
     def _run(
         self,
         question: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
-    ) -> str:
+    ) -> CitedAnswer:
         """Use the tool."""
 
-        config=None
+        config = None
         if run_manager:
-            config=RunnableConfig(
-                    run_name=self.__class__.__name__,
-                    callbacks=run_manager,
-                )
+            config = RunnableConfig(
+                run_name=self.__class__.__name__,
+                callbacks=run_manager,
+            )
         chain_response: TracedResponse[str] = self.answer_chain.run(
             question=question,
             config=config,
         )
 
-        return chain_response.value
+        return CitedAnswer(
+            source=self.name,
+            answer=chain_response.value,
+        )
 
 
 def get_generic_tools(
     llm: BaseLanguageModel,
     embeddings: Embeddings,
     answer_examples_file: Optional[Path] = None,
 ) -> list[BaseDocugamiTool]:
```

### Comparing `docugami_langchain-0.0.8/docugami_langchain/tools/reports.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/tools/reports.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 from langchain_community.tools.sql_database.tool import BaseSQLDatabaseTool
 from langchain_community.utilities.sql_database import SQLDatabase
 from langchain_core.callbacks import CallbackManagerForToolRun
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.runnables import RunnableConfig
 
-from docugami_langchain.agents.models import Invocation
-from docugami_langchain.chains.querying.sql_fixup_chain import SQLFixupChain
-from docugami_langchain.chains.querying.sql_result_chain import SQLResultChain
+from docugami_langchain.agents.models import Citation, CitedAnswer, Invocation
+from docugami_langchain.chains.querying import (
+    DocugamiExplainedSQLQueryChain,
+    SQLFixupChain,
+    SQLQueryExplainerChain,
+    SQLResultChain,
+)
 from docugami_langchain.config import MAX_PARAMS_CUTOFF_LENGTH_CHARS
 from docugami_langchain.tools.common import NOT_FOUND, BaseDocugamiTool
 
 
 class CustomReportRetrievalTool(BaseSQLDatabaseTool, BaseDocugamiTool):
     db: SQLDatabase
-    chain: SQLResultChain
+    chain: DocugamiExplainedSQLQueryChain
     name: str = "report_answer_tool"
     description: str = ""
 
     def _is_sql_like(self, question: str) -> bool:
         question = question.lower().strip()
         return question.startswith("select") and "from" in question
 
@@ -35,21 +39,22 @@
         else:
             return f"Querying report: {invocation.tool_input}"
 
     def _run(
         self,
         question: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
-    ) -> str:  # type: ignore
+    ) -> CitedAnswer:  # type: ignore
         """Use the tool."""
 
         if self._is_sql_like(question):
-            return (
-                "Looks like you passed in a SQL query. This tool takes natural language questions, and automatically translates them to SQL queries. "
-                "Please try again with a natural language version of this question."
+            return CitedAnswer(
+                source=self.name,
+                answer="Looks like you passed in a SQL query. This tool takes natural language questions, and automatically translates them to SQL queries. "
+                "Please try again with a natural language version of this question.",
             )
 
         try:
             config = None
             if run_manager:
                 config = RunnableConfig(
                     run_name=self.__class__.__name__,
@@ -57,21 +62,42 @@
                 )
 
             chain_response = self.chain.run(
                 question=question,
                 config=config,
             )
             if chain_response.value:
-                sql_result = chain_response.value.get("sql_result")
-                if sql_result:
-                    return str(sql_result)
+                results = chain_response.value.get("results")
+                if results:
+                    sql_result = results.get("sql_result", "")  # type: ignore
+                    sql_query = results.get("sql_query", "")  # type: ignore
+                    explained_sql_query = results.get("explained_sql_query", "")  # type: ignore
+                    if sql_result:
+                        return CitedAnswer(
+                            source=self.name,
+                            answer=sql_result,
+                            citations=(
+                                [
+                                    Citation(
+                                        label="Query",
+                                        details=explained_sql_query,
+                                        link=sql_query if sql_query else "",
+                                    )
+                                ]
+                                if explained_sql_query
+                                else []
+                            ),
+                        )
 
-            return NOT_FOUND
+            return CitedAnswer(source=self.name, answer=NOT_FOUND)
         except Exception as exc:
-            return f"There was an error. Please try a different question, or a different tool. Details: {exc}"
+            return CitedAnswer(
+                source=self.name,
+                answer=f"There was an error. Please try a different question, or a different tool. Details: {exc}",
+            )
 
 
 def report_name_to_report_query_tool_function_name(name: str) -> str:
     """
     Converts a report name to a report query tool function name.
 
     Report query tool function names follow these conventions:
@@ -155,14 +181,15 @@
 
 def get_retrieval_tool_for_report(
     local_xlsx_path: Path,
     report_name: str,
     retrieval_tool_function_name: str,
     retrieval_tool_description: str,
     sql_llm: BaseLanguageModel,
+    explainer_llm: BaseLanguageModel,
     embeddings: Embeddings,
     sql_fixup_examples_file: Optional[Path] = None,
     sql_examples_file: Optional[Path] = None,
 ) -> Optional[BaseDocugamiTool]:
     if not local_xlsx_path.exists():
         return None
 
@@ -174,19 +201,29 @@
 
     sql_result_chain = SQLResultChain(
         llm=sql_llm,
         embeddings=embeddings,
         db=db,
         sql_fixup_chain=fixup_chain,
     )
-
     if sql_examples_file:
         sql_result_chain.load_examples(sql_examples_file)
-
     sql_result_chain.optimize()
 
+    sql_query_explainer_chain = SQLQueryExplainerChain(
+        llm=explainer_llm,
+        embeddings=embeddings,
+    )
+    if sql_examples_file:
+        sql_query_explainer_chain.load_examples(sql_examples_file)
+
     return CustomReportRetrievalTool(
         db=db,
-        chain=sql_result_chain,
+        chain=DocugamiExplainedSQLQueryChain(
+            llm=explainer_llm,
+            embeddings=embeddings,
+            sql_result_chain=sql_result_chain,
+            sql_query_explainer_chain=sql_query_explainer_chain,
+        ),
         name=retrieval_tool_function_name,
         description=retrieval_tool_description,
     )
```

### Comparing `docugami_langchain-0.0.8/docugami_langchain/tools/retrieval.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/tools/retrieval.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.runnables import RunnableConfig
 from langchain_core.vectorstores import VectorStore
 from rerankers.models.ranker import BaseRanker
 
-from docugami_langchain.agents.models import Invocation
+from docugami_langchain.agents.models import Citation, CitedAnswer, Invocation
 from docugami_langchain.chains.documents.describe_document_set_chain import (
     DescribeDocumentSetChain,
 )
 from docugami_langchain.chains.rag.simple_rag_chain import SimpleRAGChain
 from docugami_langchain.config import DEFAULT_RETRIEVER_K, MAX_FULL_DOCUMENT_TEXT_LENGTH
 from docugami_langchain.retrievers.fused_summary import (
     FULL_DOC_SUMMARY_ID_KEY,
@@ -36,37 +36,50 @@
         """Converts tool invocation to human readable string."""
         return f"Searching documents: {invocation.tool_input}"
 
     def _run(
         self,
         question: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
-    ) -> str:  # type: ignore
+    ) -> CitedAnswer:  # type: ignore
         """Use the tool."""
 
         if not question:
-            return "Please specify a question that you want to answer from this docset"
+            return CitedAnswer(
+                source=self.name,
+                answer="Please specify a question that you want to answer from this docset",
+            )
 
         try:
             config = None
             if run_manager:
                 config = RunnableConfig(
                     run_name=self.__class__.__name__,
                     callbacks=run_manager,
                 )
             chain_response = self.chain.run(
                 question=question,
                 config=config,
             )
             if chain_response.value:
-                return chain_response.value
+                answer = chain_response.value.get("answer")
+                sources = chain_response.value.get("sources", [])
+                if answer:
+                    return CitedAnswer(
+                        source=self.name,
+                        answer=answer,
+                        citations=[Citation(label=s) for s in sources]
+                    )
 
-            return NOT_FOUND
+            return CitedAnswer(source=self.name, answer=NOT_FOUND)
         except Exception as exc:
-            return f"There was an error. Please try a different question, or a different tool. Details: {exc}"
+            return CitedAnswer(
+                source=self.name,
+                answer=f"There was an error. Please try a different question, or a different tool. Details: {exc}",
+            )
 
 
 def docset_name_to_direct_retrieval_tool_function_name(name: str) -> str:
     """
     Converts a docset name to a direct retriever tool function name.
 
     Direct retriever tool function names follow these conventions:
```

### Comparing `docugami_langchain-0.0.8/docugami_langchain/utils/documents.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/utils/documents.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/utils/sql.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/utils/sql.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/docugami_langchain/utils/string_cleanup.py` & `docugami_langchain-0.0.9rc1/docugami_langchain/utils/string_cleanup.py`

 * *Files identical despite different names*

### Comparing `docugami_langchain-0.0.8/pyproject.toml` & `docugami_langchain-0.0.9rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docugami-langchain"
-version = "0.0.8"
+version = "0.0.9rc1"
 description = "An integration package connecting Docugami and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/docugami/docugami-langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `docugami_langchain-0.0.8/PKG-INFO` & `docugami_langchain-0.0.9rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugami-langchain
-Version: 0.0.8
+Version: 0.0.9rc1
 Summary: An integration package connecting Docugami and LangChain
 Home-page: https://github.com/docugami/docugami-langchain
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

