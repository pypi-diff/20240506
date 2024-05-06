# Comparing `tmp/vital-ai-haley-0.1.3.tar.gz` & `tmp/vital-ai-haley-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-ai-haley-0.1.3.tar", last modified: Sat May  4 22:26:33 2024, max compression
+gzip compressed data, was "vital-ai-haley-0.1.4.tar", last modified: Mon May  6 21:51:29 2024, max compression
```

## Comparing `vital-ai-haley-0.1.3.tar` & `vital-ai-haley-0.1.4.tar`

### file list

```diff
@@ -1,897 +1,897 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:26:33.911378 vital-ai-haley-0.1.3/
--rw-r--r--   0 hadfield   (501) staff       (20)      485 2024-05-04 22:26:33.911113 vital-ai-haley-0.1.3/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:53:31.000000 vital-ai-haley-0.1.3/README.md
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:26:33.730995 vital-ai-haley-0.1.3/com_vitalai_haley_domain/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:35:40.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:26:33.857755 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/
--rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/AgentDeveloper.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/AgentDeveloper.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Customer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Customer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1434 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/DialogTask.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/DialogTask.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/DomainOntology.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1541 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasAccountDataSharedWith.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasAccountDataSharedWith.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2172 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessAccountRole.py
--rw-r--r--   0 hadfield   (501) staff       (20)      442 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessAccountRole.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2160 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessBotRole.py
--rw-r--r--   0 hadfield   (501) staff       (20)      438 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessBotRole.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2166 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessLoginRole.py
--rw-r--r--   0 hadfield   (501) staff       (20)      440 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessLoginRole.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessOfficePolicy.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessOfficePolicy.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessOfficeRole.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessOfficeRole.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessPolicy.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessPolicy.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1608 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRight.py
--rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRight.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightContext.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightContext.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1458 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightGraphObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightGraphObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1446 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightProperty.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessTeamPolicy.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessTeamPolicy.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessTeamRole.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessTeamRole.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOffice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOffice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOfficeLocation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOfficeLocation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOfficeMember.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOfficeMember.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountTeam.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountTeam.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountTeamMember.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountTeamMember.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaActionCondition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaActionCondition.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1334 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaActionSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaActionSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaCondition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaCondition.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaGoalCondition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      161 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaGoalCondition.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaPartialGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaPartialGoal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaPrimaryGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaPrimaryGoal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaStep.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaStep.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPartialGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPartialGoal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionCondition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      161 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionCondition.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1373 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstanceDestination.py
--rw-r--r--   0 hadfield   (501) staff       (20)      171 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstanceDestination.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1358 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstanceSource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstanceSource.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanCondition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanCondition.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanLevel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanLevel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanStep.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanStep.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPrimaryGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPrimaryGoal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindQueryAnswer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindQueryAnswer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindQueryAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindQueryAnswerBinding.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindRuleParameter.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindRuleParameter.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1346 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindRuleParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindRuleParameterBinding.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyOriginRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyOriginRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyReport.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyReport.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherAlert.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherAlert.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherDailyReport.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherDailyReport.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherHourlyReport.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherHourlyReport.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherMinutelyReport.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherMinutelyReport.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasProofJustificationReason.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasProofJustificationReason.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1403 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasProofTreeNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasProofTreeNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1268 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/GlobalManager.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/GlobalManager.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1658 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAPIKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAPIKey.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1400 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessAccountPolicyRule.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessAccountPolicyRule.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessAccountRole.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessAccountRole.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessBotRole.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessBotRole.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1853 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessGrant.py
--rw-r--r--   0 hadfield   (501) staff       (20)      289 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessGrant.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessGrantStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessGrantStatus.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessGrantType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessGrantType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1494 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessLoginPolicyRule.py
--rw-r--r--   0 hadfield   (501) staff       (20)      186 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessLoginPolicyRule.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessLoginRole.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessLoginRole.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessLoginType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessLoginType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessOfficePolicy.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessOfficePolicy.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessOfficeRole.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessOfficeRole.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessPolicy.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessPolicy.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1589 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRight.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRight.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1398 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightContext.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightContext.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1633 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightGraphObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      254 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightGraphObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1617 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightMessageDirection.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightMessageDirection.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightMessageRule.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightMessageRule.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1621 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightProperty.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightPropertyRule.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightPropertyRule.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightRuleType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightRuleType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRoleGrantAspect.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRoleGrantAspect.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRoleGrantExtent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRoleGrantExtent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRoleGrantType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRoleGrantType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRoleScope.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRoleScope.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessTeamPolicy.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessTeamPolicy.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessTeamRole.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessTeamRole.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessViolationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessViolationType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccount.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1433 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountDataShareFilterRule.py
--rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountDataShareFilterRule.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountDataShareScope.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountDataShareScope.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1498 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountOffice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountOffice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountOfficeLocation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      456 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountOfficeLocation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1488 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountTeam.py
--rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountTeam.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAirQualityReport.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAirQualityReport.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1495 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAnalyticsContainer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      190 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAnalyticsContainer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAnalyticsWindowSize.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAnalyticsWindowSize.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1553 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAppEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAppEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1552 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCanadianProvinceOrTerritory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCanadianProvinceOrTerritory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCelestialBody.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCelestialBody.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1285 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyChannelAnswer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyChannelAnswer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyChannelQuestion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyChannelQuestion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1452 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      174 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCollection.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCollection.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCommandGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCommandGroup.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCommandStateType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCommandStateType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1607 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCompassDirection.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCompassDirection.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1466 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCountry.py
--rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCountry.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1286 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCountryDivision.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCountryDivision.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1653 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCryptoKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCryptoKey.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1355 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDataTable.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDataTable.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1967 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDialogMapping.py
--rw-r--r--   0 hadfield   (501) staff       (20)      324 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDialogMapping.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDialogMappingType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDialogMappingType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDialogResponseType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDialogResponseType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDialogRouteType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDialogRouteType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDocGenProcessorRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDocGenProcessorRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1594 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDomainMethod.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDomainMethod.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDomainMethodContextType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDomainMethodContextType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1472 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyFileResource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyFileResource.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1436 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyGraph.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyGraph.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1393 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyGraphContainerProxy.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyGraphContainerProxy.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyGraphType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyGraphType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyHandlerErrorType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyHandlerErrorType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyHandlerValidationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyHandlerValidationType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     3232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyIntentCommand.py
--rw-r--r--   0 hadfield   (501) staff       (20)      880 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyIntentCommand.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyInterAccountNotification.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyInterAccountNotification.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2966 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyInterAccountRecord.py
--rw-r--r--   0 hadfield   (501) staff       (20)      761 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyInterAccountRecord.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyInterAccountRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyInterAccountRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyInterAccountResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyInterAccountResponse.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMailingList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMailingList.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMailingListEntity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMailingListEntity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1392 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindActionResult.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindActionResult.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindActionResultType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindActionResultType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgenda.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgenda.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaActionCondition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaActionCondition.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaActionSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaActionSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaCondition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaCondition.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaGoal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaGoalCondition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaGoalCondition.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaPartialGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaPartialGoal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaPrimaryGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaPrimaryGoal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaStep.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaStep.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1254 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindApp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindApp.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAskMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAskMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAskPlanAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAskPlanAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1286 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindBotEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindBotEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindBotPlanAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindBotPlanAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindCommandAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindCommandAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1854 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindContext.py
--rw-r--r--   0 hadfield   (501) staff       (20)      269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindContext.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindDatascriptPlanAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindDatascriptPlanAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindGoal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindInferenceType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindInferenceType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2002 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindMetaQLDataset.py
--rw-r--r--   0 hadfield   (501) staff       (20)      347 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindMetaQLDataset.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1439 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindMetaQLQueryOperation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindMetaQLQueryOperation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindOperation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindOperation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindOperationResult.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindOperationResult.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPartialGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPartialGoal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlan.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlan.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanActionCondition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanActionCondition.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1401 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanActionInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanActionInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanActionSlot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanActionSlot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanCondition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanCondition.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanGoalCondition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanGoalCondition.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanLevel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanLevel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1388 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      161 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanRequestType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanRequestType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanStep.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanStep.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPredictionPlanAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPredictionPlanAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPrimaryGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPrimaryGoal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1334 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorPlanAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorPlanAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2298 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      494 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorRequestType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorRequestType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1914 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      318 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorResponse.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorResponseType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorResponseType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2108 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      394 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindQuery.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1716 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindQueryAnswer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      273 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindQueryAnswer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2908 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindQueryAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      670 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindQueryAnswerBinding.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindQueryStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindQueryStatus.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindReceiveMessagePlanAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindReceiveMessagePlanAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRecommendationPlanAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRecommendationPlanAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     3118 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      855 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     3332 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      922 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindResponse.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindResponseStatusType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindResponseStatusType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1455 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRule.py
--rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRule.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleGraphResolveType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleGraphResolveType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1606 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleInvocation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleInvocation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleInvocationGraphDataManagementType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleInvocationGraphDataManagementType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2161 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleParameter.py
--rw-r--r--   0 hadfield   (501) staff       (20)      431 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleParameter.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2959 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      717 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleParameterBinding.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleParameterMode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleParameterMode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleParameterType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleParameterType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindSendMessagePlanAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindSendMessagePlanAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindServiceRequestType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindServiceRequestType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTaskEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTaskEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTaskPlanAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTaskPlanAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTellMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTellMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTellPlanAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTellPlanAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTickRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTickRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindUserEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindUserEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyNaturalPlanetarySatellite.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyNaturalPlanetarySatellite.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyNotification.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyNotification.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyObjectAccessType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyObjectAccessType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1463 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyPermitStreamingResponseMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyPermitStreamingResponseMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyPlace.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyPlace.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyPlanet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyPlanet.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1504 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProcessorRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProcessorRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProcessorStepType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProcessorStepType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProgressStatusType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProgressStatusType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProgressUnitType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProgressUnitType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1350 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProvenance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProvenance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1678 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRegion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRegion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1429 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRelayResponseMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      188 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRelayResponseMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRelayStatusMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRelayStatusMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyReport.py
--rw-r--r--   0 hadfield   (501) staff       (20)      115 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyReport.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1827 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyReportInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyReportInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2324 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      467 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRequestGraph.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRequestGraph.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     3034 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRequestMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      834 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRequestMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRequestResponseType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRequestResponseType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     4208 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyResponseMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1225 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyResponseMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyResponseType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyResponseType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1707 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyResultMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      261 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyResultMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyStar.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyStar.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1629 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleySymmetricCryptoKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleySymmetricCryptoKey.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2155 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyTask.py
--rw-r--r--   0 hadfield   (501) staff       (20)      365 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyTask.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1459 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyUSCounty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      174 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyUSCounty.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1879 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyUSPostalRegion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      297 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyUSPostalRegion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1525 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyUSStateOrTerritory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyUSStateOrTerritory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1464 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyUserEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyUserEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherAlert.py
--rw-r--r--   0 hadfield   (501) staff       (20)      413 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherAlert.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherAlertCertainty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherAlertCertainty.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherAlertSeverity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherAlertSeverity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1405 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherDailyReport.py
--rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherDailyReport.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1408 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherHourlyReport.py
--rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherHourlyReport.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherMinutelyReport.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherMinutelyReport.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherMoonPhase.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherMoonPhase.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     4744 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherReport.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherReport.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1807 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2031 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HyperEdge_hasAccessGrant.py
--rw-r--r--   0 hadfield   (501) staff       (20)      382 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HyperEdge_hasAccessGrant.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HyperEdge_hasHaleyMindRuleGraphMembership.py
--rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HyperEdge_hasHaleyMindRuleGraphMembership.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1317 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HyperEdge_hasReferenceObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HyperEdge_hasReferenceObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1533 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/PermitStreamingRequestMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/PermitStreamingRequestMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/PermitStreamingType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/PermitStreamingType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofAnswerType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofAnswerType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofDecision.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofDecision.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1245 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofGoal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationAnswerType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationAnswerType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     3586 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationReason.py
--rw-r--r--   0 hadfield   (501) staff       (20)      934 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationReason.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1332 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationReasonComparatorType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationReasonComparatorType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationReasonType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationReasonType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1268 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofPrimaryGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofPrimaryGoal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofProgressType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofProgressType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofSpecialValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofSpecialValue.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTertiaryGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTertiaryGoal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1458 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTree.py
--rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTree.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1517 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeAncestorNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeAncestorNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1502 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeAskNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeAskNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1818 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeConclusionNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      306 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeConclusionNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1639 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeDependencyNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      261 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeDependencyNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeDeriveNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeDeriveNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeJustificationNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      462 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeJustificationNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1469 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      184 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Seller.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Seller.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:35:40.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:26:33.909467 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/
--rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAPIKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAPIKeyIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAPIKeySessionKeyIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantMemberURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantOutcomeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantProviderAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantProviderBot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantProviderLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantRoleOutcomeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessObjectTypes.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessOutcomeSerialized.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessRightChannelContextURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeBotURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeChannelURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeDatasetURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeLoginURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeOfficeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeTeamURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccountClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      254 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccountDataShareFilterRuleIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccountDataShareFilterRuleURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccountDataShareScopeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccountObjectAccessTypes.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccountOfficeExternalIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccountOfficeIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccountTeamExternalIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAccountTeamIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAffectedResourceCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAirQualityIrradiance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAirQualityOzone.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAirQualityUltraVioletIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAnalyticsDataJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAnalyticsWindowSizeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAnalyzedContent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAnalyzedName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAnswerBindingVariable.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasAnswerToRuleURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasApplicationObjectAccessTypes.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasBinaryAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasBinaryParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasBooleanAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasBooleanParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCentroidLatitude.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCentroidLongitude.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCommandChildEndDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCommandChildReceivedDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCommandChildSentDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCommandEndDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCommandProcessorEndDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      258 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCommandProcessorNotificationChannelURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCommandProcessorReceivedDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCommandProcessorSentDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCommandReceivedDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCommandSentDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCommandStartDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCompassDirectionLabel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCompassDirectionPosition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCompassDirectionSymbol.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasCountyRegionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasDatasetAccessURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasDateTimeAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasDateTimeParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasDefaultRecurrenceTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasDialogProfileURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasDialogResponseTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasDialogText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasDialogURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasDivisionRegionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasDomainMethodContextType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasDoubleAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasDoubleParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasEncryptedAPIKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasEncryptedKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasEntityURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasErrorCode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasEventDetails.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasEventObjectURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasExceptionMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasFIPSCode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasGraphProxyURIList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasGraphResolveTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasGraphTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessLoginTypeClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessReferenceClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessReferenceObjectURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightGraphObjectClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightMessageClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightMessageDirectionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightPropertyClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightRuleTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessViolationDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessViolationTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyContextIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyCountryISOCode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyLimit.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindActionResultTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindAnswerDerivationTree.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindAnswerExplanation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindAppURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindContextIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindInferenceQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindOperationURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindPlanAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindPlanRequestTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindProcessorRequestTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindProcessorResponseTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindQueryAnswerResult.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindQueryErrorCode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindQueryErrorMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindQueryModule.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindQueryParameters.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindQueryStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindResponseStatusTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindServiceMetaQLName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindServiceRequestTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindServiceRuleName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindServiceRuleURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyOffset.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyProcessorRequestStepName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyProcessorStepTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyProgressAmount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyProgressPercentage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyProgressStatusTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyProgressUnitTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyResponseTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyTotalResults.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyWeatherAlertCertaintyURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyWeatherAlertSeverityURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyWeatherMoonPhaseURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasHaleyWeatherWindCompassDirectionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasImplementingGroovyClass.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasImplementingGroovyMethod.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInferenceQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInferenceUpdate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasIntegerAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasIntegerParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountDestinationChannelURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountRecipientAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountRecipientLoginURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountReplyMessageURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountRequestDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountRequestURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountResponseDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountResponseStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountResponseURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountSenderAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountSenderLoginURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountSenderMessageURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountSerializedRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountSerializedResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInterAccountSourceChannelURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      254 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInvocationGraphDataManagementTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasInvocationToRuleURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasKeySubject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasKeySubjectIdentity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasKnowledgeGraphID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasLastAttemptTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListBinaryAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListBinaryParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListBooleanAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListBooleanParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListDateTimeAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListDateTimeParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListDoubleAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListDoubleParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListIntegerAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListIntegerParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListStringAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListStringParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListURIAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasListURIParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasLoginAccessURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasLoginTypeClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasLoginUsername.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasMappedEdgeClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasMappedNodeClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasMappedNodeInstanceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasMappingType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasMemberURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasMindResponseStatusMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasNormalizedText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasOfficeAccessURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressCity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressCountry.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressCounty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressLine1.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressLine2.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressPostalCode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressProvince.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressState.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasOfficeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasOriginDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasOriginURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      192 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasOwner.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasParameterBindingVariable.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasPayloadMessageURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasPermitStreamingAgentInstallURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasPermitStreamingRequestURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasPermitStreamingTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasPostalAbbreviation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasPostalCode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasPostalCodePlusFour.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProcessorCommandConsumerID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProcessorCommandConsumerPartition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      276 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProcessorCommandConsumerPartitionAssignmentList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProcessorCommandEndDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProcessorCommandReceivedDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProcessorCommandSentDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProcessorRequestURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofAnswerTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofConclusionExplanation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofDecisionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationAnswerTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationGoal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationIteration.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationReasonTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationResult.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationRuleIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationRuleMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofPrimaryGoalURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofReasonResult.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofTertiaryGoalURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofTreeAskNodeOriginURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofTreeDependencyNodeOriginURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofTreeNodeIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasProofTreeRuleName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasQueryToRuleURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonComparatorTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintFunctionName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintInputValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintInstanceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintKeyName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintMLModelName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintPropertyURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintValueClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintValueDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonEncoding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonParse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonProvenanceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonReferenceInstanceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReasonReferenceTimestamp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRecentRegionPopulation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRecentRegionPopulationYear.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReferenceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasReportURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRequestChannelHistory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRequestMessageResponseSerialized.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRequestMessageSerialized.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRequestOrder.py
--rw-r--r--   0 hadfield   (501) staff       (20)      258 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRequestOriginMessageResponseSerialized.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRequestOriginMessageSerialized.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRequestResponseTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasResourceFilePath.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasResourceVersion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRespondingToClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasResponseChannelURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasResultSequence.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRoleGrantAspectURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRoleGrantExtentURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRoleGrantTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleInvocationURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleMetaQLObjectCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleMetaQLParameterMap.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleMetaQLQueryName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleMetaQLTimestamp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleMethod.py
--rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterClassRestrictionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterModeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterResolveObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterResolveObjectGraph.py
--rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterResolveObjectList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleProvenanceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasRuleURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasScheduledExecutionTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasStringAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasStringParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasSymmetricCryptoKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      254 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasSymmetricCryptoKeyGenerationDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasSymmetricCryptoKeyIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasTableData.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasTeamAccessURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasTeamURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasTimeZoneIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasURIAnswerBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasURIParameterBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherAirPressure.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherAlertDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherAlertEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherAlertExpiration.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherAlertHeadline.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherAlertOnset.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherAlertSender.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherCloudCover.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherDewPoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherElevation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherFeelsLikeTemperature.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherHumidity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherMoonRise.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherMoonSet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherPrecipitationTotal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherPrecipitationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportIcon.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportIconInteger.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportLatitude.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportLongitude.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportSummary.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportTimeZoneIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportUnits.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherSunrise.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherSunset.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherTemperature.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherTypeDescriptor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherTypeIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherTypeLargeIconPath.py
--rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherTypeMediumIconPath.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherTypeSmallIconPath.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherVisibility.py
--rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWeatherWindChill.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWikiDataID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWikiURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWindAngle.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWindDirection.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_hasWindSpeed.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_isEnableEcho.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_isFinalJustification.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_isGenerateExemplar.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_isHaleyTestCase.py
--rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_isStatusOk.py
--rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_isTopPriority.py
--rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/Property_isWeatherReportHistorical.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:35:40.000000 vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/properties/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-04 22:26:33.911427 vital-ai-haley-0.1.3/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      892 2024-05-04 22:24:21.000000 vital-ai-haley-0.1.3/setup.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 22:26:33.910738 vital-ai-haley-0.1.3/vital_ai_haley.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      485 2024-05-04 22:26:33.000000 vital-ai-haley-0.1.3/vital_ai_haley.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)    58913 2024-05-04 22:26:33.000000 vital-ai-haley-0.1.3/vital_ai_haley.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-04 22:26:33.000000 vital-ai-haley-0.1.3/vital_ai_haley.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       74 2024-05-04 22:26:33.000000 vital-ai-haley-0.1.3/vital_ai_haley.egg-info/entry_points.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       21 2024-05-04 22:26:33.000000 vital-ai-haley-0.1.3/vital_ai_haley.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       25 2024-05-04 22:26:33.000000 vital-ai-haley-0.1.3/vital_ai_haley.egg-info/top_level.txt
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:51:29.896907 vital-ai-haley-0.1.4/
+-rw-r--r--   0 hadfield   (501) staff       (20)      485 2024-05-06 21:51:29.896659 vital-ai-haley-0.1.4/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:53:31.000000 vital-ai-haley-0.1.4/README.md
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:51:29.768317 vital-ai-haley-0.1.4/com_vitalai_haley_domain/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:35:40.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:51:29.842874 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/AgentDeveloper.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/AgentDeveloper.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Customer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Customer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1434 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/DialogTask.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/DialogTask.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/DomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1541 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasAccountDataSharedWith.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasAccountDataSharedWith.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2172 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessAccountRole.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      442 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessAccountRole.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2160 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessBotRole.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      438 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessBotRole.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2166 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessLoginRole.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      440 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessLoginRole.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessOfficePolicy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessOfficePolicy.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessOfficeRole.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessOfficeRole.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessPolicy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessPolicy.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1608 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRight.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRight.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightContext.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightContext.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1458 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightGraphObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightGraphObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1446 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightProperty.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessTeamPolicy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessTeamPolicy.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessTeamRole.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessTeamRole.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOffice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOffice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOfficeLocation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOfficeLocation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOfficeMember.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOfficeMember.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountTeam.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountTeam.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountTeamMember.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountTeamMember.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaActionCondition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaActionCondition.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1334 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaActionSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaActionSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaCondition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaCondition.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaGoalCondition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      161 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaGoalCondition.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaPartialGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaPartialGoal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaPrimaryGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaPrimaryGoal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaStep.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaStep.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPartialGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPartialGoal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionCondition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      161 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionCondition.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1373 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstanceDestination.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      171 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstanceDestination.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1358 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstanceSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstanceSource.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanCondition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanCondition.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanLevel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanLevel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanStep.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanStep.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPrimaryGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPrimaryGoal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindQueryAnswer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindQueryAnswer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindQueryAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindQueryAnswerBinding.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindRuleParameter.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindRuleParameter.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1346 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindRuleParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindRuleParameterBinding.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyOriginRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyOriginRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyReport.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyReport.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherAlert.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherAlert.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherDailyReport.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherDailyReport.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherHourlyReport.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherHourlyReport.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherMinutelyReport.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherMinutelyReport.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasProofJustificationReason.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasProofJustificationReason.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1403 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasProofTreeNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasProofTreeNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1268 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/GlobalManager.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/GlobalManager.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1658 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAPIKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAPIKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1400 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessAccountPolicyRule.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessAccountPolicyRule.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessAccountRole.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessAccountRole.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessBotRole.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessBotRole.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1853 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessGrant.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      289 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessGrant.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessGrantStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessGrantStatus.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessGrantType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessGrantType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1494 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessLoginPolicyRule.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      186 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessLoginPolicyRule.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessLoginRole.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessLoginRole.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessLoginType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessLoginType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1313 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessOfficePolicy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessOfficePolicy.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessOfficeRole.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessOfficeRole.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessPolicy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessPolicy.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1589 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRight.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRight.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1398 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightContext.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightContext.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1633 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightGraphObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      254 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightGraphObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1617 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightMessageDirection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightMessageDirection.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightMessageRule.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightMessageRule.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1621 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightProperty.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightPropertyRule.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightPropertyRule.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightRuleType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightRuleType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRoleGrantAspect.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRoleGrantAspect.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRoleGrantExtent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRoleGrantExtent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRoleGrantType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRoleGrantType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRoleScope.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRoleScope.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessTeamPolicy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessTeamPolicy.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessTeamRole.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessTeamRole.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessViolationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessViolationType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccount.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1433 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountDataShareFilterRule.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountDataShareFilterRule.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountDataShareScope.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountDataShareScope.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1498 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountOffice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountOffice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountOfficeLocation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      456 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountOfficeLocation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1488 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountTeam.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountTeam.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAirQualityReport.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAirQualityReport.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1495 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAnalyticsContainer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      190 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAnalyticsContainer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAnalyticsWindowSize.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAnalyticsWindowSize.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1553 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAppEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAppEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1552 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCanadianProvinceOrTerritory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCanadianProvinceOrTerritory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCelestialBody.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCelestialBody.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1285 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyChannelAnswer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyChannelAnswer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyChannelQuestion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyChannelQuestion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1452 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      174 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCollection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCollection.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCommandGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCommandGroup.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCommandStateType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCommandStateType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1607 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCompassDirection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCompassDirection.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1466 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCountry.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCountry.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1286 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCountryDivision.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCountryDivision.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1653 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCryptoKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCryptoKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1355 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDataTable.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDataTable.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1967 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDialogMapping.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      324 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDialogMapping.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDialogMappingType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDialogMappingType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDialogResponseType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDialogResponseType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDialogRouteType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDialogRouteType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDocGenProcessorRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDocGenProcessorRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1594 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDomainMethod.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDomainMethod.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDomainMethodContextType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDomainMethodContextType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1472 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyFileResource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyFileResource.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1436 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyGraph.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyGraph.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1393 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyGraphContainerProxy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyGraphContainerProxy.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyGraphType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyGraphType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyHandlerErrorType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyHandlerErrorType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyHandlerValidationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyHandlerValidationType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     3232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyIntentCommand.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      880 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyIntentCommand.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyInterAccountNotification.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyInterAccountNotification.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2966 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyInterAccountRecord.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      761 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyInterAccountRecord.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyInterAccountRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyInterAccountRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyInterAccountResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyInterAccountResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMailingList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMailingList.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMailingListEntity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMailingListEntity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1392 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindActionResult.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindActionResult.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindActionResultType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindActionResultType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgenda.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgenda.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaActionCondition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaActionCondition.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaActionSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaActionSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaCondition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaCondition.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaGoal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaGoalCondition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaGoalCondition.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaPartialGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaPartialGoal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1328 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaPrimaryGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaPrimaryGoal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaStep.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaStep.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1254 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindApp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindApp.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAskMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAskMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAskPlanAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAskPlanAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1286 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindBotEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindBotEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindBotPlanAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindBotPlanAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindCommandAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindCommandAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1854 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindContext.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindContext.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindDatascriptPlanAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindDatascriptPlanAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindGoal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindInferenceType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindInferenceType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2002 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindMetaQLDataset.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      347 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindMetaQLDataset.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1439 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindMetaQLQueryOperation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindMetaQLQueryOperation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindOperation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindOperation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindOperationResult.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindOperationResult.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPartialGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPartialGoal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlan.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlan.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanActionCondition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanActionCondition.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1401 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanActionInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanActionInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanActionSlot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanActionSlot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanCondition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanCondition.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanGoalCondition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanGoalCondition.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanLevel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanLevel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1388 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      161 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanRequestType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanRequestType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanStep.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanStep.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPredictionPlanAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPredictionPlanAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPrimaryGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPrimaryGoal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1334 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorPlanAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorPlanAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2298 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      494 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorRequestType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorRequestType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1914 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      318 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorResponseType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorResponseType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2108 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      394 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1716 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindQueryAnswer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      273 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindQueryAnswer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2908 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindQueryAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      670 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindQueryAnswerBinding.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindQueryStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindQueryStatus.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindReceiveMessagePlanAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindReceiveMessagePlanAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRecommendationPlanAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRecommendationPlanAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     3118 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      855 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     3332 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      922 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindResponseStatusType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindResponseStatusType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1455 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRule.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRule.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleGraphResolveType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleGraphResolveType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1606 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleInvocation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleInvocation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleInvocationGraphDataManagementType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleInvocationGraphDataManagementType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2161 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleParameter.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      431 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleParameter.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2959 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      717 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleParameterBinding.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleParameterMode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleParameterMode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleParameterType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleParameterType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1340 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindSendMessagePlanAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindSendMessagePlanAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindServiceRequestType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindServiceRequestType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTaskEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTaskEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTaskPlanAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTaskPlanAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTellMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTellMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTellPlanAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTellPlanAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTickRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTickRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindUserEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindUserEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyNaturalPlanetarySatellite.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyNaturalPlanetarySatellite.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyNotification.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyNotification.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyObjectAccessType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyObjectAccessType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1463 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyPermitStreamingResponseMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyPermitStreamingResponseMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyPlace.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyPlace.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyPlanet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyPlanet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1504 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProcessorRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProcessorRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProcessorStepType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProcessorStepType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProgressStatusType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProgressStatusType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProgressUnitType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProgressUnitType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1350 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProvenance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProvenance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1678 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRegion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRegion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1429 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRelayResponseMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      188 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRelayResponseMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRelayStatusMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRelayStatusMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyReport.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      115 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyReport.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1827 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyReportInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyReportInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2324 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      467 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRequestGraph.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRequestGraph.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     3034 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRequestMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      834 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRequestMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRequestResponseType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRequestResponseType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     4208 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyResponseMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1225 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyResponseMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyResponseType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyResponseType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1707 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyResultMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      261 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyResultMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyStar.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyStar.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1629 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleySymmetricCryptoKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleySymmetricCryptoKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2155 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyTask.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      365 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyTask.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1459 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyUSCounty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      174 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyUSCounty.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1879 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyUSPostalRegion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      297 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyUSPostalRegion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1525 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyUSStateOrTerritory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyUSStateOrTerritory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1464 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyUserEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyUserEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherAlert.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      413 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherAlert.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherAlertCertainty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherAlertCertainty.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherAlertSeverity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherAlertSeverity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1405 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherDailyReport.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherDailyReport.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1408 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherHourlyReport.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherHourlyReport.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherMinutelyReport.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherMinutelyReport.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherMoonPhase.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherMoonPhase.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     4744 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherReport.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherReport.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1807 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      296 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2031 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HyperEdge_hasAccessGrant.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      382 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HyperEdge_hasAccessGrant.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HyperEdge_hasHaleyMindRuleGraphMembership.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HyperEdge_hasHaleyMindRuleGraphMembership.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1317 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HyperEdge_hasReferenceObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HyperEdge_hasReferenceObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1533 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/PermitStreamingRequestMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/PermitStreamingRequestMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/PermitStreamingType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/PermitStreamingType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofAnswerType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofAnswerType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofDecision.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofDecision.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1245 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofGoal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationAnswerType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationAnswerType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     3586 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationReason.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      934 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationReason.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1332 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationReasonComparatorType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationReasonComparatorType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationReasonType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationReasonType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1268 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofPrimaryGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofPrimaryGoal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofProgressType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofProgressType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofSpecialValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofSpecialValue.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTertiaryGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTertiaryGoal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1458 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTree.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTree.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1517 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeAncestorNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeAncestorNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1502 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeAskNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeAskNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1818 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeConclusionNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      306 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeConclusionNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1639 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeDependencyNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      261 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeDependencyNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1289 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeDeriveNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeDeriveNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeJustificationNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      462 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeJustificationNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1469 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      184 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Seller.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Seller.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:35:40.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:51:29.895546 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAPIKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAPIKeyIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAPIKeySessionKeyIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantMemberURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantOutcomeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantProviderAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantProviderBot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantProviderLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantRoleOutcomeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessGrantType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessObjectTypes.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessOutcomeSerialized.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessRightChannelContextURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeBotURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeChannelURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeDatasetURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeLoginURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeOfficeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeTeamURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccessRoleScopeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccountClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      254 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccountDataShareFilterRuleIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccountDataShareFilterRuleURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccountDataShareScopeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccountObjectAccessTypes.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccountOfficeExternalIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccountOfficeIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccountTeamExternalIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAccountTeamIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAffectedResourceCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAirQualityIrradiance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAirQualityOzone.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAirQualityUltraVioletIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAnalyticsDataJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAnalyticsWindowSizeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAnalyzedContent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAnalyzedName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAnswerBindingVariable.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasAnswerToRuleURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasApplicationObjectAccessTypes.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasBinaryAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasBinaryParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasBooleanAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasBooleanParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCentroidLatitude.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCentroidLongitude.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCommandChildEndDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCommandChildReceivedDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCommandChildSentDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCommandEndDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCommandProcessorEndDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      258 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCommandProcessorNotificationChannelURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCommandProcessorReceivedDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCommandProcessorSentDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCommandReceivedDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCommandSentDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCommandStartDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCompassDirectionLabel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCompassDirectionPosition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCompassDirectionSymbol.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasCountyRegionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasDatasetAccessURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasDateTimeAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasDateTimeParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasDefaultRecurrenceTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasDialogProfileURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasDialogResponseTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasDialogText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasDialogURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasDivisionRegionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasDomainMethodContextType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasDoubleAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasDoubleParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasEncryptedAPIKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasEncryptedKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasEntityURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasErrorCode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasEventDetails.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasEventObjectURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasExceptionMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasFIPSCode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasGraphProxyURIList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasGraphResolveTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasGraphTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessLoginTypeClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessReferenceClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessReferenceObjectURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightGraphObjectClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightMessageClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightMessageDirectionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightPropertyClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightRuleTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessRightURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessViolationDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyAccessViolationTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyContextIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyCountryISOCode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyLimit.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindActionResultTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindAnswerDerivationTree.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindAnswerExplanation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindAppURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindContextIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindInferenceQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindOperationURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindPlanAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindPlanRequestTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindProcessorRequestTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindProcessorResponseTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindQueryAnswerResult.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindQueryErrorCode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindQueryErrorMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindQueryModule.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindQueryParameters.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindQueryStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindResponseStatusTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindServiceMetaQLName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindServiceRequestTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindServiceRuleName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyMindServiceRuleURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyOffset.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyProcessorRequestStepName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyProcessorStepTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyProgressAmount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyProgressPercentage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyProgressStatusTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyProgressUnitTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyResponseTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyTotalResults.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyWeatherAlertCertaintyURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyWeatherAlertSeverityURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyWeatherMoonPhaseURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasHaleyWeatherWindCompassDirectionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasImplementingGroovyClass.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasImplementingGroovyMethod.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInferenceQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInferenceUpdate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasIntegerAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasIntegerParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountDestinationChannelURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountRecipientAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountRecipientLoginURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountReplyMessageURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountRequestDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountRequestURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountResponseDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountResponseStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountResponseURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountSenderAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountSenderLoginURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountSenderMessageURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountSerializedRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountSerializedResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInterAccountSourceChannelURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      254 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInvocationGraphDataManagementTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasInvocationToRuleURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasKeySubject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasKeySubjectIdentity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasKnowledgeGraphID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasLastAttemptTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListBinaryAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListBinaryParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListBooleanAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListBooleanParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListDateTimeAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListDateTimeParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListDoubleAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListDoubleParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListIntegerAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListIntegerParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListStringAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListStringParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListURIAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasListURIParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasLoginAccessURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasLoginTypeClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasLoginUsername.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasMappedEdgeClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasMappedNodeClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasMappedNodeInstanceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasMappingType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasMemberURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasMindResponseStatusMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasNormalizedText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasOfficeAccessURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressCity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressCountry.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressCounty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressLine1.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressLine2.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressPostalCode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressProvince.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasOfficeLocationAddressState.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasOfficeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasOriginDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasOriginURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      192 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasOwner.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasParameterBindingVariable.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasPayloadMessageURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasPermitStreamingAgentInstallURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasPermitStreamingRequestURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasPermitStreamingTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasPostalAbbreviation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasPostalCode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasPostalCodePlusFour.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProcessorCommandConsumerID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProcessorCommandConsumerPartition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      276 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProcessorCommandConsumerPartitionAssignmentList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProcessorCommandEndDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProcessorCommandReceivedDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProcessorCommandSentDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProcessorRequestURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofAnswerTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofConclusionExplanation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofDecisionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationAnswerTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationGoal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationIteration.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationReasonTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationResult.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationRuleIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationRuleMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofJustificationTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofPrimaryGoalURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofReasonResult.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofTertiaryGoalURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofTreeAskNodeOriginURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      248 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofTreeDependencyNodeOriginURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofTreeNodeIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasProofTreeRuleName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasQueryToRuleURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonComparatorTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintFunctionName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintInputValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintInstanceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintKeyName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintMLModelName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintPropertyURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintValueClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonConstraintValueDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonEncoding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonParse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonProvenanceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonReferenceInstanceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReasonReferenceTimestamp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRecentRegionPopulation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRecentRegionPopulationYear.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReferenceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasReportURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRequestChannelHistory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRequestMessageResponseSerialized.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRequestMessageSerialized.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRequestOrder.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      258 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRequestOriginMessageResponseSerialized.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRequestOriginMessageSerialized.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRequestResponseTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasResourceFilePath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasResourceVersion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRespondingToClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasResponseChannelURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasResultSequence.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRoleGrantAspectURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRoleGrantExtentURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRoleGrantTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleInvocationURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleMetaQLObjectCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleMetaQLParameterMap.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleMetaQLQueryName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleMetaQLTimestamp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleMethod.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      246 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterClassRestrictionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterModeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      234 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterResolveObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterResolveObjectGraph.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      242 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterResolveObjectList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleParameterTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleProvenanceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasRuleURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasScheduledExecutionTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasStringAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasStringParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasSymmetricCryptoKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      254 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasSymmetricCryptoKeyGenerationDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      238 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasSymmetricCryptoKeyIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasTableData.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasTeamAccessURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasTeamURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasTimeZoneIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasURIAnswerBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      220 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasURIParameterBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherAirPressure.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherAlertDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherAlertEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherAlertExpiration.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherAlertHeadline.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherAlertOnset.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherAlertSender.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherCloudCover.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherDewPoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherElevation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherFeelsLikeTemperature.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherHumidity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherMoonRise.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherMoonSet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherPrecipitationTotal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherPrecipitationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportIcon.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportIconInteger.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportLatitude.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportLongitude.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportSummary.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportTimeZoneIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherReportUnits.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherSunrise.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherSunset.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherTemperature.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherTypeDescriptor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherTypeIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherTypeLargeIconPath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      232 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherTypeMediumIconPath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherTypeSmallIconPath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherVisibility.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      214 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWeatherWindChill.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWikiDataID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWikiURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWindAngle.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWindDirection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_hasWindSpeed.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_isEnableEcho.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_isFinalJustification.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_isGenerateExemplar.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_isHaleyTestCase.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_isStatusOk.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      202 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_isTopPriority.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      226 2024-05-04 22:21:49.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/Property_isWeatherReportHistorical.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 16:35:40.000000 vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/properties/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-06 21:51:29.896950 vital-ai-haley-0.1.4/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)      892 2024-05-06 21:50:17.000000 vital-ai-haley-0.1.4/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:51:29.896350 vital-ai-haley-0.1.4/vital_ai_haley.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      485 2024-05-06 21:51:29.000000 vital-ai-haley-0.1.4/vital_ai_haley.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)    58913 2024-05-06 21:51:29.000000 vital-ai-haley-0.1.4/vital_ai_haley.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-06 21:51:29.000000 vital-ai-haley-0.1.4/vital_ai_haley.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       74 2024-05-06 21:51:29.000000 vital-ai-haley-0.1.4/vital_ai_haley.egg-info/entry_points.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       21 2024-05-06 21:51:29.000000 vital-ai-haley-0.1.4/vital_ai_haley.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       25 2024-05-06 21:51:29.000000 vital-ai-haley-0.1.4/vital_ai_haley.egg-info/top_level.txt
```

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/AgentDeveloper.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/AgentDeveloper.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Customer.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Customer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/DialogTask.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/DialogTask.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasAccountDataSharedWith.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasAccountDataSharedWith.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessAccountRole.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessAccountRole.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessBotRole.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessBotRole.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessLoginRole.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessLoginRole.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessOfficePolicy.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessOfficePolicy.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessOfficeRole.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessOfficeRole.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessPolicy.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessPolicy.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRight.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRight.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightContext.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightContext.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightGraphObject.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightGraphObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightMessage.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightProperty.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessRightProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessTeamPolicy.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessTeamPolicy.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccessTeamRole.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccessTeamRole.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOffice.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOffice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOfficeLocation.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOfficeLocation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOfficeMember.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountOfficeMember.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountTeam.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountTeam.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyAccountTeamMember.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyAccountTeamMember.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaActionCondition.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaActionCondition.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaActionSlot.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaActionSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaCondition.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaCondition.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaGoalCondition.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaGoalCondition.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaPartialGoal.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaPartialGoal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaPrimaryGoal.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaPrimaryGoal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaStep.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindAgendaStep.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPartialGoal.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPartialGoal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionCondition.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionCondition.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstance.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstanceDestination.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstanceDestination.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstanceSource.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionInstanceSource.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionSlot.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanActionSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanCondition.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanCondition.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanLevel.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanLevel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanStep.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPlanStep.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindPrimaryGoal.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindPrimaryGoal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindQueryAnswer.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindQueryAnswer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindQueryAnswerBinding.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindQueryAnswerBinding.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindRuleParameter.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindRuleParameter.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyMindRuleParameterBinding.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyMindRuleParameterBinding.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyOriginRequest.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyOriginRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyReport.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyReport.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyRequest.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherAlert.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherAlert.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherDailyReport.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherDailyReport.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherHourlyReport.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherHourlyReport.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherMinutelyReport.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasHaleyWeatherMinutelyReport.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasProofJustificationReason.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasProofJustificationReason.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Edge_hasProofTreeNode.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Edge_hasProofTreeNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/GlobalManager.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/GlobalManager.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAPIKey.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAPIKey.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessAccountPolicyRule.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessAccountPolicyRule.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessAccountRole.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessAccountRole.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessBotRole.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessBotRole.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessGrant.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessGrant.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessGrantStatus.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessGrantStatus.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessGrantType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessGrantType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessLoginPolicyRule.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessLoginPolicyRule.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessLoginRole.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessLoginRole.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessLoginType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessLoginType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessOfficePolicy.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessOfficePolicy.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessOfficeRole.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessOfficeRole.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessPolicy.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessPolicy.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRight.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRight.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightContext.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightContext.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightGraphObject.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightGraphObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightMessage.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightMessageDirection.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightMessageDirection.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightMessageRule.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightMessageRule.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightProperty.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightPropertyRule.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightPropertyRule.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightRuleType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightRuleType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRightType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRightType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRoleGrantAspect.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRoleGrantAspect.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRoleGrantExtent.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRoleGrantExtent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRoleGrantType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRoleGrantType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessRoleScope.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessRoleScope.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessTeamPolicy.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessTeamPolicy.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessTeamRole.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessTeamRole.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccessViolationType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccessViolationType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccount.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccount.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountDataShareFilterRule.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountDataShareFilterRule.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountDataShareScope.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountDataShareScope.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountOffice.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountOffice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountOfficeLocation.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountOfficeLocation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAccountTeam.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAccountTeam.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAirQualityReport.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAirQualityReport.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAnalyticsContainer.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAnalyticsContainer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAnalyticsWindowSize.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAnalyticsWindowSize.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyAppEvent.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyAppEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCanadianProvinceOrTerritory.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCanadianProvinceOrTerritory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCelestialBody.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCelestialBody.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyChannelAnswer.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyChannelAnswer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyChannelQuestion.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyChannelQuestion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCity.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCollection.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCollection.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCommandGroup.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCommandGroup.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCommandStateType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCommandStateType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCompassDirection.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCompassDirection.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCountry.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCountry.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCountryDivision.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCountryDivision.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyCryptoKey.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyCryptoKey.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDataTable.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDataTable.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDialogMapping.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDialogMapping.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDialogMappingType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDialogMappingType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDialogResponseType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDialogResponseType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDialogRouteType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDialogRouteType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDocGenProcessorRequest.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDocGenProcessorRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDomainMethod.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDomainMethod.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyDomainMethodContextType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyDomainMethodContextType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyFileResource.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyFileResource.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyGraph.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyGraph.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyGraphContainerProxy.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyGraphContainerProxy.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyGraphType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyGraphType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyHandlerErrorType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyHandlerErrorType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyHandlerValidationType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyHandlerValidationType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyIntentCommand.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyIntentCommand.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyIntentCommand.pyi` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyIntentCommand.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyInterAccountNotification.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyInterAccountNotification.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyInterAccountRecord.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyInterAccountRecord.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyInterAccountRecord.pyi` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyInterAccountRecord.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyInterAccountRequest.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyInterAccountRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyInterAccountResponse.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyInterAccountResponse.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMailingList.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMailingList.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMailingListEntity.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMailingListEntity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindActionResult.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindActionResult.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindActionResultType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindActionResultType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgenda.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgenda.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaActionCondition.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaActionCondition.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaActionSlot.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaActionSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaCondition.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaCondition.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaGoal.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaGoal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaGoalCondition.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaGoalCondition.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaPartialGoal.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaPartialGoal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaPrimaryGoal.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaPrimaryGoal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAgendaStep.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAgendaStep.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindApp.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindApp.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAskMessage.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAskMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindAskPlanAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindAskPlanAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindBotEvent.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindBotEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindBotPlanAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindBotPlanAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindCommandAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindCommandAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindContext.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindContext.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindDatascriptPlanAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindDatascriptPlanAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindEvent.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindGoal.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindGoal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindInferenceType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindInferenceType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindMessage.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindMetaQLDataset.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindMetaQLDataset.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindMetaQLQueryOperation.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindMetaQLQueryOperation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindOperation.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindOperation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindOperationResult.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindOperationResult.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPartialGoal.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPartialGoal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlan.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlan.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanActionCondition.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanActionCondition.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanActionInstance.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanActionInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanActionSlot.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanActionSlot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanCondition.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanCondition.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanGoalCondition.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanGoalCondition.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanInstance.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanLevel.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanLevel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanRequest.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanRequestType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanRequestType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPlanStep.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPlanStep.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPredictionPlanAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPredictionPlanAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindPrimaryGoal.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindPrimaryGoal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorPlanAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorPlanAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorRequest.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorRequestType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorRequestType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorResponse.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorResponse.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindProcessorResponseType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindProcessorResponseType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindQuery.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindQuery.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindQueryAnswer.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindQueryAnswer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindQueryAnswerBinding.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindQueryAnswerBinding.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindQueryAnswerBinding.pyi` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindQueryAnswerBinding.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindQueryStatus.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindQueryStatus.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindReceiveMessagePlanAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindReceiveMessagePlanAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRecommendationPlanAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRecommendationPlanAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRequest.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRequest.pyi` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRequest.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindResponse.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindResponse.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindResponse.pyi` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindResponse.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindResponseStatusType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindResponseStatusType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRule.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRule.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleGraphResolveType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleGraphResolveType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleInvocation.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleInvocation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleInvocationGraphDataManagementType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleInvocationGraphDataManagementType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleParameter.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleParameter.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleParameterBinding.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleParameterBinding.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleParameterBinding.pyi` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleParameterBinding.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleParameterMode.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleParameterMode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindRuleParameterType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindRuleParameterType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindSendMessagePlanAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindSendMessagePlanAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindServiceRequestType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindServiceRequestType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTaskEvent.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTaskEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTaskPlanAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTaskPlanAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTellMessage.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTellMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTellPlanAction.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTellPlanAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindTickRequest.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindTickRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyMindUserEvent.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyMindUserEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyNaturalPlanetarySatellite.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyNaturalPlanetarySatellite.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyNotification.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyNotification.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyObjectAccessType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyObjectAccessType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyPermitStreamingResponseMessage.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyPermitStreamingResponseMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyPlace.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyPlace.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyPlanet.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyPlanet.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProcessorRequest.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProcessorRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProcessorStepType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProcessorStepType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProgressStatusType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProgressStatusType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProgressUnitType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProgressUnitType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyProvenance.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyProvenance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRegion.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRegion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRelayResponseMessage.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRelayResponseMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRelayStatusMessage.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRelayStatusMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyReport.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyReport.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyReportInstance.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyReportInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRequest.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRequestGraph.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRequestGraph.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRequestMessage.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRequestMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRequestMessage.pyi` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRequestMessage.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyRequestResponseType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyRequestResponseType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyResponseMessage.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyResponseMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyResponseMessage.pyi` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyResponseMessage.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyResponseType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyResponseType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyResultMessage.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyResultMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyStar.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyStar.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleySymmetricCryptoKey.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleySymmetricCryptoKey.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyTask.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyTask.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyUSCounty.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyUSCounty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyUSPostalRegion.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyUSPostalRegion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyUSStateOrTerritory.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyUSStateOrTerritory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyUserEvent.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyUserEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherAlert.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherAlert.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherAlertCertainty.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherAlertCertainty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherAlertSeverity.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherAlertSeverity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherDailyReport.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherDailyReport.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherHourlyReport.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherHourlyReport.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherMinutelyReport.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherMinutelyReport.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherMoonPhase.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherMoonPhase.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherReport.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherReport.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherReport.pyi` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherReport.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HaleyWeatherType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HaleyWeatherType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HyperEdge_hasAccessGrant.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HyperEdge_hasAccessGrant.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HyperEdge_hasHaleyMindRuleGraphMembership.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HyperEdge_hasHaleyMindRuleGraphMembership.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/HyperEdge_hasReferenceObject.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/HyperEdge_hasReferenceObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/PermitStreamingRequestMessage.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/PermitStreamingRequestMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/PermitStreamingType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/PermitStreamingType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofAnswerType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofAnswerType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofDecision.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofDecision.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofGoal.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofGoal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationAnswerType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationAnswerType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationReason.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationReason.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationReason.pyi` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationReason.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationReasonComparatorType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationReasonComparatorType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationReasonType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationReasonType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofJustificationType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofJustificationType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofPrimaryGoal.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofPrimaryGoal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofProgressType.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofProgressType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofSpecialValue.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofSpecialValue.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTertiaryGoal.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTertiaryGoal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTree.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTree.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeAncestorNode.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeAncestorNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeAskNode.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeAskNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeConclusionNode.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeConclusionNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeDependencyNode.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeDependencyNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeDeriveNode.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeDeriveNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeJustificationNode.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeJustificationNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/ProofTreeNode.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/ProofTreeNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/com_vitalai_haley_domain/model/Seller.py` & `vital-ai-haley-0.1.4/com_vitalai_haley_domain/model/Seller.py`

 * *Files identical despite different names*

### Comparing `vital-ai-haley-0.1.3/setup.py` & `vital-ai-haley-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vital-ai-haley',
-    version='0.1.3',
+    version='0.1.4',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='VitalSigns haley domain',
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
-            'vital-ai-aimp==0.1.3',
+            'vital-ai-aimp>=0.1.4',
         ],
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.10',
```

### Comparing `vital-ai-haley-0.1.3/vital_ai_haley.egg-info/SOURCES.txt` & `vital-ai-haley-0.1.4/vital_ai_haley.egg-info/SOURCES.txt`

 * *Files identical despite different names*

