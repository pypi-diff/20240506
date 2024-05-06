# Comparing `tmp/vital-ai-social-0.1.3.tar.gz` & `tmp/vital-ai-social-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-ai-social-0.1.3.tar", last modified: Sat May  4 21:26:50 2024, max compression
+gzip compressed data, was "vital-ai-social-0.1.4.tar", last modified: Mon May  6 21:46:01 2024, max compression
```

## Comparing `vital-ai-social-0.1.3.tar` & `vital-ai-social-0.1.4.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:26:50.081610 vital-ai-social-0.1.3/
--rw-r--r--   0 hadfield   (501) staff       (20)      523 2024-05-04 21:26:50.081384 vital-ai-social-0.1.3/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 02:46:51.000000 vital-ai-social-0.1.3/README.md
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:26:50.061817 vital-ai-social-0.1.3/com_vitalai_domain_social/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:23.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:26:50.071290 vital-ai-social-0.1.3/com_vitalai_domain_social/model/
--rw-r--r--   0 hadfield   (501) staff       (20)     1485 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/CampaignAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/CampaignAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1998 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/DirectMessage.py
--rw-r--r--   0 hadfield   (501) staff       (20)      300 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/DirectMessage.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/DomainOntology.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasCampaignAction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasCampaignAction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1344 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasCampaignActionDocument.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasCampaignActionDocument.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1359 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasCampaignActionFilterElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasCampaignActionFilterElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasContextAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasContextAccount.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasFanCountry.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasFanCountry.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasFilter.py
--rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasFilter.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1317 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasFilterElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasFilterElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasSocialLocation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasSocialLocation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1332 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasSocialMediaAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasSocialMediaAccount.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1335 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasSocialMediaCampaign.py
--rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasSocialMediaCampaign.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1649 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasTwitterAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasTwitterAccount.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasTwitterApp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasTwitterApp.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1727 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/FacebookAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      256 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/FacebookAccount.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/FanCountry.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/FanCountry.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1243 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Filter.py
--rw-r--r--   0 hadfield   (501) staff       (20)      114 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Filter.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1264 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/FilterElement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/FilterElement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2030 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/InstagramAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      317 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/InstagramAccount.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1492 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/SocialLocation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/SocialLocation.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1698 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/SocialMediaAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/SocialMediaAccount.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1267 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/SocialMediaApp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/SocialMediaApp.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1282 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/SocialMediaCampaign.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/SocialMediaCampaign.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     3290 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/SoundCloudAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      629 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/SoundCloudAccount.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1282 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/TrackingHandle.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/TrackingHandle.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1285 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/TrackingHashTag.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/TrackingHashTag.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1282 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/TrackingPhrase.py
--rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/TrackingPhrase.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2940 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Tweet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      554 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/Tweet.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2150 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/TwitterAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      364 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/TwitterAccount.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1584 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/TwitterApp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/TwitterApp.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1267 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/TwitterContext.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/TwitterContext.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2333 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/YouTubeAccount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      400 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/YouTubeAccount.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1780 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/YouTubeComment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/YouTubeComment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:23.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:26:50.080362 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasAccessToken.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasActionStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasAuthorID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasAuthorName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasAuthorScreenName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasBio.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasChannelID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasCity.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasCommentCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasCommentID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasConsumerKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasConsumerSecret.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasCountry.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasDirectMessageID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasDiscogsName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasExpiresIn.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasFacebookCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasFacebookID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasFavoriteCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasFollowersCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasFollowingCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasInReplyToScreenName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasInReplyToTweetID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasInReplyToUserID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasInstagramID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasMediaCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasMinutesBetweenTweets.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasMyspaceName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasOAuthTokenSecret.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasOriginalAuthorID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasOriginalAuthorName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasOriginalAuthorScreenName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasPageFansCountry.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasPermalink.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasPermalinkURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasPictureURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasPlaylistsCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasPublishedAt.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasRecipientID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasRecipientName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasRecipientScreenName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasRefreshToken.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasRetweetCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasScreenName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasSocialDescription.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasSocialLikeCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasSocialLocation.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasSocialLocationRadius.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasSocialUsername.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasSoundCloudID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasSoundCloudURI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasSubscriberCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasTracksCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasTweetID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasTweetStatus.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasTweetsCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasTwitterID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasTwitterLatitude.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasTwitterLongitude.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasTwitterOAuthToken.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasVideoCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasVideoID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasViewCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasWebsite.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_hasWebsiteTitle.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_isRetweet.py
--rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_isStreamContextUser.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/Property_isTokenValid.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:23.000000 vital-ai-social-0.1.3/com_vitalai_domain_social/model/properties/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-04 21:26:50.081770 vital-ai-social-0.1.3/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)      931 2024-05-04 21:16:24.000000 vital-ai-social-0.1.3/setup.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-04 21:26:50.081085 vital-ai-social-0.1.3/vital_ai_social.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      523 2024-05-04 21:26:50.000000 vital-ai-social-0.1.3/vital_ai_social.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)     8827 2024-05-04 21:26:50.000000 vital-ai-social-0.1.3/vital_ai_social.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-04 21:26:50.000000 vital-ai-social-0.1.3/vital_ai_social.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       76 2024-05-04 21:26:50.000000 vital-ai-social-0.1.3/vital_ai_social.egg-info/entry_points.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       43 2024-05-04 21:26:50.000000 vital-ai-social-0.1.3/vital_ai_social.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       26 2024-05-04 21:26:50.000000 vital-ai-social-0.1.3/vital_ai_social.egg-info/top_level.txt
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:46:01.730774 vital-ai-social-0.1.4/
+-rw-r--r--   0 hadfield   (501) staff       (20)      523 2024-05-06 21:46:01.730331 vital-ai-social-0.1.4/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 02:46:51.000000 vital-ai-social-0.1.4/README.md
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:46:01.709308 vital-ai-social-0.1.4/com_vitalai_domain_social/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:23.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:46:01.719184 vital-ai-social-0.1.4/com_vitalai_domain_social/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)     1485 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/CampaignAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      176 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/CampaignAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1998 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/DirectMessage.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      300 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/DirectMessage.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/DomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasCampaignAction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasCampaignAction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1344 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasCampaignActionDocument.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasCampaignActionDocument.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1359 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasCampaignActionFilterElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasCampaignActionFilterElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasContextAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasContextAccount.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasFanCountry.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasFanCountry.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1296 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasFilter.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      151 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasFilter.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1317 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasFilterElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasFilterElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1320 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasSocialLocation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasSocialLocation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1332 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasSocialMediaAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      163 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasSocialMediaAccount.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1335 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasSocialMediaCampaign.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      164 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasSocialMediaCampaign.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1649 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasTwitterAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      244 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasTwitterAccount.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1308 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasTwitterApp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      155 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasTwitterApp.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1727 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/FacebookAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      256 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/FacebookAccount.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1364 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/FanCountry.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/FanCountry.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1243 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Filter.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      114 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Filter.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1264 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/FilterElement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      121 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/FilterElement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2030 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/InstagramAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      317 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/InstagramAccount.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1492 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/SocialLocation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      178 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/SocialLocation.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1698 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/SocialMediaAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/SocialMediaAccount.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1267 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/SocialMediaApp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/SocialMediaApp.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1282 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/SocialMediaCampaign.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/SocialMediaCampaign.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     3290 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/SoundCloudAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      629 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/SoundCloudAccount.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1282 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/TrackingHandle.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/TrackingHandle.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1285 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/TrackingHashTag.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/TrackingHashTag.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1282 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/TrackingPhrase.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      137 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/TrackingPhrase.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2940 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Tweet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      554 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/Tweet.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2150 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/TwitterAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      364 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/TwitterAccount.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1584 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/TwitterApp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      204 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/TwitterApp.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1267 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/TwitterContext.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/TwitterContext.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2333 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/YouTubeAccount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      400 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/YouTubeAccount.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1780 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/YouTubeComment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      231 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/YouTubeComment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:23.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:46:01.729106 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasAccessToken.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasActionStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasAuthorID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasAuthorName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasAuthorScreenName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasBio.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasChannelID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasCity.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasCommentCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasCommentID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasConsumerKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasConsumerSecret.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasCountry.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasDirectMessageID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasDiscogsName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasExpiresIn.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasFacebookCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasFacebookID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasFavoriteCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasFollowersCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasFollowingCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasInReplyToScreenName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasInReplyToTweetID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasInReplyToUserID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasInstagramID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasMediaCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasMinutesBetweenTweets.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasMyspaceName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasOAuthTokenSecret.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasOriginalAuthorID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasOriginalAuthorName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      237 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasOriginalAuthorScreenName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasPageFansCountry.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasPermalink.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasPermalinkURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasPictureURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasPlaylistsCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasPublishedAt.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasRecipientID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasRecipientName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasRecipientScreenName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasRefreshToken.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasRetweetCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasScreenName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasSocialDescription.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasSocialLikeCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasSocialLocation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasSocialLocationRadius.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasSocialUsername.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasSoundCloudID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasSoundCloudURI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasSubscriberCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasTracksCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasTweetID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasTweetStatus.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasTweetsCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasTwitterID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasTwitterLatitude.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasTwitterLongitude.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasTwitterOAuthToken.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasVideoCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasVideoID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasViewCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasWebsite.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_hasWebsiteTitle.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_isRetweet.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      221 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_isStreamContextUser.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 21:21:48.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/Property_isTokenValid.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-20 04:38:23.000000 vital-ai-social-0.1.4/com_vitalai_domain_social/model/properties/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-06 21:46:01.730841 vital-ai-social-0.1.4/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)      931 2024-05-06 21:44:02.000000 vital-ai-social-0.1.4/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-06 21:46:01.729898 vital-ai-social-0.1.4/vital_ai_social.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      523 2024-05-06 21:46:01.000000 vital-ai-social-0.1.4/vital_ai_social.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)     8827 2024-05-06 21:46:01.000000 vital-ai-social-0.1.4/vital_ai_social.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-06 21:46:01.000000 vital-ai-social-0.1.4/vital_ai_social.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       76 2024-05-06 21:46:01.000000 vital-ai-social-0.1.4/vital_ai_social.egg-info/entry_points.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       43 2024-05-06 21:46:01.000000 vital-ai-social-0.1.4/vital_ai_social.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       26 2024-05-06 21:46:01.000000 vital-ai-social-0.1.4/vital_ai_social.egg-info/top_level.txt
```

### Comparing `vital-ai-social-0.1.3/PKG-INFO` & `vital-ai-social-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: vital-ai-social
-Version: 0.1.3
+Version: 0.1.4
 Summary: VitalSigns social domain
 Home-page: https://github.com/vital-ai/vitalhome-aimp
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: vital-ai-domain==0.1.3
-Requires-Dist: vital-ai-nlp==0.1.3
+Requires-Dist: vital-ai-domain>=0.1.4
+Requires-Dist: vital-ai-nlp>=0.1.4
```

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/CampaignAction.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/CampaignAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/DirectMessage.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/DirectMessage.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasCampaignAction.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasCampaignAction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasCampaignActionDocument.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasCampaignActionDocument.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasCampaignActionFilterElement.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasCampaignActionFilterElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasContextAccount.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasContextAccount.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasFanCountry.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasFanCountry.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasFilter.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasFilter.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasFilterElement.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasFilterElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasSocialLocation.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasSocialLocation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasSocialMediaAccount.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasSocialMediaAccount.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasSocialMediaCampaign.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasSocialMediaCampaign.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasTwitterAccount.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasTwitterAccount.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Edge_hasTwitterApp.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Edge_hasTwitterApp.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/FacebookAccount.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/FacebookAccount.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/FanCountry.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/FanCountry.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Filter.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Filter.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/FilterElement.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/FilterElement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/InstagramAccount.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/InstagramAccount.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/SocialLocation.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/SocialLocation.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/SocialMediaAccount.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/SocialMediaAccount.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/SocialMediaApp.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/SocialMediaApp.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/SocialMediaCampaign.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/SocialMediaCampaign.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/SoundCloudAccount.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/SoundCloudAccount.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/SoundCloudAccount.pyi` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/SoundCloudAccount.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/TrackingHandle.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/TrackingHandle.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/TrackingHashTag.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/TrackingHashTag.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/TrackingPhrase.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/TrackingPhrase.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Tweet.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Tweet.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/Tweet.pyi` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/Tweet.pyi`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/TwitterAccount.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/TwitterAccount.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/TwitterApp.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/TwitterApp.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/TwitterContext.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/TwitterContext.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/YouTubeAccount.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/YouTubeAccount.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/com_vitalai_domain_social/model/YouTubeComment.py` & `vital-ai-social-0.1.4/com_vitalai_domain_social/model/YouTubeComment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-social-0.1.3/setup.py` & `vital-ai-social-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vital-ai-social',
-    version='0.1.3',
+    version='0.1.4',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='VitalSigns social domain',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/vitalhome-aimp',
     packages=find_packages(),
@@ -16,16 +16,16 @@
         ]
     },
     package_data={
          '': ['*.pyi'],
     },
     license='Apache License 2.0',
     install_requires=[
-            'vital-ai-domain==0.1.3',
-            'vital-ai-nlp==0.1.3'
+            'vital-ai-domain>=0.1.4',
+            'vital-ai-nlp>=0.1.4'
         ],
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.10',
```

### Comparing `vital-ai-social-0.1.3/vital_ai_social.egg-info/PKG-INFO` & `vital-ai-social-0.1.4/vital_ai_social.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: vital-ai-social
-Version: 0.1.3
+Version: 0.1.4
 Summary: VitalSigns social domain
 Home-page: https://github.com/vital-ai/vitalhome-aimp
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: vital-ai-domain==0.1.3
-Requires-Dist: vital-ai-nlp==0.1.3
+Requires-Dist: vital-ai-domain>=0.1.4
+Requires-Dist: vital-ai-nlp>=0.1.4
```

### Comparing `vital-ai-social-0.1.3/vital_ai_social.egg-info/SOURCES.txt` & `vital-ai-social-0.1.4/vital_ai_social.egg-info/SOURCES.txt`

 * *Files identical despite different names*

