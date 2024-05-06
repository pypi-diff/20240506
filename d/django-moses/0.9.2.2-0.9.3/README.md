# Comparing `tmp/django_moses-0.9.2.2.tar.gz` & `tmp/django_moses-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_moses-0.9.2.2.tar", max compression
+gzip compressed data, was "django_moses-0.9.3.tar", max compression
```

## Comparing `django_moses-0.9.2.2.tar` & `django_moses-0.9.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1460 2023-07-27 16:00:53.711409 django_moses-0.9.2.2/LICENSE
--rw-r--r--   0        0        0        0 2023-07-27 16:00:53.711807 django_moses-0.9.2.2/moses/__init__.py
--rw-r--r--   0        0        0     2614 2023-12-18 20:26:51.401247 django_moses-0.9.2.2/moses/admin.py
--rw-r--r--   0        0        0       85 2023-07-27 16:00:53.712065 django_moses-0.9.2.2/moses/apps.py
--rw-r--r--   0        0        0     8746 2023-11-07 09:52:53.549699 django_moses-0.9.2.2/moses/authentication.py
--rw-r--r--   0        0        0     2967 2023-11-07 09:52:53.550151 django_moses-0.9.2.2/moses/conf.py
--rw-r--r--   0        0        0      933 2023-07-27 16:00:53.712450 django_moses-0.9.2.2/moses/decorators.py
--rw-r--r--   0        0        0      632 2023-11-07 09:52:53.550287 django_moses-0.9.2.2/moses/errors.py
--rw-r--r--   0        0        0     4952 2023-11-07 13:27:21.034450 django_moses-0.9.2.2/moses/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-27 16:00:53.712684 django_moses-0.9.2.2/moses/migrations/__init__.py
--rw-r--r--   0        0        0    10590 2023-11-07 09:52:53.550492 django_moses-0.9.2.2/moses/models.py
--rw-r--r--   0        0        0     9736 2023-11-07 09:52:53.550912 django_moses-0.9.2.2/moses/serializers.py
--rw-r--r--   0        0        0     2740 2023-12-18 20:08:01.447532 django_moses-0.9.2.2/moses/templates/admin/login.html
--rw-r--r--   0        0        0      561 2023-11-07 09:52:53.551278 django_moses-0.9.2.2/moses/urls.py
--rw-r--r--   0        0        0        1 2023-11-07 09:52:53.551599 django_moses-0.9.2.2/moses/views/__init__.py
--rw-r--r--   0        0        0      309 2023-11-07 09:52:53.551908 django_moses-0.9.2.2/moses/views/token_obtain_pair.py
--rw-r--r--   0        0        0    20965 2023-11-07 09:52:53.552073 django_moses-0.9.2.2/moses/views/user.py
--rw-r--r--   0        0        0      931 2023-12-18 20:26:51.396236 django_moses-0.9.2.2/pyproject.toml
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 django_moses-0.9.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1460 2023-07-27 16:00:53.711409 django_moses-0.9.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-27 16:00:53.711807 django_moses-0.9.3/moses/__init__.py
+-rw-r--r--   0        0        0     2614 2023-12-18 20:26:51.401247 django_moses-0.9.3/moses/admin.py
+-rw-r--r--   0        0        0       85 2023-07-27 16:00:53.712065 django_moses-0.9.3/moses/apps.py
+-rw-r--r--   0        0        0     8746 2023-11-07 09:52:53.549699 django_moses-0.9.3/moses/authentication.py
+-rw-r--r--   0        0        0     3067 2024-01-02 14:01:06.753171 django_moses-0.9.3/moses/conf.py
+-rw-r--r--   0        0        0      933 2023-07-27 16:00:53.712450 django_moses-0.9.3/moses/decorators.py
+-rw-r--r--   0        0        0      632 2023-11-07 09:52:53.550287 django_moses-0.9.3/moses/errors.py
+-rw-r--r--   0        0        0     4952 2023-11-07 13:27:21.034450 django_moses-0.9.3/moses/migrations/0001_initial.py
+-rw-r--r--   0        0        0      888 2024-01-02 11:56:26.274979 django_moses-0.9.3/moses/migrations/0002_remove_customuser_last_password_reset_sms_sent_at_and_more.py
+-rw-r--r--   0        0        0      622 2024-01-02 14:01:18.842455 django_moses-0.9.3/moses/migrations/0003_rename_last_phone_number_candidate_confirmation_pin_sent_customuser_last_phone_number_confirmation_p.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:00:53.712684 django_moses-0.9.3/moses/migrations/__init__.py
+-rw-r--r--   0        0        0    10724 2024-01-02 14:01:06.747017 django_moses-0.9.3/moses/models.py
+-rw-r--r--   0        0        0    12641 2024-01-02 14:51:04.845131 django_moses-0.9.3/moses/serializers.py
+-rw-r--r--   0        0        0     2740 2023-12-18 20:08:01.447532 django_moses-0.9.3/moses/templates/admin/login.html
+-rw-r--r--   0        0        0      561 2023-11-07 09:52:53.551278 django_moses-0.9.3/moses/urls.py
+-rw-r--r--   0        0        0        1 2023-11-07 09:52:53.551599 django_moses-0.9.3/moses/views/__init__.py
+-rw-r--r--   0        0        0      309 2023-11-07 09:52:53.551908 django_moses-0.9.3/moses/views/token_obtain_pair.py
+-rw-r--r--   0        0        0    17866 2024-01-02 14:02:38.804532 django_moses-0.9.3/moses/views/user.py
+-rw-r--r--   0        0        0      927 2024-01-02 11:50:53.954037 django_moses-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 django_moses-0.9.3/PKG-INFO
```

### Comparing `django_moses-0.9.2.2/LICENSE` & `django_moses-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_moses-0.9.2.2/moses/admin.py` & `django_moses-0.9.3/moses/admin.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.9.2.2/moses/authentication.py` & `django_moses-0.9.3/moses/authentication.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.9.2.2/moses/conf.py` & `django_moses-0.9.3/moses/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,19 +25,21 @@
 default_settings = {
     "PHONE_NUMBER_VALIDATOR": None,
     "DEFAULT_LANGUAGE": None,
     "SEND_SMS_HANDLER": None,
     "DOMAIN": None,
     "URL_PREFIX": None,
     "IP_HEADER": None,
-    "MINUTES_BETWEEN_CONFIRMATION_PIN_SMS": 1,
-    "MAX_PHONE_NUMBER_CONFIRMATION_ATTEMPTS": 3,
-    "MAX_EMAIL_CONFIRMATION_ATTEMPTS": 3,
+    "PHONE_NUMBER_CONFIRMATION_ATTEMPTS_LIMIT": 3,
+    "EMAIL_CONFIRMATION_ATTEMPTS_LIMIT": 3,
+    "PASSWORD_RESET_SMS_MINUTES_PERIOD": 1,
+    "PHONE_NUMBER_CONFIRMATION_SMS_MINUTES_PERIOD": 1,
+    "PASSWORD_RESET_TIMEOUT_MINUTES": 5,
     "LANGUAGE_CHOICES": (
-        (1, _("English")),
+        ("en", _("English")),
     ),
 }
 
 SETTINGS_TO_IMPORT = ["SEND_SMS_HANDLER", "PHONE_NUMBER_VALIDATOR"]
 
 
 class Settings:
```

### Comparing `django_moses-0.9.2.2/moses/decorators.py` & `django_moses-0.9.3/moses/decorators.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.9.2.2/moses/errors.py` & `django_moses-0.9.3/moses/errors.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.9.2.2/moses/migrations/0001_initial.py` & `django_moses-0.9.3/moses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.9.2.2/moses/models.py` & `django_moses-0.9.3/moses/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import random
 import uuid
-from datetime import timedelta
 from enum import Enum
 
 import pyotp as pyotp
 from django.conf import settings as django_settings
 from django.contrib.auth.base_user import AbstractBaseUser, BaseUserManager
 from django.contrib.auth.models import PermissionsMixin
 from django.core.mail import send_mail
 from django.db import models
 from django.utils import timezone, translation
+from django.utils.timezone import now
 from django.utils.translation import gettext as _
 
 from moses.conf import settings as moses_settings
 
 
 class CustomUserManager(BaseUserManager):
     use_in_migrations = True
@@ -25,16 +25,16 @@
         return user
 
     def create_user(self, phone_number=None, password=None, **extra_fields):
         extra_fields.setdefault('is_staff', False)
         extra_fields.setdefault('is_superuser', False)
         extra_fields.setdefault('is_active', True)
         user = self._create_user(phone_number, password, **extra_fields)
-        user.send_phone_number_confirmation_sms(generate_new=True)
-        user.send_email_confirmation_email(generate_new=True)
+        user.send_credential_confirmation_code(Credential.EMAIL, generate_new=True)
+        user.send_credential_confirmation_code(Credential.PHONE_NUMBER, generate_new=True)
         return user
 
     def create_superuser(self, phone_number, password, **extra_fields):
         extra_fields.setdefault('is_staff', True)
         extra_fields.setdefault('is_superuser', True)
 
         if extra_fields.get('is_staff') is not True:
@@ -81,18 +81,22 @@
     phone_number_confirmation_pin = models.PositiveIntegerField(default=0, verbose_name=_("Phone number confirm PIN"))
     phone_number_candidate_confirmation_pin = models.PositiveIntegerField(default=0, verbose_name=_(
         "Phone number candidate confirm PIN"))
     phone_number_confirmation_attempts = models.PositiveSmallIntegerField(
         default=0,
         verbose_name=_("Phone number confirm attempts")
     )
-    last_password_reset_sms_sent_at = models.DateTimeField(
+    password_reset_code_sms_sent_at = models.DateTimeField(
         blank=True,
         null=True,
-        verbose_name=_("Last password reset sms sent at")
+        verbose_name=_("Last password reset code sent at")
+    )
+    password_reset_code = models.PositiveIntegerField(
+        blank=True,
+        null=True
     )
 
     first_name = models.CharField(max_length=200, verbose_name=_("First name"), blank=True)
     last_name = models.CharField(max_length=200, verbose_name=_("Last name"), blank=True)
 
     is_active = models.BooleanField(default=True, verbose_name=_("Is active"))
     is_staff = models.BooleanField(default=False, verbose_name=_("Is staff"))
@@ -102,82 +106,49 @@
         default=moses_settings.DEFAULT_LANGUAGE,
         max_length=10,
         verbose_name=_("Preferred language")
     )
     created_at = models.DateTimeField(default=timezone.now, blank=True, null=True, verbose_name=_("Created at"))
 
     mfa_secret_key = models.CharField(blank=True, default='', max_length=160)
-    last_phone_number_confirmation_pin_sent = models.DateTimeField(null=True, blank=True)
-    last_phone_number_candidate_confirmation_pin_sent = models.DateTimeField(null=True, blank=True)
-    userpic = models.ImageField(upload_to='images/userpics/', blank=True, null=True)
+    last_phone_number_confirmation_pins_sent = models.DateTimeField(null=True, blank=True)
 
     USERNAME_FIELD = 'phone_number'
 
     objects = CustomUserManager()
 
     def check_mfa_otp(self, otp):
         if self.is_superuser and not django_settings.DEBUG and not self.mfa_secret_key:
             return False
         elif not self.mfa_secret_key:
             return True
         totp = pyotp.totp.TOTP(self.mfa_secret_key.encode('utf-8'))
         return totp.verify(otp)
 
-    def send_phone_number_confirmation_sms(self, generate_new=False):
-        if generate_new or self.phone_number_confirmation_pin == 0:
-            self.phone_number_confirmation_pin = random.randint(0, 999999)
-        self.last_phone_number_confirmation_pin_sent = timezone.now()
-        self.save()
-        with translation.override(self.preferred_language):
-            moses_settings.SEND_SMS_HANDLER(
-                self.phone_number,
-                _("Phone number confirmation PIN: ") + str(self.phone_number_confirmation_pin).zfill(6)
-            )
-
-    def send_phone_number_candidate_confirmation_sms(self, generate_new=False):
-        if not self.phone_number_candidate:
-            return
-        if generate_new or self.phone_number_candidate_confirmation_pin == 0:
-            self.phone_number_candidate_confirmation_pin = random.randint(0, 999999)
-        if (
-                self.last_phone_number_candidate_confirmation_pin_sent is not None and
-                self.last_phone_number_candidate_confirmation_pin_sent > timezone.now() - timedelta(
-            minutes=moses_settings.MINUTES_BETWEEN_CONFIRMATION_PIN_SMS
-        )):
-            return
-        self.last_phone_number_candidate_confirmation_pin_sent = timezone.now()
-        self.save()
-        with translation.override(self.preferred_language):
-            moses_settings.SEND_SMS_HANDLER(
-                self.phone_number_candidate,
-                _("Phone number confirmation PIN: ") + str(
-                    self.phone_number_candidate_confirmation_pin).zfill(
-                    6))
-
     def try_to_confirm_credential(self, credential: Credential, main_pin_str: str, candidate_pin_str: str):
         match credential:
             case Credential.PHONE_NUMBER:
                 attempts_field = 'phone_number_confirmation_attempts'
                 current_credential_field = 'phone_number'
                 candidate_credential_field = 'phone_number_candidate'
                 current_credential_confirmation_field = 'is_phone_number_confirmed'
-                max_attempts_limit = moses_settings.MAX_PHONE_NUMBER_CONFIRMATION_ATTEMPTS
+                max_attempts_limit = moses_settings.PHONE_NUMBER_CONFIRMATION_ATTEMPTS_LIMIT
                 current_pin_field = 'phone_number_confirmation_pin'
                 candidate_pin_field = 'phone_number_candidate_confirmation_pin'
             case Credential.EMAIL:
                 attempts_field = 'email_confirmation_attempts'
                 current_credential_field = 'email'
                 candidate_credential_field = 'email_candidate'
                 current_credential_confirmation_field = 'is_email_confirmed'
-                max_attempts_limit = moses_settings.MAX_EMAIL_CONFIRMATION_ATTEMPTS
+                max_attempts_limit = moses_settings.EMAIL_CONFIRMATION_ATTEMPTS_LIMIT
                 current_pin_field = 'email_confirmation_pin'
                 candidate_pin_field = 'email_candidate_confirmation_pin'
             case _:
                 raise ValueError('invalid_credential')
-        if getattr(self, attempts_field) == max_attempts_limit:
+        if getattr(self, attempts_field) >= max_attempts_limit:
             return False, False
         received_pin, received_candidate_pin = int(main_pin_str or '0'), int(candidate_pin_str or '0')
         is_main_pin_correct = received_pin == getattr(self, current_pin_field)
         is_candidate_pin_correct = None
         if getattr(self, candidate_credential_field):
             is_candidate_pin_correct = getattr(self, candidate_pin_field) == received_candidate_pin
         if is_main_pin_correct and (is_candidate_pin_correct is None or is_candidate_pin_correct):
@@ -190,29 +161,67 @@
                 setattr(self, candidate_credential_field, '')
             self.save()
         else:
             setattr(self, attempts_field, getattr(self, attempts_field) + 1)
             self.save()
         return is_main_pin_correct, is_candidate_pin_correct
 
-    def send_email_confirmation_email(self, generate_new=False):
-        if generate_new or self.email_confirmation_pin == 0:
-            self.email_confirmation_pin = random.randint(0, 999999)
-            self.save()
-        with translation.override(self.preferred_language):
-            send_mail(_("Email confirmation PIN"),
-                      _("Your email confirmation PIN is: ") + str(self.email_confirmation_pin),
-                      'noreply@' + moses_settings.DOMAIN, [self.email])
-
-    def send_email_candidate_confirmation_email(self, generate_new=False):
-        if not self.email_candidate:
-            return
-        if generate_new or self.email_candidate_confirmation_pin == 0:
-            self.email_candidate_confirmation_pin = random.randint(0, 999999)
-            self.save()
+    def send_credential_confirmation_code(self, credential_type: Credential, candidate=False, generate_new=False):
+        match credential_type:
+            case Credential.PHONE_NUMBER:
+                send_function = moses_settings.SEND_SMS_HANDLER
+                setattr(self, 'last_phone_number_confirmation_pins_sent', now())
+                if candidate:
+                    credential_field = 'phone_number_candidate'
+                    pin_field = 'phone_number_candidate_confirmation_pin'
+                else:
+                    credential_field = 'phone_number'
+                    pin_field = 'phone_number_confirmation_pin'
+            case Credential.EMAIL:
+                def send_email_confirmation_message(email: str, body: str):
+                    send_mail(_("Email confirmation PIN"), body, 'noreply@' + moses_settings.DOMAIN, [email])
+
+                send_function = send_email_confirmation_message
+                if candidate:
+                    credential_field = 'email_candidate'
+                    pin_field = 'email_candidate_confirmation_pin'
+                else:
+                    credential_field = 'email'
+                    pin_field = 'email_confirmation_pin'
+            case _:
+                raise ValueError('invalid_credential')
+        if generate_new:
+            setattr(self, pin_field, random.randint(0, 999999))
+        self.save()
         with translation.override(self.preferred_language):
-            send_mail(_("Email confirmation PIN"),
-                      _("Your email confirmation PIN is: ") + str(self.email_candidate_confirmation_pin),
-                      'noreply@' + django_settings.DOMAIN, [self.email_candidate])
+            send_function(getattr(self, credential_field),
+                          _("Your confirmation PIN is: ") + str(getattr(self, pin_field)).zfill(6))
+
+    def send_password_reset_code(self, credential: str) -> bool:
+        self.password_reset_code = random.randint(0, 1000000)
+        self.save()
+        message_body = _(f"Your password reset code is {self.password_reset_code}")
+        match credential:
+            case self.email:
+                if self.is_email_confirmed:
+                    send_mail(_("Password reset"), message_body, 'noreply@' + moses_settings.DOMAIN, [self.email])
+                    return True
+                return False
+            case self.phone_number:
+                sms_limit_reached =  self.password_reset_code_sms_sent_at is not None and (
+                        timezone.now() - self.password_reset_code_sms_sent_at
+                ).minutes < moses_settings.PASSWORD_RESET_SMS_MINUTES_PERIOD
+                if self.is_phone_number_confirmed and not sms_limit_reached:
+                    self.password_reset_code_sms_sent_at = timezone.now()
+                    self.save()
+                    moses_settings.SEND_SMS_HANDLER(self.phone_number, message_body)
+                    return True
+                return False
+            case _:
+                return False
 
     def __str__(self):
         return f'{self.first_name} {self.last_name}'
+
+
+def generate_sms_code():
+    return random.randint(0, 1000000)
```

### Comparing `django_moses-0.9.2.2/moses/serializers.py` & `django_moses-0.9.3/moses/serializers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+from datetime import timedelta
+
 from django.contrib.auth import authenticate
 from django.contrib.auth.models import Group
 from django.contrib.auth.password_validation import validate_password
 from django.contrib.sites.models import Site
 from django.core import exceptions as django_exceptions
 from django.core.validators import EmailValidator
 from django.db import IntegrityError, transaction
+from django.db.models import Q
+from django.utils import timezone
 from django.utils.translation import gettext as _
 from djoser import constants
 from rest_framework import serializers, exceptions
+from rest_framework.exceptions import ValidationError
 from rest_framework.fields import CharField
 from rest_framework.serializers import raise_errors_on_nested_writes, ModelSerializer, Serializer
 from rest_framework.utils import model_meta
 from rest_framework_simplejwt.serializers import TokenObtainSerializer
 from rest_framework_simplejwt.tokens import RefreshToken
 
 from moses import errors
 from moses.conf import settings as moses_settings
-from moses.models import CustomUser
+from moses.models import CustomUser, Credential
 
 
 class PinSerializer(Serializer):
     pin = CharField()
     candidate_pin = CharField(required=False)
 
 
@@ -62,16 +67,16 @@
 
 class ShortCustomUserSerializer(serializers.ModelSerializer):
     income_subscription = serializers.BooleanField(read_only=True)
     outcome_subscription = serializers.BooleanField(read_only=True)
 
     class Meta:
         model = CustomUser
-        fields = ['id', 'first_name', 'last_name', 'userpic', 'outcome_subscription', 'income_subscription']
-        read_only_fields = ['id', 'first_name', 'last_name', 'userpic', 'income_subscription',
+        fields = ['id', 'first_name', 'last_name', 'outcome_subscription', 'income_subscription']
+        read_only_fields = ['id', 'first_name', 'last_name', 'income_subscription',
                             'outcome_subscription']
 
 
 class PublicCustomUserSerializer(serializers.ModelSerializer):
     class Meta:
         model = CustomUser
         fields = [
@@ -83,15 +88,14 @@
 
 class PrivateCustomUserSerializer(serializers.ModelSerializer):
     is_mfa_enabled = serializers.SerializerMethodField()
 
     def get_is_mfa_enabled(self, obj):
         return len(obj.mfa_secret_key) > 0
 
-
     def update(self, instance, validated_data):
         raise_errors_on_nested_writes('update', self, validated_data)
         info = model_meta.get_field_info(instance)
         if 'phone_number' in validated_data:
             _phone_number = validated_data.pop('phone_number')
             if _phone_number == instance.phone_number:
                 instance.phone_number_candidate = ''
@@ -100,55 +104,60 @@
                 instance.phone_number_confirm_attempts = 0
                 instance.save()
             elif _phone_number != (instance.phone_number_candidate or instance.phone_number):
                 if instance.is_phone_number_confirmed:
                     instance.phone_number_candidate = _phone_number
                     instance.phone_number_confirm_attempts = 0
                     instance.save()
-                    instance.send_phone_number_confirmation_sms(generate_new=True)
-                    instance.send_phone_number_candidate_confirmation_sms(generate_new=True)
+
+                    instance.send_credential_confirmation_code(Credential.PHONE_NUMBER, candidate=False,
+                                                               generate_new=True)
+
+                    instance.send_credential_confirmation_code(Credential.PHONE_NUMBER, candidate=True,
+                                                               generate_new=True)
                 else:
                     instance.phone_number = _phone_number
                     instance.phone_number_confirm_attempts = 0
                     instance.save()
-                    instance.send_phone_number_confirmation_sms(generate_new=True)
+
+                    instance.send_credential_confirmation_code(Credential.PHONE_NUMBER, candidate=False,
+                                                               generate_new=True)
         if 'email' in validated_data:
             _email = validated_data.pop('email')
             if _email == instance.email:
                 instance.email_candidate = ''
                 instance.email_confirm_pin = 0
                 instance.email_candidate_confirm_pin = 0
                 instance.email_confirm_attempts = 0
                 instance.save()
             elif _email != (instance.email_candidate or instance.email):
                 if instance.is_email_confirmed:
                     instance.email_candidate = _email
                     instance.email_confirm_attempts = 0
                     instance.save()
-                    instance.send_email_confirmation_email(generate_new=True)
-                    instance.send_email_candidate_confirmation_email(generate_new=True)
+                    instance.send_credential_confirmation_code(Credential.EMAIL, candidate=False, generate_new=True)
+                    instance.send_credential_confirmation_code(Credential.EMAIL, candidate=True, generate_new=True)
                 else:
                     instance.email = _email
                     instance.email_confirm_attempts = 0
                     instance.save()
-                    instance.send_email_confirmation_email(generate_new=True)
+                    instance.send_credential_confirmation_code(Credential.EMAIL, generate_new=True)
         for attr, value in validated_data.items():
             if attr in info.relations and info.relations[attr].to_many:
                 field = getattr(instance, attr)
                 field.set(value)
             else:
                 setattr(instance, attr, value)
         instance.save()
         return instance
 
     class Meta:
         model = CustomUser
         fields = [
             'id',
-            'userpic',
             'email',
             'email_candidate',
             'first_name',
             'last_name',
             'phone_number',
             'phone_number_candidate',
             'is_phone_number_confirmed',
@@ -158,14 +167,15 @@
         ]
 
 
 def site_with_domain_exists(value):
     if not Site.objects.filter(domain=value).exists():
         raise serializers.ValidationError(errors.SITE_WITH_DOMAIN_DOES_NOT_EXIST)
 
+
 def validate_phone_number_with_provided_validator(value):
     if not Site.objects.filter(domain=value).exists():
         raise serializers.ValidationError(errors.SITE_WITH_DOMAIN_DOES_NOT_EXIST)
 
 
 class CustomUserCreateSerializer(serializers.ModelSerializer):
     phone_number = serializers.CharField(validators=[moses_settings.PHONE_NUMBER_VALIDATOR])
@@ -213,16 +223,15 @@
             user = self.perform_create(validated_data)
         except IntegrityError as e:
             self.fail('cannot_create_user')
         return user
 
     def perform_create(self, validated_data):
         with transaction.atomic():
-            user = CustomUser.objects.create_user(**validated_data)
-            user.preferred_language = 'en'
+            user = CustomUser.objects.create_user(preferred_language=moses_settings.DEFAULT_LANGUAGE, **validated_data)
         return user
 
 
 class TokenObtainPairSerializer(TokenObtainSerializer):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.fields['otp'] = serializers.CharField(required=False, allow_blank=True, allow_null=True)
@@ -255,7 +264,64 @@
         data = {}
 
         refresh = self.get_token(self.user)
 
         data['refresh'] = str(refresh)
         data['access'] = str(refresh.access_token)
         return data
+
+
+class PasswordSerializer(serializers.Serializer):
+    new_password = serializers.CharField(style={"input_type": "password"})
+
+    def validate(self, attrs):
+        user = getattr(self, "user", None) or self.context["request"].user
+        # why assert? There are ValidationError / fail everywhere
+        assert user is not None
+
+        try:
+            validate_password(attrs["new_password"], user)
+        except django_exceptions.ValidationError as e:
+            raise serializers.ValidationError({"new_password": list(e.messages)})
+        return super().validate(attrs)
+
+
+class ResetPasswordSerializer(serializers.Serializer):
+    credential = serializers.CharField()
+    domain = serializers.CharField()
+
+    def validate(self, attrs):
+        validated_data = super().validate(attrs)
+        try:
+            self.user = CustomUser.objects.get(
+                Q(phone_number=validated_data['credential'], is_phone_number_confirmed=True) | Q(email=validated_data['credential'], is_email_confirmed=True),
+                site__domain=validated_data['domain'],
+            )
+        except (CustomUser.DoesNotExist, ValueError, TypeError, OverflowError):
+            key_error = "code_not_found"
+            raise ValidationError(
+                {"credential": [errors.USER_WITH_PROVIDED_CREDENTIALS_DOES_NOT_REGISTERED_ON_SPECIFIED_DOMAIN]}, code=key_error
+            )
+        return validated_data
+
+
+class ConfirmResetPasswordSerializer(PasswordSerializer):
+    credential = serializers.CharField()
+    domain = serializers.CharField()
+    code = serializers.CharField()
+
+    def validate(self, attrs):
+        validated_data = super().validate(attrs)
+        try:
+            self.user = CustomUser.objects.get(
+                Q(phone_number=validated_data['credential']) | Q(email=validated_data['credential']),
+                site__domain=validated_data['domain'],
+                password_reset_code=validated_data['code'],
+                password_reset_code_sms_sent_at__gte=timezone.now() - timedelta(
+                    minutes=moses_settings.PASSWORD_RESET_TIMEOUT_MINUTES)
+            )
+        except (CustomUser.DoesNotExist, ValueError, TypeError, OverflowError):
+            key_error = "code_not_found"
+            raise ValidationError(
+                {"phone_number": ['code_not_found']}, code=key_error
+            )
+        return validated_data
```

### Comparing `django_moses-0.9.2.2/moses/templates/admin/login.html` & `django_moses-0.9.3/moses/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django_moses-0.9.2.2/moses/urls.py` & `django_moses-0.9.3/moses/urls.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.9.2.2/moses/views/user.py` & `django_moses-0.9.3/moses/views/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 import random
 import string
 
 import pyotp
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Group
 from django.contrib.auth.tokens import default_token_generator
-from django.contrib.sites.models import Site
 from django.core.mail import send_mail
 from django.db.models import Q
-from django.utils import translation, timezone
+from django.utils import translation
 from django.utils.timezone import now
 from django.utils.translation import gettext as _
 from djoser import signals, utils
 from djoser.compat import get_user_email
 from djoser.conf import settings as djoser_settings
-from djoser.utils import logout_user, encode_uid
+from djoser.utils import logout_user
 from rest_framework import status, viewsets
 from rest_framework.decorators import action
 from rest_framework.exceptions import NotFound
 from rest_framework.response import Response
 
 from moses import errors
 from moses.conf import settings as moses_settings
@@ -68,32 +67,14 @@
             self.permission_classes = djoser_settings.PERMISSIONS.set_password
         elif self.action == "destroy" or (
                 self.action == "me" and self.request and self.request.method == "DELETE"
         ):
             self.permission_classes = djoser_settings.PERMISSIONS.user_delete
         return super().get_permissions()
 
-    def send_password_reset_email(self, user):
-        context = {'user': user}
-        to = [get_user_email(user)]
-        if user.is_email_confirmed:
-            with translation.override(user.preferred_language):
-                djoser_settings.EMAIL.password_reset(self.request, context).send(to)
-        else:
-            raise ValueError(_("Email is not confirmed"))
-
-    def send_password_reset_sms(self, user):
-        url = moses_settings.URL_PREFIX + '/' + djoser_settings.PASSWORD_RESET_CONFIRM_URL.format(
-            token=default_token_generator.make_token(user),
-            uid=encode_uid(user.pk)
-        )
-        moses_settings.SEND_SMS_HANDLER(to=user.phone_number, body=url)
-        user.last_password_reset_sms_sent_at = timezone.now()
-        user.save()
-
     def get_serializer_class(self):
         if self.action == "create":
             if djoser_settings.USER_CREATE_PASSWORD_RETYPE:
                 return djoser_settings.SERIALIZERS.user_create_password_retype
             return djoser_settings.SERIALIZERS.user_create
         elif self.action == "destroy" or (
                 self.action == "me" and self.request and self.request.method == "DELETE"
@@ -212,15 +193,18 @@
         djoser_settings.EMAIL.activation(self.request, context).send(to)
 
         return Response(status=status.HTTP_204_NO_CONTENT)
 
     @action(["post"], detail=False)
     def set_password(self, request, *args, **kwargs):
         if not request.user.check_password(request.data.get('current_password')):
-            return Response({'current_password': [errors.INVALID_PASSWORD]}, status=status.HTTP_400_BAD_REQUEST)
+            return Response(
+                {'current_password': [errors.INVALID_PASSWORD]},
+                status=status.HTTP_400_BAD_REQUEST
+            )
 
         self.request.user.set_password(request.data.get('new_password'))
         self.request.user.save()
         with translation.override(self.request.user.preferred_language):
             send_mail(_("Password changed"),
                       _(
                           "Your password has been changed. "
@@ -229,77 +213,18 @@
         if djoser_settings.LOGOUT_ON_PASSWORD_CHANGE:
             logout_user(self.request)
 
         return Response(status=status.HTTP_204_NO_CONTENT)
 
     @action(["post"], detail=False)
     def reset_password(self, request, *args, **kwargs):
-        if not Site.objects.filter(domain=request.data.get('domain')).exists():
-            return Response(
-                {
-                    'domain': [errors.SITE_WITH_DOMAIN_DOES_NOT_EXIST]
-                },
-                status=status.HTTP_400_BAD_REQUEST
-            )
-        if 'email' in request.data:
-            users = CustomUser.objects.filter(
-                site__domain=request.data['domain'],
-                email=request.data['email']
-            )
-            if not users:
-                return Response(
-                    {
-                        'phone_number': [errors.USER_WITH_PROVIDED_CREDENTIALS_DOES_NOT_REGISTERED_ON_SPECIFIED_DOMAIN]
-                    },
-                    status=status.HTTP_400_BAD_REQUEST
-                )
-            for user in users:
-                if user.is_email_confirmed:
-                    self.send_password_reset_email(user)
-                else:
-                    return Response(
-                        {
-                            'email': [errors.CREDENTIAL_NOT_CONFIRMED]
-                        },
-                        status=status.HTTP_400_BAD_REQUEST
-                    )
-
-        if 'phone_number' in request.data:
-            users = CustomUser.objects.filter(
-                site__domain=request.data['domain'],
-                phone_number=request.data['phone_number']
-            )
-            if not users:
-                return Response(
-                    {
-                        'phone_number': [errors.USER_WITH_PROVIDED_CREDENTIALS_DOES_NOT_REGISTERED_ON_SPECIFIED_DOMAIN]
-                    },
-                    status=status.HTTP_400_BAD_REQUEST
-                )
-            for user in users:
-                if user.is_phone_number_confirmed:
-                    if not user.last_password_reset_sms_sent_at or (
-                            timezone.now() - user.last_password_reset_sms_sent_at
-                    ).days > 0:
-                        self.send_password_reset_sms(user)
-                    else:
-                        return Response(
-                            {
-                                'non_field_errors': [errors.TOO_FREQUENT_SMS_REQUESTS]
-                            },
-                            status=status.HTTP_400_BAD_REQUEST
-                        )
-                else:
-                    return Response(
-                        {
-                            'phone_number': [errors.CREDENTIAL_NOT_CONFIRMED]
-                        },
-                        status=status.HTTP_400_BAD_REQUEST
-                    )
-        return Response({}, status=status.HTTP_204_NO_CONTENT)
+        serializer = self.get_serializer(data=request.data)
+        serializer.is_valid(raise_exception=True)
+        serializer.user.send_password_reset_code(serializer.data["credential"])
+        return Response(status=status.HTTP_204_NO_CONTENT)
 
     @action(["post"], detail=False)
     def reset_password_confirm(self, request, *args, **kwargs):
         serializer = self.get_serializer(data=request.data)
         serializer.is_valid(raise_exception=True)
 
         serializer.user.set_password(serializer.data["new_password"])
@@ -417,18 +342,18 @@
             {
                 'success': 'mfa has been successfully disabled'
             }
         )
 
     @action(["post"], detail=False)
     def request_phone_number_confirmation_pin(self, request):
-        if (now() - request.user.last_phone_number_confirmation_pin_sent).days > 0 and \
-                (now() - request.user.last_phone_number_candidate_confirmation_pin_sent).days > 0:
-            request.user.send_phone_number_confirmation_sms()
-            request.user.send_phone_number_candidate_confirmation_sms()
+        if request.user.last_phone_number_confirmation_pins_sent is None or (
+                now() - request.user.last_phone_number_confirmation_pins_sent).seconds >= 60 * moses_settings.PHONE_NUMBER_CONFIRMATION_SMS_MINUTES_PERIOD:
+            request.user.send_credential_confirmation_code(Credential.PHONE_NUMBER)
+            request.user.send_credential_confirmation_code(Credential.PHONE_NUMBER, candidate=True)
             return Response({})
         return Response({'non_field_errors': ['too_frequent_sms_request']}, status=status.HTTP_400_BAD_REQUEST)
 
     @action(["post"], detail=False)
     def request_email_confirmation_pin(self, request):
         request.user.send_email_confirmation_email()
         request.user.send_email_candidate_confirmation_email()
```

### Comparing `django_moses-0.9.2.2/pyproject.toml` & `django_moses-0.9.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "django-moses"
-version = "0.9.2.2"
+version = "0.9.3"
 dependencies = [
     "djangorestframework-simplejwt = ^5.2.2",
     "djoser = ^2.2.0",
     "pyotp = ^2.8.0"
 ]
 
 [tool.poetry]
 name = "django-moses"
 description = "Advanced authentication with OTP and phone number verification"
-version = "0.9.2.2"
+version = "0.9.3"
 authors = ["Vassily Vorobyov <vassily.v.v@gmail.com>"]
 packages = [{ include = "moses/**/*", from = "." }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 django = "^4.2.2"
 djangorestframework-simplejwt = "^5.2.2"
```

### Comparing `django_moses-0.9.2.2/PKG-INFO` & `django_moses-0.9.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-moses
-Version: 0.9.2.2
+Version: 0.9.3
 Summary: Advanced authentication with OTP and phone number verification
 Author: Vassily Vorobyov
 Author-email: vassily.v.v@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

