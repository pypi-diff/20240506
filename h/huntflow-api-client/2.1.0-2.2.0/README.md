# Comparing `tmp/huntflow_api_client-2.1.0.tar.gz` & `tmp/huntflow_api_client-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huntflow_api_client-2.1.0.tar", last modified: Fri May  3 07:48:37 2024, max compression
+gzip compressed data, was "huntflow_api_client-2.2.0.tar", last modified: Mon May  6 08:56:12 2024, max compression
```

## Comparing `huntflow_api_client-2.1.0.tar` & `huntflow_api_client-2.2.0.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0     1065 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/LICENSE
--rw-r--r--   0        0        0      488 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/README.md
--rw-r--r--   0        0        0       76 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/__init__.py
--rw-r--r--   0        0        0     5735 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/api.py
--rw-r--r--   0        0        0     2880 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/__init__.py
--rw-r--r--   0        0        0     1251 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/account_offers.py
--rw-r--r--   0        0        0     1770 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/account_vacancy_request.py
--rw-r--r--   0        0        0     1449 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/accounts.py
--rw-r--r--   0        0        0     1631 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/action_logs.py
--rw-r--r--   0        0        0     2595 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_logs.py
--rw-r--r--   0        0        0     2859 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_offers.py
--rw-r--r--   0        0        0     2958 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_on_vacancy.py
--rw-r--r--   0        0        0      735 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_on_vacancy_status.py
--rw-r--r--   0        0        0     1238 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_reponse.py
--rw-r--r--   0        0        0     6966 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/applicants.py
--rw-r--r--   0        0        0      941 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/base.py
--rw-r--r--   0        0        0     2733 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/coworkers.py
--rw-r--r--   0        0        0      748 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/delayed_tasks.py
--rw-r--r--   0        0        0     3022 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/dictionaries.py
--rw-r--r--   0        0        0     2564 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/divisions.py
--rw-r--r--   0        0        0      888 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/email_templates.py
--rw-r--r--   0        0        0     1140 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/file.py
--rw-r--r--   0        0        0     2145 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/multi_vacancies.py
--rw-r--r--   0        0        0     1955 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/organization_settings.py
--rw-r--r--   0        0        0     6797 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/production_calendars.py
--rw-r--r--   0        0        0     2995 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/questionary.py
--rw-r--r--   0        0        0      623 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/regions.py
--rw-r--r--   0        0        0      718 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/rejection_reason.py
--rw-r--r--   0        0        0     3772 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/resume.py
--rw-r--r--   0        0        0     1575 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/survey_type_a.py
--rw-r--r--   0        0        0     4331 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/survey_type_q.py
--rw-r--r--   0        0        0     4558 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/tags.py
--rw-r--r--   0        0        0      993 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/user_settings.py
--rw-r--r--   0        0        0      690 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/users.py
--rw-r--r--   0        0        0     5763 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/users_management.py
--rw-r--r--   0        0        0    11740 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/vacancies.py
--rw-r--r--   0        0        0     2933 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/vacancy_requests.py
--rw-r--r--   0        0        0     1815 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/entities/webhooks.py
--rw-r--r--   0        0        0      553 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/errors/__init__.py
--rw-r--r--   0        0        0     1128 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/errors/errors.py
--rw-r--r--   0        0        0     3732 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/errors/handlers.py
--rw-r--r--   0        0        0      361 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/errors/response_hooks.py
--rw-r--r--   0        0        0        0 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/models/__init__.py
--rw-r--r--   0        0        0     9669 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/models/common.py
--rw-r--r--   0        0        0     3435 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/models/consts.py
--rw-r--r--   0        0        0        0 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/__init__.py
--rw-r--r--   0        0        0     2640 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicant_logs.py
--rw-r--r--   0        0        0      326 2024-05-03 07:48:23.798954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicant_offers.py
--rw-r--r--   0        0        0     3618 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicant_on_vacancy.py
--rw-r--r--   0        0        0     2980 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicants.py
--rw-r--r--   0        0        0     1492 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/dictionaries.py
--rw-r--r--   0        0        0      691 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/divisions.py
--rw-r--r--   0        0        0      957 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/file.py
--rw-r--r--   0        0        0     4553 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/multi_vacancies.py
--rw-r--r--   0        0        0      920 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/production_calendars.py
--rw-r--r--   0        0        0      670 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/resume.py
--rw-r--r--   0        0        0      279 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/survey.py
--rw-r--r--   0        0        0      436 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/tags.py
--rw-r--r--   0        0        0      108 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/users_management.py
--rw-r--r--   0        0        0     3711 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/vacancies.py
--rw-r--r--   0        0        0     1393 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/vacancy_requests.py
--rw-r--r--   0        0        0      482 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/request/webhooks.py
--rw-r--r--   0        0        0        0 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/__init__.py
--rw-r--r--   0        0        0      602 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/account_offers.py
--rw-r--r--   0        0        0     1909 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/account_vacancy_request.py
--rw-r--r--   0        0        0     1595 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/accounts.py
--rw-r--r--   0        0        0     1187 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/action_logs.py
--rw-r--r--   0        0        0     8554 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_logs.py
--rw-r--r--   0        0        0      622 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_offers.py
--rw-r--r--   0        0        0     1044 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_on_vacancy.py
--rw-r--r--   0        0        0      773 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_on_vacancy_status.py
--rw-r--r--   0        0        0     1197 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_response.py
--rw-r--r--   0        0        0     5657 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicants.py
--rw-r--r--   0        0        0     1306 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/coworkers.py
--rw-r--r--   0        0        0     1381 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/delayed_tasks.py
--rw-r--r--   0        0        0     2261 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/dictionaries.py
--rw-r--r--   0        0        0     1507 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/divisions.py
--rw-r--r--   0        0        0     1262 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/email_templates.py
--rw-r--r--   0        0        0     2022 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/file.py
--rw-r--r--   0        0        0      156 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/muilti_vacancies.py
--rw-r--r--   0        0        0     1297 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/organization_settings.py
--rw-r--r--   0        0        0     1525 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/production_calendars.py
--rw-r--r--   0        0        0     1365 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/questionary.py
--rw-r--r--   0        0        0      718 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/regions.py
--rw-r--r--   0        0        0      476 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/rejection_reason.py
--rw-r--r--   0        0        0    13292 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/resume.py
--rw-r--r--   0        0        0     2953 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/survey.py
--rw-r--r--   0        0        0      490 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/tags.py
--rw-r--r--   0        0        0     1509 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/user_settings.py
--rw-r--r--   0        0        0      795 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/users.py
--rw-r--r--   0        0        0     1494 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/users_management.py
--rw-r--r--   0        0        0     6357 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/vacancies.py
--rw-r--r--   0        0        0     2865 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/vacancy_requests.py
--rw-r--r--   0        0        0      719 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/models/response/webhooks.py
--rw-r--r--   0        0        0       53 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/tokens/__init__.py
--rw-r--r--   0        0        0     1871 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/tokens/locker.py
--rw-r--r--   0        0        0     5186 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/tokens/proxy.py
--rw-r--r--   0        0        0      730 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/tokens/storage.py
--rw-r--r--   0        0        0      548 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/huntflow_api_client/tokens/token.py
--rw-r--r--   0        0        0     1649 2024-05-03 07:48:37.511069 huntflow_api_client-2.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/__init__.py
--rw-r--r--   0        0        0     4829 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/api.py
--rw-r--r--   0        0        0       79 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/conftest.py
--rw-r--r--   0        0        0      176 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/fixtures/server.py
--rw-r--r--   0        0        0      924 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/fixtures/tokens.py
--rw-r--r--   0        0        0        0 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/__init__.py
--rw-r--r--   0        0        0     3225 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_account_divisions.py
--rw-r--r--   0        0        0     5097 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_account_offers.py
--rw-r--r--   0        0        0     3886 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_account_vacancy_request.py
--rw-r--r--   0        0        0     2329 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_accounts.py
--rw-r--r--   0        0        0     1385 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_action_logs.py
--rw-r--r--   0        0        0     7422 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_applicant_logs.py
--rw-r--r--   0        0        0     3089 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_applicant_offers.py
--rw-r--r--   0        0        0     3664 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_applicant_on_vacancy.py
--rw-r--r--   0        0        0     1244 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_applicant_on_vacancy_statuses.py
--rw-r--r--   0        0        0     1574 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_applicant_response.py
--rw-r--r--   0        0        0    11555 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_applicants.py
--rw-r--r--   0        0        0     2909 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_coworkers.py
--rw-r--r--   0        0        0     1358 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_delayed_tasks.py
--rw-r--r--   0        0        0     4497 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_dictionaries.py
--rw-r--r--   0        0        0     2012 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_email_templates.py
--rw-r--r--   0        0        0     1778 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_file.py
--rw-r--r--   0        0        0     2925 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_multi_vacancies.py
--rw-r--r--   0        0        0     2508 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_organization_settings.py
--rw-r--r--   0        0        0     7896 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_production_calendar.py
--rw-r--r--   0        0        0     3445 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_questionary.py
--rw-r--r--   0        0        0     1015 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_regions.py
--rw-r--r--   0        0        0     1069 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_rejection_reasons.py
--rw-r--r--   0        0        0    15232 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_resume.py
--rw-r--r--   0        0        0     2058 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_survey_type_a.py
--rw-r--r--   0        0        0     8613 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_survey_type_q.py
--rw-r--r--   0        0        0     4638 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_tags.py
--rw-r--r--   0        0        0     2237 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_user_settings.py
--rw-r--r--   0        0        0     1052 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_users.py
--rw-r--r--   0        0        0     6510 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_users_management.py
--rw-r--r--   0        0        0    16866 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_vacancies.py
--rw-r--r--   0        0        0     4406 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_vacancy_request.py
--rw-r--r--   0        0        0     2584 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_entities/test_webhooks.py
--rw-r--r--   0        0        0        0 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_errors/__init__.py
--rw-r--r--   0        0        0     8107 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_errors/test_error_handlers.py
--rw-r--r--   0        0        0        0 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_tokens/__init__.py
--rw-r--r--   0        0        0     5556 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_tokens/test_access_token.py
--rw-r--r--   0        0        0     2008 2024-05-03 07:48:23.802954 huntflow_api_client-2.1.0/tests/test_tokens/test_huntflow_token_proxy.py
--rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 huntflow_api_client-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/LICENSE
+-rw-r--r--   0        0        0      488 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/README.md
+-rw-r--r--   0        0        0       76 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/__init__.py
+-rw-r--r--   0        0        0     5735 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/api.py
+-rw-r--r--   0        0        0     2880 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/account_offers.py
+-rw-r--r--   0        0        0     1770 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/account_vacancy_request.py
+-rw-r--r--   0        0        0     1449 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/accounts.py
+-rw-r--r--   0        0        0     1631 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/action_logs.py
+-rw-r--r--   0        0        0     2595 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/applicant_logs.py
+-rw-r--r--   0        0        0     2859 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/applicant_offers.py
+-rw-r--r--   0        0        0     2958 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/applicant_on_vacancy.py
+-rw-r--r--   0        0        0      735 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/applicant_on_vacancy_status.py
+-rw-r--r--   0        0        0     1238 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/applicant_reponse.py
+-rw-r--r--   0        0        0     6966 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/applicants.py
+-rw-r--r--   0        0        0      941 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/base.py
+-rw-r--r--   0        0        0     2733 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/coworkers.py
+-rw-r--r--   0        0        0      748 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/delayed_tasks.py
+-rw-r--r--   0        0        0     3022 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/dictionaries.py
+-rw-r--r--   0        0        0     2564 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/divisions.py
+-rw-r--r--   0        0        0      888 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/email_templates.py
+-rw-r--r--   0        0        0     1140 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/file.py
+-rw-r--r--   0        0        0     2145 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/multi_vacancies.py
+-rw-r--r--   0        0        0     1955 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/organization_settings.py
+-rw-r--r--   0        0        0     6797 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/production_calendars.py
+-rw-r--r--   0        0        0     2995 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/questionary.py
+-rw-r--r--   0        0        0      623 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/regions.py
+-rw-r--r--   0        0        0      718 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/rejection_reason.py
+-rw-r--r--   0        0        0     3772 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/resume.py
+-rw-r--r--   0        0        0     1575 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/survey_type_a.py
+-rw-r--r--   0        0        0     4331 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/survey_type_q.py
+-rw-r--r--   0        0        0     4558 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/tags.py
+-rw-r--r--   0        0        0      993 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/user_settings.py
+-rw-r--r--   0        0        0      690 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/users.py
+-rw-r--r--   0        0        0     6048 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/users_management.py
+-rw-r--r--   0        0        0    11740 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/vacancies.py
+-rw-r--r--   0        0        0     2933 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/vacancy_requests.py
+-rw-r--r--   0        0        0     1815 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/entities/webhooks.py
+-rw-r--r--   0        0        0      553 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/errors/__init__.py
+-rw-r--r--   0        0        0     1128 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/errors/errors.py
+-rw-r--r--   0        0        0     3732 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/errors/handlers.py
+-rw-r--r--   0        0        0      361 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/errors/response_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/__init__.py
+-rw-r--r--   0        0        0     9669 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/common.py
+-rw-r--r--   0        0        0     3435 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/consts.py
+-rw-r--r--   0        0        0        0 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/__init__.py
+-rw-r--r--   0        0        0     2640 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/applicant_logs.py
+-rw-r--r--   0        0        0      326 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/applicant_offers.py
+-rw-r--r--   0        0        0     3618 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/applicant_on_vacancy.py
+-rw-r--r--   0        0        0     2980 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/applicants.py
+-rw-r--r--   0        0        0     1492 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/dictionaries.py
+-rw-r--r--   0        0        0      691 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/divisions.py
+-rw-r--r--   0        0        0      957 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/file.py
+-rw-r--r--   0        0        0     4553 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/multi_vacancies.py
+-rw-r--r--   0        0        0      920 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/production_calendars.py
+-rw-r--r--   0        0        0      670 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/resume.py
+-rw-r--r--   0        0        0      279 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/survey.py
+-rw-r--r--   0        0        0      436 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/tags.py
+-rw-r--r--   0        0        0      108 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/users_management.py
+-rw-r--r--   0        0        0     3711 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/vacancies.py
+-rw-r--r--   0        0        0     1393 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/vacancy_requests.py
+-rw-r--r--   0        0        0      482 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/request/webhooks.py
+-rw-r--r--   0        0        0        0 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/__init__.py
+-rw-r--r--   0        0        0      602 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/account_offers.py
+-rw-r--r--   0        0        0     1909 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/account_vacancy_request.py
+-rw-r--r--   0        0        0     1595 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/accounts.py
+-rw-r--r--   0        0        0     1187 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/action_logs.py
+-rw-r--r--   0        0        0     8554 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/applicant_logs.py
+-rw-r--r--   0        0        0      622 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/applicant_offers.py
+-rw-r--r--   0        0        0     1044 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/applicant_on_vacancy.py
+-rw-r--r--   0        0        0      773 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/applicant_on_vacancy_status.py
+-rw-r--r--   0        0        0     1197 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/applicant_response.py
+-rw-r--r--   0        0        0     5657 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/applicants.py
+-rw-r--r--   0        0        0     1306 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/coworkers.py
+-rw-r--r--   0        0        0     1381 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/delayed_tasks.py
+-rw-r--r--   0        0        0     2261 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/dictionaries.py
+-rw-r--r--   0        0        0     1507 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/divisions.py
+-rw-r--r--   0        0        0     1262 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/email_templates.py
+-rw-r--r--   0        0        0     2022 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/file.py
+-rw-r--r--   0        0        0      156 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/muilti_vacancies.py
+-rw-r--r--   0        0        0     1297 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/organization_settings.py
+-rw-r--r--   0        0        0     1525 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/production_calendars.py
+-rw-r--r--   0        0        0     1365 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/questionary.py
+-rw-r--r--   0        0        0      718 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/regions.py
+-rw-r--r--   0        0        0      476 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/rejection_reason.py
+-rw-r--r--   0        0        0    13292 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/resume.py
+-rw-r--r--   0        0        0     2953 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/survey.py
+-rw-r--r--   0        0        0      490 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/tags.py
+-rw-r--r--   0        0        0     1509 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/user_settings.py
+-rw-r--r--   0        0        0      795 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/users.py
+-rw-r--r--   0        0        0     1494 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/users_management.py
+-rw-r--r--   0        0        0     6357 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/vacancies.py
+-rw-r--r--   0        0        0     2865 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/vacancy_requests.py
+-rw-r--r--   0        0        0      719 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/models/response/webhooks.py
+-rw-r--r--   0        0        0       53 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/tokens/__init__.py
+-rw-r--r--   0        0        0     1871 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/tokens/locker.py
+-rw-r--r--   0        0        0     5186 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/tokens/proxy.py
+-rw-r--r--   0        0        0      730 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/tokens/storage.py
+-rw-r--r--   0        0        0      548 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/huntflow_api_client/tokens/token.py
+-rw-r--r--   0        0        0     1649 2024-05-06 08:56:12.025327 huntflow_api_client-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     4829 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/tests/api.py
+-rw-r--r--   0        0        0       79 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      176 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/tests/fixtures/server.py
+-rw-r--r--   0        0        0      924 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/tests/fixtures/tokens.py
+-rw-r--r--   0        0        0        0 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/tests/test_entities/__init__.py
+-rw-r--r--   0        0        0     3225 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/tests/test_entities/test_account_divisions.py
+-rw-r--r--   0        0        0     5097 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/tests/test_entities/test_account_offers.py
+-rw-r--r--   0        0        0     3886 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/tests/test_entities/test_account_vacancy_request.py
+-rw-r--r--   0        0        0     2329 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/tests/test_entities/test_accounts.py
+-rw-r--r--   0        0        0     1385 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/tests/test_entities/test_action_logs.py
+-rw-r--r--   0        0        0     7422 2024-05-06 08:56:00.781283 huntflow_api_client-2.2.0/tests/test_entities/test_applicant_logs.py
+-rw-r--r--   0        0        0     3089 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_applicant_offers.py
+-rw-r--r--   0        0        0     3664 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_applicant_on_vacancy.py
+-rw-r--r--   0        0        0     1244 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_applicant_on_vacancy_statuses.py
+-rw-r--r--   0        0        0     1574 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_applicant_response.py
+-rw-r--r--   0        0        0    11555 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_applicants.py
+-rw-r--r--   0        0        0     2909 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_coworkers.py
+-rw-r--r--   0        0        0     1358 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_delayed_tasks.py
+-rw-r--r--   0        0        0     4497 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_dictionaries.py
+-rw-r--r--   0        0        0     2012 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_email_templates.py
+-rw-r--r--   0        0        0     1778 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_file.py
+-rw-r--r--   0        0        0     2925 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_multi_vacancies.py
+-rw-r--r--   0        0        0     2508 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_organization_settings.py
+-rw-r--r--   0        0        0     7896 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_production_calendar.py
+-rw-r--r--   0        0        0     3445 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_questionary.py
+-rw-r--r--   0        0        0     1015 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_regions.py
+-rw-r--r--   0        0        0     1069 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_rejection_reasons.py
+-rw-r--r--   0        0        0    15232 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_resume.py
+-rw-r--r--   0        0        0     2058 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_survey_type_a.py
+-rw-r--r--   0        0        0     8613 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_survey_type_q.py
+-rw-r--r--   0        0        0     4638 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_tags.py
+-rw-r--r--   0        0        0     2237 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_user_settings.py
+-rw-r--r--   0        0        0     1052 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_users.py
+-rw-r--r--   0        0        0     7978 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_users_management.py
+-rw-r--r--   0        0        0    16866 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_vacancies.py
+-rw-r--r--   0        0        0     4406 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_vacancy_request.py
+-rw-r--r--   0        0        0     2584 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_entities/test_webhooks.py
+-rw-r--r--   0        0        0        0 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_errors/__init__.py
+-rw-r--r--   0        0        0     8107 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_errors/test_error_handlers.py
+-rw-r--r--   0        0        0        0 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_tokens/__init__.py
+-rw-r--r--   0        0        0     5556 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_tokens/test_access_token.py
+-rw-r--r--   0        0        0     2008 2024-05-06 08:56:00.785283 huntflow_api_client-2.2.0/tests/test_tokens/test_huntflow_token_proxy.py
+-rw-r--r--   0        0        0     1076 1970-01-01 00:00:00.000000 huntflow_api_client-2.2.0/PKG-INFO
```

### Comparing `huntflow_api_client-2.1.0/LICENSE` & `huntflow_api_client-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/api.py` & `huntflow_api_client-2.2.0/huntflow_api_client/api.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/__init__.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/account_offers.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/account_offers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/account_vacancy_request.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/account_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/accounts.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/accounts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/action_logs.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/action_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_logs.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/applicant_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_offers.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/applicant_offers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_on_vacancy.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_on_vacancy_status.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/applicant_on_vacancy_status.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/applicant_reponse.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/applicant_reponse.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/applicants.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/applicants.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/base.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/base.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/coworkers.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/coworkers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/delayed_tasks.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/delayed_tasks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/dictionaries.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/divisions.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/email_templates.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/email_templates.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/file.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/file.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/multi_vacancies.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/multi_vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/organization_settings.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/organization_settings.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/production_calendars.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/production_calendars.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/questionary.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/questionary.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/regions.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/regions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/rejection_reason.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/rejection_reason.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/resume.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/resume.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/survey_type_a.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/survey_type_a.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/survey_type_q.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/survey_type_q.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/tags.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/tags.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/user_settings.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/user_settings.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/users.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/users.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/users_management.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/users_management.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 from huntflow_api_client.entities.base import BaseEntity
+from huntflow_api_client.models.consts import MemberType
 from huntflow_api_client.models.request.users_management import ForeignUserRequest
 from huntflow_api_client.models.response.users_management import (
     CreatedUserControlTaskResponse,
     ForeignUserResponse,
     ForeignUsersListResponse,
     UserControlTaskResponse,
     UserInternalIDResponse,
 )
 
 
 class UsersManagement(BaseEntity):
     async def get_users_with_foreign(
         self,
         account_id: int,
+        member_types: Optional[List[MemberType]] = None,
         count: Optional[int] = 30,
         page: Optional[int] = 1,
     ) -> ForeignUsersListResponse:
         """
         API method reference
             https://api.huntflow.ai/v2/docs#get-/accounts/-account_id-/users/foreign
 
         :param account_id: Organization ID
+        :param member_types: Array of member types
         :param count: Number of items per page
         :param page: Page number
 
         :return: All users in organization with their permissions
             (vacancies permissions are not included),
             available divisions and their manager's identifiers.
             All identifiers in response are foreign.
         """
         params: Dict[str, Any] = {"count": count, "page": page}
+        if member_types:
+            params["member_types"] = [member_type.value for member_type in member_types]
         response = await self._api.request(
             "GET",
             f"/accounts/{account_id}/users/foreign",
             params=params,
         )
         return ForeignUsersListResponse.model_validate(response.json())
```

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/vacancies.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/vacancy_requests.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/vacancy_requests.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/entities/webhooks.py` & `huntflow_api_client-2.2.0/huntflow_api_client/entities/webhooks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/errors/__init__.py` & `huntflow_api_client-2.2.0/huntflow_api_client/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/errors/errors.py` & `huntflow_api_client-2.2.0/huntflow_api_client/errors/errors.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/errors/handlers.py` & `huntflow_api_client-2.2.0/huntflow_api_client/errors/handlers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/common.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/common.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/consts.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/consts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicant_logs.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/request/applicant_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicant_on_vacancy.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/request/applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/request/applicants.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/request/applicants.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/request/dictionaries.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/request/dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/request/divisions.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/request/divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/request/file.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/request/file.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/request/multi_vacancies.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/request/multi_vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/request/production_calendars.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/request/production_calendars.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/request/resume.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/request/resume.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/request/vacancies.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/request/vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/request/vacancy_requests.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/request/vacancy_requests.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/account_offers.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/account_offers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/account_vacancy_request.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/account_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/accounts.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/accounts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/action_logs.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/action_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_logs.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/applicant_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_offers.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/applicant_offers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_on_vacancy.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_on_vacancy_status.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/applicant_on_vacancy_status.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicant_response.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/applicant_response.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/applicants.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/applicants.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/coworkers.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/coworkers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/delayed_tasks.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/delayed_tasks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/dictionaries.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/divisions.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/email_templates.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/email_templates.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/file.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/file.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/organization_settings.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/organization_settings.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/production_calendars.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/production_calendars.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/questionary.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/questionary.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/regions.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/regions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/resume.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/resume.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/survey.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/survey.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/user_settings.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/user_settings.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/users.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/users.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/users_management.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/users_management.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/vacancies.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/vacancy_requests.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/vacancy_requests.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/models/response/webhooks.py` & `huntflow_api_client-2.2.0/huntflow_api_client/models/response/webhooks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/tokens/locker.py` & `huntflow_api_client-2.2.0/huntflow_api_client/tokens/locker.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/tokens/proxy.py` & `huntflow_api_client-2.2.0/huntflow_api_client/tokens/proxy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/tokens/storage.py` & `huntflow_api_client-2.2.0/huntflow_api_client/tokens/storage.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/huntflow_api_client/tokens/token.py` & `huntflow_api_client-2.2.0/huntflow_api_client/tokens/token.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/pyproject.toml` & `huntflow_api_client-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "huntflow-api-client"
-version = "2.1.0"
+version = "2.2.0"
 description = "Huntflow API Client for Python"
 authors = [
     { name = "Developers huntflow", email = "developer@huntflow.ru" },
 ]
 dependencies = [
     "httpx>=0.23.3",
     "email-validator>=1.3.1",
```

### Comparing `huntflow_api_client-2.1.0/tests/api.py` & `huntflow_api_client-2.2.0/tests/api.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/fixtures/tokens.py` & `huntflow_api_client-2.2.0/tests/fixtures/tokens.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_account_divisions.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_account_divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_account_offers.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_account_offers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_account_vacancy_request.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_account_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_accounts.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_accounts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_action_logs.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_action_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_applicant_logs.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_applicant_logs.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_applicant_offers.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_applicant_offers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_applicant_on_vacancy.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_applicant_on_vacancy_statuses.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_applicant_on_vacancy_statuses.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_applicant_response.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_applicant_response.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_applicants.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_applicants.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_coworkers.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_coworkers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_delayed_tasks.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_delayed_tasks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_dictionaries.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_email_templates.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_email_templates.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_file.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_file.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_multi_vacancies.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_multi_vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_organization_settings.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_organization_settings.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_production_calendar.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_production_calendar.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_questionary.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_questionary.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_regions.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_regions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_rejection_reasons.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_rejection_reasons.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_resume.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_resume.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_survey_type_a.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_survey_type_a.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_survey_type_q.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_survey_type_q.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_tags.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_tags.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_user_settings.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_users.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_users.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_users_management.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_users_management.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,42 @@
             "head_id": "user-032044",
             "division_ids": ["division-154", "division-871"],
             "permissions": ["string"],
             "meta": {},
         },
     ],
 }
+GET_USERS_RESPONSE_TWO_MEMBERS: Dict[str, Any] = {
+    "page": 1,
+    "count": 30,
+    "total_pages": 1,
+    "total_items": 2,
+    "items": [
+        {
+            "id": "some_foreign_id_1",
+            "name": "John Doe",
+            "email": "mail@gmail.com",
+            "type": "owner",
+            "head_id": "user-032044",
+            "division_ids": ["division-154", "division-871"],
+            "permissions": ["string"],
+            "meta": {},
+        },
+        {
+            "id": "some_foreign_id_2",
+            "name": "Nick Smith",
+            "email": "mail@example.com",
+            "type": "manager",
+            "head_id": "user-1234",
+            "division_ids": ["division-123", "division-321"],
+            "permissions": ["string"],
+            "meta": {},
+        },
+    ],
+}
 GET_USER_BY_FOREIGN_RESPONSE: Dict[str, Any] = {
     "id": FOREIGN_USER_ID,
     "name": "John Doe",
     "email": "mail@gmail.com",
     "type": "owner",
     "head_id": "user-032044",
     "division_ids": ["division-154", "division-871"],
@@ -71,23 +99,41 @@
 
 
 async def test_get_users_with_foreign(
     httpx_mock: HTTPXMock,
     token_proxy: HuntflowTokenProxy,
 ) -> None:
     httpx_mock.add_response(
-        url=f"{VERSIONED_BASE_URL}/accounts/{ACCOUNT_ID}/users/foreign?count=30&page=1",
+        url=f"{VERSIONED_BASE_URL}/accounts/{ACCOUNT_ID}/users/"
+        f"foreign?count=30&page=1&member_types=owner",
         json=GET_USERS_RESPONSE,
     )
     api_client = HuntflowAPI(BASE_URL, token_proxy=token_proxy)
     users_management = UsersManagement(api_client)
 
-    response = await users_management.get_users_with_foreign(account_id=ACCOUNT_ID)
+    response = await users_management.get_users_with_foreign(
+        account_id=ACCOUNT_ID,
+        member_types=[MemberType.owner],
+    )
     assert response == ForeignUsersListResponse(**GET_USERS_RESPONSE)
 
+    httpx_mock.add_response(
+        url=f"{VERSIONED_BASE_URL}/accounts/{ACCOUNT_ID}/users/"
+        f"foreign?count=30&page=1&member_types=owner&member_types=manager",
+        json=GET_USERS_RESPONSE_TWO_MEMBERS,
+    )
+    api_client = HuntflowAPI(BASE_URL, token_proxy=token_proxy)
+    users_management = UsersManagement(api_client)
+
+    response = await users_management.get_users_with_foreign(
+        account_id=ACCOUNT_ID,
+        member_types=[MemberType.owner, MemberType.manager],
+    )
+    assert response == ForeignUsersListResponse(**GET_USERS_RESPONSE_TWO_MEMBERS)
+
 
 async def test_get_user_by_foreign(
     httpx_mock: HTTPXMock,
     token_proxy: HuntflowTokenProxy,
 ) -> None:
     httpx_mock.add_response(
         url=f"{VERSIONED_BASE_URL}/accounts/{ACCOUNT_ID}/users/foreign/{FOREIGN_USER_ID}",
```

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_vacancies.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_vacancy_request.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_entities/test_webhooks.py` & `huntflow_api_client-2.2.0/tests/test_entities/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_errors/test_error_handlers.py` & `huntflow_api_client-2.2.0/tests/test_errors/test_error_handlers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_tokens/test_access_token.py` & `huntflow_api_client-2.2.0/tests/test_tokens/test_access_token.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/tests/test_tokens/test_huntflow_token_proxy.py` & `huntflow_api_client-2.2.0/tests/test_tokens/test_huntflow_token_proxy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-2.1.0/PKG-INFO` & `huntflow_api_client-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huntflow-api-client
-Version: 2.1.0
+Version: 2.2.0
 Summary: Huntflow API Client for Python
 Author-Email: Developers huntflow <developer@huntflow.ru>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

