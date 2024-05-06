# Comparing `tmp/vital-ai-aimp-0.1.3.tar.gz` & `tmp/vital-ai-aimp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-ai-aimp-0.1.3.tar", last modified: Sat May  4 21:34:18 2024, max compression
+gzip compressed data, was "vital-ai-aimp-0.1.4.tar", last modified: Mon May  6 21:49:09 2024, max compression
```

## Comparing `vital-ai-aimp-0.1.3.tar` & `vital-ai-aimp-0.1.4.tar`

### file list

```diff
@@ -1,1852 +1,1852 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:34:18.011744 vital-ai-aimp-0.1.3/
--rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-02-06 19:34:55.000000 vital-ai-aimp-0.1.3/LICENSE
--rw-r--r--   0 hadfield   (501) staff       (20)      596 2024-05-04 21:34:18.011472 vital-ai-aimp-0.1.3/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)       16 2024-02-06 19:49:29.000000 vital-ai-aimp-0.1.3/README.md
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:34:17.552503 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:22.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:34:17.873663 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/
--rw-r--r--   0 hadfield   (501) staff       (20)     1557 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      185 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPDevice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPEmailMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPEmailMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     6757 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1579 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1368 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPMessageDef.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPMessageDef.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPMessageFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPMessageFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1388 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPMessagePayloadDef.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPMessagePayloadDef.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1250 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPThing.py
--rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPThing.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1254 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/APIEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/APIEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1228 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/APILogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)       97 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/APILogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1903 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      314 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountEventType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountEventType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountInteraction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountInteraction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1531 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountInteractionPart.py
--rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountInteractionPart.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1589 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountInteractionTransaction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountInteractionTransaction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1750 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      292 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1767 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      299 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityEventType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityEventType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1804 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityInvitation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      323 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityInvitation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityInvitationStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityInvitationStatus.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1523 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityMember.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityMember.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityStatus.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1981 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountResourceLock.py
--rw-r--r--   0 hadfield   (501) staff       (20)      373 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountResourceLock.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountResourceLockStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountResourceLockStatus.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountResourceLockType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountResourceLockType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountResourceType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountResourceType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountStatus.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ActivateMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ActivateMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2010 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ActivityCard.py
--rw-r--r--   0 hadfield   (501) staff       (20)      328 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ActivityCard.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AdUnitEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AdUnitEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1338 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Agent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Agent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1277 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentConfiguration.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentConfiguration.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1886 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentDatascriptCallRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentDatascriptCallRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2495 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentDatascriptCallResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      405 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentDatascriptCallResponse.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1254 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentError.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentError.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1681 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentImage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentImage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1259 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstall.py
--rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstall.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstallConfiguration.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstallConfiguration.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstanceDeployment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstanceDeployment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1523 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstanceMessageDeployment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      192 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstanceMessageDeployment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1529 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstancePayloadDeployment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstancePayloadDeployment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentMedia.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentMedia.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentMessagePayloadType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentMessagePayloadType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentMessageType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentMessageType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1736 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentPolicy.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentPolicy.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1465 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentStatusRequest.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentStatusRequest.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1767 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentStatusResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentStatusResponse.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1459 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentText.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1250 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentVideo.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentVideo.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1466 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaAccount.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1365 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaDevice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1362 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1327 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1375 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AmazonEchoAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AmazonEchoAccount.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1339 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnonymousLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnonymousLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnonymousProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnonymousProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1637 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Answer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Answer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1363 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerChoice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerChoice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2410 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      422 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1849 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerRealtimeUpdateMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      290 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerRealtimeUpdateMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2102 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerStatusMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      329 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerStatusMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2425 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerUnsetMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      427 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerUnsetMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1905 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerUpdateMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      285 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerUpdateMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ApnsEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ApnsEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2180 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ArticleObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      347 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ArticleObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1436 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Asset.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Asset.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1495 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AssetConditionMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      182 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AssetConditionMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1397 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AssetLocationMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AssetLocationMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AssetMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AssetMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Audio.py
--rw-r--r--   0 hadfield   (501) staff       (20)      102 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Audio.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2369 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AudioObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      388 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AudioObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BB8Device.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BB8Device.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BaseInteraction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BaseInteraction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BaseInteractionPart.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BaseInteractionPart.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BaseInteractionTransaction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BaseInteractionTransaction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1452 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BaseProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BaseProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BinaryMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BinaryMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BooleanPropertyFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BooleanPropertyFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1759 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Bot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Bot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1947 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BridgeSessionMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      330 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BridgeSessionMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BuilderClassBot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BuilderClassBot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BuilderDesignerBot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BuilderDesignerBot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1358 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BuilderStringBot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BuilderStringBot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1726 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Button.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Button.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1484 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ButtonClickedMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ButtonClickedMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1938 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ButtonStateMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      320 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ButtonStateMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1248 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Calendar.py
--rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Calendar.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1571 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarEntry.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarEntry.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1879 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      102 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1553 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1422 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CancelCommandMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      185 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CancelCommandMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1438 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Card.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Card.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2595 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Channel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      471 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Channel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1393 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelClosedMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelClosedMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2521 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelHistoryResponseMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      423 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelHistoryResponseMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelViewLeftMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelViewLeftMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelViewSwitchedMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelViewSwitchedMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1527 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Chart.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Chart.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1245 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatDialog.py
--rw-r--r--   0 hadfield   (501) staff       (20)      110 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatDialog.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1365 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1374 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatModeMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatModeMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1664 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatRule.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatRule.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatRuleSet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatRuleSet.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1360 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatRuleSetFile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatRuleSetFile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1351 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CheckItem.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CheckItem.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1236 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CheckList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      103 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CheckList.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1946 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Choice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      275 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Choice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1251 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChoiceAnswer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      112 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChoiceAnswer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1358 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ClearChatHistory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ClearChatHistory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1444 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CloseIFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CloseIFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1402 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ClosePanelCommand.py
--rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ClosePanelCommand.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CloseSessionMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CloseSessionMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1370 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CommandMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CommandMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1435 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Comment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Comment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1443 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Contact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Contact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ContextChangedMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ContextChangedMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1457 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Contract.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Contract.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1347 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CreateEndpointProfileMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CreateEndpointProfileMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CurrentBotMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CurrentBotMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1248 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Customer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Customer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1772 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DataModificationEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DataModificationEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1461 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DataScript.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DataScript.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1377 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DataScriptInput.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DataScriptInput.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1395 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DateTimePropertyFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DateTimePropertyFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeactiveMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeactiveMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1729 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Device.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Device.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceActivateMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceActivateMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceDeactivateMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceDeactivateMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1370 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceMotionMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceMotionMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceSettingMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceSettingMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1518 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceStateChangeMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceStateChangeMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1396 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceStatusMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceStatusMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceStatusRequestMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceStatusRequestMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1658 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Dialog.py
--rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Dialog.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1480 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogAd.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogAd.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2114 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogAssignFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      344 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogAssignFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogBegin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogBegin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1665 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogButton.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogButton.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1401 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogButtonClickedMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogButtonClickedMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1586 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogCallDialog.py
--rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogCallDialog.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2480 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogChatRules.py
--rw-r--r--   0 hadfield   (501) staff       (20)      481 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogChatRules.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2100 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogCondition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      332 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogCondition.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1589 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogDatascript.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogDatascript.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1942 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogDatascriptAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      313 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogDatascriptAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2312 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogDownloadFile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      393 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogDownloadFile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1461 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogEnd.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogEnd.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1383 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogExitBot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogExitBot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2018 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogExitDialog.py
--rw-r--r--   0 hadfield   (501) staff       (20)      325 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogExitDialog.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogGenerator.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogGenerator.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1498 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogInnerMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      186 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogInnerMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogLoop.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogLoop.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1499 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPageElementMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPageElementMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPart.py
--rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPart.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPassThrough.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPassThrough.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1798 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPayment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPayment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2021 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPersistFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      326 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPersistFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPredict.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPredict.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1832 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPredictAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      286 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPredictAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogProcess.py
--rw-r--r--   0 hadfield   (501) staff       (20)      389 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogProcess.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1587 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQuery.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2788 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQueryAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      553 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQueryAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1790 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQuestion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      258 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQuestion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQuestionEnd.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQuestionEnd.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQuestionStart.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQuestionStart.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2378 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogReceiveAIMPMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      440 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogReceiveAIMPMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1820 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRecommend.py
--rw-r--r--   0 hadfield   (501) staff       (20)      282 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRecommend.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1511 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRecommendations.py
--rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRecommendations.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1593 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRemoveFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRemoveFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1400 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRestartQuestion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRestartQuestion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogResume.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogResume.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1456 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRow.py
--rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRow.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2341 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSendAIMPMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      411 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSendAIMPMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSerialize.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSerialize.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSession.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSession.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1384 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogStatusMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogStatusMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1465 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogStep.py
--rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogStep.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSubroutine.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSubroutine.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSwitchBot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSwitchBot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1589 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSwitchToBot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSwitchToBot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogText.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1673 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogTextCard.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogTextCard.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2113 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogTextMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      345 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogTextMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     3280 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogUploadFile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      674 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogUploadFile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogWorkflow.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogWorkflow.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DirectMessageReceived.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DirectMessageReceived.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1496 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DirectTextMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      185 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DirectTextMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DocumentSignatureEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DocumentSignatureEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1270 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DocumentSignatureLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      111 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DocumentSignatureLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DocumentSignatureProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DocumentSignatureProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 21:21:47.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DomainOntology.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1389 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DoublePropertyFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DoublePropertyFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EMailTag.py
--rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EMailTag.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1327 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAIMPMessagePayloadDef.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAIMPMessagePayloadDef.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAPILogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAPILogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1348 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityInvitation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      161 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityInvitation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1336 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityMember.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityMember.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1366 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityMemberInvitation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityMemberInvitation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1279 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentConfiguration.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentConfiguration.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1339 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstallConfiguration.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstallConfiguration.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1333 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceDeployment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceDeployment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceDeploymentChannel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceDeploymentChannel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceMessageDeployment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceMessageDeployment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstancePayloadDeployment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstancePayloadDeployment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentPolicy.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentPolicy.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAlexaLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAlexaLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAnonymousLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAnonymousLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1303 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAssetNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAssetNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAssignedPerson.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAssignedPerson.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAssignee.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAssignee.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAttendee.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAttendee.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1294 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAuthor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAuthor.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1285 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBotChatRuleSet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBotChatRuleSet.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1505 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBotDialog.py
--rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBotDialog.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBotImplementation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBotImplementation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1336 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBusinessRelationshipWith.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBusinessRelationshipWith.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasCalendarLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasCalendarLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChannel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChannel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1505 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChannelBot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChannelBot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChatRule.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChatRule.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChatRuleSet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChatRuleSet.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChatRuleSetFile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChatRuleSetFile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChildChannel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChildChannel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1294 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChoice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChoice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasContract.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasContract.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1341 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasCustomer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasCustomer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDataScript.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDataScript.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDataScriptInput.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDataScriptInput.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1324 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDependentProjectTask.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDependentProjectTask.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1294 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDevice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1294 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialog.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialog.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialogAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialogAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialogCondition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialogCondition.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1291 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialogRow.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialogRow.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialogSession.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialogSession.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDocument.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDocument.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1342 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDocumentSignatureLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDocumentSignatureLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEmailAttachment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEmailAttachment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEmailForward.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEmailForward.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEmailLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEmailLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEmailSummary.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEmailSummary.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEndpointProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEndpointProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEntityProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEntityProperty.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1303 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEntitySet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEntitySet.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasExternalAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasExternalAccount.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasFacebookLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasFacebookLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasFileNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasFileNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1282 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasFolder.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasFolder.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasIFrameTemplate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasIFrameTemplate.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasInvoice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasInvoice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedCustomer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedCustomer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1342 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInCompanyAffiliation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInCompanyAffiliation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1333 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInRecipientInvite.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInRecipientInvite.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1336 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInRecipientMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInRecipientMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1324 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInSenderInvite.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInSenderInvite.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1327 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInSenderMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInSenderMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLoginChannelBot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLoginChannelBot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasPayment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasPayment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasPaymentLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasPaymentLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasPermittedSender.py
--rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasPermittedSender.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProfileSession.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProfileSession.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProjectList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProjectList.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProjectStep.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProjectStep.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProjectTask.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProjectTask.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProposal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProposal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1291 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasQuery.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1428 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasQueryCriterion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      184 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasQueryCriterion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasReferencedNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasReferencedNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1406 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasRelationship.py
--rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasRelationship.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1336 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasRelationshipProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasRelationshipProperty.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasRelationshipSet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasRelationshipSet.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1550 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSelectedDataScript.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSelectedDataScript.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1525 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSelectedQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSelectedQuery.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSessionChannel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSessionChannel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSignedDocument.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSignedDocument.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSlackLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSlackLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSmsLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSmsLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasTwitterLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasTwitterLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasUserAvatar.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasUserAvatar.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1359 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailAttachment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailAttachment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1327 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2967 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      528 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1374 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1389 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailReceived.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailReceived.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2762 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailSummary.py
--rw-r--r--   0 hadfield   (501) staff       (20)      474 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailSummary.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailsList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      104 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailsList.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1739 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmbeddedCard.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmbeddedCard.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1395 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EnclosingPageNotification.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EnclosingPageNotification.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1432 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EnclosingPageURLButtonClickedMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EnclosingPageURLButtonClickedMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1669 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Endpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Endpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1570 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EndpointProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      188 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EndpointProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EndpointProfileMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EndpointProfileMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1533 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EndpointProfilesMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EndpointProfilesMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1400 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EnlargeCardCommand.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EnlargeCardCommand.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1341 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Entity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Entity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1396 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntityCommandMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntityCommandMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntityFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntityFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1366 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntityMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntityMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1483 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntityProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntityProperty.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntitySet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntitySet.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1747 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ErrorNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ErrorNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ExternalInteraction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ExternalInteraction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1538 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ExternalInteractionPart.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ExternalInteractionPart.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1594 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ExternalInteractionTransaction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ExternalInteractionTransaction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1803 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      264 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookIncomingMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookIncomingMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1336 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookOutgoingMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookOutgoingMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1678 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookPost.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookPost.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1787 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1378 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FactsListMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FactsListMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FavoriteTweet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FavoriteTweet.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2033 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FileAnswer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      301 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FileAnswer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FileChatRuleSet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FileChatRuleSet.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1563 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FileQuestion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      192 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FileQuestion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1454 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FileUploadObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FileUploadObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1242 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Folder.py
--rw-r--r--   0 hadfield   (501) staff       (20)      115 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Folder.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1245 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FormDialog.py
--rw-r--r--   0 hadfield   (501) staff       (20)      110 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FormDialog.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FormPageAnswersMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FormPageAnswersMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1373 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GeoLocationAnswer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GeoLocationAnswer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1507 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GeoLocationPropertyFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GeoLocationPropertyFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2103 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetChannelHistoryMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      325 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetChannelHistoryMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1384 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetFactsMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetFactsMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetJoinedChannels.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetJoinedChannels.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1498 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetObjectMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetObjectMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1510 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetObjectResultsMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetObjectResultsMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GoogleHomeDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GoogleHomeDevice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GraphLabel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GraphLabel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1476 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GraphObjectFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GraphObjectFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1500 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GroupStringPropertyFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GroupStringPropertyFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1507 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyActivityMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      192 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyActivityMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2111 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyArticleMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      337 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyArticleMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyAudioMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyAudioMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1236 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      105 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBot.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotConfiguration.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotConfiguration.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotInstall.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotInstall.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotInstallConfiguration.py
--rw-r--r--   0 hadfield   (501) staff       (20)      185 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotInstallConfiguration.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotInstance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotInstance.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1344 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotInstanceDeployment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotInstanceDeployment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotPolicy.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotPolicy.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyCalendarMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyCalendarMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1317 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyChannelCardsListMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyChannelCardsListMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyChartMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyChartMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyCheckListMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyCheckListMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyChildResponseMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyChildResponseMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1388 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyCommandMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyCommandMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyDevice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyDeviceDetailsMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyDeviceDetailsMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyDialogAppMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyDialogAppMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyEmailsListMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyEmailsListMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyFacebookMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyFacebookMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1426 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyFacebookStatusPanelMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyFacebookStatusPanelMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1874 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyFileDownloadMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      271 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyFileDownloadMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyFileUploadMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyFileUploadMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyImageGalleryMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyImageGalleryMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1999 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyImageMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyImageMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1326 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyKnowledgeExtractionMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyKnowledgeExtractionMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1335 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInInviteMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInInviteMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1396 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1329 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInPostMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInPostMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1335 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInSearchMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInSearchMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1329 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInTextMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInTextMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2520 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyMapMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      458 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyMapMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2456 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      464 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyMovieDetailsMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyMovieDetailsMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1344 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyMoviesRecommendationsListMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyMoviesRecommendationsListMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyNotificationMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyNotificationMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1326 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyPaymentConfirmationMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyPaymentConfirmationMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyProductMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyProductMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyProgressMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyProgressMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyQuestionDialogAppMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyQuestionDialogAppMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyRealtimeMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyRealtimeMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleySearchResultsMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleySearchResultsMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyShoppingCartMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyShoppingCartMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1599 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyStatusMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyStatusMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1268 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyStatusType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyStatusType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyTextMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyTextMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyThingMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyThingMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyThingWideMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyThingWideMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyTranslationMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyTranslationMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyTweetMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyTweetMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyTwitterStatusPanelMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyTwitterStatusPanelMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyVideoMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyVideoMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1800 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyWeatherMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      258 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyWeatherMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyWebviewMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyWebviewMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1484 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HeartbeatMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HeartbeatMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HueLightDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HueLightDevice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasAccountAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasAccountAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1355 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasBridgeInteractionPartChain.py
--rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasBridgeInteractionPartChain.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasCardPart.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasCardPart.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasChannelCard.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasChannelCard.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasDialogPart.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasDialogPart.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionChain.py
--rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionChain.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1346 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionPart.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionPart.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1361 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionPartChain.py
--rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionPartChain.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1367 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionTransaction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionTransaction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasGraphObjectFactElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasGraphObjectFactElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionChain.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionChain.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionPart.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionPart.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionPartChain.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionPartChain.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionTransaction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionTransaction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1418 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasListFactElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasListFactElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasMessagePayload.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasMessagePayload.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasProjectListElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasProjectListElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1679 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IFrameEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IFrameEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1488 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IFrameEventMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      175 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IFrameEventMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1366 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IFrameTemplate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IFrameTemplate.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Image.py
--rw-r--r--   0 hadfield   (501) staff       (20)      102 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Image.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1352 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ImageGallery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ImageGallery.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2174 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ImageObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      345 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ImageObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InformationMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InformationMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IntegerPropertyFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IntegerPropertyFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1440 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Intent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Intent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1479 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IntentMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IntentMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1493 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InterAccountMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InterAccountMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1402 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InteractionModeMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InteractionModeMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1422 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InterruptProcessorMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      175 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InterruptProcessorMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InvalidateMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InvalidateMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1404 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InvalidateQuestionMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InvalidateQuestionMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1454 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Invoice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Invoice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1592 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IosDeviceProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IosDeviceProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/JiboDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/JiboDevice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/JoinChannel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/JoinChannel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1392 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/KnowledgeExtractionCard.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/KnowledgeExtractionCard.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LeaveChannel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LeaveChannel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LightDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LightDevice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2065 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInCompanyProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      358 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInCompanyProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInInvitation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInInvitation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1336 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1368 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2270 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInPersonProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      412 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInPersonProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1362 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInPost.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInPost.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1395 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListChannelsRequestMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListChannelsRequestMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListChannelsResultsMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListChannelsResultsMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1344 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListEndpointProfilesMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      175 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListEndpointProfilesMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1455 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1326 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListJoinedChannelsResultsMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListJoinedChannelsResultsMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1553 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LoginDataEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      182 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LoginDataEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1286 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LoginOnboardingStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LoginOnboardingStatus.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LoginStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LoginStatus.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ManagedChatRuleSet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ManagedChatRuleSet.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2478 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MapObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      428 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MapObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1228 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Media.py
--rw-r--r--   0 hadfield   (501) staff       (20)      103 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Media.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MemoryFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MemoryFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1474 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MenuClickedMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MenuClickedMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MessageService.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MessageService.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MetaQLMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MetaQLMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1893 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MetaQLResultsMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      265 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MetaQLResultsMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1252 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MmsAttachment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      111 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MmsAttachment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MotionMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MotionMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2557 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Movie.py
--rw-r--r--   0 hadfield   (501) staff       (20)      437 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Movie.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MoviesList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      104 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MoviesList.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1916 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MultiChoiceQuestion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      295 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MultiChoiceQuestion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/NextAudioCommand.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/NextAudioCommand.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/NotificationMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/NotificationMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1642 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/OpenIFrame.py
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/OpenIFrame.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1399 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/OpenPanelCommand.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/OpenPanelCommand.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1666 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Opportunity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Opportunity.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1371 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PauseMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PauseMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PayloadStyleType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PayloadStyleType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1744 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Payment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Payment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2074 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentConfirmation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      302 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentConfirmation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1240 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      101 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1531 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentProcessorEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentProcessorEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1465 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentQuestion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentQuestion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1586 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PermittedSender.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PermittedSender.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1286 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PermittedSenderStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PermittedSenderStatus.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PermittedSenderType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PermittedSenderType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PlayAudioCommand.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PlayAudioCommand.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PlayVideoCommand.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PlayVideoCommand.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PredictionFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PredictionFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1326 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorAreYouAliveMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorAreYouAliveMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorError.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorError.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1483 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorEvent.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1277 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorEventType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorEventType.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorHeartbeatMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorHeartbeatMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorJoinedMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorJoinedMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorLeftMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorLeftMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1484 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      175 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorRequestMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorRequestMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1616 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorResponseMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorResponseMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1467 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProgressItem.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProgressItem.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProgressObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProgressObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1245 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Project.py
--rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Project.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProjectList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProjectList.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProjectStep.py
--rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProjectStep.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1772 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProjectTask.py
--rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProjectTask.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1562 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PropertyFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      184 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PropertyFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1248 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Proposal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Proposal.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PurgeSessionMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PurgeSessionMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1861 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PushNotification.py
--rw-r--r--   0 hadfield   (501) staff       (20)      251 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PushNotification.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1442 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Query.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Query.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1681 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QueryCriterion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QueryCriterion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     6374 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Question.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1554 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Question.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2560 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      492 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1793 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionUpdateMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      251 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionUpdateMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     3334 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionsPageMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      725 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionsPageMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1430 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionsPageNavigationMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionsPageNavigationMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1277 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionsPageTheme.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionsPageTheme.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RealtimeTickMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RealtimeTickMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RefreshChannelCommand.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RefreshChannelCommand.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1414 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationshipCommandMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationshipCommandMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1384 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationshipMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationshipMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1507 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationshipProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationshipProperty.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationshipSet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationshipSet.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1397 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RemoveCardCommand.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RemoveCardCommand.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1347 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RemoveEndpointProfileMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RemoveEndpointProfileMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1493 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RemoveQuestionMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      180 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RemoveQuestionMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1866 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ResultListFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ResultListFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1333 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Review.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Review.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1564 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ReviewSummary.py
--rw-r--r--   0 hadfield   (501) staff       (20)      188 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ReviewSummary.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RobotDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RobotDevice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1411 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ScrollToQuestionMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ScrollToQuestionMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2017 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SearchRequestMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      325 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SearchRequestMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1759 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SearchResult.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SearchResult.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1363 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SearchResultsList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SearchResultsList.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendDirectMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendDirectMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1377 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendEmail.py
--rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendEmail.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendPushNotificationMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendPushNotificationMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendSms.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendSms.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendTweet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendTweet.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendVoiceMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendVoiceMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1851 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Session.py
--rw-r--r--   0 hadfield   (501) staff       (20)      254 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Session.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SessionClosedMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SessionClosedMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SessionEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SessionEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SessionExpiredMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SessionExpiredMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1381 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SetFactMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SetFactMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SettingsMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SettingsMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1542 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ShoppingCart.py
--rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ShoppingCart.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1397 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ShrinkCardCommand.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ShrinkCardCommand.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1404 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SingleSignOnProvider.py
--rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SingleSignOnProvider.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackIncomingMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackIncomingMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1327 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1784 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackOutgoingMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackOutgoingMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1586 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackTextMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      361 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackTextMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmartDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmartDevice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1824 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Sms.py
--rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Sms.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      111 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1374 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1368 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsReceived.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsReceived.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1575 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsTextMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsTextMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SolutionFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SolutionFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SpeechMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SpeechMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SpheroDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SpheroDevice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StatusMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StatusMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StopAudioCommand.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StopAudioCommand.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StopVideoCommand.py
--rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StopVideoCommand.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1389 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StringPropertyFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StringPropertyFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1448 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StripePayment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StripePayment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SwitchDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SwitchDevice.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1375 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SwitchEnclosingPageToURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SwitchEnclosingPageToURL.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SystemTickMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SystemTickMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1629 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Task.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Task.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     4026 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ThingCard.py
--rw-r--r--   0 hadfield   (501) staff       (20)      833 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ThingCard.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ThingWideCard.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ThingWideCard.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ThinkingMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ThinkingMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TickMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TickMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TimeoutMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TimeoutMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1876 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Translation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      269 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Translation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TreeQuestion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TreeQuestion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TrendResult.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TrendResult.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TrueFalseAnswer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TrueFalseAnswer.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2007 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TrueFalseQuestion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      313 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TrueFalseQuestion.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1384 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TruthPropertyFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TruthPropertyFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1378 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TweetReceived.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TweetReceived.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1485 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TweetTextMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TweetTextMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1469 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterEndpoint.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1333 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterLogin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      115 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterLogin.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1487 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      180 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2216 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterQueryRequestMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      359 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterQueryRequestMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2315 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterQueryResultsMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      380 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterQueryResultsMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1374 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/URIPropertyFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/URIPropertyFact.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UnsetFactMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UnsetFactMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UpdateSessionMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UpdateSessionMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1625 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserAnswerDialogAppMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserAnswerDialogAppMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserAvatar.py
--rw-r--r--   0 hadfield   (501) staff       (20)      108 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserAvatar.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserChatRequestMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserChatRequestMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1385 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserCommandMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserCommandMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1711 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserDialogAppMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserDialogAppMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserLeftApp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserLeftApp.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserLoggedIn.py
--rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserLoggedIn.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserLoggedOut.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserLoggedOut.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserProfile.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserProfileMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserProfileMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1381 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserStatusMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserStatusMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserTextMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserTextMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Video.py
--rw-r--r--   0 hadfield   (501) staff       (20)      102 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Video.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2369 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/VideoObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      388 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/VideoObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/VirtualLoginRequestMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/VirtualLoginRequestMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1512 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/VirtualLoginResponseMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/VirtualLoginResponseMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1856 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/VoiceMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      253 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/VoiceMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/WeMoSwitch.py
--rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/WeMoSwitch.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1764 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/WeatherForecast.py
--rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/WeatherForecast.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1550 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/WebviewCard.py
--rw-r--r--   0 hadfield   (501) staff       (20)      175 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/WebviewCard.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:22.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:34:18.010123 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountEventAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountEventDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountEventIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountEventLoginURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountEventTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountInstantiationClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountInteractionFee.py
--rw-r--r--   0 hadfield   (501) staff       (20)      239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountInteractionTotalFee.py
--rw-r--r--   0 hadfield   (501) staff       (20)      245 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityConvertDate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      249 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityEventDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      253 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityEventIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityEventTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      251 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityInvitationCode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      251 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityInvitationDate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      253 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityInvitationEmail.py
--rw-r--r--   0 hadfield   (501) staff       (20)      261 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityInvitationStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      241 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      245 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountResourceLockAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      255 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountResourceLockOwnerIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountResourceLockStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountResourceLockTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      249 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountResourceLockUserLoginURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountResourceTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAccountURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasActivityItemJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasActivityMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasActivityTaskIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAddress.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAgentAccessAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAgentAccessURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAgentGenerationDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAgentGeneratorURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAgentMessagePayloadTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAgentMessageTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAgentText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAgentTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAlexaSkillName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAlexaUserID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAmount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAnswerDataJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAnswerURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAssetID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAssetType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAssetURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAttachmentsCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAuthSessionID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAuthor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAvatarURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasAverageRating.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBackgroundColor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBadge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBase64BinaryData.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBccRecipients.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBindingNames.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBodyHtml.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBodyPlain.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBooleanValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBotCreatorIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBotID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBotURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBridgeAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBridgeChannelURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBridgeSequenceNumber.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBridgeSessionID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBuilderClass.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasBuilderString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasButton.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasButtonType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasButtonURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCalendarURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCalendars.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCampaignURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCancelCommandMessageURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCardHeader.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCardType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCardURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCcRecipients.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChannelTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChannelURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChannels.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChannelsHistory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChargeAmount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChartData.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChartOptions.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChartType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChatMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChatMode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChatRuleID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChatRulePattern.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChatRuleProcessingType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChatRuleResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChatRuleSetURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChatRulesOutputChannelFactName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChatRulesOutputFactName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChildChannelURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChoiceLabel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChoiceListSource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasChoiceValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasClearScope.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasColor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasColumnsDefinition.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCommand.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasComments.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCommentsCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasComparator.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasConditionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasConditionalLogic.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasConstraints.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCriteriaType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCriterionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasCurrencySymbol.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDatascriptScope.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDateSent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDateValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDebugMessageAfter.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDebugMessageBefore.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDeliveryDate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDestinationAccountName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDestinationAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDestinationFactName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDestinationFactScope.py
--rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDestinationReferenceClass.py
--rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDestinationReferenceIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDeviceID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDeviceInfo.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDeviceName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDeviceNewState.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDeviceOldState.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDeviceStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDeviceType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDialogMode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDialogPageURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDialogToCallName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDialogToCallScope.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDirectionsEndAddress.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDirectionsJSONResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDirectionsStartAddress.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDocuSignEnvelopeID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDocuSignStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDoubleValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDueDate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasDurationSeconds.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasEMailTagURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasEchoUserID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasEmail.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasEncryptedPayload.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasEndDate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasEndpointID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasEndpointURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasEntityPropertyType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasEntitySetURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasEntityURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasEntryText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasErrorMessagePropertyName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasEventTimestamp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasEventType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasExpression.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasExternalInteractionFee.py
--rw-r--r--   0 hadfield   (501) staff       (20)      241 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasExternalInteractionTotalFee.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasFacebookUserID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasFactClassName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasFactPropertyName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasFactScope.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasFalseLabel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasFileNodeClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasFileNodeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasFileTypeConstraint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasFileUploadProcessingType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasFirstName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasFormattedContent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasFullName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasFunctionName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasGender.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasGenre.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasGeoAPIJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasGeolocation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasGettingStartedText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasGraphLabelURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasGreetingText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasHaleyStatusMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasHaleyStatusTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasHandlerResultFactName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasHumidity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasId.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasImageCaption.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasImageFileNodeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasImageURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasImdbRating.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasInputFactScope.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasInputFileFactName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasInputFileFactScope.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasInputPropertyName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasIntegerValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasIntent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasIntentPropertyName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasInteractionMode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasInternalID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasInternalProcessingChoice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasInterruptedFactName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasIpAddress.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasItemStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasJson.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasKeyHash.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasKnowledgeExtractionJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLastActiveDate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLastActivityTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLastLeftAppMessageTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLastLoginAttemptDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLastName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLatitude.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLikesCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLimit.py
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLink.py
--rw-r--r--   0 hadfield   (501) staff       (20)      241 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInCompanyLogoImageURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInCompanyName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInCompanyURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInEmailAddress.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInFirstName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInIndustry.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInLastName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInNumberOfEmployees.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInOccupation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInProfileId.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInProfilePageURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInUniversalName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLinkedinProfileImageURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLocalTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLocale.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLocation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLocationString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLoginAttemptCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLoginAuthLockedDateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLoginOnboardingStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLoginStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLongDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasLongitude.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMasterUserID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMaxFileLength.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMaxRetriesCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMaxTimestamp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMd5checksum.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMemberEmailAddress.py
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMenu.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMenuURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMessageClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMessageID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMessageSerialized.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMessageServiceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMessageURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMessageURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMinTimestamp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasMultiChoiceQuestionInstruction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasNeLatitude.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasNeLongitude.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasNewStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasNextButtonLabel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasNextExecutionDateMinutesSource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasNotificationJsonBody.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasOAuthSecret.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasOAuthToken.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasObjectClassURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasObjectCreationTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasObjectURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasObjectUpdateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasOffset.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasOpportunityStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasOptionalData.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasOrderInUI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasOrientationInUI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasOutputCardsPropertyName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasOutputMessagePropertyName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPageTypeIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPanelName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasParameterValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasParentFactURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasParentObjectURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasParentQuestionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasParentURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasParseString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPartialResultMessageCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPartialResultPayloadCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPartialResultTotalMessageCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPartialResultTotalPayloadCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPayload.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPayloadStyleTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPaymentProcessorEventId.py
--rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPaymentProviderEventType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPecrentComplete.py
--rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPermittedSenderStatusURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPermittedSenderTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPersistFactOperationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPersistedMenuJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPg.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPhoneNumber.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPlaceholder.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPrefilledAnswer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPreviousAnswer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPreviousButtonLabel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPriority.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasProcessorEventJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasProcessorEventTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasProcessorID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasProcessorType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasProfilePic.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasProfileURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasProgress.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasProjectTag.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPropertyName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPropertyType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPropertyValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasProvider.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPublicKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasPublicationDate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasQuantityData.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasQueryCriterionGroup.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasQueryType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasQuestionContent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasQuestionDataJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasQuestionID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasQuestionOption.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasQuestionPreviousContent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasQuestionSubType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasQuestionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasQuestionURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasQuestionsPageThemeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasQueueName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRadius.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRating.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasReactionToSessionID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRecipient.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRecipientAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRecipientIdentity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRecipientReferenceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRecipients.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasReferenceIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRelationshipFactName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRelationshipFactScope.py
--rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRelationshipPropertyType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRelationshipSetURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      245 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasReplyBridgeReferenceObjectURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRequestType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRequestURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRequestedPage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRequestedPayloadStyleTypeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasResultListFactURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRoleURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasRottenTomatoesRating.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSameAsCheckBoxLabel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasScore.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasScriptBody.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasScriptName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasScrollToQuestionIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSearchCategoryURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSearchExcludedCategoryURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSearchGeoURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSearchString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSectionHeaderHTML.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSecurityProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSelectedDatascriptName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSelectedQueryName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSender.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSenderAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSenderIdentity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSenderOrRecipient.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSenderReferenceURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSerializedBridgeMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasServiceName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasShippingFee.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasShortDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSignature.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSingleSignOnIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSingleSignOnProviderIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSingleSignOnProviderURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSlackChannelID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSlackEventType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSlackFileShareName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSlackFileShareURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSlackMessageJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSlackRecipientChannelID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSlackRecipientTeamID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSlackRecipientThreadID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSlackRecipientUserID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSlackTeamID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSlackThreadID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSlackUserID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSolutionFactURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSound.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSourceAccountName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSourceAccountURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSourceFactName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSourceFactScope.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSourceLanguage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSourcePronounciation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSourceReferenceClass.py
--rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSourceReferenceIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSourceText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSourceUserID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSourceUserName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasStackTrace.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasStartDate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasStateManager.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasStateSerialized.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasStatusMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasStatusPropertyName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasStringValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSubject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSubmitButtonLabel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSubpropertyName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSwLatitude.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasSwLongitude.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTargetChannel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTargetLanguage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTargetPronounciation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTargetService.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTargetStep.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTargetText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTax.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTemperature.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTemplateID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTextChannelFactName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTextFactName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTextToSpeak.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasThreadURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasThumbnailImageFileNodeURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasThumbnailImageURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTimeoutPropertyName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTimeoutSeconds.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTimezone.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTitle.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasToken.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTokens.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTotalPages.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTotalResults.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTotalReviews.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTreeJson.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTrueLabel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTruthValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasTweetIDs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasUpdateContent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasUpdateType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasUriValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasUrl.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasUserCategoryURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasUserCreatorIdentifier.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasUserID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasUuid.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasValidationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasViewURIs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasWeatherJSONResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasWebviewHeightRatio.py
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasYear.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_hasZoomLevel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_haslLastRunTimestamp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isAcceptSystemTicks.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isAccountInternalAdmin.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isActivityCancelEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isActivityCanceled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isActivityComplete.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isActivitySpinnerEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isAnonymousChannel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isAnswerSkipped.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isAudioDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isAuthLoginProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isAuthLoginTunnel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isAutoLoadUserProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isAutoPlay.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isAutosaveOnChange.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isBroadcastOnly.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isChannelRandomized.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isChildChannel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isCommentedOut.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isCompressed.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isConsumeImmediately.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isContainsPII.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isCountOnly.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isCreateResultListFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isCreateSolutionFact.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isCurrencyISymbolnFrontOf.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isCurrentChannelTarget.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isCurrentProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isCustomerServiceEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isDebugEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isDefaultBot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isDefaultChannel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isDefaultDialog.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isDefaultEndpoint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isDeleteOnSuccess.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isDetailsEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isDirectMessageResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isDisplayInUI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isDistribute.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isDownloadEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isEditing.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isExclusive.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isFinalResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isFullDayEvent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isGetStartedButtonEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isGlobalBot.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isGlobalChatRuleSet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isGlobalDatascript.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isGlobalDialog.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isGlobalEntitySet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isGlobalQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isGlobalRelationshipSet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isGoBackSelected.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isGoodbyePage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isGraphObjectsLinked.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isHaleyMessageTextHidden.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isHandlerEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isHelpRequested.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isHidden.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isHidePageCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isHideShareButton.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isHistoryMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isIgnoreStandardIntents.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isIncludeDependentObjects.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isIncludeSubclasses.py
--rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isInterAccountSearchableRecipient.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isInteractMode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isInternalAnswerProcessingEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isInternalOnly.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isKeepChannelEntryText.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isKeepLoaded.py
--rw-r--r--   0 hadfield   (501) staff       (20)      239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isLoginAuthForcePasswordReset.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isLoginAuthLocked.py
--rw-r--r--   0 hadfield   (501) staff       (20)      239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isMemberEmailAddressValidated.py
--rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isMms.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isMultivalue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isMultivalueProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isNextButtonEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isNotificationsEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isOpenInitially.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isOtherChannelTarget.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isPartialResult.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isPlaying.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isPremium.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isPreviousButtonEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isProcessWithChatRules.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isProcessed.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isProgressBarEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isPurgeSession.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isQuestionClosed.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isQuestionCountExcluded.py
--rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isQuestionCountPanelDisabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isRead.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isReadOnlyQuestion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isRemoveWholeProfile.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isRenderQuickReplies.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isReplyTo.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isRequestCompression.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSameAsCheckboxEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSaveAnswersOnGoingBack.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSelected.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSendAsAttachment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSendAsUser.py
--rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSent.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSignedVersion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSkippable.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSlackResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSmsResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isStaticQuestionsList.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSubmitButtonEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSubpropertyEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSynchronize.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isSystemChannel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isTextEntryHidden.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isTimeoutEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isTrackingOpens.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isTrueAnswerOnly.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isTunnelingEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isTweetResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isUpdateAnswer.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isUrlAvailable.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isVisualDevice.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/Property_isVitalRulesEnabled.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:22.000000 vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/properties/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-04 21:34:18.011789 vital-ai-aimp-0.1.3/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      961 2024-05-04 21:19:13.000000 vital-ai-aimp-0.1.3/setup.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:34:18.011144 vital-ai-aimp-0.1.3/vital_ai_aimp.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      596 2024-05-04 21:34:17.000000 vital-ai-aimp-0.1.3/vital_ai_aimp.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)   107019 2024-05-04 21:34:17.000000 vital-ai-aimp-0.1.3/vital_ai_aimp.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-04 21:34:17.000000 vital-ai-aimp-0.1.3/vital_ai_aimp.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       72 2024-05-04 21:34:17.000000 vital-ai-aimp-0.1.3/vital_ai_aimp.egg-info/entry_points.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       66 2024-05-04 21:34:17.000000 vital-ai-aimp-0.1.3/vital_ai_aimp.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       24 2024-05-04 21:34:17.000000 vital-ai-aimp-0.1.3/vital_ai_aimp.egg-info/top_level.txt
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:49:09.026940 vital-ai-aimp-0.1.4/
+-rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-02-06 19:34:55.000000 vital-ai-aimp-0.1.4/LICENSE
+-rw-r--r--   0 hadfield   (501) staff       (20)      596 2024-05-06 21:49:09.026655 vital-ai-aimp-0.1.4/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)       16 2024-02-06 19:49:29.000000 vital-ai-aimp-0.1.4/README.md
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:49:08.676924 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:22.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:49:08.941446 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)     1557 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      185 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPDevice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPEmailMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPEmailMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     6757 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1579 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1368 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPMessageDef.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPMessageDef.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPMessageFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPMessageFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1388 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPMessagePayloadDef.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPMessagePayloadDef.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1250 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPThing.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPThing.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1254 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/APIEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/APIEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1228 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/APILogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       97 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/APILogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1903 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      314 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountEventType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountEventType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountInteraction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountInteraction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1531 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountInteractionPart.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      216 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountInteractionPart.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1589 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountInteractionTransaction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountInteractionTransaction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1750 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      292 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1767 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      299 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1304 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityEventType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityEventType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1804 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityInvitation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      323 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityInvitation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityInvitationStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityInvitationStatus.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1523 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityMember.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityMember.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityStatus.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1981 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountResourceLock.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      373 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountResourceLock.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountResourceLockStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountResourceLockStatus.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountResourceLockType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountResourceLockType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountResourceType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountResourceType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountStatus.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ActivateMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ActivateMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2010 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ActivityCard.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      328 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ActivityCard.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AdUnitEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AdUnitEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1338 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Agent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Agent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1277 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentConfiguration.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentConfiguration.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1886 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentDatascriptCallRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentDatascriptCallRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2495 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentDatascriptCallResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      405 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentDatascriptCallResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1254 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentError.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentError.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1681 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentImage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentImage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1259 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstall.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstall.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1298 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstallConfiguration.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstallConfiguration.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstanceDeployment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstanceDeployment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1523 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstanceMessageDeployment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      192 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstanceMessageDeployment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1529 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstancePayloadDeployment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      198 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstancePayloadDeployment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentMedia.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentMedia.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1292 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentMessagePayloadType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentMessagePayloadType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentMessageType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentMessageType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1736 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      228 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentPolicy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentPolicy.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1465 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentStatusRequest.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentStatusRequest.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1767 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentStatusResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      224 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentStatusResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1459 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentText.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1250 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentVideo.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentVideo.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1466 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaAccount.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1365 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaDevice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1362 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1327 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1375 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AmazonEchoAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AmazonEchoAccount.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1339 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnonymousLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnonymousLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnonymousProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnonymousProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1637 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Answer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Answer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1363 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerChoice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerChoice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2410 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      422 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1849 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerRealtimeUpdateMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      290 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerRealtimeUpdateMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2102 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerStatusMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      329 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerStatusMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2425 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerUnsetMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      427 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerUnsetMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1905 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerUpdateMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      285 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerUpdateMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ApnsEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ApnsEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2180 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ArticleObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      347 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ArticleObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1436 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Asset.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Asset.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1495 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AssetConditionMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      182 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AssetConditionMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1397 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AssetLocationMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AssetLocationMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AssetMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AssetMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Audio.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      102 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Audio.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2369 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AudioObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      388 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AudioObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BB8Device.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BB8Device.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1283 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BaseInteraction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BaseInteraction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1295 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BaseInteractionPart.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BaseInteractionPart.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BaseInteractionTransaction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BaseInteractionTransaction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1452 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BaseProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BaseProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BinaryMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BinaryMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BooleanPropertyFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BooleanPropertyFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1759 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Bot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Bot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1947 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BridgeSessionMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      330 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BridgeSessionMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BuilderClassBot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BuilderClassBot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BuilderDesignerBot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BuilderDesignerBot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1358 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BuilderStringBot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BuilderStringBot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1726 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Button.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Button.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1484 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ButtonClickedMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ButtonClickedMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1938 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ButtonStateMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      320 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ButtonStateMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1248 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Calendar.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Calendar.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1571 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarEntry.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarEntry.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1879 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      102 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1553 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1422 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CancelCommandMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      185 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CancelCommandMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1438 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Card.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Card.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2595 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Channel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      471 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Channel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1393 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelClosedMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelClosedMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2521 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelHistoryResponseMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      423 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelHistoryResponseMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelViewLeftMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelViewLeftMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelViewSwitchedMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelViewSwitchedMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1527 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Chart.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Chart.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1245 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatDialog.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      110 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatDialog.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1365 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1374 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatModeMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatModeMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1664 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatRule.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatRule.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatRuleSet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatRuleSet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1360 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatRuleSetFile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatRuleSetFile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1351 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CheckItem.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CheckItem.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1236 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CheckList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      103 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CheckList.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1946 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Choice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      275 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Choice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1251 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChoiceAnswer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      112 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChoiceAnswer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1358 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ClearChatHistory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ClearChatHistory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1444 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CloseIFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CloseIFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1402 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ClosePanelCommand.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ClosePanelCommand.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CloseSessionMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CloseSessionMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1370 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CommandMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CommandMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1435 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Comment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Comment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1443 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Contact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Contact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ContextChangedMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ContextChangedMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1457 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Contract.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Contract.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1347 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CreateEndpointProfileMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CreateEndpointProfileMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CurrentBotMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CurrentBotMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1248 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Customer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Customer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1772 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DataModificationEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      236 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DataModificationEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1461 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DataScript.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DataScript.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1377 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DataScriptInput.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DataScriptInput.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1395 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DateTimePropertyFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DateTimePropertyFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeactiveMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeactiveMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1729 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Device.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Device.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceActivateMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceActivateMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceDeactivateMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceDeactivateMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1370 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceMotionMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceMotionMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceSettingMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceSettingMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1518 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceStateChangeMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceStateChangeMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1396 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceStatusMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceStatusMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceStatusRequestMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceStatusRequestMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1658 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Dialog.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      218 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Dialog.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1480 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogAd.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogAd.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2114 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogAssignFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      344 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogAssignFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogBegin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogBegin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1665 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogButton.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogButton.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1401 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogButtonClickedMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogButtonClickedMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1586 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogCallDialog.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      200 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogCallDialog.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2480 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogChatRules.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      481 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogChatRules.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2100 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogCondition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      332 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogCondition.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1589 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogDatascript.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogDatascript.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1942 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogDatascriptAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      313 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogDatascriptAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2312 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogDownloadFile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      393 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogDownloadFile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1461 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogEnd.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogEnd.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1383 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogExitBot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogExitBot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2018 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogExitDialog.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      325 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogExitDialog.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogGenerator.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogGenerator.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1498 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogInnerMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      186 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogInnerMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogLoop.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogLoop.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1499 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPageElementMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPageElementMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPart.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPart.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPassThrough.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPassThrough.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1798 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPayment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPayment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2021 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPersistFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      326 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPersistFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPredict.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPredict.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1832 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPredictAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      286 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPredictAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogProcess.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      389 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogProcess.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1587 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2788 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQueryAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      553 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQueryAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1790 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQuestion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      258 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQuestion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQuestionEnd.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQuestionEnd.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQuestionStart.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQuestionStart.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2378 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogReceiveAIMPMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      440 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogReceiveAIMPMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1820 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRecommend.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      282 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRecommend.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1511 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRecommendations.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRecommendations.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1593 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRemoveFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRemoveFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1400 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRestartQuestion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRestartQuestion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogResume.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogResume.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1456 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRow.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRow.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2341 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSendAIMPMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      411 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSendAIMPMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSerialize.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSerialize.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1262 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSession.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSession.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1384 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogStatusMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogStatusMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1465 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogStep.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogStep.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSubroutine.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSubroutine.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSwitchBot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSwitchBot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1589 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSwitchToBot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSwitchToBot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogText.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1673 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogTextCard.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogTextCard.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2113 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogTextMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      345 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogTextMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     3280 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogUploadFile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      674 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogUploadFile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogWorkflow.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogWorkflow.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DirectMessageReceived.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DirectMessageReceived.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1496 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DirectTextMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      185 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DirectTextMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DocumentSignatureEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DocumentSignatureEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1270 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DocumentSignatureLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      111 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DocumentSignatureLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DocumentSignatureProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DocumentSignatureProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 21:21:47.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1389 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DoublePropertyFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DoublePropertyFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EMailTag.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EMailTag.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1327 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAIMPMessagePayloadDef.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAIMPMessagePayloadDef.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAPILogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAPILogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1348 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityInvitation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      161 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityInvitation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1336 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityMember.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityMember.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1366 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityMemberInvitation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityMemberInvitation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1279 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentConfiguration.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentConfiguration.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1339 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstallConfiguration.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstallConfiguration.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1333 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceDeployment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceDeployment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceDeploymentChannel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceDeploymentChannel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceMessageDeployment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceMessageDeployment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1354 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstancePayloadDeployment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstancePayloadDeployment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentPolicy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentPolicy.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAlexaLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAlexaLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAnonymousLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAnonymousLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1303 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAssetNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAssetNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAssignedPerson.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAssignedPerson.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAssignee.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAssignee.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAttendee.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAttendee.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1294 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAuthor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAuthor.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1285 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBotChatRuleSet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBotChatRuleSet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1505 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBotDialog.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      196 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBotDialog.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBotImplementation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBotImplementation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1336 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBusinessRelationshipWith.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBusinessRelationshipWith.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasCalendarLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasCalendarLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChannel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChannel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1505 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChannelBot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChannelBot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChatRule.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChatRule.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChatRuleSet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChatRuleSet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChatRuleSetFile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChatRuleSetFile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChildChannel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChildChannel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1294 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChoice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChoice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasContract.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasContract.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1341 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasCustomer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasCustomer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDataScript.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDataScript.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDataScriptInput.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDataScriptInput.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1324 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDependentProjectTask.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDependentProjectTask.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1294 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDevice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1294 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialog.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialog.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialogAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialogAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialogCondition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialogCondition.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1291 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialogRow.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialogRow.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialogSession.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialogSession.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDocument.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDocument.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1342 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDocumentSignatureLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDocumentSignatureLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEmailAttachment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEmailAttachment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEmailForward.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEmailForward.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEmailLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEmailLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEmailSummary.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEmailSummary.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEndpointProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEndpointProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEntityProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEntityProperty.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1303 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEntitySet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEntitySet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasExternalAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasExternalAccount.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasFacebookLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasFacebookLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasFileNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasFileNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1282 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasFolder.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasFolder.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasIFrameTemplate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasIFrameTemplate.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasInvoice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasInvoice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedCustomer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedCustomer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1342 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInCompanyAffiliation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInCompanyAffiliation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1333 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInRecipientInvite.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInRecipientInvite.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1336 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInRecipientMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInRecipientMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1324 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInSenderInvite.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInSenderInvite.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1327 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInSenderMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInSenderMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLoginChannelBot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLoginChannelBot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasPayment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasPayment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasPaymentLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasPaymentLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasPermittedSender.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasPermittedSender.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProfileSession.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProfileSession.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProjectList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProjectList.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProjectStep.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProjectStep.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProjectTask.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProjectTask.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProposal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProposal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1291 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1428 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasQueryCriterion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      184 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasQueryCriterion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasReferencedNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasReferencedNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1406 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasRelationship.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasRelationship.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1336 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasRelationshipProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasRelationshipProperty.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasRelationshipSet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasRelationshipSet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1550 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSelectedDataScript.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSelectedDataScript.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1525 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSelectedQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSelectedQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSessionChannel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSessionChannel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSignedDocument.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSignedDocument.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSlackLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSlackLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1300 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSmsLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSmsLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasTwitterLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasTwitterLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasUserAvatar.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasUserAvatar.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1359 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailAttachment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailAttachment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1327 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2967 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      528 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1374 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1389 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailReceived.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailReceived.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2762 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailSummary.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      474 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailSummary.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailsList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      104 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailsList.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1739 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmbeddedCard.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmbeddedCard.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1395 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EnclosingPageNotification.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EnclosingPageNotification.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1432 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EnclosingPageURLButtonClickedMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EnclosingPageURLButtonClickedMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1669 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Endpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Endpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1570 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EndpointProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      188 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EndpointProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EndpointProfileMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EndpointProfileMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1533 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EndpointProfilesMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      210 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EndpointProfilesMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1400 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EnlargeCardCommand.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EnlargeCardCommand.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1341 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Entity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Entity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1396 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntityCommandMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntityCommandMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntityFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntityFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1366 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntityMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntityMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1483 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntityProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntityProperty.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntitySet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntitySet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1747 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ErrorNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ErrorNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ExternalInteraction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ExternalInteraction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1538 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ExternalInteractionPart.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ExternalInteractionPart.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1594 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ExternalInteractionTransaction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ExternalInteractionTransaction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1803 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      264 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookIncomingMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookIncomingMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1336 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookOutgoingMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookOutgoingMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1678 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookPost.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookPost.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1787 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1378 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FactsListMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FactsListMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FavoriteTweet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FavoriteTweet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2033 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FileAnswer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      301 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FileAnswer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FileChatRuleSet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FileChatRuleSet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1563 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FileQuestion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      192 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FileQuestion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1454 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FileUploadObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FileUploadObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1242 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Folder.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      115 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Folder.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1245 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FormDialog.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      110 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FormDialog.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FormPageAnswersMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FormPageAnswersMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1373 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GeoLocationAnswer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GeoLocationAnswer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1507 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GeoLocationPropertyFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GeoLocationPropertyFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2103 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetChannelHistoryMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      325 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetChannelHistoryMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1384 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetFactsMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetFactsMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetJoinedChannels.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetJoinedChannels.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1498 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetObjectMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetObjectMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1510 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetObjectResultsMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetObjectResultsMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GoogleHomeDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GoogleHomeDevice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1253 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GraphLabel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GraphLabel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1476 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GraphObjectFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GraphObjectFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1500 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GroupStringPropertyFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GroupStringPropertyFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1507 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyActivityMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      192 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyActivityMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2111 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyArticleMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      337 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyArticleMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyAudioMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyAudioMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1236 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      105 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBot.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotConfiguration.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotConfiguration.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotInstall.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotInstall.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotInstallConfiguration.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      185 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotInstallConfiguration.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotInstance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotInstance.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1344 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotInstanceDeployment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotInstanceDeployment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotPolicy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotPolicy.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyCalendarMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyCalendarMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1317 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyChannelCardsListMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyChannelCardsListMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyChartMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyChartMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyCheckListMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyCheckListMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyChildResponseMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyChildResponseMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1388 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyCommandMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyCommandMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyDevice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyDeviceDetailsMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyDeviceDetailsMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyDialogAppMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyDialogAppMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyEmailsListMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyEmailsListMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyFacebookMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyFacebookMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1426 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyFacebookStatusPanelMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyFacebookStatusPanelMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1874 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyFileDownloadMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      271 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyFileDownloadMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1299 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyFileUploadMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      140 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyFileUploadMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyImageGalleryMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyImageGalleryMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1999 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyImageMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      306 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyImageMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1326 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyKnowledgeExtractionMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyKnowledgeExtractionMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1335 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInInviteMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInInviteMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1396 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1329 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInPostMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInPostMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1335 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInSearchMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInSearchMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1329 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInTextMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInTextMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2520 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyMapMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      458 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyMapMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2456 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      464 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyMovieDetailsMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyMovieDetailsMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1344 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyMoviesRecommendationsListMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyMoviesRecommendationsListMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyNotificationMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyNotificationMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1326 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyPaymentConfirmationMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyPaymentConfirmationMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyProductMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyProductMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyProgressMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyProgressMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyQuestionDialogAppMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyQuestionDialogAppMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyRealtimeMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyRealtimeMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleySearchResultsMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      143 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleySearchResultsMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyShoppingCartMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyShoppingCartMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1599 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyStatusMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyStatusMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1268 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyStatusType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyStatusType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyTextMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyTextMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyThingMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyThingMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyThingWideMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyThingWideMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1302 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyTranslationMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyTranslationMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyTweetMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyTweetMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyTwitterStatusPanelMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyTwitterStatusPanelMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyVideoMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyVideoMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1800 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyWeatherMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      258 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyWeatherMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyWebviewMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyWebviewMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1484 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HeartbeatMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HeartbeatMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HueLightDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HueLightDevice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1316 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasAccountAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasAccountAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1355 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasBridgeInteractionPartChain.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasBridgeInteractionPartChain.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasCardPart.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasCardPart.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasChannelCard.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasChannelCard.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasDialogPart.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasDialogPart.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionChain.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      160 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionChain.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1346 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionPart.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionPart.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1361 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionPartChain.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionPartChain.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1367 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionTransaction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionTransaction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasGraphObjectFactElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasGraphObjectFactElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1325 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionChain.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionChain.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionPart.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionPart.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1337 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionPartChain.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionPartChain.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionTransaction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionTransaction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1418 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasListFactElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasListFactElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1319 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasMessagePayload.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasMessagePayload.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1331 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasProjectListElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasProjectListElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1679 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IFrameEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IFrameEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1488 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IFrameEventMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      175 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IFrameEventMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1366 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IFrameTemplate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IFrameTemplate.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Image.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      102 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Image.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1352 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ImageGallery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ImageGallery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2174 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ImageObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      345 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ImageObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InformationMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InformationMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IntegerPropertyFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IntegerPropertyFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1440 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Intent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Intent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1479 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IntentMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IntentMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1493 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InterAccountMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InterAccountMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1402 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InteractionModeMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InteractionModeMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1422 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InterruptProcessorMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      175 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InterruptProcessorMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InvalidateMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InvalidateMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1404 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InvalidateQuestionMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InvalidateQuestionMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1454 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Invoice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Invoice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1592 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IosDeviceProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IosDeviceProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/JiboDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/JiboDevice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/JoinChannel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/JoinChannel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1392 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/KnowledgeExtractionCard.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/KnowledgeExtractionCard.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LeaveChannel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LeaveChannel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LightDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LightDevice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2065 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInCompanyProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      358 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInCompanyProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInInvitation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInInvitation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1336 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1368 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2270 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInPersonProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      412 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInPersonProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1362 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInPost.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInPost.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1395 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListChannelsRequestMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListChannelsRequestMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListChannelsResultsMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListChannelsResultsMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1344 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListEndpointProfilesMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      175 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListEndpointProfilesMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1455 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1326 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListJoinedChannelsResultsMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListJoinedChannelsResultsMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1553 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LoginDataEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      182 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LoginDataEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1286 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LoginOnboardingStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LoginOnboardingStatus.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LoginStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LoginStatus.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ManagedChatRuleSet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ManagedChatRuleSet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2478 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MapObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      428 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MapObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1228 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Media.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      103 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Media.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MemoryFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      146 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MemoryFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1474 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MenuClickedMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MenuClickedMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MessageService.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MessageService.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MetaQLMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MetaQLMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1893 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MetaQLResultsMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      265 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MetaQLResultsMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1252 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MmsAttachment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      111 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MmsAttachment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MotionMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MotionMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2557 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Movie.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      437 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Movie.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MoviesList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      104 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MoviesList.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1916 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MultiChoiceQuestion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      295 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MultiChoiceQuestion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/NextAudioCommand.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/NextAudioCommand.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/NotificationMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/NotificationMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1642 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/OpenIFrame.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/OpenIFrame.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1399 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/OpenPanelCommand.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/OpenPanelCommand.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1666 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Opportunity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Opportunity.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1371 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PauseMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PauseMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1271 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PayloadStyleType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PayloadStyleType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1744 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Payment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Payment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2074 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentConfirmation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      302 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentConfirmation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1240 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      101 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1531 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentProcessorEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      212 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentProcessorEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1465 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentQuestion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentQuestion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1586 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PermittedSender.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PermittedSender.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1286 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PermittedSenderStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PermittedSenderStatus.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1280 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PermittedSenderType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PermittedSenderType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PlayAudioCommand.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PlayAudioCommand.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PlayVideoCommand.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PlayVideoCommand.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PredictionFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PredictionFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1326 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorAreYouAliveMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorAreYouAliveMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorError.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorError.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1483 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorEvent.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1277 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorEventType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorEventType.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorHeartbeatMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorHeartbeatMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorJoinedMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorJoinedMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1305 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorLeftMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorLeftMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1484 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      175 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorRequestMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorRequestMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1616 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorResponseMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorResponseMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1467 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProgressItem.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProgressItem.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1349 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProgressObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProgressObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1245 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Project.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Project.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProjectList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProjectList.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProjectStep.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      120 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProjectStep.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1772 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProjectTask.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProjectTask.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1562 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PropertyFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      184 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PropertyFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1248 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Proposal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      117 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Proposal.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PurgeSessionMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PurgeSessionMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1861 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PushNotification.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      251 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PushNotification.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1442 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Query.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Query.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1681 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QueryCriterion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QueryCriterion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     6374 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Question.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1554 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Question.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2560 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      492 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1793 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionUpdateMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      251 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionUpdateMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     3334 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionsPageMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      725 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionsPageMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1430 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionsPageNavigationMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionsPageNavigationMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1277 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionsPageTheme.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionsPageTheme.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RealtimeTickMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RealtimeTickMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1314 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RefreshChannelCommand.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RefreshChannelCommand.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1414 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationshipCommandMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationshipCommandMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1384 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationshipMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationshipMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1507 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationshipProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationshipProperty.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1380 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationshipSet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationshipSet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1397 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RemoveCardCommand.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RemoveCardCommand.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1347 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RemoveEndpointProfileMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RemoveEndpointProfileMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1493 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RemoveQuestionMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      180 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RemoveQuestionMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1866 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ResultListFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ResultListFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1333 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Review.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Review.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1564 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ReviewSummary.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      188 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ReviewSummary.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RobotDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RobotDevice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1411 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ScrollToQuestionMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ScrollToQuestionMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2017 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SearchRequestMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      325 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SearchRequestMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1759 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SearchResult.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SearchResult.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1363 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SearchResultsList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SearchResultsList.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendDirectMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendDirectMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1377 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendEmail.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendEmail.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1311 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendPushNotificationMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendPushNotificationMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendSms.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendSms.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendTweet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendTweet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendVoiceMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendVoiceMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1851 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Session.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      254 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Session.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SessionClosedMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SessionClosedMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SessionEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SessionEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SessionExpiredMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SessionExpiredMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1381 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SetFactMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SetFactMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1284 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SettingsMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SettingsMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1542 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ShoppingCart.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      170 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ShoppingCart.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1397 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ShrinkCardCommand.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ShrinkCardCommand.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1404 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SingleSignOnProvider.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SingleSignOnProvider.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackIncomingMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackIncomingMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1327 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      113 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1784 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      252 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1293 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackOutgoingMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackOutgoingMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1586 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      208 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackTextMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      361 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackTextMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1260 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmartDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      123 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmartDevice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1824 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Sms.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Sms.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      111 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1374 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      154 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1368 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsReceived.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsReceived.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1575 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsTextMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      194 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsTextMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1257 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SolutionFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      118 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SolutionFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SpeechMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SpeechMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SpheroDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SpheroDevice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1278 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StatusMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StatusMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StopAudioCommand.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StopAudioCommand.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StopVideoCommand.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      165 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StopVideoCommand.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1389 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StringPropertyFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StringPropertyFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1448 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StripePayment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StripePayment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SwitchDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      124 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SwitchDevice.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1375 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SwitchEnclosingPageToURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SwitchEnclosingPageToURL.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1281 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SystemTickMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SystemTickMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1629 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Task.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Task.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     4026 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ThingCard.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      833 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ThingCard.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ThingWideCard.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ThingWideCard.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1275 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ThinkingMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ThinkingMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TickMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TickMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TimeoutMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TimeoutMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1876 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Translation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      269 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Translation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1356 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TreeQuestion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TreeQuestion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TrendResult.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TrendResult.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TrueFalseAnswer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TrueFalseAnswer.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2007 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TrueFalseQuestion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      313 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TrueFalseQuestion.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1384 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TruthPropertyFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TruthPropertyFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1378 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TweetReceived.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TweetReceived.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1485 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TweetTextMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TweetTextMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1469 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      162 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterEndpoint.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1333 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterLogin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      115 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterLogin.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1487 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      180 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2216 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterQueryRequestMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      359 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterQueryRequestMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2315 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterQueryResultsMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      380 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterQueryResultsMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1374 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/URIPropertyFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/URIPropertyFact.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2321 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UnsetFactMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      394 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UnsetFactMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1290 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UpdateSessionMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      135 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UpdateSessionMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1625 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserAnswerDialogAppMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      222 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserAnswerDialogAppMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserAvatar.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      108 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserAvatar.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserChatRequestMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserChatRequestMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1385 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserCommandMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserCommandMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1711 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserDialogAppMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserDialogAppMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1266 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserLeftApp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserLeftApp.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1269 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserLoggedIn.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      130 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserLoggedIn.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1272 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserLoggedOut.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserLoggedOut.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      142 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserProfile.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1287 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserProfileMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserProfileMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1381 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserStatusMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserStatusMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserTextMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserTextMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Video.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      102 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Video.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2369 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/VideoObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      388 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/VideoObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/VirtualLoginRequestMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/VirtualLoginRequestMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1512 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/VirtualLoginResponseMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      181 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/VirtualLoginResponseMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1856 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/VoiceMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      253 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/VoiceMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1263 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/WeMoSwitch.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      128 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/WeMoSwitch.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1764 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/WeatherForecast.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      230 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/WeatherForecast.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1550 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/WebviewCard.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      175 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/WebviewCard.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:22.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:49:09.025456 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountEventAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountEventDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountEventIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountEventLoginURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountEventTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountInstantiationClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountInteractionFee.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountInteractionTotalFee.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      245 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityConvertDate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      249 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityEventDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      253 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityEventIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityEventTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      251 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityInvitationCode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      251 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityInvitationDate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      253 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityInvitationEmail.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      261 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityInvitationStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      241 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountOpportunityURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      245 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountResourceLockAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      255 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountResourceLockOwnerIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountResourceLockStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountResourceLockTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      249 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountResourceLockUserLoginURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountResourceTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAccountURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasActivityItemJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasActivityMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasActivityTaskIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAddress.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAgentAccessAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAgentAccessURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAgentGenerationDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAgentGeneratorURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAgentMessagePayloadTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAgentMessageTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAgentText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAgentTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAlexaSkillName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAlexaUserID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAmount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAnswerDataJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAnswerURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAssetID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAssetType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAssetURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAttachmentsCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAuthSessionID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAuthor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAvatarURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasAverageRating.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBackgroundColor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBadge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBase64BinaryData.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBccRecipients.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBindingNames.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBodyHtml.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBodyPlain.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBooleanValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBotCreatorIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBotID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBotURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBridgeAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBridgeChannelURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBridgeSequenceNumber.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBridgeSessionID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBuilderClass.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasBuilderString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasButton.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasButtonType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasButtonURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCalendarURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCalendars.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCampaignURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCancelCommandMessageURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCardHeader.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCardType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCardURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCcRecipients.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChannelTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChannelURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChannels.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChannelsHistory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChargeAmount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChartData.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChartOptions.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChartType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChatMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChatMode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChatRuleID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChatRulePattern.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChatRuleProcessingType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChatRuleResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChatRuleSetURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChatRulesOutputChannelFactName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChatRulesOutputFactName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChildChannelURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChoiceLabel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChoiceListSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasChoiceValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasClearScope.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasColor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasColumnsDefinition.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCommand.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasComments.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCommentsCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasComparator.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasConditionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasConditionalLogic.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasConstraints.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCriteriaType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCriterionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasCurrencySymbol.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDatascriptScope.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDateSent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDateValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDebugMessageAfter.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDebugMessageBefore.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDeliveryDate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDestinationAccountName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDestinationAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDestinationFactName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDestinationFactScope.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDestinationReferenceClass.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDestinationReferenceIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDeviceID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDeviceInfo.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDeviceName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDeviceNewState.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDeviceOldState.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDeviceStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDeviceType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDialogMode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDialogPageURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDialogToCallName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDialogToCallScope.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDirectionsEndAddress.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDirectionsJSONResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDirectionsStartAddress.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDocuSignEnvelopeID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDocuSignStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDoubleValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDueDate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasDurationSeconds.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasEMailTagURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasEchoUserID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasEmail.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasEncryptedPayload.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasEndDate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasEndpointID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasEndpointURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasEntityPropertyType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasEntitySetURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasEntityURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasEntryText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasErrorMessagePropertyName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasEventTimestamp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasEventType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasExpression.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasExternalInteractionFee.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      241 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasExternalInteractionTotalFee.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasFacebookUserID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasFactClassName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasFactPropertyName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasFactScope.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasFalseLabel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasFileNodeClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasFileNodeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasFileTypeConstraint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasFileUploadProcessingType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasFirstName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasFormattedContent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasFullName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasFunctionName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasGender.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasGenre.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasGeoAPIJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasGeolocation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasGettingStartedText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasGraphLabelURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasGreetingText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasHaleyStatusMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasHaleyStatusTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasHandlerResultFactName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasHumidity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasId.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasImageCaption.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasImageFileNodeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasImageURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasImdbRating.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasInputFactScope.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasInputFileFactName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasInputFileFactScope.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasInputPropertyName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasIntegerValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasIntent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasIntentPropertyName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasInteractionMode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasInternalID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasInternalProcessingChoice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasInterruptedFactName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasIpAddress.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasItemStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasJson.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasKeyHash.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasKnowledgeExtractionJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLastActiveDate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLastActivityTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLastLeftAppMessageTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLastLoginAttemptDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLastName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLatitude.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLikesCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLimit.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLink.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      241 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInCompanyLogoImageURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInCompanyName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInCompanyURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInEmailAddress.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInFirstName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInIndustry.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInLastName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInNumberOfEmployees.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInOccupation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInProfileId.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInProfilePageURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedInUniversalName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLinkedinProfileImageURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLocalTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLocale.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLocation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLocationString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLoginAttemptCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLoginAuthLockedDateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLoginOnboardingStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLoginStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLongDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasLongitude.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMasterUserID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMaxFileLength.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMaxRetriesCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMaxTimestamp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMd5checksum.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMemberEmailAddress.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMenu.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMenuURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMessageClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMessageID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMessageSerialized.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMessageServiceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMessageURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMessageURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMinTimestamp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasMultiChoiceQuestionInstruction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasNeLatitude.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasNeLongitude.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasNewStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasNextButtonLabel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasNextExecutionDateMinutesSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasNotificationJsonBody.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasOAuthSecret.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasOAuthToken.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasObjectClassURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasObjectCreationTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasObjectURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasObjectUpdateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasOffset.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasOpportunityStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasOptionalData.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasOrderInUI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasOrientationInUI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasOutputCardsPropertyName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasOutputMessagePropertyName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPageTypeIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPanelName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasParameterValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasParentFactURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasParentObjectURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasParentQuestionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasParentURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasParseString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPartialResultMessageCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPartialResultPayloadCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPartialResultTotalMessageCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPartialResultTotalPayloadCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPayload.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPayloadStyleTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPaymentProcessorEventId.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPaymentProviderEventType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPecrentComplete.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPermittedSenderStatusURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPermittedSenderTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPersistFactOperationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPersistedMenuJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPg.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPhoneNumber.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPlaceholder.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPrefilledAnswer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPreviousAnswer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPreviousButtonLabel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPriority.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasProcessorEventJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasProcessorEventTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasProcessorID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasProcessorType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasProfilePic.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasProfileURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasProgress.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasProjectTag.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPropertyName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPropertyType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPropertyValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasProvider.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPublicKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasPublicationDate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasQuantityData.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasQueryCriterionGroup.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasQueryType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasQuestionContent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasQuestionDataJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasQuestionID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasQuestionOption.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasQuestionPreviousContent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasQuestionSubType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasQuestionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasQuestionURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasQuestionsPageThemeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasQueueName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRadius.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRating.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasReactionToSessionID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRecipient.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRecipientAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRecipientIdentity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRecipientReferenceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRecipients.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasReferenceIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRelationshipFactName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRelationshipFactScope.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      235 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRelationshipPropertyType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRelationshipSetURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      245 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasReplyBridgeReferenceObjectURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRequestType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRequestURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRequestedPage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      243 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRequestedPayloadStyleTypeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasResultListFactURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRoleURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasRottenTomatoesRating.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSameAsCheckBoxLabel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasScore.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasScriptBody.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasScriptName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasScrollToQuestionIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSearchCategoryURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSearchExcludedCategoryURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSearchGeoURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSearchString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSectionHeaderHTML.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSecurityProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSelectedDatascriptName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSelectedQueryName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSender.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSenderAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSenderIdentity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSenderOrRecipient.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSenderReferenceURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSerializedBridgeMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasServiceName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasShippingFee.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasShortDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSignature.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSingleSignOnIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSingleSignOnProviderIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSingleSignOnProviderURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSlackChannelID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSlackEventType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSlackFileShareName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSlackFileShareURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSlackMessageJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSlackRecipientChannelID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSlackRecipientTeamID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSlackRecipientThreadID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSlackRecipientUserID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSlackTeamID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSlackThreadID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSlackUserID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSolutionFactURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSound.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSourceAccountName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSourceAccountURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSourceFactName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSourceFactScope.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSourceLanguage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSourcePronounciation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSourceReferenceClass.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSourceReferenceIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSourceText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSourceUserID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSourceUserName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasStackTrace.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasStartDate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasStateManager.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasStateSerialized.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasStatusMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasStatusPropertyName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasStringValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSubject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSubmitButtonLabel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSubpropertyName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSwLatitude.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasSwLongitude.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTargetChannel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTargetLanguage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTargetPronounciation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTargetService.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTargetStep.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTargetText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTax.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTemperature.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTemplateID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTextChannelFactName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTextFactName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTextToSpeak.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasThreadURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasThumbnailImageFileNodeURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasThumbnailImageURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTimeoutPropertyName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTimeoutSeconds.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTimezone.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTitle.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasToken.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTokens.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTotalPages.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTotalResults.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTotalReviews.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTreeJson.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTrueLabel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTruthValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasTweetIDs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasUpdateContent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasUpdateType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasUriValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasUrl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasUserCategoryURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasUserCreatorIdentifier.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasUserID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasUuid.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasValidationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasViewURIs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasWeatherJSONResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasWebviewHeightRatio.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasYear.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_hasZoomLevel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_haslLastRunTimestamp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isAcceptSystemTicks.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isAccountInternalAdmin.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isActivityCancelEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isActivityCanceled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isActivityComplete.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isActivitySpinnerEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isAnonymousChannel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isAnswerSkipped.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isAudioDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isAuthLoginProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isAuthLoginTunnel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isAutoLoadUserProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isAutoPlay.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isAutosaveOnChange.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isBroadcastOnly.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isChannelRandomized.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isChildChannel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isCommentedOut.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isCompressed.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isConsumeImmediately.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isContainsPII.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isCountOnly.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isCreateResultListFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isCreateSolutionFact.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isCurrencyISymbolnFrontOf.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isCurrentChannelTarget.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isCurrentProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isCustomerServiceEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isDebugEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isDefaultBot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isDefaultChannel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isDefaultDialog.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isDefaultEndpoint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isDeleteOnSuccess.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isDetailsEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isDirectMessageResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isDisplayInUI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isDistribute.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isDownloadEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isEditing.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isExclusive.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isFinalResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isFullDayEvent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isGetStartedButtonEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isGlobalBot.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isGlobalChatRuleSet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isGlobalDatascript.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isGlobalDialog.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isGlobalEntitySet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isGlobalQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isGlobalRelationshipSet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isGoBackSelected.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isGoodbyePage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isGraphObjectsLinked.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isHaleyMessageTextHidden.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isHandlerEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isHelpRequested.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isHidden.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isHidePageCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isHideShareButton.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isHistoryMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isIgnoreStandardIntents.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isIncludeDependentObjects.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isIncludeSubclasses.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isInterAccountSearchableRecipient.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isInteractMode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      247 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isInternalAnswerProcessingEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isInternalOnly.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isKeepChannelEntryText.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isKeepLoaded.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isLoginAuthForcePasswordReset.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isLoginAuthLocked.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      239 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isMemberEmailAddressValidated.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isMms.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isMultivalue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isMultivalueProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isNextButtonEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isNotificationsEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isOpenInitially.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isOtherChannelTarget.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isPartialResult.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isPlaying.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isPremium.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isPreviousButtonEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isProcessWithChatRules.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isProcessed.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isProgressBarEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isPurgeSession.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isQuestionClosed.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isQuestionCountExcluded.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isQuestionCountPanelDisabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isRead.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isReadOnlyQuestion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isRemoveWholeProfile.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isRenderQuickReplies.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isReplyTo.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isRequestCompression.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSameAsCheckboxEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSaveAnswersOnGoingBack.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSelected.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSendAsAttachment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSendAsUser.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSent.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSignedVersion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSkippable.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSlackResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSmsResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isStaticQuestionsList.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSubmitButtonEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSubpropertyEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSynchronize.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isSystemChannel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isTextEntryHidden.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isTimeoutEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isTrackingOpens.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isTrueAnswerOnly.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isTunnelingEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isTweetResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isUpdateAnswer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isUrlAvailable.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isVisualDevice.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/Property_isVitalRulesEnabled.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:22.000000 vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/properties/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-06 21:49:09.026988 vital-ai-aimp-0.1.4/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)      961 2024-05-06 21:46:58.000000 vital-ai-aimp-0.1.4/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:49:09.026248 vital-ai-aimp-0.1.4/vital_ai_aimp.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      596 2024-05-06 21:49:08.000000 vital-ai-aimp-0.1.4/vital_ai_aimp.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)   107019 2024-05-06 21:49:08.000000 vital-ai-aimp-0.1.4/vital_ai_aimp.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-06 21:49:08.000000 vital-ai-aimp-0.1.4/vital_ai_aimp.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       72 2024-05-06 21:49:08.000000 vital-ai-aimp-0.1.4/vital_ai_aimp.egg-info/entry_points.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       66 2024-05-06 21:49:08.000000 vital-ai-aimp-0.1.4/vital_ai_aimp.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       24 2024-05-06 21:49:08.000000 vital-ai-aimp-0.1.4/vital_ai_aimp.egg-info/top_level.txt
```

### Comparing `vital-ai-aimp-0.1.3/LICENSE` & `vital-ai-aimp-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/PKG-INFO` & `vital-ai-aimp-0.1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: vital-ai-aimp
-Version: 0.1.3
+Version: 0.1.4
 Summary: VitalSigns aimp domain
 Home-page: https://github.com/vital-ai/vitalhome-aimp
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vital-ai-domain==0.1.3
-Requires-Dist: vital-ai-social==0.1.3
-Requires-Dist: vital-ai-nlp==0.1.3
+Requires-Dist: vital-ai-domain>=0.1.4
+Requires-Dist: vital-ai-social>=0.1.4
+Requires-Dist: vital-ai-nlp>=0.1.4
 
 # vital-ai-aimp
```

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPDevice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPDevice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPEmailMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPEmailMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPEvent.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPMessage.pyi` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPMessage.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPMessageDef.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPMessageDef.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPMessageFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPMessageFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPMessagePayloadDef.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPMessagePayloadDef.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AIMPThing.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AIMPThing.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/APIEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/APIEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/APILogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/APILogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountAction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountEvent.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountEventType.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountEventType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountInteraction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountInteraction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountInteractionPart.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountInteractionPart.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountInteractionTransaction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountInteractionTransaction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunity.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityEvent.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityEventType.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityEventType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityInvitation.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityInvitation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityInvitationStatus.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityInvitationStatus.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityMember.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityMember.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountOpportunityStatus.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountOpportunityStatus.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountResourceLock.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountResourceLock.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountResourceLockStatus.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountResourceLockStatus.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountResourceLockType.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountResourceLockType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountResourceType.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountResourceType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AccountStatus.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AccountStatus.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ActivateMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ActivateMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ActivityCard.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ActivityCard.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AdUnitEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AdUnitEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Agent.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Agent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentConfiguration.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentConfiguration.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentDatascriptCallRequest.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentDatascriptCallRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentDatascriptCallResponse.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentDatascriptCallResponse.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentError.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentError.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentImage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentImage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstall.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstall.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstallConfiguration.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstallConfiguration.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstance.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstanceDeployment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstanceDeployment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstanceMessageDeployment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstanceMessageDeployment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentInstancePayloadDeployment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentInstancePayloadDeployment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentMedia.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentMedia.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentMessagePayloadType.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentMessagePayloadType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentMessageType.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentMessageType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentObject.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentPolicy.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentPolicy.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentStatusRequest.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentStatusRequest.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentStatusResponse.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentStatusResponse.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentText.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentText.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentType.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AgentVideo.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AgentVideo.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaAccount.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaAccount.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaDevice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaDevice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AlexaProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AlexaProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AmazonEchoAccount.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AmazonEchoAccount.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnonymousLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnonymousLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnonymousProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnonymousProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Answer.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Answer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerChoice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerChoice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerRealtimeUpdateMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerRealtimeUpdateMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerStatusMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerStatusMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerUnsetMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerUnsetMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AnswerUpdateMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AnswerUpdateMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ApnsEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ApnsEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ArticleObject.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ArticleObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Asset.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Asset.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AssetConditionMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AssetConditionMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AssetLocationMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AssetLocationMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AssetMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AssetMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Audio.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Audio.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/AudioObject.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/AudioObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BB8Device.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BB8Device.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BaseInteraction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BaseInteraction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BaseInteractionPart.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BaseInteractionPart.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BaseInteractionTransaction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BaseInteractionTransaction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BaseProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BaseProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BinaryMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BinaryMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BooleanPropertyFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BooleanPropertyFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Bot.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Bot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BridgeSessionMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BridgeSessionMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BuilderClassBot.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BuilderClassBot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BuilderDesignerBot.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BuilderDesignerBot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/BuilderStringBot.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/BuilderStringBot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Button.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Button.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ButtonClickedMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ButtonClickedMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ButtonStateMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ButtonStateMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Calendar.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Calendar.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarEntry.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarEntry.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarEvent.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarObject.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CalendarProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CalendarProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CancelCommandMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CancelCommandMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Card.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Card.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Channel.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Channel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelClosedMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelClosedMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelHistoryResponseMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelHistoryResponseMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelType.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelViewLeftMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelViewLeftMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChannelViewSwitchedMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChannelViewSwitchedMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Chart.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Chart.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatDialog.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatDialog.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatModeMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatModeMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatRule.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatRule.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatRuleSet.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatRuleSet.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChatRuleSetFile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChatRuleSetFile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CheckItem.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CheckItem.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CheckList.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CheckList.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Choice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Choice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ChoiceAnswer.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ChoiceAnswer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ClearChatHistory.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ClearChatHistory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CloseIFrame.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CloseIFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ClosePanelCommand.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ClosePanelCommand.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CloseSessionMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CloseSessionMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CommandMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CommandMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Comment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Comment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Contact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Contact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ContextChangedMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ContextChangedMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Contract.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Contract.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CreateEndpointProfileMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CreateEndpointProfileMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/CurrentBotMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/CurrentBotMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Customer.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Customer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DataModificationEvent.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DataModificationEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DataScript.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DataScript.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DataScriptInput.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DataScriptInput.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DateTimePropertyFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DateTimePropertyFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeactiveMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeactiveMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Device.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Device.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceActivateMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceActivateMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceDeactivateMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceDeactivateMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceMotionMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceMotionMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceSettingMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceSettingMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceStateChangeMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceStateChangeMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceStatusMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceStatusMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DeviceStatusRequestMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DeviceStatusRequestMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Dialog.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Dialog.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogAction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogAd.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogAd.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogAssignFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogAssignFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogBegin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogBegin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogButton.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogButton.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogButtonClickedMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogButtonClickedMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogCallDialog.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogCallDialog.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogChatRules.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogChatRules.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogCondition.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogCondition.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogDatascript.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogDatascript.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogDatascriptAction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogDatascriptAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogDownloadFile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogDownloadFile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogElement.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogEnd.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogEnd.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogExitBot.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogExitBot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogExitDialog.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogExitDialog.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogGenerator.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogGenerator.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogInnerMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogInnerMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogLoop.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogLoop.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPageElementMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPageElementMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPart.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPart.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPassThrough.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPassThrough.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPayment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPayment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPersistFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPersistFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPredict.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPredict.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogPredictAction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogPredictAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogProcess.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogProcess.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQuery.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQuery.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQueryAction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQueryAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQueryAction.pyi` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQueryAction.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQuestion.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQuestion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQuestionEnd.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQuestionEnd.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogQuestionStart.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogQuestionStart.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogReceiveAIMPMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogReceiveAIMPMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRecommend.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRecommend.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRecommendations.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRecommendations.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRemoveFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRemoveFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRestartQuestion.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRestartQuestion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogResume.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogResume.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogRow.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogRow.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSendAIMPMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSendAIMPMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSerialize.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSerialize.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSession.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSession.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogStatusMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogStatusMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogStep.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogStep.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSubroutine.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSubroutine.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSwitchBot.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSwitchBot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogSwitchToBot.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogSwitchToBot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogText.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogText.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogTextCard.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogTextCard.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogTextMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogTextMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogUploadFile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogUploadFile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogUploadFile.pyi` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogUploadFile.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DialogWorkflow.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DialogWorkflow.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DirectMessageReceived.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DirectMessageReceived.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DirectTextMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DirectTextMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DocumentSignatureEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DocumentSignatureEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DocumentSignatureLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DocumentSignatureLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DocumentSignatureProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DocumentSignatureProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/DoublePropertyFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/DoublePropertyFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EMailTag.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EMailTag.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAIMPMessagePayloadDef.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAIMPMessagePayloadDef.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAPILogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAPILogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityInvitation.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityInvitation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityMember.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityMember.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityMemberInvitation.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAccountOpportunityMemberInvitation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgent.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentConfiguration.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentConfiguration.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstallConfiguration.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstallConfiguration.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceDeployment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceDeployment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceDeploymentChannel.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceDeploymentChannel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceMessageDeployment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstanceMessageDeployment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentInstancePayloadDeployment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentInstancePayloadDeployment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAgentPolicy.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAgentPolicy.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAlexaLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAlexaLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAnonymousLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAnonymousLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAssetNode.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAssetNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAssignedPerson.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAssignedPerson.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAssignee.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAssignee.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAttendee.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAttendee.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasAuthor.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasAuthor.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBot.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBotChatRuleSet.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBotChatRuleSet.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBotDialog.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBotDialog.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBotImplementation.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBotImplementation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasBusinessRelationshipWith.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasBusinessRelationshipWith.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasCalendarLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasCalendarLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChannel.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChannel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChannelBot.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChannelBot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChatRule.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChatRule.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChatRuleSet.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChatRuleSet.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChatRuleSetFile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChatRuleSetFile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChildChannel.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChildChannel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasChoice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasChoice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasContract.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasContract.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasCustomer.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasCustomer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDataScript.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDataScript.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDataScriptInput.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDataScriptInput.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDependentProjectTask.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDependentProjectTask.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDevice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDevice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialog.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialog.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialogAction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialogAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialogCondition.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialogCondition.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialogRow.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialogRow.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDialogSession.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDialogSession.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDocument.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDocument.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasDocumentSignatureLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasDocumentSignatureLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEmailAttachment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEmailAttachment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEmailForward.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEmailForward.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEmailLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEmailLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEmailSummary.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEmailSummary.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEndpointProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEndpointProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEntityProperty.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEntityProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasEntitySet.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasEntitySet.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasExternalAccount.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasExternalAccount.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasFacebookLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasFacebookLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasFileNode.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasFileNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasFolder.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasFolder.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasIFrameTemplate.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasIFrameTemplate.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasInvoice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasInvoice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedCustomer.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedCustomer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInCompanyAffiliation.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInCompanyAffiliation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInRecipientInvite.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInRecipientInvite.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInRecipientMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInRecipientMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInSenderInvite.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInSenderInvite.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLinkedInSenderMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLinkedInSenderMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasLoginChannelBot.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasLoginChannelBot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasPayment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasPayment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasPaymentLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasPaymentLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasPermittedSender.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasPermittedSender.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProfileSession.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProfileSession.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProjectList.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProjectList.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProjectStep.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProjectStep.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProjectTask.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProjectTask.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasProposal.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasProposal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasQuery.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasQuery.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasQueryCriterion.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasQueryCriterion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasReferencedNode.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasReferencedNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasRelationship.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasRelationship.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasRelationshipProperty.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasRelationshipProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasRelationshipSet.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasRelationshipSet.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSelectedDataScript.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSelectedDataScript.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSelectedQuery.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSelectedQuery.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSessionChannel.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSessionChannel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSignedDocument.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSignedDocument.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSlackLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSlackLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasSmsLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasSmsLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasTwitterLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasTwitterLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Edge_hasUserAvatar.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Edge_hasUserAvatar.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailAttachment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailAttachment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailMessage.pyi` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailMessage.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailReceived.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailReceived.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailSummary.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailSummary.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmailsList.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmailsList.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EmbeddedCard.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EmbeddedCard.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EnclosingPageNotification.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EnclosingPageNotification.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EnclosingPageURLButtonClickedMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EnclosingPageURLButtonClickedMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Endpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Endpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EndpointProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EndpointProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EndpointProfileMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EndpointProfileMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EndpointProfilesMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EndpointProfilesMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EnlargeCardCommand.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EnlargeCardCommand.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Entity.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Entity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntityCommandMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntityCommandMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntityFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntityFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntityMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntityMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntityProperty.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntityProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/EntitySet.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/EntitySet.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ErrorNode.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ErrorNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ExternalInteraction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ExternalInteraction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ExternalInteractionPart.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ExternalInteractionPart.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ExternalInteractionTransaction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ExternalInteractionTransaction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookIncomingMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookIncomingMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookOutgoingMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookOutgoingMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookPost.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookPost.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FacebookProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FacebookProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FactsListMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FactsListMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FavoriteTweet.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FavoriteTweet.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FileAnswer.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FileAnswer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FileChatRuleSet.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FileChatRuleSet.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FileQuestion.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FileQuestion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FileUploadObject.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FileUploadObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Folder.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Folder.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FormDialog.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FormDialog.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/FormPageAnswersMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/FormPageAnswersMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GeoLocationAnswer.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GeoLocationAnswer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GeoLocationPropertyFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GeoLocationPropertyFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetChannelHistoryMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetChannelHistoryMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetFactsMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetFactsMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetJoinedChannels.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetJoinedChannels.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetObjectMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetObjectMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GetObjectResultsMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GetObjectResultsMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GoogleHomeDevice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GoogleHomeDevice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GraphLabel.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GraphLabel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GraphObjectFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GraphObjectFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/GroupStringPropertyFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/GroupStringPropertyFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyActivityMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyActivityMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyArticleMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyArticleMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyAudioMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyAudioMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBot.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBot.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotConfiguration.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotConfiguration.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotInstall.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotInstall.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotInstallConfiguration.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotInstallConfiguration.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotInstance.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotInstance.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotInstanceDeployment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotInstanceDeployment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyBotPolicy.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyBotPolicy.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyCalendarMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyCalendarMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyChannelCardsListMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyChannelCardsListMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyChartMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyChartMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyCheckListMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyCheckListMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyChildResponseMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyChildResponseMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyCommandMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyCommandMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyDevice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyDevice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyDeviceDetailsMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyDeviceDetailsMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyDialogAppMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyDialogAppMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyEmailsListMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyEmailsListMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyFacebookMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyFacebookMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyFacebookStatusPanelMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyFacebookStatusPanelMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyFileDownloadMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyFileDownloadMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyFileUploadMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyFileUploadMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyImageGalleryMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyImageGalleryMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyImageMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyImageMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyKnowledgeExtractionMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyKnowledgeExtractionMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInInviteMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInInviteMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInPostMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInPostMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInSearchMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInSearchMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyLinkedInTextMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyLinkedInTextMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyMapMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyMapMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyMovieDetailsMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyMovieDetailsMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyMoviesRecommendationsListMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyMoviesRecommendationsListMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyNotificationMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyNotificationMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyPaymentConfirmationMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyPaymentConfirmationMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyProductMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyProductMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyProgressMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyProgressMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyQuestionDialogAppMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyQuestionDialogAppMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyRealtimeMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyRealtimeMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleySearchResultsMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleySearchResultsMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyShoppingCartMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyShoppingCartMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyStatusMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyStatusMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyStatusType.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyStatusType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyTextMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyTextMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyThingMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyThingMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyThingWideMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyThingWideMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyTranslationMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyTranslationMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyTweetMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyTweetMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyTwitterStatusPanelMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyTwitterStatusPanelMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyVideoMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyVideoMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyWeatherMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyWeatherMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HaleyWebviewMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HaleyWebviewMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HeartbeatMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HeartbeatMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HueLightDevice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HueLightDevice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasAccountAction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasAccountAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasBridgeInteractionPartChain.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasBridgeInteractionPartChain.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasCardPart.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasCardPart.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasChannelCard.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasChannelCard.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasDialogPart.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasDialogPart.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionChain.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionChain.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionPart.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionPart.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionPartChain.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionPartChain.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionTransaction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasExternalInteractionTransaction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasGraphObjectFactElement.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasGraphObjectFactElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionChain.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionChain.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionPart.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionPart.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionPartChain.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionPartChain.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionTransaction.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasInteractionTransaction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasListFactElement.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasListFactElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasMessagePayload.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasMessagePayload.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/HyperEdge_hasProjectListElement.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/HyperEdge_hasProjectListElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IFrameEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IFrameEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IFrameEventMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IFrameEventMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IFrameTemplate.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IFrameTemplate.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Image.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Image.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ImageGallery.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ImageGallery.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ImageObject.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ImageObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InformationMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InformationMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IntegerPropertyFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IntegerPropertyFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Intent.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Intent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IntentMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IntentMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InterAccountMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InterAccountMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InteractionModeMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InteractionModeMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InterruptProcessorMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InterruptProcessorMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InvalidateMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InvalidateMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/InvalidateQuestionMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/InvalidateQuestionMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Invoice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Invoice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/IosDeviceProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/IosDeviceProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/JiboDevice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/JiboDevice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/JoinChannel.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/JoinChannel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/KnowledgeExtractionCard.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/KnowledgeExtractionCard.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LeaveChannel.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LeaveChannel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LightDevice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LightDevice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInCompanyProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInCompanyProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInInvitation.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInInvitation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInPersonProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInPersonProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInPost.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInPost.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LinkedInProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LinkedInProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListChannelsRequestMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListChannelsRequestMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListChannelsResultsMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListChannelsResultsMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListEndpointProfilesMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListEndpointProfilesMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ListJoinedChannelsResultsMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ListJoinedChannelsResultsMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LoginDataEvent.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LoginDataEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LoginOnboardingStatus.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LoginOnboardingStatus.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/LoginStatus.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/LoginStatus.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ManagedChatRuleSet.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ManagedChatRuleSet.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MapObject.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MapObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Media.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Media.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MemoryFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MemoryFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MenuClickedMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MenuClickedMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MessageService.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MessageService.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MetaQLMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MetaQLMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MetaQLResultsMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MetaQLResultsMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MmsAttachment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MmsAttachment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MotionMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MotionMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Movie.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Movie.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MoviesList.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MoviesList.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/MultiChoiceQuestion.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/MultiChoiceQuestion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/NextAudioCommand.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/NextAudioCommand.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/NotificationMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/NotificationMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/OpenIFrame.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/OpenIFrame.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/OpenPanelCommand.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/OpenPanelCommand.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Opportunity.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Opportunity.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PauseMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PauseMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PayloadStyleType.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PayloadStyleType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Payment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Payment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentConfirmation.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentConfirmation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentProcessorEvent.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentProcessorEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PaymentQuestion.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PaymentQuestion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PermittedSender.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PermittedSender.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PermittedSenderStatus.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PermittedSenderStatus.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PermittedSenderType.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PermittedSenderType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PlayAudioCommand.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PlayAudioCommand.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PlayVideoCommand.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PlayVideoCommand.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PredictionFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PredictionFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorAreYouAliveMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorAreYouAliveMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorError.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorError.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorEvent.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorEvent.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorEventType.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorEventType.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorHeartbeatMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorHeartbeatMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorJoinedMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorJoinedMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorLeftMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorLeftMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorRequestMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorRequestMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProcessorResponseMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProcessorResponseMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProgressItem.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProgressItem.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProgressObject.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProgressObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Project.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Project.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProjectList.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProjectList.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProjectStep.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProjectStep.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ProjectTask.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ProjectTask.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PropertyFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PropertyFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Proposal.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Proposal.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PurgeSessionMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PurgeSessionMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/PushNotification.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/PushNotification.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Query.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Query.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QueryCriterion.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QueryCriterion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Question.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Question.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Question.pyi` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Question.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionUpdateMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionUpdateMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionsPageMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionsPageMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionsPageMessage.pyi` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionsPageMessage.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionsPageNavigationMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionsPageNavigationMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/QuestionsPageTheme.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/QuestionsPageTheme.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RealtimeTickMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RealtimeTickMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RefreshChannelCommand.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RefreshChannelCommand.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationshipCommandMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationshipCommandMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationshipMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationshipMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationshipProperty.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationshipProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RelationshipSet.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RelationshipSet.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RemoveCardCommand.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RemoveCardCommand.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RemoveEndpointProfileMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RemoveEndpointProfileMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RemoveQuestionMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RemoveQuestionMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ResultListFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ResultListFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Review.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Review.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ReviewSummary.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ReviewSummary.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/RobotDevice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/RobotDevice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ScrollToQuestionMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ScrollToQuestionMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SearchRequestMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SearchRequestMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SearchResult.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SearchResult.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SearchResultsList.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SearchResultsList.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendDirectMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendDirectMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendEmail.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendEmail.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendPushNotificationMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendPushNotificationMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendSms.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendSms.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendTweet.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendTweet.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SendVoiceMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SendVoiceMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Session.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Session.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SessionClosedMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SessionClosedMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SessionEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SessionEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SessionExpiredMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SessionExpiredMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SetFactMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SetFactMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SettingsMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SettingsMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ShoppingCart.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ShoppingCart.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ShrinkCardCommand.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ShrinkCardCommand.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SingleSignOnProvider.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SingleSignOnProvider.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackIncomingMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackIncomingMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackOutgoingMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackOutgoingMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SlackTextMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SlackTextMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmartDevice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmartDevice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Sms.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Sms.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsReceived.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsReceived.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SmsTextMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SmsTextMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SolutionFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SolutionFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SpeechMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SpeechMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SpheroDevice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SpheroDevice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StatusMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StatusMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StopAudioCommand.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StopAudioCommand.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StopVideoCommand.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StopVideoCommand.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StringPropertyFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StringPropertyFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/StripePayment.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/StripePayment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SwitchDevice.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SwitchDevice.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SwitchEnclosingPageToURL.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SwitchEnclosingPageToURL.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/SystemTickMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/SystemTickMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Task.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Task.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ThingCard.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ThingCard.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ThingCard.pyi` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ThingCard.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ThingWideCard.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ThingWideCard.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/ThinkingMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/ThinkingMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TickMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TickMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TimeoutMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TimeoutMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Translation.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Translation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TreeQuestion.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TreeQuestion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TrendResult.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TrendResult.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TrueFalseAnswer.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TrueFalseAnswer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TrueFalseQuestion.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TrueFalseQuestion.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TruthPropertyFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TruthPropertyFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TweetReceived.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TweetReceived.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TweetTextMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TweetTextMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterEndpoint.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterEndpoint.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterLogin.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterLogin.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterQueryRequestMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterQueryRequestMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/TwitterQueryResultsMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/TwitterQueryResultsMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/URIPropertyFact.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/URIPropertyFact.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UnsetFactMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UnsetFactMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UpdateSessionMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UpdateSessionMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserAnswerDialogAppMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserAnswerDialogAppMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserAvatar.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserAvatar.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserChatRequestMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserChatRequestMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserCommandMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserCommandMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserDialogAppMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserDialogAppMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserLeftApp.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserLeftApp.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserLoggedIn.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserLoggedIn.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserLoggedOut.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserLoggedOut.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserProfile.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserProfile.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserProfileMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserProfileMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserStatusMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserStatusMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/UserTextMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/UserTextMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/Video.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/Video.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/VideoObject.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/VideoObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/VirtualLoginRequestMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/VirtualLoginRequestMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/VirtualLoginResponseMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/VirtualLoginResponseMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/VoiceMessage.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/VoiceMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/WeMoSwitch.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/WeMoSwitch.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/WeatherForecast.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/WeatherForecast.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/com_vitalai_aimp_domain/model/WebviewCard.py` & `vital-ai-aimp-0.1.4/com_vitalai_aimp_domain/model/WebviewCard.py`

 * *Files identical despite different names*

### Comparing `vital-ai-aimp-0.1.3/vital_ai_aimp.egg-info/PKG-INFO` & `vital-ai-aimp-0.1.4/vital_ai_aimp.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: vital-ai-aimp
-Version: 0.1.3
+Version: 0.1.4
 Summary: VitalSigns aimp domain
 Home-page: https://github.com/vital-ai/vitalhome-aimp
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: vital-ai-domain==0.1.3
-Requires-Dist: vital-ai-social==0.1.3
-Requires-Dist: vital-ai-nlp==0.1.3
+Requires-Dist: vital-ai-domain>=0.1.4
+Requires-Dist: vital-ai-social>=0.1.4
+Requires-Dist: vital-ai-nlp>=0.1.4
 
 # vital-ai-aimp
```

### Comparing `vital-ai-aimp-0.1.3/vital_ai_aimp.egg-info/SOURCES.txt` & `vital-ai-aimp-0.1.4/vital_ai_aimp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

