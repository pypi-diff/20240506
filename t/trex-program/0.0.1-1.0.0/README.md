# Comparing `tmp/trex-program-0.0.1.tar.gz` & `tmp/trex-program-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-program-0.0.1.tar", last modified: Mon Apr 29 02:46:57 2024, max compression
+gzip compressed data, was "trex-program-1.0.0.tar", last modified: Mon May  6 07:41:26 2024, max compression
```

## Comparing `trex-program-0.0.1.tar` & `trex-program-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-29 02:46:57.684144 trex-program-0.0.1/
--rw-r--r--   0 jacklok    (501) staff       (20)      454 2024-04-29 02:46:57.684038 trex-program-0.0.1/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       29 2024-04-29 02:35:10.000000 trex-program-0.0.1/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-04-29 02:46:57.684573 trex-program-0.0.1/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)     1035 2024-04-29 02:10:38.000000 trex-program-0.0.1/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-29 02:46:57.671360 trex-program-0.0.1/trex-program/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-29 02:09:35.000000 trex-program-0.0.1/trex-program/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-29 02:46:57.671604 trex-program-0.0.1/trex-program/membership/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-13 09:03:21.000000 trex-program-0.0.1/trex-program/membership/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-29 02:46:57.671851 trex-program-0.0.1/trex-program/referral/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-29 02:12:22.000000 trex-program-0.0.1/trex-program/referral/__init__.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-29 02:46:57.679095 trex-program-0.0.1/trex-program/reward_program/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-04-20 08:07:50.000000 trex-program-0.0.1/trex-program/reward_program/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      967 2024-04-29 02:15:05.000000 trex-program-0.0.1/trex-program/reward_program/birthday_reward_program.py
--rw-r--r--   0 jacklok    (501) staff       (20)     9338 2024-04-29 02:15:12.000000 trex-program-0.0.1/trex-program/reward_program/giveaway_new_joined_membership_reward_program.py
--rw-r--r--   0 jacklok    (501) staff       (20)     8906 2024-04-29 02:15:20.000000 trex-program-0.0.1/trex-program/reward_program/giveaway_reward_program.py
--rw-r--r--   0 jacklok    (501) staff       (20)    17970 2024-04-29 02:15:28.000000 trex-program-0.0.1/trex-program/reward_program/lucky_draw_program.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7714 2024-04-29 02:15:36.000000 trex-program-0.0.1/trex-program/reward_program/point_reward_program.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6292 2024-04-29 02:15:45.000000 trex-program-0.0.1/trex-program/reward_program/prepaid_program.py
--rw-r--r--   0 jacklok    (501) staff       (20)    26657 2023-12-17 14:33:16.000000 trex-program-0.0.1/trex-program/reward_program/reward_program_base.py
--rw-r--r--   0 jacklok    (501) staff       (20)    42280 2024-04-29 02:14:47.000000 trex-program-0.0.1/trex-program/reward_program/reward_program_factory.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7356 2024-04-29 02:16:12.000000 trex-program-0.0.1/trex-program/reward_program/stamp_reward_program.py
--rw-r--r--   0 jacklok    (501) staff       (20)      470 2024-04-29 02:45:50.000000 trex-program-0.0.1/trex-program/reward_program/tier_membership_program.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12649 2024-04-29 02:19:06.000000 trex-program-0.0.1/trex-program/reward_program/tier_reward_program.py
--rw-r--r--   0 jacklok    (501) staff       (20)      975 2024-04-29 02:16:41.000000 trex-program-0.0.1/trex-program/reward_program/voucher_reward_program.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-29 02:46:57.679854 trex-program-0.0.1/trex-program/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-29 02:20:35.000000 trex-program-0.0.1/trex-program/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15373 2023-04-12 03:14:25.000000 trex-program-0.0.1/trex-program/utils/tier_reward_program_helper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-04-29 02:46:57.683587 trex-program-0.0.1/trex_program.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      454 2024-04-29 02:46:57.000000 trex-program-0.0.1/trex_program.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1075 2024-04-29 02:46:57.000000 trex-program-0.0.1/trex_program.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-04-29 02:46:57.000000 trex-program-0.0.1/trex_program.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       20 2024-04-29 02:46:57.000000 trex-program-0.0.1/trex_program.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       13 2024-04-29 02:46:57.000000 trex-program-0.0.1/trex_program.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:41:26.106272 trex-program-1.0.0/
+-rw-r--r--   0 jacklok    (501) staff       (20)      454 2024-05-06 07:41:26.106169 trex-program-1.0.0/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       29 2024-04-29 02:35:10.000000 trex-program-1.0.0/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2024-05-06 07:41:26.106702 trex-program-1.0.0/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)     1035 2024-05-06 07:41:12.000000 trex-program-1.0.0/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:41:26.105745 trex-program-1.0.0/trex_program.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      454 2024-05-06 07:41:26.000000 trex-program-1.0.0/trex_program.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1087 2024-05-06 07:41:26.000000 trex-program-1.0.0/trex_program.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2024-05-06 07:41:26.000000 trex-program-1.0.0/trex_program.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       20 2024-05-06 07:41:26.000000 trex-program-1.0.0/trex_program.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       12 2024-05-06 07:41:26.000000 trex-program-1.0.0/trex_program.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:41:26.084406 trex-program-1.0.0/trexprogram/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-29 02:09:35.000000 trex-program-1.0.0/trexprogram/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:41:26.084621 trex-program-1.0.0/trexprogram/membership/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-13 09:03:21.000000 trex-program-1.0.0/trexprogram/membership/__init__.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:41:26.085090 trex-program-1.0.0/trexprogram/referral/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-29 02:12:22.000000 trex-program-1.0.0/trexprogram/referral/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    21427 2024-05-02 09:13:35.000000 trex-program-1.0.0/trexprogram/referral/referral_program.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:41:26.102614 trex-program-1.0.0/trexprogram/reward_program/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-04-20 08:07:50.000000 trex-program-1.0.0/trexprogram/reward_program/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1010 2024-05-02 05:39:48.000000 trex-program-1.0.0/trexprogram/reward_program/birthday_reward_program.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     9240 2024-05-02 05:35:43.000000 trex-program-1.0.0/trexprogram/reward_program/giveaway_new_joined_membership_reward_program.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     8862 2024-05-02 05:35:48.000000 trex-program-1.0.0/trexprogram/reward_program/giveaway_reward_program.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    17991 2024-05-02 05:36:10.000000 trex-program-1.0.0/trexprogram/reward_program/lucky_draw_program.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7697 2024-05-02 05:36:18.000000 trex-program-1.0.0/trexprogram/reward_program/point_reward_program.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6211 2024-05-02 05:36:29.000000 trex-program-1.0.0/trexprogram/reward_program/prepaid_program.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    26812 2024-05-02 03:01:13.000000 trex-program-1.0.0/trexprogram/reward_program/reward_program_base.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    42252 2024-05-02 05:36:42.000000 trex-program-1.0.0/trexprogram/reward_program/reward_program_factory.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7339 2024-05-02 05:36:53.000000 trex-program-1.0.0/trexprogram/reward_program/stamp_reward_program.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12546 2024-05-02 05:38:06.000000 trex-program-1.0.0/trexprogram/reward_program/tier_reward_program.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      974 2024-05-02 05:38:13.000000 trex-program-1.0.0/trexprogram/reward_program/voucher_reward_program.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2024-05-06 07:41:26.104733 trex-program-1.0.0/trexprogram/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2024-04-29 02:20:35.000000 trex-program-1.0.0/trexprogram/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2412 2024-05-02 05:39:57.000000 trex-program-1.0.0/trexprogram/utils/reward_program_helper.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15336 2024-05-02 05:38:20.000000 trex-program-1.0.0/trexprogram/utils/tier_reward_program_helper.py
```

### Comparing `trex-program-0.0.1/setup.py` & `trex-program-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 setuptools.setup(
     #Application name and details
      name='trex-program',
      description="TRex Program package",
      long_description=long_description,
      long_description_content_type="text/markdown",  
      url="https://bitbucket.org/lokjac/trex-program",
-     version='0.0.1',
+     version='1.0.0',
      
      #Author details
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      
      #packages=setuptools.find_packages(),
      packages=setuptools.find_packages(),
```

### Comparing `trex-program-0.0.1/trex-program/reward_program/birthday_reward_program.py` & `trex-program-1.0.0/trexprogram/reward_program/birthday_reward_program.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Created on 15 Sep 2021
 
 @author: jacklok
 '''
-from trexmodel import program_conf
+from trexconf import program_conf
 import logging
 from trexprogram.reward_program.giveaway_reward_program import GiveawayRewardProgram
 
 logger = logging.getLogger('reward-program-lib')
 
 class BirthdayRewardProgram(GiveawayRewardProgram):
     
@@ -15,9 +15,11 @@
         super(BirthdayRewardProgram, self).__init__(program_configuration, currency=currency)
         
         self.reward_format          = program_configuration.get('reward_format')
         self.giveaway_method        = program_conf.PROGRAM_REWARD_GIVEAWAY_METHOD_SYSTEM
         
         logger.debug('GiveawayRewardProgram: reward_format=%s', self.reward_format)
         
-        if not self.reward_format in (program_conf.REWARD_FORMAT_POINT, program_conf.REWARD_FORMAT_STAMP, program_conf.REWARD_FORMAT_VOUCHER, program_conf.REWARD_FORMAT_MIXED):
+        if not self.reward_format in (program_conf.REWARD_FORMAT_POINT, 
+                                      program_conf.REWARD_FORMAT_STAMP, 
+                                      program_conf.REWARD_FORMAT_VOUCHER):
             raise Exception('Invalid program configuration')
```

### Comparing `trex-program-0.0.1/trex-program/reward_program/giveaway_new_joined_membership_reward_program.py` & `trex-program-1.0.0/trexprogram/reward_program/giveaway_new_joined_membership_reward_program.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 '''
 Created on 13 Mar 2023
 
 @author: jacklok
 '''
+from trexprogram.utils.reward_program_helper import calculate_expiry_date
 
 '''
 Created on 19 May 2021
 
 @author: jacklok
 '''
 
 from trexprogram.reward_program.reward_program_base import SchemeRewardProgram, VoucherRewardProgramBase,\
     EntitledVoucherSummary
 from trexmodel.models.datastore.reward_models import CustomerPointReward,\
     CustomerStampReward, CustomerEntitledVoucher
-from trexmodel import program_conf
-from trexadmin import conf as app_conf
+from trexconf import program_conf
 import logging
-from datetime import datetime, timedelta
 from trexmodel.models.datastore.voucher_models import MerchantVoucher
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
 
 logger = logging.getLogger('reward-program-lib')
 
 class GiveawayNewJoinedMembershipRewardProgram(SchemeRewardProgram, VoucherRewardProgramBase):
     
@@ -35,15 +34,15 @@
         logger.debug('GiveawayRewardProgram: reward_format=%s', self.reward_format)
         logger.debug('GiveawayRewardProgram: giveaway_system_condition=%s', self.giveaway_system_condition)
         
         if not self.reward_format in (program_conf.REWARD_FORMAT_POINT, 
                                       program_conf.REWARD_FORMAT_STAMP,
                                       program_conf.REWARD_FORMAT_PREPAID, 
                                       program_conf.REWARD_FORMAT_VOUCHER, 
-                                      program_conf.REWARD_FORMAT_MIXED):
+                                      ):
             raise Exception('Invalid program configuration')    
     
     def give(self, customer_acct, transaction_details, reward_set=1): 
         if self.is_eligible_based_on_exclusivity(customer_acct):
             
             logger.debug('GiveawayRewardProgram: Going to give reward')
             logger.debug('GiveawayRewardProgram: reward_format=%s', self.reward_format)
@@ -59,29 +58,28 @@
             transact_by                     = transaction_details.transact_by_user
             
             transact_outlet                 = transaction_details.transact_outlet_details
             
             reward_unit                     = reward_set
             
             is_membership_purchase          = transaction_details.is_membership_purchase
-            default_reward_unit             = 0
             
             if is_membership_purchase:
-                 pass
+                pass
                 
             
             reward_amount                   = self.calculate_entitle_reward_amount(reward_unit=reward_unit)
             
             effective_date                  = transact_datetime.date()
             
             logger.debug('GiveawayRewardProgram: reward_unit=%s', reward_unit)
             
             if self.reward_format == program_conf.REWARD_FORMAT_POINT:
                 
-                expiry_date                     = self.calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
+                expiry_date                     = calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
                 
                 point_reward = CustomerPointReward.create( 
                                                 customer_acct       = customer_acct, 
                                                 reward_amount       = reward_amount,
                                                 transact_outlet     = transact_outlet, 
                                                 effective_date      = effective_date,
                                                 expiry_date         = expiry_date, 
@@ -105,15 +103,15 @@
 
                 
                 return prepaid_topup_reward
             
             
             elif self.reward_format == program_conf.REWARD_FORMAT_STAMP:
                 
-                expiry_date                     = self.calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
+                expiry_date                     = calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
                 
                 stamp_reward    = CustomerStampReward.create( 
                                             customer_acct       = customer_acct, 
                                             reward_amount       = reward_amount,
                                             transact_outlet     = transact_outlet, 
                                             expiry_date         = expiry_date, 
                                             effective_date      = effective_date,
```

### Comparing `trex-program-0.0.1/trex-program/reward_program/giveaway_reward_program.py` & `trex-program-1.0.0/trexprogram/reward_program/giveaway_reward_program.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 @author: jacklok
 '''
 
 from trexprogram.reward_program.reward_program_base import SchemeRewardProgram, VoucherRewardProgramBase,\
     EntitledVoucherSummary
 from trexmodel.models.datastore.reward_models import CustomerPointReward,\
     CustomerStampReward, CustomerEntitledVoucher
-from trexmodel import program_conf
-from trexadmin import conf as app_conf
+from trexconf import program_conf
 import logging
-from datetime import datetime, timedelta
 from trexmodel.models.datastore.voucher_models import MerchantVoucher
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
+from trexprogram.utils.reward_program_helper import calculate_expiry_date
 
 logger = logging.getLogger('reward-program-lib')
 
 class GiveawayRewardProgram(SchemeRewardProgram, VoucherRewardProgramBase):
     
     def __init__(self, program_configuration, currency=None):
         super(GiveawayRewardProgram, self).__init__(program_configuration, currency=currency)
@@ -27,15 +26,15 @@
         
         logger.debug('GiveawayRewardProgram: reward_format=%s', self.reward_format)
         
         if not self.reward_format in (program_conf.REWARD_FORMAT_POINT, 
                                       program_conf.REWARD_FORMAT_STAMP,
                                       program_conf.REWARD_FORMAT_PREPAID, 
                                       program_conf.REWARD_FORMAT_VOUCHER, 
-                                      program_conf.REWARD_FORMAT_MIXED):
+                                      ):
             raise Exception('Invalid program configuration')    
     
     def give(self, customer_acct, transaction_details, reward_set=1): 
         if self.is_eligible_based_on_exclusivity(customer_acct):
             
             logger.debug('GiveawayRewardProgram: Going to give reward')
             logger.debug('GiveawayRewardProgram: reward_format=%s', self.reward_format)
@@ -60,15 +59,15 @@
             
             effective_date                  = transact_datetime.date()
             
             logger.debug('GiveawayRewardProgram: reward_unit=%s', reward_unit)
             
             if self.reward_format == program_conf.REWARD_FORMAT_POINT:
                 
-                expiry_date                     = self.calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
+                expiry_date                     = calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
                 
                 point_reward = CustomerPointReward.create( 
                                                 customer_acct       = customer_acct, 
                                                 reward_amount       = reward_amount,
                                                 transact_outlet     = transact_outlet, 
                                                 effective_date      = effective_date,
                                                 expiry_date         = expiry_date,
```

### Comparing `trex-program-0.0.1/trex-program/reward_program/lucky_draw_program.py` & `trex-program-1.0.0/trexprogram/reward_program/lucky_draw_program.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 '''
 Created on 30 Jun 2023
 
 @author: jacklok
 '''
 import logging
-from trexmodel import program_conf
+from trexconf import program_conf
 from trexmodel.models.datastore.reward_models import CustomerPointReward,\
     CustomerEntitledVoucher, CustomerStampReward,\
     VoucherRewardDetailsForUpstreamData
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
-from trexprogram.reward_program.reward_program_base import DATE_FORMAT,\
-    EntitledVoucherSummary
+from trexprogram.reward_program.reward_program_base import EntitledVoucherSummary
 from trexmodel.models.datastore.voucher_models import MerchantVoucher
-from datetime import datetime, date
-from dateutil.relativedelta import relativedelta
+from datetime import datetime
 from trexlib.utils.string_util import is_not_empty
 from trexmodel.models.datastore.customer_model_helpers import update_prepaid_summary_with_new_prepaid,\
     update_reward_summary_with_new_reward,\
     update_customer_entiteld_voucher_summary_with_new_voucher_info
 from trexanalytics.bigquery_upstream_data_config import create_merchant_customer_reward_upstream_for_merchant
+from trexprogram.utils.reward_program_helper import calculate_expiry_date,\
+    calculate_effective_date
 
 logger = logging.getLogger('reward-program-lib')
 
 class LuckyDrawRewardProgram():
     
     def __init__(self, drawed_details=None, transact_outlet=None, transaction_details=None, customer_acct=None):
         
@@ -50,15 +50,15 @@
         customer_prepaid_summary            = self.customer_acct.prepaid_summary
         
         if self.prize_type == program_conf.REWARD_FORMAT_POINT:
             reward_amount       = self.won_prize.get('amount')
             effective_date      = datetime.today()
             expiration_type     = self.won_prize.get('expiration_type')
             expiration_value    = self.won_prize.get('expiration_value')    
-            expiry_date         = self.calculate_expiry_date(expiration_type, expiration_value, start_date=effective_date)
+            expiry_date         = calculate_expiry_date(expiration_type, expiration_value, start_date=effective_date)
             
             point_reward = CustomerPointReward.create( 
                                             customer_acct       = self.customer_acct, 
                                             reward_amount       = reward_amount,
                                             transact_outlet     = self.transact_outlet, 
                                             effective_date      = effective_date,
                                             expiry_date         = expiry_date, 
@@ -95,15 +95,15 @@
         
         
         elif self.prize_type == program_conf.REWARD_FORMAT_STAMP:
             reward_amount       = self.won_prize.get('voucher_amount')
             effective_date      = datetime.today()
             expiration_type     = self.won_prize.get('expiration_type')
             expiration_value    = self.won_prize.get('expiration_value')    
-            expiry_date         = self.calculate_expiry_date(expiration_type, expiration_value, start_date=effective_date)
+            expiry_date         = calculate_expiry_date(expiration_type, expiration_value, start_date=effective_date)
             
             stamp_reward    = CustomerStampReward.create( 
                                         customer_acct       = self.customer_acct, 
                                         reward_amount       = reward_amount,
                                         transact_outlet     = self.transact_outlet, 
                                         expiry_date         = expiry_date, 
                                         effective_date      = effective_date,
@@ -128,24 +128,24 @@
             effective_date      = self.won_prize.get('effective_date')
             expiration_type     = self.won_prize.get('expiration_type')
             expiration_value    = self.won_prize.get('expiration_value')
             
             if effective_date is not None:
                 effective_date = datetime.strptime('%d-%m-%Y', effective_date).date()
             else:
-                effective_date  = self.calculate_effective_date(effective_type, effective_value)
+                effective_date  = calculate_effective_date(effective_type, effective_value)
             
             merchant_voucher = MerchantVoucher.fetch(voucher_key)
             
             entiteld_voucher_brief  = EntitledVoucherSummary()
             customer_voucher_list   = []
             
             if merchant_voucher:
                 
-                expiry_date   = self.calculate_expiry_date(expiration_type, expiration_value, start_date=effective_date)
+                expiry_date   = calculate_expiry_date(expiration_type, expiration_value, start_date=effective_date)
                 
                 logger.debug('LuckyDrawRewardProgram debug: merchant_voucher=%s', merchant_voucher)
                 
                 for v in range(voucher_amount):
                     
                     customer_voucher = CustomerEntitledVoucher.create(
                                                                 merchant_voucher,
@@ -246,15 +246,15 @@
         
         self.transaction_details.entitled_reward_summary     = transaction_reward_summary
         self.transaction_details.entitled_prepaid_summary    = transaction_prepaid_summary
         self.transaction_details.entitled_voucher_summary    = transaction_voucher_summary    
         
         self.transaction_details.put()
             
-        
+    '''    
     def calculate_expiry_date(self, expiration_type, expiration_value, start_date=None):
         expiry_date = None
         
         logger.debug('calculate_expiry_date: expiration_type=%s', expiration_type)
         logger.debug('calculate_expiry_date: expiration_value=%s', expiration_value)
         
         if start_date is None:
@@ -291,7 +291,8 @@
             return start_date + relativedelta(weeks=effective_value)
         
         elif effective_type == program_conf.REWARD_EFFECTIVE_TYPE_AFTER_DAY:
             return start_date + relativedelta(days=effective_value)
         
         elif effective_type == program_conf.REWARD_EFFECTIVE_TYPE_IMMEDIATE:
             return start_date
+    '''
```

### Comparing `trex-program-0.0.1/trex-program/reward_program/point_reward_program.py` & `trex-program-1.0.0/trexprogram/reward_program/point_reward_program.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 Created on 20 Apr 2021
 
 @author: jacklok
 '''
 from trexprogram.reward_program.reward_program_base import SchemeRewardProgram,\
     GiveawayRewardBaseProgram
 from trexmodel.models.datastore.reward_models import CustomerPointReward
-from trexmodel import program_conf
-from datetime import datetime, timedelta
-from trexadmin import conf as app_conf
+from trexconf import program_conf
 import logging
+from trexprogram.utils.reward_program_helper import calculate_expiry_date
 
 logger = logging.getLogger('reward-program-lib')
 
 class PointSchemeProgram(SchemeRewardProgram):
     
     def __init__(self, program_configuration, currency=None):
         super(PointSchemeProgram, self).__init__(program_configuration, currency=currency)
@@ -56,15 +55,15 @@
                 
                 transact_by                     = transaction_details.transact_by_user
                 
                 transact_outlet                 = transaction_details.transact_outlet_details
                 
                 
                 effective_date                  = transact_datetime.date()
-                expiry_date                     = self.calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
+                expiry_date                     = calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
                  
                 
                 logger.debug('-------> Going to create point reward where reward amount=%f',reward_amount)
                 
                 reward_status = program_conf.REWARD_STATUS_VALID
                 if is_reach_reward_limit and reward_amount==0:
                     reward_status = program_conf.REWARD_STATUS_REACH_LIMIT
@@ -113,15 +112,15 @@
                 
                 transact_by                     = transaction_details.transact_by_user
                 
                 transact_outlet                 = transaction_details.transact_outlet_details
                 
                 
                 effective_date                  = transact_datetime.date()
-                expiry_date                     = self.calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
+                expiry_date                     = calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
                  
                 
                 logger.debug('-------> Going to create point reward where reward amount=%f',reward_amount)
                 
                 reward_status = program_conf.REWARD_STATUS_VALID
                 
                 point_reward = CustomerPointReward.create(
```

### Comparing `trex-program-0.0.1/trex-program/reward_program/prepaid_program.py` & `trex-program-1.0.0/trexprogram/reward_program/prepaid_program.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 Created on 13 Mar 2023
 
 @author: jacklok
 '''
 
 from trexprogram.reward_program.reward_program_base import SchemeRewardProgram,\
     GiveawayRewardBaseProgram
-from trexmodel import program_conf
-from datetime import datetime, timedelta
-from trexadmin import conf as app_conf
+from trexconf import program_conf
 import logging
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
 
 #logger = logging.getLogger('reward-program-lib')
 logger = logging.getLogger('debug')
 
 class PrepaidSchemeProgram(SchemeRewardProgram):
```

### Comparing `trex-program-0.0.1/trex-program/reward_program/reward_program_base.py` & `trex-program-1.0.0/trexprogram/reward_program/reward_program_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 '''
 Created on 20 Apr 2021
 
 @author: jacklok
 '''
 from datetime import datetime
 from dateutil.relativedelta import relativedelta
-from trexadmin import conf as app_conf
-from trexmodel import program_conf
+from trexconf import conf as app_conf
+from trexconf import program_conf
 import logging
 from trexlib.utils.string_util import is_empty, is_not_empty
 from trexlib.utils.common.currency_util import currency_amount_based_on_currency
 from trexmodel.models.datastore.reward_models import CustomerEntitledVoucher
-from google.cloud import ndb
 from trexmodel.models.datastore.voucher_models import MerchantVoucher
-from datetime import datetime, timedelta, date
+from datetime import date
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
 from dateutil.relativedelta import relativedelta
+from trexconf.program_conf import REWARD_PROGRAM_DATE_FORMAT
+from trexprogram.utils.reward_program_helper import calculate_expiry_date,\
+    calculate_effective_date
 
 logger = logging.getLogger('reward-program-lib')
 #logger = logging.getLogger('debug')
 
 
-DATE_FORMAT = '%d-%m-%Y'
+#DATE_FORMAT = '%d-%m-%Y'
 
 class RewardProgramBase(object):
     """
     Define the interface for reward program
     """
 
     def __init__(self, program_configuration):
@@ -106,14 +108,15 @@
         giveaway_reward_sales_amount = transact_amount - tax_amount
         
         return giveaway_reward_sales_amount 
     
     def get_reward_format(self):
         pass
     
+    '''
     def calculate_expiry_date(self, expiration_type, expiration_value, start_date=None):
         expiry_date = None
         
         logger.debug('calculate_expiry_date: expiration_type=%s', expiration_type)
         logger.debug('calculate_expiry_date: expiration_value=%s', expiration_value)
         
         if start_date is None:
@@ -128,21 +131,22 @@
         elif expiration_type == program_conf.REWARD_EXPIRATION_TYPE_AFTER_WEEK:
             expiry_date =  start_date + relativedelta(weeks=expiration_value)
         
         elif expiration_type == program_conf.REWARD_EXPIRATION_TYPE_AFTER_DAY:
             expiry_date =  start_date + relativedelta(days=expiration_value)
         
         elif expiration_type == program_conf.REWARD_EXPIRATION_TYPE_SPECIFIC_DATE:
-            expiry_date =  datetime.strptime(expiration_value, DATE_FORMAT)
+            expiry_date =  datetime.strptime(expiration_value, REWARD_PROGRAM_DATE_FORMAT)
         
         if isinstance(expiry_date, date):
             return expiry_date
         else:
             return expiry_date.date()   
     
+    
     def calculate_effective_date(self, effective_type, effective_value, start_date=None):
         if start_date is None:
             start_date = datetime.utcnow().date()
         
         if effective_type == program_conf.REWARD_EFFECTIVE_TYPE_AFTER_MONTH:
             return start_date + relativedelta(months=effective_value)
         
@@ -150,15 +154,15 @@
             return start_date + relativedelta(weeks=effective_value)
         
         elif effective_type == program_conf.REWARD_EFFECTIVE_TYPE_AFTER_DAY:
             return start_date + relativedelta(days=effective_value)
         
         elif effective_type == program_conf.REWARD_EFFECTIVE_TYPE_IMMEDIATE:
             return start_date
-
+    '''
 class SchemeBaseRewardProgram(RewardProgramBase):
     
     def __init__(self, program_configuration, currency=None):
         super(SchemeBaseRewardProgram, self).__init__(program_configuration)
         
         self.is_recurring_scheme    = self.program_settings.get('is_recurring_scheme')
         self.spending_currency      = self.program_settings.get('scheme').get('spending_currency')
@@ -431,22 +435,22 @@
                 effective_type          = voucher.get('effective_type')
                 effective_value         = voucher.get('effective_value')
                 effective_date_str      = voucher.get('effective_date')
                 
                  
                 if effective_type == program_conf.REWARD_EFFECTIVE_TYPE_SPECIFIC_DATE:
                     if is_not_empty(effective_date_str):
-                        effective_date = datetime.strptime(effective_date_str, DATE_FORMAT)
+                        effective_date = datetime.strptime(effective_date_str, REWARD_PROGRAM_DATE_FORMAT)
                 else:
-                    effective_date = self.calculate_effective_date(effective_type, effective_value, start_date = transact_date)
+                    effective_date = calculate_effective_date(effective_type, effective_value, start_date = transact_date)
                  
                 expiration_type         = voucher.get('expiration_type')
                 expiration_value        = voucher.get('expiration_value')
                  
-                expiry_date             = self.calculate_expiry_date(expiration_type, expiration_value, start_date=effective_date)
+                expiry_date             = calculate_expiry_date(expiration_type, expiration_value, start_date=effective_date)
                 
                 voucher_amount          = voucher.get('voucher_amount')
                 sales_amount            = self.get_giveaway_reward_sales_amount(transaction_details) if transaction_details else 0
                 
                 reward_unit             = self.calculate_reward_unit(sales_amount)
                  
                 voucher_details         = {
```

### Comparing `trex-program-0.0.1/trex-program/reward_program/reward_program_factory.py` & `trex-program-1.0.0/trexprogram/reward_program/reward_program_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 '''
 Created on 21 Apr 2021
 
 @author: jacklok
 '''
-from trexmodel import program_conf
+from trexconf import program_conf
 from trexprogram.reward_program.point_reward_program import PointSchemeProgram,\
     PointGiveawayProgram
 from trexprogram.reward_program.stamp_reward_program import StampSchemeProgram,\
     StampGiveawayProgram
-from trexadmin import conf
 import logging
 from datetime import datetime
 from trexprogram.reward_program.voucher_reward_program import VoucherProgram
 from trexmodel.models.datastore.reward_models import CustomerCountableReward,\
     VoucherRewardDetailsForUpstreamData
 from trexmodel.models.datastore.customer_model_helpers import update_reward_summary_with_new_reward,\
     update_customer_entiteld_voucher_summary_with_new_voucher_info,\
@@ -23,16 +22,16 @@
 import time
 from trexlib.utils.string_util import is_not_empty
 from trexprogram.reward_program.tier_reward_program import TierRewardProgram
 from trexprogram.reward_program.prepaid_program import PrepaidSchemeProgram,\
     PrepaidGiveawayProgram
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
 
-#logger = logging.getLogger('reward-program-lib')
-logger = logging.getLogger('debug')
+logger = logging.getLogger('reward-program-lib')
+#logger = logging.getLogger('debug')
 
 class RewardProgramFactory:
     
     def __get_spending_mechanism_reward_program(self, program_configuration, currency=None):
         desc            = program_configuration.get('desc')
         reward_base     = program_configuration.get('reward_base')
         reward_format   = program_configuration.get('reward_format')
```

### Comparing `trex-program-0.0.1/trex-program/reward_program/stamp_reward_program.py` & `trex-program-1.0.0/trexprogram/reward_program/stamp_reward_program.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 
 @author: jacklok
 '''
 
 from trexprogram.reward_program.reward_program_base import SchemeRewardProgram,\
     GiveawayRewardBaseProgram
 from trexmodel.models.datastore.reward_models import CustomerStampReward
-from trexmodel import program_conf
-from datetime import datetime, timedelta
-from trexadmin import conf as app_conf
+from trexconf import program_conf
 import logging
+from trexprogram.utils.reward_program_helper import calculate_expiry_date
 
 logger = logging.getLogger('reward-program-lib')
 
 class StampSchemeProgram(SchemeRewardProgram):
     
     def __init__(self, program_configuration, currency=None):
         super(StampSchemeProgram, self).__init__(program_configuration, currency=currency)
@@ -56,15 +55,15 @@
                 invoice_id                      = transaction_details.invoice_id
                 
                 transact_by                     = transaction_details.transact_by_user
                 
                 transact_outlet                 = transaction_details.transact_outlet_details
                 
                 effective_date                  = transact_datetime.date()
-                expiry_date                     = self.calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
+                expiry_date                     = calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
                 
                 reward_status = program_conf.REWARD_STATUS_VALID
                 
                 if is_reach_reward_limit and reward_amount==0:
                     reward_status = program_conf.REWARD_STATUS_REACH_LIMIT
                 
                 stamp_reward = CustomerStampReward.create( 
@@ -107,15 +106,15 @@
                 
                 transact_by                     = transaction_details.transact_by_user
                 
                 transact_outlet                 = transaction_details.transact_outlet_details
                 
                 
                 effective_date                  = transact_datetime.date()
-                expiry_date                     = self.calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
+                expiry_date                     = calculate_expiry_date(self.expiration_type, self.expiration_value, start_date=effective_date)
                  
                 
                 logger.debug('-------> Going to create point reward where reward amount=%f',reward_amount)
                 
                 reward_status = program_conf.REWARD_STATUS_VALID
                 
                 stamp_reward = CustomerStampReward.create(
```

### Comparing `trex-program-0.0.1/trex-program/reward_program/tier_reward_program.py` & `trex-program-1.0.0/trexprogram/reward_program/tier_reward_program.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 '''
 Created on 4 Oct 2021
 
 @author: jacklok
 '''
-from trexprogram.reward_program.reward_program_base import RewardProgramBase, DATE_FORMAT, EntitledVoucherSummary
+from trexprogram.reward_program.reward_program_base import RewardProgramBase, EntitledVoucherSummary
 from trexmodel.models.datastore.reward_models import CustomerEntitledVoucher
-from trexmodel import program_conf
+from trexconf import program_conf
 from datetime import datetime
 import logging
 from trexmodel.models.datastore.program_models import MerchantTierRewardProgram
 from trexlib.utils.string_util import is_not_empty
 from trexmodel.models.datastore.voucher_models import MerchantVoucher
 from trexprogram.utils.tier_reward_program_helper import update_and_get_unlock_tier_index_list
-from trexanalytics.bigquery_upstream_data_config import create_merchant_customer_redemption_upstream_for_merchant
-from trexmodel.models.datastore.redeem_models import CustomerRedemption
-from trexlib import conf as lib_conf
+from trexconf import conf as lib_conf 
 from trexlib.utils.google.cloud_tasks_util import create_task
 import json
+from trexprogram.utils.reward_program_helper import calculate_expiry_date,\
+    calculate_effective_date
 
 #logger = logging.getLogger('reward-program-lib')
 logger = logging.getLogger('debug')
 
 class TierRewardProgram(RewardProgramBase):
     
     def __init__(self, program_configuration):
@@ -47,20 +47,20 @@
             effective_date_str      = voucher_details.get('effective_date')
             
              
             if effective_type == program_conf.REWARD_EFFECTIVE_TYPE_SPECIFIC_DATE:
                 if is_not_empty(effective_date_str):
                     effective_date = datetime.strptime(effective_date_str, DATE_FORMAT)
             else:
-                effective_date  = self.calculate_effective_date(effective_type, effective_value, start_date = transaction_details.transact_datetime.date())
+                effective_date  = calculate_effective_date(effective_type, effective_value, start_date = transaction_details.transact_datetime.date())
              
             expiration_type         = voucher_details.get('expiration_type')
             expiration_value        = voucher_details.get('expiration_value')
              
-            expiry_date             = self.calculate_expiry_date(expiration_type, expiration_value, start_date=effective_date)
+            expiry_date             = calculate_expiry_date(expiration_type, expiration_value, start_date=effective_date)
             
             voucher_amount          = voucher_details.get('voucher_amount')
             
             voucher_details         = {
                                         'voucher_key'       : voucher_details.get('voucher_key'),
                                         'use_in_store'      : voucher_details.get('use_in_store'),
                                         'use_online'        : voucher_details.get('use_online'),
```

### Comparing `trex-program-0.0.1/trex-program/reward_program/voucher_reward_program.py` & `trex-program-1.0.0/trexprogram/reward_program/voucher_reward_program.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Created on 21 Apr 2021
 
 @author: jacklok
 '''
 
 from trexprogram.reward_program.reward_program_base import VoucherRewardProgramBase,\
     GiveawayRewardBaseProgram
-from trexmodel import program_conf
+from trexconf import program_conf
 
 class VoucherProgram(VoucherRewardProgramBase):
     
     def __init__(self, program_configuration):
         super(VoucherProgram, self).__init__(program_configuration)
```

### Comparing `trex-program-0.0.1/trex-program/utils/tier_reward_program_helper.py` & `trex-program-1.0.0/trexprogram/utils/tier_reward_program_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 '''
 Created on 5 Oct 2021
 
 @author: jacklok
 '''
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
 from trexmodel.models.datastore.reward_models import CustomerEntitledTierRewardSummary
-from trexmodel import program_conf 
-from datetime import datetime, time
+from trexconf import program_conf 
 import logging
 
 #logger = logging.getLogger('helper')
 logger = logging.getLogger('debug')
 
 def update_and_get_unlock_tier_index_list(customer, tier_reward_program, transaction_details):
     logger.debug('---update_and_get_unlock_tier_index_list---, transaction_id=%s', transaction_details.transaction_id)
```

