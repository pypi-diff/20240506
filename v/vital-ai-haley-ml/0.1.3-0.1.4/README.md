# Comparing `tmp/vital-ai-haley-ml-0.1.3.tar.gz` & `tmp/vital-ai-haley-ml-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-ai-haley-ml-0.1.3.tar", last modified: Sat May  4 22:36:59 2024, max compression
+gzip compressed data, was "vital-ai-haley-ml-0.1.4.tar", last modified: Mon May  6 21:55:11 2024, max compression
```

## Comparing `vital-ai-haley-ml-0.1.3.tar` & `vital-ai-haley-ml-0.1.4.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:36:59.822239 vital-ai-haley-ml-0.1.3/
--rw-r--r--   0 hadfield   (501) staff       (20)      492 2024-05-04 22:36:59.822015 vital-ai-haley-ml-0.1.3/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:54:23.000000 vital-ai-haley-ml-0.1.3/README.md
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:36:59.798548 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:36:59.814242 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/
--rw-r--r--   0 hadfield   (501) staff       (20)     1510 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/ActorMindRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/ActorMindRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/AddContextMindRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/AddContextMindRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/DomainOntology.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasFeatureValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasFeatureValue.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasHaleyIntentSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasHaleyIntentSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasHaleyIntentSlotIntance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasHaleyIntentSlotIntance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasPredictionModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasPredictionModel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasPredictionModelInput.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasPredictionModelInput.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasPrompt.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasPrompt.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasPromptInput.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasPromptInput.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1334 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasRecommendationModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasRecommendationModel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasRecommendationModelInput.py
--rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasRecommendationModelInput.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1578 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasSelectedPredictionModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasSelectedPredictionModel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1533 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasSelectedPrompt.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasSelectedPrompt.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1598 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasSelectedRecommendationModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      249 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasSelectedRecommendationModel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasTargetValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasTargetValue.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/FeatureGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/FeatureGroup.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/FeatureType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/FeatureType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1781 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/FeatureValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      251 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/FeatureValue.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1370 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1605 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1971 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentSlotInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      339 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentSlotInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1398 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentSlotSymbol.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentSlotSymbol.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentSlotType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentSlotType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2286 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyPredictionModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      433 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyPredictionModel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyPredictionModelClass.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyPredictionModelClass.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1465 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyPrompt.py
--rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyPrompt.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2094 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyRecommendationModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      383 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyRecommendationModel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1393 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PredictionModelInput.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PredictionModelInput.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PredictionModelProvider.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PredictionModelProvider.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PredictionModelStructureType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PredictionModelStructureType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PredictionModelType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PredictionModelType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PrefetchDataMindRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PrefetchDataMindRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1261 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PromptInput.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PromptInput.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1401 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PromptMindRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PromptMindRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PurgeDataMindRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PurgeDataMindRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1405 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/RecommendationModelInput.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/RecommendationModelInput.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/RecommendationModelStructureType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/RecommendationModelStructureType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/RecommendationModelType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/RecommendationModelType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/RemoveContextMindRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/RemoveContextMindRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/TargetGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/TargetGroup.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1254 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/TargetType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/TargetType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2220 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/TargetValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      381 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/TargetValue.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:36:59.821024 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasActorSequence.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasFeatureKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasFeatureStringValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasFeatureType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasFeatureURIValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasFeatureWeight.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentScore.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSlotContent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSlotEndRange.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSlotScore.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSlotStartRange.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSlotTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSlotURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSourceText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasHaleyPromptURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasModelIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasModelIntentIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasPredictionImplementingClass.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasPredictionModelClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasPredictionModelEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasPredictionModelProvider.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasPredictionModelStructureType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasPredictionModelType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasPromptString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasRecommendationImplementingClass.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasRecommendationModelEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasRecommendationModelStructureType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasRecommendationModelType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasSelectedPredictionModelName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasSelectedPromptName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasSelectedRecommendationModelName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasTargetBooleanValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasTargetDoubleValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasTargetEncodedStringValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasTargetIntegerValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasTargetKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasTargetStringValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasTargetType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasTargetURIValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasTargetWeight.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_hasVersion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_isGlobalPredictionModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_isGlobalPrompt.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_isGlobalRecommendationModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/Property_isStreamModelResults.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/properties/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-04 22:36:59.822286 vital-ai-haley-ml-0.1.3/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      886 2024-05-04 22:34:45.000000 vital-ai-haley-ml-0.1.3/setup.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:36:59.821736 vital-ai-haley-ml-0.1.3/vital_ai_haley_ml.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      492 2024-05-04 22:36:59.000000 vital-ai-haley-ml-0.1.3/vital_ai_haley_ml.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)     7985 2024-05-04 22:36:59.000000 vital-ai-haley-ml-0.1.3/vital_ai_haley_ml.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-04 22:36:59.000000 vital-ai-haley-ml-0.1.3/vital_ai_haley_ml.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       62 2024-05-04 22:36:59.000000 vital-ai-haley-ml-0.1.3/vital_ai_haley_ml.egg-info/entry_points.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       22 2024-05-04 22:36:59.000000 vital-ai-haley-ml-0.1.3/vital_ai_haley_ml.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       19 2024-05-04 22:36:59.000000 vital-ai-haley-ml-0.1.3/vital_ai_haley_ml.egg-info/top_level.txt
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:55:11.706011 vital-ai-haley-ml-0.1.4/
+-rw-r--r--   0 hadfield   (501) staff       (20)      492 2024-05-06 21:55:11.705777 vital-ai-haley-ml-0.1.4/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:54:23.000000 vital-ai-haley-ml-0.1.4/README.md
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:55:11.684884 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:55:11.697691 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)     1510 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/ActorMindRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/ActorMindRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/AddContextMindRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/AddContextMindRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/DomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasFeatureValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasFeatureValue.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasHaleyIntentSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasHaleyIntentSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasHaleyIntentSlotIntance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasHaleyIntentSlotIntance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasPredictionModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasPredictionModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasPredictionModelInput.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasPredictionModelInput.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasPrompt.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasPrompt.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasPromptInput.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasPromptInput.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1334 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasRecommendationModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasRecommendationModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasRecommendationModelInput.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasRecommendationModelInput.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1578 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasSelectedPredictionModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasSelectedPredictionModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1533 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasSelectedPrompt.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasSelectedPrompt.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1598 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasSelectedRecommendationModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      249 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasSelectedRecommendationModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasTargetValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasTargetValue.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/FeatureGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/FeatureGroup.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/FeatureType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/FeatureType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1781 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/FeatureValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      251 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/FeatureValue.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1370 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1605 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1971 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentSlotInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      339 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentSlotInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1398 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentSlotSymbol.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentSlotSymbol.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentSlotType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentSlotType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2286 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyPredictionModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      433 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyPredictionModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyPredictionModelClass.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyPredictionModelClass.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1465 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyPrompt.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyPrompt.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2094 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyRecommendationModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      383 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyRecommendationModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1393 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PredictionModelInput.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PredictionModelInput.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PredictionModelProvider.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PredictionModelProvider.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PredictionModelStructureType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PredictionModelStructureType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PredictionModelType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PredictionModelType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PrefetchDataMindRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PrefetchDataMindRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1261 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PromptInput.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PromptInput.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1401 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PromptMindRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PromptMindRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PurgeDataMindRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PurgeDataMindRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1405 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/RecommendationModelInput.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/RecommendationModelInput.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/RecommendationModelStructureType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/RecommendationModelStructureType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/RecommendationModelType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/RecommendationModelType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/RemoveContextMindRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/RemoveContextMindRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/TargetGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/TargetGroup.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1254 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/TargetType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/TargetType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2220 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/TargetValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      381 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/TargetValue.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:55:11.704468 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasActorSequence.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasFeatureKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasFeatureStringValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasFeatureType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasFeatureURIValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasFeatureWeight.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentScore.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSlotContent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSlotEndRange.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSlotScore.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSlotStartRange.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSlotTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSlotURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentSourceText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasHaleyIntentURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasHaleyPromptURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasModelIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasModelIntentIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasPredictionImplementingClass.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasPredictionModelClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasPredictionModelEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasPredictionModelProvider.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasPredictionModelStructureType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasPredictionModelType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasPromptString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasRecommendationImplementingClass.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasRecommendationModelEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasRecommendationModelStructureType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasRecommendationModelType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasSelectedPredictionModelName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasSelectedPromptName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasSelectedRecommendationModelName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasTargetBooleanValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasTargetDoubleValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasTargetEncodedStringValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasTargetIntegerValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasTargetKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasTargetStringValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasTargetType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasTargetURIValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasTargetWeight.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_hasVersion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_isGlobalPredictionModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_isGlobalPrompt.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_isGlobalRecommendationModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/Property_isStreamModelResults.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:39:48.000000 vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/properties/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-06 21:55:11.706056 vital-ai-haley-ml-0.1.4/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)      886 2024-05-06 21:54:27.000000 vital-ai-haley-ml-0.1.4/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:55:11.705506 vital-ai-haley-ml-0.1.4/vital_ai_haley_ml.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      492 2024-05-06 21:55:11.000000 vital-ai-haley-ml-0.1.4/vital_ai_haley_ml.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)     7985 2024-05-06 21:55:11.000000 vital-ai-haley-ml-0.1.4/vital_ai_haley_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-06 21:55:11.000000 vital-ai-haley-ml-0.1.4/vital_ai_haley_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       62 2024-05-06 21:55:11.000000 vital-ai-haley-ml-0.1.4/vital_ai_haley_ml.egg-info/entry_points.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       22 2024-05-06 21:55:11.000000 vital-ai-haley-ml-0.1.4/vital_ai_haley_ml.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       19 2024-05-06 21:55:11.000000 vital-ai-haley-ml-0.1.4/vital_ai_haley_ml.egg-info/top_level.txt
```

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/ActorMindRequest.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/ActorMindRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/AddContextMindRequest.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/AddContextMindRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasFeatureValue.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasFeatureValue.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasHaleyIntentSlot.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasHaleyIntentSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasHaleyIntentSlotIntance.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasHaleyIntentSlotIntance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasPredictionModel.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasPredictionModel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasPredictionModelInput.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasPredictionModelInput.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasPrompt.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasPrompt.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasPromptInput.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasPromptInput.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasRecommendationModel.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasRecommendationModel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasRecommendationModelInput.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasRecommendationModelInput.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasSelectedPredictionModel.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasSelectedPredictionModel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasSelectedPrompt.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasSelectedPrompt.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasSelectedRecommendationModel.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasSelectedRecommendationModel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/Edge_hasTargetValue.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/Edge_hasTargetValue.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/FeatureGroup.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/FeatureGroup.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/FeatureType.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/FeatureType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/FeatureValue.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/FeatureValue.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntent.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentInstance.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentSlot.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentSlotInstance.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentSlotInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentSlotSymbol.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentSlotSymbol.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyIntentSlotType.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyIntentSlotType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyPredictionModel.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyPredictionModel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyPredictionModelClass.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyPredictionModelClass.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyPrompt.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyPrompt.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/HaleyRecommendationModel.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/HaleyRecommendationModel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PredictionModelInput.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PredictionModelInput.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PredictionModelProvider.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PredictionModelProvider.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PredictionModelStructureType.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PredictionModelStructureType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PredictionModelType.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PredictionModelType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PrefetchDataMindRequest.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PrefetchDataMindRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PromptInput.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PromptInput.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PromptMindRequest.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PromptMindRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/PurgeDataMindRequest.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/PurgeDataMindRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/RecommendationModelInput.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/RecommendationModelInput.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/RecommendationModelStructureType.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/RecommendationModelStructureType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/RecommendationModelType.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/RecommendationModelType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/RemoveContextMindRequest.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/RemoveContextMindRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/TargetGroup.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/TargetGroup.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/TargetType.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/TargetType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/ai_haley_ml_domain/model/TargetValue.py` & `vital-ai-haley-ml-0.1.4/ai_haley_ml_domain/model/TargetValue.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-ml-0.1.3/setup.py` & `vital-ai-haley-ml-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vital-ai-haley-ml',
-    version='0.1.3',
+    version='0.1.4',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='VitalSigns haley ml domain',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/vitalhome-haley',
     packages=find_packages(),
@@ -16,15 +16,15 @@
         ]
     },
     package_data={
          '': ['*.pyi'],
     },
     license='Apache License 2.0',
     install_requires=[
-            'vital-ai-haley==0.1.3',
+            'vital-ai-haley>=0.1.4',
         ],
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.10',
```

### Comparing `vital-ai-haley-ml-0.1.3/vital_ai_haley_ml.egg-info/SOURCES.txt` & `vital-ai-haley-ml-0.1.4/vital_ai_haley_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

