# Comparing `tmp/vital-ai-nlp-0.1.3.tar.gz` & `tmp/vital-ai-nlp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-ai-nlp-0.1.3.tar", last modified: Sat May  4 21:24:24 2024, max compression
+gzip compressed data, was "vital-ai-nlp-0.1.4.tar", last modified: Mon May  6 21:42:45 2024, max compression
```

## Comparing `vital-ai-nlp-0.1.3.tar` & `vital-ai-nlp-0.1.4.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:24:24.894457 vital-ai-nlp-0.1.3/
--rw-r--r--   0 hadfield   (501) staff       (20)      482 2024-05-04 21:24:24.894235 vital-ai-nlp-0.1.3/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 02:45:51.000000 vital-ai-nlp-0.1.3/README.md
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:24:24.868359 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:23.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:24:24.881941 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/
--rw-r--r--   0 hadfield   (501) staff       (20)     1455 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Abbreviation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Abbreviation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1893 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/AbbreviationInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      271 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/AbbreviationInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1461 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Annotation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Annotation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1438 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Content.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Content.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     3079 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Document.py
--rw-r--r--   0 hadfield   (501) staff       (20)      579 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Document.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/DomainOntology.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasAbbreviation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasAbbreviation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1335 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasAbbreviationInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasAbbreviationInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasAnnotation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasAnnotation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasContent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasContent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1317 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEntityInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEntityInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1329 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEquivalenceElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEquivalenceElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEquivalenceRelationInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEquivalenceRelationInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1410 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEventElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEventElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEventInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEventInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEventTrigger.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEventTrigger.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1317 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasImageReference.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasImageReference.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1426 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasNormalizedEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      183 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasNormalizedEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasNormalizedTopic.py
--rw-r--r--   0 hadfield   (501) staff       (20)      182 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasNormalizedTopic.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasNounPhrase.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasNounPhrase.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1341 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasPhraseNormalizedEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasPhraseNormalizedEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasPosTag.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasPosTag.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1422 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasRelationElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasRelationElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1323 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasRelationInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      161 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasRelationInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasSentence.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasSentence.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1359 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasSentenceAbbreviationInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasSentenceAbbreviationInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1341 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasSentenceEntityInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasSentenceEntityInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTagElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTagElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTargetNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTargetNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTextBlock.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTextBlock.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasToken.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasToken.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTopic.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTopic.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTranslation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTranslation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasVerbPhrase.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasVerbPhrase.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1510 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/EquivalenceRelationInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      182 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/EquivalenceRelationInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1470 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/EventInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/EventInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1468 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/FlowPredictModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/FlowPredictModel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1852 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Image.py
--rw-r--r--   0 hadfield   (501) staff       (20)      265 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Image.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1875 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/ImageReference.py
--rw-r--r--   0 hadfield   (501) staff       (20)      273 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/ImageReference.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1656 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpEntityInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      361 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpEntityInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2562 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpNormalizedEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      427 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpNormalizedEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1870 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpNormalizedTopic.py
--rw-r--r--   0 hadfield   (501) staff       (20)      260 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpNormalizedTopic.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1483 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpRelationInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      171 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpRelationInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1462 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NounPhrase.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NounPhrase.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1240 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Phrase.py
--rw-r--r--   0 hadfield   (501) staff       (20)      114 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Phrase.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1438 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/PosTag.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/PosTag.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1996 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Sentence.py
--rw-r--r--   0 hadfield   (501) staff       (20)      323 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Sentence.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1859 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/TagElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      262 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/TagElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1662 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/TargetNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/TargetNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1674 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/TextBlock.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/TextBlock.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1542 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Token.py
--rw-r--r--   0 hadfield   (501) staff       (20)      180 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Token.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1440 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Topic.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Topic.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1462 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/VerbPhrase.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/VerbPhrase.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:23.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:24:24.893281 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasAnalyzedBody.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasAnalyzedTitle.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasAnnotationName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasAnnotationValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasBody.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasClassifierName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasConfidence.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasContentID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasContentTag.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasContentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasContext.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasDmozPath.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasDocumentPublicationDate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasDocumentSourceName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasDocumentTitle.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasDocumentUrl.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasDocumentUrlRoot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasEndPosition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasEndTokenIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasEntityAuthor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasEntityOffset.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasEntityOffsetInSentence.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasEntityType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasEquivalenceType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasEventInstanceType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasEventRole.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasExactString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasExtractSource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasExtractedText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasExtractedTitle.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasHeightPx.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasImageData.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasImageDate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasImageURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasLang.py
--rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasLength.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasLengthInSentence.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasLongForm.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasLongFormEnd.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasLongFormStart.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasModelPath.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasModelType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasModelURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasNameVariants.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasNlpEntityCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasNormConfidence.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasPosTagsConfidenceString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasPosTagsValuesString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasRelationRole.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasRelationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasRelevance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasSentenceNumber.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasSentimentScore.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasShortForm.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasShortFormEnd.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasShortFormStart.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasShortname.py
--rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasSlug.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasSourceDomain.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasSpanType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasStartPosition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasStartTokenIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasSymbol.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasTagValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasTargetDoubleValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasTargetScore.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasTargetStringValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasTextBlockLength.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasTextBlockOffset.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasTextBlockText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasTicker.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasTokenText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasTokensPositionsString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasTokensTextString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasTopicScore.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasTransformationVector.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasWidthPx.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasWikipediaURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_hasWordnetURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_isClosingTag.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_isOpeningTag.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_isSentimentMixed.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/Property_isStandaloneTag.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:23.000000 vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/properties/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-04 21:24:24.894497 vital-ai-nlp-0.1.3/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      885 2024-05-04 21:08:32.000000 vital-ai-nlp-0.1.3/setup.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:24:24.893950 vital-ai-nlp-0.1.3/vital_ai_nlp.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      482 2024-05-04 21:24:24.000000 vital-ai-nlp-0.1.3/vital_ai_nlp.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)    11587 2024-05-04 21:24:24.000000 vital-ai-nlp-0.1.3/vital_ai_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-04 21:24:24.000000 vital-ai-nlp-0.1.3/vital_ai_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       70 2024-05-04 21:24:24.000000 vital-ai-nlp-0.1.3/vital_ai_nlp.egg-info/entry_points.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       23 2024-05-04 21:24:24.000000 vital-ai-nlp-0.1.3/vital_ai_nlp.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       23 2024-05-04 21:24:24.000000 vital-ai-nlp-0.1.3/vital_ai_nlp.egg-info/top_level.txt
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:42:45.439580 vital-ai-nlp-0.1.4/
+-rw-r--r--   0 hadfield   (501) staff       (20)      482 2024-05-06 21:42:45.439334 vital-ai-nlp-0.1.4/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 02:45:51.000000 vital-ai-nlp-0.1.4/README.md
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:42:45.412674 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:23.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:42:45.427404 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)     1455 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Abbreviation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Abbreviation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1893 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/AbbreviationInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      271 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/AbbreviationInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1461 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Annotation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Annotation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1438 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Content.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Content.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     3079 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Document.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      579 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Document.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/DomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasAbbreviation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasAbbreviation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1335 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasAbbreviationInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasAbbreviationInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasAnnotation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasAnnotation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasContent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasContent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1317 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEntityInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEntityInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1329 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEquivalenceElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEquivalenceElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEquivalenceRelationInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEquivalenceRelationInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1410 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEventElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEventElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEventInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEventInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEventTrigger.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEventTrigger.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1317 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasImageReference.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasImageReference.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1426 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasNormalizedEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      183 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasNormalizedEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasNormalizedTopic.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      182 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasNormalizedTopic.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasNounPhrase.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasNounPhrase.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1341 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasPhraseNormalizedEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasPhraseNormalizedEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasPosTag.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasPosTag.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1422 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasRelationElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasRelationElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1323 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasRelationInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      161 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasRelationInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasSentence.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasSentence.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1359 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasSentenceAbbreviationInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasSentenceAbbreviationInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1341 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasSentenceEntityInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasSentenceEntityInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTagElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTagElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTargetNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTargetNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTextBlock.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTextBlock.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasToken.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasToken.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTopic.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTopic.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTranslation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTranslation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasVerbPhrase.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasVerbPhrase.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1510 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/EquivalenceRelationInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      182 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/EquivalenceRelationInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1470 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/EventInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/EventInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1468 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/FlowPredictModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/FlowPredictModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1852 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Image.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      265 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Image.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1875 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/ImageReference.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      273 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/ImageReference.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1656 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpEntityInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      361 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpEntityInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2562 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpNormalizedEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      427 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpNormalizedEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1870 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpNormalizedTopic.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      260 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpNormalizedTopic.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1483 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpRelationInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      171 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpRelationInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1462 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NounPhrase.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NounPhrase.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1240 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Phrase.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      114 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Phrase.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1438 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/PosTag.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/PosTag.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1996 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Sentence.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      323 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Sentence.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1859 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/TagElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      262 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/TagElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1662 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/TargetNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/TargetNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1674 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/TextBlock.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/TextBlock.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1542 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Token.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      180 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Token.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1440 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Topic.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Topic.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1462 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/VerbPhrase.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/VerbPhrase.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:23.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:42:45.438338 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasAnalyzedBody.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasAnalyzedTitle.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasAnnotationName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasAnnotationValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasBody.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasClassifierName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasConfidence.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasContentID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasContentTag.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasContentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasContext.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasDmozPath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasDocumentPublicationDate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasDocumentSourceName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasDocumentTitle.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasDocumentUrl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasDocumentUrlRoot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasEndPosition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasEndTokenIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasEntityAuthor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasEntityOffset.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasEntityOffsetInSentence.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasEntityType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasEquivalenceType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasEventInstanceType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasEventRole.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasExactString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasExtractSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasExtractedText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasExtractedTitle.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasHeightPx.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasImageData.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasImageDate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasImageURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasLang.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasLength.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasLengthInSentence.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasLongForm.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasLongFormEnd.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasLongFormStart.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasModelPath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasModelType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasModelURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasNameVariants.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasNlpEntityCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasNormConfidence.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasPosTagsConfidenceString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasPosTagsValuesString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasRelationRole.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasRelationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasRelevance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasSentenceNumber.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasSentimentScore.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasShortForm.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasShortFormEnd.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasShortFormStart.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasShortname.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasSlug.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasSourceDomain.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasSpanType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasStartPosition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasStartTokenIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasSymbol.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasTagValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasTargetDoubleValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasTargetScore.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasTargetStringValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasTextBlockLength.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasTextBlockOffset.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasTextBlockText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasTicker.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasTokenText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasTokensPositionsString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasTokensTextString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasTopicScore.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasTransformationVector.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasWidthPx.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasWikipediaURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_hasWordnetURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_isClosingTag.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_isOpeningTag.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_isSentimentMixed.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/Property_isStandaloneTag.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:23.000000 vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/properties/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-06 21:42:45.439625 vital-ai-nlp-0.1.4/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)      885 2024-05-06 21:39:39.000000 vital-ai-nlp-0.1.4/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:42:45.439050 vital-ai-nlp-0.1.4/vital_ai_nlp.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      482 2024-05-06 21:42:45.000000 vital-ai-nlp-0.1.4/vital_ai_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)    11587 2024-05-06 21:42:45.000000 vital-ai-nlp-0.1.4/vital_ai_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-06 21:42:45.000000 vital-ai-nlp-0.1.4/vital_ai_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       70 2024-05-06 21:42:45.000000 vital-ai-nlp-0.1.4/vital_ai_nlp.egg-info/entry_points.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       23 2024-05-06 21:42:45.000000 vital-ai-nlp-0.1.4/vital_ai_nlp.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       23 2024-05-06 21:42:45.000000 vital-ai-nlp-0.1.4/vital_ai_nlp.egg-info/top_level.txt
```

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Abbreviation.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Abbreviation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/AbbreviationInstance.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/AbbreviationInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Annotation.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Annotation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Content.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Content.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Document.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Document.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Document.pyi` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Document.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasAbbreviation.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasAbbreviation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasAbbreviationInstance.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasAbbreviationInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasAnnotation.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasAnnotation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasCategory.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasContent.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasContent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEntity.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEntityInstance.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEntityInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEquivalenceElement.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEquivalenceElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEquivalenceRelationInstance.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEquivalenceRelationInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEventElement.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEventElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEventInstance.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEventInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasEventTrigger.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasEventTrigger.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasImageReference.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasImageReference.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasNormalizedEntity.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasNormalizedEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasNormalizedTopic.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasNormalizedTopic.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasNounPhrase.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasNounPhrase.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasPhraseNormalizedEntity.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasPhraseNormalizedEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasPosTag.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasPosTag.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasRelationElement.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasRelationElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasRelationInstance.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasRelationInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasSentence.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasSentence.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasSentenceAbbreviationInstance.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasSentenceAbbreviationInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasSentenceEntityInstance.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasSentenceEntityInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTagElement.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTagElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTargetNode.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTargetNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTextBlock.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTextBlock.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasToken.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasToken.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTopic.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTopic.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasTranslation.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasTranslation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Edge_hasVerbPhrase.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Edge_hasVerbPhrase.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/EquivalenceRelationInstance.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/EquivalenceRelationInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/EventInstance.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/EventInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/FlowPredictModel.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/FlowPredictModel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Image.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Image.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/ImageReference.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/ImageReference.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpEntity.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpEntityInstance.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpEntityInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpNormalizedEntity.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpNormalizedEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpNormalizedTopic.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpNormalizedTopic.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NlpRelationInstance.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NlpRelationInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/NounPhrase.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/NounPhrase.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Phrase.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Phrase.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/PosTag.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/PosTag.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Sentence.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Sentence.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/TagElement.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/TagElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/TargetNode.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/TargetNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/TextBlock.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/TextBlock.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Token.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Token.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/Topic.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/Topic.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/com_vitalai_domain_nlp/model/VerbPhrase.py` & `vital-ai-nlp-0.1.4/com_vitalai_domain_nlp/model/VerbPhrase.py`

 * *Files identical despite different names*

### Comparing `vital-ai-nlp-0.1.3/setup.py` & `vital-ai-nlp-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vital-ai-nlp',
-    version='0.1.3',
+    version='0.1.4',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='VitalSigns nlp domain',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/vitalhome-aimp',
     packages=find_packages(),
@@ -16,15 +16,15 @@
         ]
     },
     package_data={
          '': ['*.pyi'],
     },
     license='Apache License 2.0',
     install_requires=[
-            'vital-ai-domain==0.1.3',
+            'vital-ai-domain>=0.1.4',
         ],
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.10',
```

### Comparing `vital-ai-nlp-0.1.3/vital_ai_nlp.egg-info/SOURCES.txt` & `vital-ai-nlp-0.1.4/vital_ai_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

