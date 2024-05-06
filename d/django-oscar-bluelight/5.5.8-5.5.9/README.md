# Comparing `tmp/django_oscar_bluelight-5.5.8.tar.gz` & `tmp/django_oscar_bluelight-5.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_oscar_bluelight-5.5.8.tar", max compression
+gzip compressed data, was "django_oscar_bluelight-5.5.9.tar", max compression
```

## Comparing `django_oscar_bluelight-5.5.8.tar` & `django_oscar_bluelight-5.5.9.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0      747 2024-04-04 17:47:27.731552 django_oscar_bluelight-5.5.8/LICENSE
--rw-r--r--   0        0        0    16017 2024-04-04 17:47:27.731552 django_oscar_bluelight-5.5.8/README.md
--rw-r--r--   0        0        0     1137 2024-04-04 17:47:27.732552 django_oscar_bluelight-5.5.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 17:47:27.790553 django_oscar_bluelight-5.5.8/src/oscarbluelight/__init__.py
--rw-r--r--   0        0        0     5719 2024-04-04 17:47:27.739552 django_oscar_bluelight-5.5.8/src/oscarbluelight/basket_utils.py
--rw-r--r--   0        0        0     2923 2024-04-04 17:47:27.739552 django_oscar_bluelight-5.5.8/src/oscarbluelight/caching.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:27.790553 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:27.790553 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/offers/__init__.py
--rw-r--r--   0        0        0      390 2024-04-04 17:47:27.739552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/offers/api_views.py
--rw-r--r--   0        0        0     4469 2024-04-04 17:47:27.739552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/offers/apps.py
--rw-r--r--   0        0        0     9523 2024-04-04 17:47:27.739552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/offers/forms.py
--rw-r--r--   0        0        0       57 2024-04-04 17:47:27.739552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/offers/models.py
--rw-r--r--   0        0        0     1734 2024-04-04 17:47:27.739552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/offers/reports.py
--rw-r--r--   0        0        0     2628 2024-04-04 17:47:27.739552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/offers/serializers.py
--rw-r--r--   0        0        0    15456 2024-04-04 17:47:27.739552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/offers/views.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:27.793553 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/ranges/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-04 17:47:27.739552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/ranges/apps.py
--rw-r--r--   0        0        0     6304 2024-04-04 17:47:27.740552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/ranges/forms.py
--rw-r--r--   0        0        0       57 2024-04-04 17:47:27.740552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/ranges/models.py
--rw-r--r--   0        0        0     5910 2024-04-04 17:47:27.740552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/ranges/views.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:27.793553 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/vouchers/__init__.py
--rw-r--r--   0        0        0     2867 2024-04-04 17:47:27.740552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/vouchers/apps.py
--rw-r--r--   0        0        0     4450 2024-04-04 17:47:27.740552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/vouchers/forms.py
--rw-r--r--   0        0        0    15136 2024-04-04 17:47:27.740552 django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/vouchers/views.py
--rw-r--r--   0        0        0     3809 2024-04-04 17:47:27.740552 django_oscar_bluelight-5.5.8/src/oscarbluelight/defaults.py
--rw-r--r--   0        0        0      380 2024-04-04 17:47:27.740552 django_oscar_bluelight-5.5.8/src/oscarbluelight/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    37748 2024-04-04 17:47:27.740552 django_oscar_bluelight-5.5.8/src/oscarbluelight/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2024-04-04 17:47:27.740552 django_oscar_bluelight-5.5.8/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     2145 2024-04-04 17:47:27.740552 django_oscar_bluelight-5.5.8/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    12884 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/mixins.py
--rw-r--r--   0        0        0       47 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/__init__.py
--rw-r--r--   0        0        0     1984 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/admin.py
--rw-r--r--   0        0        0     9720 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/applicator.py
--rw-r--r--   0        0        0      248 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/apps.py
--rw-r--r--   0        0        0    30694 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/benefits.py
--rw-r--r--   0        0        0    15514 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/conditions.py
--rw-r--r--   0        0        0      195 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/constants.py
--rw-r--r--   0        0        0     4735 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/groups.py
--rw-r--r--   0        0        0     3028 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/handlers.py
--rw-r--r--   0        0        0    25222 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0001_initial.py
--rw-r--r--   0        0        0      539 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0002_auto_20151210_1053.py
--rw-r--r--   0        0        0     1537 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0002_compoundcondition.py
--rw-r--r--   0        0        0      326 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0003_merge.py
--rw-r--r--   0        0        0      582 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0004_conditionaloffer_groups.py
--rw-r--r--   0        0        0     3547 2024-04-04 17:47:27.741552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0005_auto_20160719_1238.py
--rw-r--r--   0        0        0     8827 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0006_bluelightabsolutediscountbenefit_bluelightcountcondition_bluelightcoveragecondition_bluelightfixedpr.py
--rw-r--r--   0        0        0     1733 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0007_auto_20170417_1354.py
--rw-r--r--   0        0        0     1707 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0008_auto_20170512_1049.py
--rw-r--r--   0        0        0      814 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0009_auto_20170517_1605.py
--rw-r--r--   0        0        0      459 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0009_auto_20200801_0817.py
--rw-r--r--   0        0        0      988 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0010_auto_20170613_1245.py
--rw-r--r--   0        0        0      696 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0010_conditionaloffer_combinations.py
--rw-r--r--   0        0        0     1990 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0011_auto_20170710_1442.py
--rw-r--r--   0        0        0      702 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0011_conditionaloffer_affects_cosmetic_pricing.py
--rw-r--r--   0        0        0     1311 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0012_auto_20180514_1142.py
--rw-r--r--   0        0        0     1166 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0012_auto_20211020_1037.py
--rw-r--r--   0        0        0      636 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0013_alter_offergroup_slug.py
--rw-r--r--   0        0        0      558 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0013_conditionaloffer_exclusive.py
--rw-r--r--   0        0        0      878 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0014_auto_20181017_1151.py
--rw-r--r--   0        0        0     3442 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0014_drop_triggers.py
--rw-r--r--   0        0        0      902 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0015_auto_20181018_1220.py
--rw-r--r--   0        0        0     1477 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0015_auto_20231012_1143.py
--rw-r--r--   0        0        0      354 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0016_remove_conditionaloffer_apply_to_displayed_prices.py
--rw-r--r--   0        0        0     2920 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0017_auto_20190705_1245.py
--rw-r--r--   0        0        0     1403 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0017_compoundbenefit.py
--rw-r--r--   0        0        0      261 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0018_merge_20190705_1247.py
--rw-r--r--   0        0        0      832 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0019_auto_20190926_1547.py
--rw-r--r--   0        0        0      331 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0020_remove_range_cache_version.py
--rw-r--r--   0        0        0      718 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0021_rangeproductset.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:27.800554 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/__init__.py
--rw-r--r--   0        0        0    15816 2024-04-04 17:47:27.742552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/models.py
--rw-r--r--   0        0        0     2400 2024-04-04 17:47:27.743552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/reports.py
--rw-r--r--   0        0        0     1984 2024-04-04 17:47:27.743552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/results.py
--rw-r--r--   0        0        0      646 2024-04-04 17:47:27.743552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/signals.py
--rw-r--r--   0        0        0     7495 2024-04-04 17:47:27.743552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/sql.py
--rw-r--r--   0        0        0     1817 2024-04-04 17:47:27.743552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/tasks.py
--rw-r--r--   0        0        0     3994 2024-04-04 17:47:27.743552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/upsells.py
--rw-r--r--   0        0        0      432 2024-04-04 17:47:27.743552 django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/utils.py
--rw-r--r--   0        0        0     1388 2024-04-04 17:47:27.743552 django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/offergroups.css
--rw-r--r--   0        0        0     1936 2024-04-04 17:47:27.743552 django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/offergroups.css.map
--rw-r--r--   0        0        0     6571 2024-04-04 17:47:27.743552 django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/offergroups.js
--rw-r--r--   0        0        0    24756 2024-04-04 17:47:27.743552 django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/offergroups.js.map
--rw-r--r--   0        0        0   210646 2024-04-04 17:47:27.745552 django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/vendor.js
--rw-r--r--   0        0        0      852 2024-04-04 17:47:27.745552 django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/vendor.js.LICENSE.txt
--rw-r--r--   0        0        0   778250 2024-04-04 17:47:27.748552 django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/vendor.js.map
--rw-r--r--   0        0        0     1293 2024-04-04 17:47:27.748552 django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/webpack-stats.json
--rw-r--r--   0        0        0     1869 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/catalogue/partials/stock_record.html
--rw-r--r--   0        0        0     1992 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_delete.html
--rw-r--r--   0        0        0     5482 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit.html
--rw-r--r--   0        0        0      410 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit_compound.html
--rw-r--r--   0        0        0     5404 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_list.html
--rw-r--r--   0        0        0      787 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_selection_form.html
--rw-r--r--   0        0        0     1997 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/condition_delete.html
--rw-r--r--   0        0        0     5389 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit.html
--rw-r--r--   0        0        0      563 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit_compound.html
--rw-r--r--   0        0        0     5391 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/condition_list.html
--rw-r--r--   0        0        0      793 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/condition_selection_form.html
--rw-r--r--   0        0        0     1959 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/image_form.html
--rw-r--r--   0        0        0     9218 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/offer_detail.html
--rw-r--r--   0        0        0     5691 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/offer_list.html
--rw-r--r--   0        0        0     1924 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_delete.html
--rw-r--r--   0        0        0     3944 2024-04-04 17:47:27.749553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_edit.html
--rw-r--r--   0        0        0     1547 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_list.html
--rw-r--r--   0        0        0      317 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/partials/offer_thumbnail.html
--rw-r--r--   0        0        0      494 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/restrictions_form.html
--rw-r--r--   0        0        0     1793 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/ranges/range_excluded_products.html
--rw-r--r--   0        0        0     5266 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/ranges/range_list.html
--rw-r--r--   0        0        0     8583 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/ranges/range_price_list.html
--rw-r--r--   0        0        0     4162 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html
--rw-r--r--   0        0        0     2792 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_add_children.html
--rw-r--r--   0        0        0     7389 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_detail.html
--rw-r--r--   0        0        0     2773 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_export_children.html
--rw-r--r--   0        0        0     2257 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_form.html
--rw-r--r--   0        0        0     3599 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list.html
--rw-r--r--   0        0        0     6453 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list_children.html
--rw-r--r--   0        0        0        0 2024-04-04 17:47:27.800554 django_oscar_bluelight-5.5.8/src/oscarbluelight/templatetags/__init__.py
--rw-r--r--   0        0        0      214 2024-04-04 17:47:27.750553 django_oscar_bluelight-5.5.8/src/oscarbluelight/templatetags/oscarbluelight_tags.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:27.800554 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:27.800554 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/__init__.py
--rw-r--r--   0        0        0     1422 2024-04-04 17:47:27.751553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/base.py
--rw-r--r--   0        0        0    19887 2024-04-04 17:47:27.751553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_benefit_absolute.py
--rw-r--r--   0        0        0    14181 2024-04-04 17:47:27.751553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_benefit_compound.py
--rw-r--r--   0        0        0     8276 2024-04-04 17:47:27.751553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_benefit_fixed_price.py
--rw-r--r--   0        0        0     8240 2024-04-04 17:47:27.751553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_benefit_fixed_price_per_item.py
--rw-r--r--   0        0        0     6558 2024-04-04 17:47:27.751553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_benefit_multibuy.py
--rw-r--r--   0        0        0    15250 2024-04-04 17:47:27.751553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_benefit_percentage.py
--rw-r--r--   0        0        0    37853 2024-04-04 17:47:27.751553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_conditions.py
--rw-r--r--   0        0        0     2862 2024-04-04 17:47:27.751553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_cosmetic_prices.py
--rw-r--r--   0        0        0    54287 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_offer_groups.py
--rw-r--r--   0        0        0    10397 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_range.py
--rw-r--r--   0        0        0    16269 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_recalculate_offer_application_totals.py
--rw-r--r--   0        0        0     6926 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_system_groups.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:27.800554 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/voucher/__init__.py
--rw-r--r--   0        0        0     7817 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/voucher/test_rules.py
--rw-r--r--   0        0        0    17766 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/voucher/test_vouchers.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:27.800554 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/__init__.py
--rw-r--r--   0        0        0     1045 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/admin.py
--rw-r--r--   0        0        0      115 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/apps.py
--rw-r--r--   0        0        0     5396 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0001_initial.py
--rw-r--r--   0        0        0      728 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0002_auto_20160503_1138.py
--rw-r--r--   0        0        0      624 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0003_voucher_parent.py
--rw-r--r--   0        0        0      524 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0004_auto_20161115_1115.py
--rw-r--r--   0        0        0      572 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0005_auto_20170613_1245.py
--rw-r--r--   0        0        0      976 2024-04-04 17:47:27.752553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0006_auto_20170710_1442.py
--rw-r--r--   0        0        0     2849 2024-04-04 17:47:27.753553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0007_auto_20180601_1348.py
--rw-r--r--   0        0        0      622 2024-04-04 17:47:27.753553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0008_auto_20190926_1547.py
--rw-r--r--   0        0        0     1702 2024-04-04 17:47:27.753553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0008_auto_20200801_0817.py
--rw-r--r--   0        0        0      556 2024-04-04 17:47:27.753553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0009_auto_20210216_1327.py
--rw-r--r--   0        0        0     2619 2024-04-04 17:47:27.753553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0010_auto_20210526_1410.py
--rw-r--r--   0        0        0      651 2024-04-04 17:47:27.753553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0011_auto_20220615_1024.py
--rw-r--r--   0        0        0      454 2024-04-04 17:47:27.753553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0012_voucher_status.py
--rw-r--r--   0        0        0      966 2024-04-04 17:47:27.753553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0013_auto_20231012_1143.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:27.805554 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/__init__.py
--rw-r--r--   0        0        0    11974 2024-04-04 17:47:27.753553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/models.py
--rw-r--r--   0        0        0     3017 2024-04-04 17:47:27.753553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/reports.py
--rw-r--r--   0        0        0     4415 2024-04-04 17:47:27.753553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/rules.py
--rw-r--r--   0        0        0     3657 2024-04-04 17:47:27.753553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/sql.py
--rw-r--r--   0        0        0      772 2024-04-04 17:47:27.753553 django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/tasks.py
--rw-r--r--   0        0        0    16872 1970-01-01 00:00:00.000000 django_oscar_bluelight-5.5.8/PKG-INFO
+-rw-r--r--   0        0        0      747 2024-04-17 16:47:59.092081 django_oscar_bluelight-5.5.9/LICENSE
+-rw-r--r--   0        0        0    16095 2024-04-17 16:47:59.092081 django_oscar_bluelight-5.5.9/README.md
+-rw-r--r--   0        0        0     1137 2024-04-17 16:47:59.093082 django_oscar_bluelight-5.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 16:47:59.150081 django_oscar_bluelight-5.5.9/src/oscarbluelight/__init__.py
+-rw-r--r--   0        0        0     5719 2024-04-17 16:47:59.100082 django_oscar_bluelight-5.5.9/src/oscarbluelight/basket_utils.py
+-rw-r--r--   0        0        0     2923 2024-04-17 16:47:59.100082 django_oscar_bluelight-5.5.9/src/oscarbluelight/caching.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:47:59.150081 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:47:59.150081 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/offers/__init__.py
+-rw-r--r--   0        0        0      390 2024-04-17 16:47:59.100082 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/offers/api_views.py
+-rw-r--r--   0        0        0     4469 2024-04-17 16:47:59.100082 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/offers/apps.py
+-rw-r--r--   0        0        0     9523 2024-04-17 16:47:59.100082 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/offers/forms.py
+-rw-r--r--   0        0        0       57 2024-04-17 16:47:59.100082 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/offers/models.py
+-rw-r--r--   0        0        0     1734 2024-04-17 16:47:59.100082 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/offers/reports.py
+-rw-r--r--   0        0        0     2628 2024-04-17 16:47:59.100082 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/offers/serializers.py
+-rw-r--r--   0        0        0    15456 2024-04-17 16:47:59.100082 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/offers/views.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:47:59.150081 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/ranges/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-17 16:47:59.100082 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/ranges/apps.py
+-rw-r--r--   0        0        0     6304 2024-04-17 16:47:59.101081 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/ranges/forms.py
+-rw-r--r--   0        0        0       57 2024-04-17 16:47:59.101081 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/ranges/models.py
+-rw-r--r--   0        0        0     5910 2024-04-17 16:47:59.101081 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/ranges/views.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:47:59.150081 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/vouchers/__init__.py
+-rw-r--r--   0        0        0     2867 2024-04-17 16:47:59.101081 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/vouchers/apps.py
+-rw-r--r--   0        0        0     4450 2024-04-17 16:47:59.101081 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/vouchers/forms.py
+-rw-r--r--   0        0        0    15164 2024-04-17 16:47:59.101081 django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/vouchers/views.py
+-rw-r--r--   0        0        0     3809 2024-04-17 16:47:59.101081 django_oscar_bluelight-5.5.9/src/oscarbluelight/defaults.py
+-rw-r--r--   0        0        0      380 2024-04-17 16:47:59.101081 django_oscar_bluelight-5.5.9/src/oscarbluelight/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    37748 2024-04-17 16:47:59.101081 django_oscar_bluelight-5.5.9/src/oscarbluelight/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2024-04-17 16:47:59.101081 django_oscar_bluelight-5.5.9/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     2145 2024-04-17 16:47:59.101081 django_oscar_bluelight-5.5.9/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    12884 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/mixins.py
+-rw-r--r--   0        0        0       47 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/__init__.py
+-rw-r--r--   0        0        0     1984 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/admin.py
+-rw-r--r--   0        0        0     9720 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/applicator.py
+-rw-r--r--   0        0        0      248 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/apps.py
+-rw-r--r--   0        0        0    30694 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/benefits.py
+-rw-r--r--   0        0        0    15514 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/conditions.py
+-rw-r--r--   0        0        0      195 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/constants.py
+-rw-r--r--   0        0        0     4735 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/groups.py
+-rw-r--r--   0        0        0     3028 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/handlers.py
+-rw-r--r--   0        0        0    25222 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0001_initial.py
+-rw-r--r--   0        0        0      539 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0002_auto_20151210_1053.py
+-rw-r--r--   0        0        0     1537 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0002_compoundcondition.py
+-rw-r--r--   0        0        0      326 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0003_merge.py
+-rw-r--r--   0        0        0      582 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0004_conditionaloffer_groups.py
+-rw-r--r--   0        0        0     3547 2024-04-17 16:47:59.102081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0005_auto_20160719_1238.py
+-rw-r--r--   0        0        0     8827 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0006_bluelightabsolutediscountbenefit_bluelightcountcondition_bluelightcoveragecondition_bluelightfixedpr.py
+-rw-r--r--   0        0        0     1733 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0007_auto_20170417_1354.py
+-rw-r--r--   0        0        0     1707 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0008_auto_20170512_1049.py
+-rw-r--r--   0        0        0      814 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0009_auto_20170517_1605.py
+-rw-r--r--   0        0        0      459 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0009_auto_20200801_0817.py
+-rw-r--r--   0        0        0      988 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0010_auto_20170613_1245.py
+-rw-r--r--   0        0        0      696 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0010_conditionaloffer_combinations.py
+-rw-r--r--   0        0        0     1990 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0011_auto_20170710_1442.py
+-rw-r--r--   0        0        0      702 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0011_conditionaloffer_affects_cosmetic_pricing.py
+-rw-r--r--   0        0        0     1311 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0012_auto_20180514_1142.py
+-rw-r--r--   0        0        0     1166 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0012_auto_20211020_1037.py
+-rw-r--r--   0        0        0      636 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0013_alter_offergroup_slug.py
+-rw-r--r--   0        0        0      558 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0013_conditionaloffer_exclusive.py
+-rw-r--r--   0        0        0      878 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0014_auto_20181017_1151.py
+-rw-r--r--   0        0        0     3442 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0014_drop_triggers.py
+-rw-r--r--   0        0        0      902 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0015_auto_20181018_1220.py
+-rw-r--r--   0        0        0     1477 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0015_auto_20231012_1143.py
+-rw-r--r--   0        0        0      354 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0016_remove_conditionaloffer_apply_to_displayed_prices.py
+-rw-r--r--   0        0        0     2920 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0017_auto_20190705_1245.py
+-rw-r--r--   0        0        0     1403 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0017_compoundbenefit.py
+-rw-r--r--   0        0        0      261 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0018_merge_20190705_1247.py
+-rw-r--r--   0        0        0      832 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0019_auto_20190926_1547.py
+-rw-r--r--   0        0        0      331 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0020_remove_range_cache_version.py
+-rw-r--r--   0        0        0      718 2024-04-17 16:47:59.103082 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0021_rangeproductset.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:47:59.157081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/__init__.py
+-rw-r--r--   0        0        0    15816 2024-04-17 16:47:59.104081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/models.py
+-rw-r--r--   0        0        0     2400 2024-04-17 16:47:59.104081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/reports.py
+-rw-r--r--   0        0        0     1984 2024-04-17 16:47:59.104081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/results.py
+-rw-r--r--   0        0        0      646 2024-04-17 16:47:59.104081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/signals.py
+-rw-r--r--   0        0        0     7495 2024-04-17 16:47:59.104081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/sql.py
+-rw-r--r--   0        0        0     1817 2024-04-17 16:47:59.104081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/tasks.py
+-rw-r--r--   0        0        0     3994 2024-04-17 16:47:59.104081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/upsells.py
+-rw-r--r--   0        0        0      432 2024-04-17 16:47:59.104081 django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/utils.py
+-rw-r--r--   0        0        0     1388 2024-04-17 16:47:59.104081 django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/offergroups.css
+-rw-r--r--   0        0        0     1936 2024-04-17 16:47:59.104081 django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/offergroups.css.map
+-rw-r--r--   0        0        0     6571 2024-04-17 16:47:59.104081 django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/offergroups.js
+-rw-r--r--   0        0        0    24756 2024-04-17 16:47:59.104081 django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/offergroups.js.map
+-rw-r--r--   0        0        0   210646 2024-04-17 16:47:59.106082 django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/vendor.js
+-rw-r--r--   0        0        0      852 2024-04-17 16:47:59.106082 django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/vendor.js.LICENSE.txt
+-rw-r--r--   0        0        0   778250 2024-04-17 16:47:59.109081 django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/vendor.js.map
+-rw-r--r--   0        0        0     1293 2024-04-17 16:47:59.109081 django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/webpack-stats.json
+-rw-r--r--   0        0        0     1869 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/catalogue/partials/stock_record.html
+-rw-r--r--   0        0        0     1992 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_delete.html
+-rw-r--r--   0        0        0     5482 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit.html
+-rw-r--r--   0        0        0      410 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit_compound.html
+-rw-r--r--   0        0        0     5404 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_list.html
+-rw-r--r--   0        0        0      787 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_selection_form.html
+-rw-r--r--   0        0        0     1997 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/condition_delete.html
+-rw-r--r--   0        0        0     5389 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit.html
+-rw-r--r--   0        0        0      563 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit_compound.html
+-rw-r--r--   0        0        0     5391 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/condition_list.html
+-rw-r--r--   0        0        0      793 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/condition_selection_form.html
+-rw-r--r--   0        0        0     1959 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/image_form.html
+-rw-r--r--   0        0        0     9218 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/offer_detail.html
+-rw-r--r--   0        0        0     5691 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/offer_list.html
+-rw-r--r--   0        0        0     1924 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_delete.html
+-rw-r--r--   0        0        0     3944 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_edit.html
+-rw-r--r--   0        0        0     1547 2024-04-17 16:47:59.110082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_list.html
+-rw-r--r--   0        0        0      317 2024-04-17 16:47:59.111081 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/partials/offer_thumbnail.html
+-rw-r--r--   0        0        0      494 2024-04-17 16:47:59.111081 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/restrictions_form.html
+-rw-r--r--   0        0        0     1793 2024-04-17 16:47:59.111081 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/ranges/range_excluded_products.html
+-rw-r--r--   0        0        0     5266 2024-04-17 16:47:59.111081 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/ranges/range_list.html
+-rw-r--r--   0        0        0     8583 2024-04-17 16:47:59.111081 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/ranges/range_price_list.html
+-rw-r--r--   0        0        0     4162 2024-04-17 16:47:59.111081 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html
+-rw-r--r--   0        0        0     2792 2024-04-17 16:47:59.111081 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_add_children.html
+-rw-r--r--   0        0        0     7389 2024-04-17 16:47:59.111081 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_detail.html
+-rw-r--r--   0        0        0     2773 2024-04-17 16:47:59.111081 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_export_children.html
+-rw-r--r--   0        0        0     2257 2024-04-17 16:47:59.111081 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_form.html
+-rw-r--r--   0        0        0     3599 2024-04-17 16:47:59.111081 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list.html
+-rw-r--r--   0        0        0     6453 2024-04-17 16:47:59.111081 django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list_children.html
+-rw-r--r--   0        0        0        0 2024-04-17 16:47:59.159082 django_oscar_bluelight-5.5.9/src/oscarbluelight/templatetags/__init__.py
+-rw-r--r--   0        0        0      214 2024-04-17 16:47:59.111081 django_oscar_bluelight-5.5.9/src/oscarbluelight/templatetags/oscarbluelight_tags.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:47:59.159082 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:47:59.159082 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/__init__.py
+-rw-r--r--   0        0        0     1422 2024-04-17 16:47:59.112081 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/base.py
+-rw-r--r--   0        0        0    19887 2024-04-17 16:47:59.112081 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_benefit_absolute.py
+-rw-r--r--   0        0        0    14181 2024-04-17 16:47:59.112081 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_benefit_compound.py
+-rw-r--r--   0        0        0     8276 2024-04-17 16:47:59.112081 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_benefit_fixed_price.py
+-rw-r--r--   0        0        0     8240 2024-04-17 16:47:59.112081 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_benefit_fixed_price_per_item.py
+-rw-r--r--   0        0        0     6558 2024-04-17 16:47:59.112081 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_benefit_multibuy.py
+-rw-r--r--   0        0        0    15250 2024-04-17 16:47:59.112081 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_benefit_percentage.py
+-rw-r--r--   0        0        0    37853 2024-04-17 16:47:59.112081 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_conditions.py
+-rw-r--r--   0        0        0     2862 2024-04-17 16:47:59.112081 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_cosmetic_prices.py
+-rw-r--r--   0        0        0    54287 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_offer_groups.py
+-rw-r--r--   0        0        0    10397 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_range.py
+-rw-r--r--   0        0        0    16269 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_recalculate_offer_application_totals.py
+-rw-r--r--   0        0        0     6926 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_system_groups.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:47:59.159082 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/voucher/__init__.py
+-rw-r--r--   0        0        0     7817 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/voucher/test_rules.py
+-rw-r--r--   0        0        0    17782 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/voucher/test_vouchers.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:47:59.159082 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/__init__.py
+-rw-r--r--   0        0        0     1045 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/admin.py
+-rw-r--r--   0        0        0      115 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/apps.py
+-rw-r--r--   0        0        0     5396 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0001_initial.py
+-rw-r--r--   0        0        0      728 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0002_auto_20160503_1138.py
+-rw-r--r--   0        0        0      624 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0003_voucher_parent.py
+-rw-r--r--   0        0        0      524 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0004_auto_20161115_1115.py
+-rw-r--r--   0        0        0      572 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0005_auto_20170613_1245.py
+-rw-r--r--   0        0        0      976 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0006_auto_20170710_1442.py
+-rw-r--r--   0        0        0     2849 2024-04-17 16:47:59.113082 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0007_auto_20180601_1348.py
+-rw-r--r--   0        0        0      622 2024-04-17 16:47:59.114081 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0008_auto_20190926_1547.py
+-rw-r--r--   0        0        0     1702 2024-04-17 16:47:59.114081 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0008_auto_20200801_0817.py
+-rw-r--r--   0        0        0      556 2024-04-17 16:47:59.114081 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0009_auto_20210216_1327.py
+-rw-r--r--   0        0        0     2619 2024-04-17 16:47:59.114081 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0010_auto_20210526_1410.py
+-rw-r--r--   0        0        0      651 2024-04-17 16:47:59.114081 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0011_auto_20220615_1024.py
+-rw-r--r--   0        0        0      454 2024-04-17 16:47:59.114081 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0012_voucher_status.py
+-rw-r--r--   0        0        0      966 2024-04-17 16:47:59.114081 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0013_auto_20231012_1143.py
+-rw-r--r--   0        0        0        0 2024-04-17 16:47:59.160081 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/__init__.py
+-rw-r--r--   0        0        0    12019 2024-04-17 16:47:59.114081 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/models.py
+-rw-r--r--   0        0        0     3017 2024-04-17 16:47:59.114081 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/reports.py
+-rw-r--r--   0        0        0     4415 2024-04-17 16:47:59.114081 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/rules.py
+-rw-r--r--   0        0        0     3657 2024-04-17 16:47:59.114081 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/sql.py
+-rw-r--r--   0        0        0      772 2024-04-17 16:47:59.114081 django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/tasks.py
+-rw-r--r--   0        0        0    16950 1970-01-01 00:00:00.000000 django_oscar_bluelight-5.5.9/PKG-INFO
```

### Comparing `django_oscar_bluelight-5.5.8/LICENSE` & `django_oscar_bluelight-5.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/README.md` & `django_oscar_bluelight-5.5.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,18 @@
 ## Usage
 
 After installation, the new functionality will show up in the Oscar
 dashboard under the Offers menu.
 
 ## Changelog
 
+### 5.5.9
+
+- Improve query performance of child-voucher creation-date table.
+
 ### 5.5.8
 
 - Improve query performance for copying parent-to-child offers relationship
 - Fix order status bug in get_recalculate_offer_application_totals_sql
 
 ### 5.5.7
```

### Comparing `django_oscar_bluelight-5.5.8/pyproject.toml` & `django_oscar_bluelight-5.5.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-oscar-bluelight"
-version = "5.5.8"
+version = "5.5.9"
 description = "Bluelight Specials - Enhancements to the offer and vouchers features for Django Oscar."
 authors = [ "thelabnyc <thelabdev@thelabnyc.com>",]
 readme = "README.md"
 homepage = "https://gitlab.com/thelabnyc/django-oscar-bluelight"
 repository = "https://gitlab.com/thelabnyc/django-oscar-bluelight"
 license = "ISC"
```

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/basket_utils.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/basket_utils.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/caching.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/caching.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/offers/apps.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/offers/apps.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/offers/forms.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/offers/forms.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/offers/reports.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/offers/reports.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/offers/serializers.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/offers/serializers.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/offers/views.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/offers/views.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/ranges/apps.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/ranges/apps.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/ranges/forms.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/ranges/forms.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/ranges/views.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/ranges/views.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/vouchers/apps.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/vouchers/apps.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/vouchers/forms.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/vouchers/forms.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/dashboard/vouchers/views.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/dashboard/vouchers/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,18 +312,18 @@
         )
         if query_kwargs:
             return f"{url}?{urlencode(query_kwargs)}"
         return url
 
     def get_created_on_counts(self):
         created_on_counts = (
-            self.parent.children.values(
-                "date_created__date",
-            )
-            .annotate(num_codes=Count("code", distinct=True))
+            self.parent.children.values("date_created__date", "code")
+            .distinct()
+            .values("date_created__date")
+            .annotate(num_codes=Count("code"))
             .order_by("-date_created__date")
         )
         return created_on_counts
 
 
 class ChildCodesListView(BulkEditMixin, generic.ListView):
     model = Voucher
```

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/defaults.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/defaults.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/locale/es/LC_MESSAGES/django.po` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.po` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/mixins.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/mixins.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/admin.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/admin.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/applicator.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/applicator.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/benefits.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/benefits.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/conditions.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/conditions.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/groups.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/groups.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/handlers.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/handlers.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0001_initial.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0002_auto_20151210_1053.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0002_auto_20151210_1053.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0002_compoundcondition.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0002_compoundcondition.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0004_conditionaloffer_groups.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0004_conditionaloffer_groups.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0005_auto_20160719_1238.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0005_auto_20160719_1238.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0006_bluelightabsolutediscountbenefit_bluelightcountcondition_bluelightcoveragecondition_bluelightfixedpr.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0006_bluelightabsolutediscountbenefit_bluelightcountcondition_bluelightcoveragecondition_bluelightfixedpr.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0007_auto_20170417_1354.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0007_auto_20170417_1354.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0008_auto_20170512_1049.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0008_auto_20170512_1049.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0009_auto_20170517_1605.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0009_auto_20170517_1605.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0010_auto_20170613_1245.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0010_auto_20170613_1245.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0010_conditionaloffer_combinations.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0010_conditionaloffer_combinations.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0011_auto_20170710_1442.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0011_auto_20170710_1442.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0011_conditionaloffer_affects_cosmetic_pricing.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0011_conditionaloffer_affects_cosmetic_pricing.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0012_auto_20180514_1142.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0012_auto_20180514_1142.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0012_auto_20211020_1037.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0012_auto_20211020_1037.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0013_alter_offergroup_slug.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0013_alter_offergroup_slug.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0013_conditionaloffer_exclusive.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0013_conditionaloffer_exclusive.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0014_auto_20181017_1151.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0014_auto_20181017_1151.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0014_drop_triggers.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0014_drop_triggers.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0015_auto_20181018_1220.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0015_auto_20181018_1220.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0015_auto_20231012_1143.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0015_auto_20231012_1143.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0017_auto_20190705_1245.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0017_auto_20190705_1245.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0017_compoundbenefit.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0017_compoundbenefit.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0019_auto_20190926_1547.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0019_auto_20190926_1547.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/migrations/0021_rangeproductset.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/migrations/0021_rangeproductset.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/models.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/models.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/reports.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/reports.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/results.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/results.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/signals.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/signals.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/sql.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/sql.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/tasks.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/tasks.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/offer/upsells.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/offer/upsells.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/offergroups.css` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/offergroups.css`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/offergroups.css.map` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/offergroups.css.map`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/offergroups.js` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/offergroups.js`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/offergroups.js.map` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/offergroups.js.map`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/vendor.js` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/vendor.js`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/vendor.js.LICENSE.txt` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/vendor.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/vendor.js.map` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/vendor.js.map`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/static/oscarbluelight/webpack-stats.json` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/static/oscarbluelight/webpack-stats.json`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/catalogue/partials/stock_record.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/catalogue/partials/stock_record.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_delete.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_delete.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_edit.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_list.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_list.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_selection_form.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/benefit_selection_form.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/condition_delete.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/condition_delete.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit_compound.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/condition_edit_compound.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/condition_list.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/condition_list.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/condition_selection_form.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/condition_selection_form.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/image_form.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/image_form.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/offer_detail.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/offer_detail.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/offer_list.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/offer_list.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_delete.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_delete.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_edit.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_edit.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_list.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/offers/offergroup_list.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/ranges/range_excluded_products.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/ranges/range_excluded_products.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/ranges/range_list.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/ranges/range_list.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/ranges/range_price_list.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/ranges/range_price_list.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/partials/voucher_details_table.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_add_children.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_add_children.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_detail.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_detail.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_export_children.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_export_children.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_form.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_form.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list_children.html` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/templates/oscar/dashboard/vouchers/voucher_list_children.html`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/base.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/base.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_benefit_absolute.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_benefit_absolute.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_benefit_compound.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_benefit_compound.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_benefit_fixed_price.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_benefit_fixed_price.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_benefit_fixed_price_per_item.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_benefit_fixed_price_per_item.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_benefit_multibuy.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_benefit_multibuy.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_benefit_percentage.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_benefit_percentage.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_conditions.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_conditions.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_cosmetic_prices.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_cosmetic_prices.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_offer_groups.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_offer_groups.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_range.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_range.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_recalculate_offer_application_totals.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_recalculate_offer_application_totals.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/offer/test_system_groups.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/offer/test_system_groups.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/voucher/test_rules.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/voucher/test_rules.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/tests/voucher/test_vouchers.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/tests/voucher/test_vouchers.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,17 +170,17 @@
             usage=Voucher.SINGLE_USE,
             start_datetime=datetime.now(),
             end_datetime=datetime.now(),
             limit_usage_by_group=False,
         )
         self.assertEqual(p.children.all().count(), 0)
 
-        # First batch. Query count should be (10 + (auto_generate_count / 1_000)), since
+        # First batch. Query count should be (3 + (auto_generate_count / 1_000)), since
         # the `bulk_create` batch size is 1_000
-        baseline_num_queries = 10
+        baseline_num_queries = 3
         insert_batch_size = 1_000
         auto_generate_count = 100_000
         with self.assertNumQueries(
             baseline_num_queries + (auto_generate_count / insert_batch_size)
         ):
             p.create_children(auto_generate_count=auto_generate_count)
 
@@ -217,14 +217,16 @@
         c1 = p.children.order_by("code").first()
         self.assertEqual(c1.name, "Test Voucher")
         self.assertTrue(c1.code.startswith("TEST-VOUCHER-0"))
         self.assertEqual(c1.usage, Voucher.SINGLE_USE)
         self.assertEqual(c1.start_datetime, p.start_datetime)
         self.assertEqual(c1.end_datetime, p.end_datetime)
         self.assertFalse(c1.limit_usage_by_group)
+
+        p.save()
         self.assertEqual(c1.groups.count(), 1)
         self.assertEqual(c1.groups.get(), customer)
 
         p.name = "Some Other Name"
         p.groups.set([csrs])
         p.save()
```

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/admin.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/admin.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0001_initial.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0002_auto_20160503_1138.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0002_auto_20160503_1138.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0003_voucher_parent.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0003_voucher_parent.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0004_auto_20161115_1115.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0004_auto_20161115_1115.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0005_auto_20170613_1245.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0005_auto_20170613_1245.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0006_auto_20170710_1442.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0006_auto_20170710_1442.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0007_auto_20180601_1348.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0007_auto_20180601_1348.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0008_auto_20190926_1547.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0008_auto_20190926_1547.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0008_auto_20200801_0817.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0008_auto_20200801_0817.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0009_auto_20210216_1327.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0009_auto_20210216_1327.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0010_auto_20210526_1410.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0010_auto_20210526_1410.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0011_auto_20220615_1024.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0011_auto_20220615_1024.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/migrations/0013_auto_20231012_1143.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/migrations/0013_auto_20231012_1143.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/models.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,17 @@
         # Generate auto codes
         auto_gen_codes = self._get_child_code_batch(auto_generate_count)
         # Update newly created child vouchers only when calling `_create_child_batch` for the last time.
         success_count += len(
             self._create_child_batch(auto_gen_codes, update_children=False)
         )
         # Save manual/custom codes
-        custom_code_successes = self._create_child_batch(custom_codes)
+        custom_code_successes = self._create_child_batch(
+            custom_codes, update_children=False
+        )
         success_count += len(custom_code_successes)
         custom_code_failures = set(custom_codes) - custom_code_successes
         for code in sorted(list(custom_code_failures)):
             errors.append(
                 _("Could not create code “%s” because it already exists.") % code
             )
         return errors, success_count
```

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/reports.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/reports.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/rules.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/rules.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/sql.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/sql.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/src/oscarbluelight/voucher/tasks.py` & `django_oscar_bluelight-5.5.9/src/oscarbluelight/voucher/tasks.py`

 * *Files identical despite different names*

### Comparing `django_oscar_bluelight-5.5.8/PKG-INFO` & `django_oscar_bluelight-5.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-bluelight
-Version: 5.5.8
+Version: 5.5.9
 Summary: Bluelight Specials - Enhancements to the offer and vouchers features for Django Oscar.
 Home-page: https://gitlab.com/thelabnyc/django-oscar-bluelight
 License: ISC
 Author: thelabnyc
 Author-email: thelabdev@thelabnyc.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
@@ -134,14 +134,18 @@
 ## Usage
 
 After installation, the new functionality will show up in the Oscar
 dashboard under the Offers menu.
 
 ## Changelog
 
+### 5.5.9
+
+- Improve query performance of child-voucher creation-date table.
+
 ### 5.5.8
 
 - Improve query performance for copying parent-to-child offers relationship
 - Fix order status bug in get_recalculate_offer_application_totals_sql
 
 ### 5.5.7
```

