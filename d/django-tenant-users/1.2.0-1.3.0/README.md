# Comparing `tmp/django_tenant_users-1.2.0.tar.gz` & `tmp/django_tenant_users-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tenant_users-1.2.0.tar", max compression
+gzip compressed data, was "django_tenant_users-1.3.0.tar", max compression
```

## Comparing `django_tenant_users-1.2.0.tar` & `django_tenant_users-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1064 2021-12-15 06:14:26.393392 django_tenant_users-1.2.0/LICENSE
--rw-r--r--   0        0        0    17372 2022-10-01 22:48:09.476925 django_tenant_users-1.2.0/README.rst
--rw-r--r--   0        0        0     2181 2023-08-08 15:40:43.843002 django_tenant_users-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-12-15 06:14:26.399164 django_tenant_users-1.2.0/tenant_users/__init__.py
--rw-r--r--   0        0        0        0 2021-12-15 06:14:26.399250 django_tenant_users-1.2.0/tenant_users/permissions/__init__.py
--rw-r--r--   0        0        0      839 2022-02-10 05:39:20.130746 django_tenant_users-1.2.0/tenant_users/permissions/backend.py
--rw-r--r--   0        0        0      861 2021-12-15 06:14:26.399412 django_tenant_users-1.2.0/tenant_users/permissions/functional.py
--rw-r--r--   0        0        0     3005 2022-10-01 18:55:54.418657 django_tenant_users-1.2.0/tenant_users/permissions/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2021-12-15 06:14:26.399563 django_tenant_users-1.2.0/tenant_users/permissions/migrations/__init__.py
--rw-r--r--   0        0        0     4091 2023-04-05 02:14:52.539281 django_tenant_users-1.2.0/tenant_users/permissions/models.py
--rw-r--r--   0        0        0        0 2023-08-08 15:18:39.704132 django_tenant_users-1.2.0/tenant_users/tenants/__init__.py
--rw-r--r--   0        0        0      246 2022-02-10 05:39:20.132041 django_tenant_users-1.2.0/tenant_users/tenants/apps.py
--rw-r--r--   0        0        0        0 2021-12-15 06:14:26.399927 django_tenant_users-1.2.0/tenant_users/tenants/migrations/__init__.py
--rw-r--r--   0        0        0    13402 2023-04-05 02:14:52.540811 django_tenant_users-1.2.0/tenant_users/tenants/models.py
--rw-r--r--   0        0        0     2478 2022-02-10 05:39:20.132749 django_tenant_users-1.2.0/tenant_users/tenants/tasks.py
--rw-r--r--   0        0        0     1532 2022-02-10 05:39:20.133130 django_tenant_users-1.2.0/tenant_users/tenants/utils.py
--rw-r--r--   0        0        0    18594 1970-01-01 00:00:00.000000 django_tenant_users-1.2.0/setup.py
--rw-r--r--   0        0        0    19039 1970-01-01 00:00:00.000000 django_tenant_users-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-12-17 15:19:01.356625 django_tenant_users-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2832 2023-09-15 20:47:08.781360 django_tenant_users-1.3.0/README.rst
+-rw-r--r--   0        0        0     2351 2023-11-14 23:22:35.165070 django_tenant_users-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-12-17 15:19:01.362917 django_tenant_users-1.3.0/tenant_users/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-17 15:19:01.363033 django_tenant_users-1.3.0/tenant_users/permissions/__init__.py
+-rw-r--r--   0        0        0      839 2023-09-13 14:11:01.837033 django_tenant_users-1.3.0/tenant_users/permissions/backend.py
+-rw-r--r--   0        0        0      861 2023-06-15 14:29:54.544965 django_tenant_users-1.3.0/tenant_users/permissions/functional.py
+-rw-r--r--   0        0        0     3005 2023-09-13 14:11:01.837225 django_tenant_users-1.3.0/tenant_users/permissions/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2021-12-17 15:19:01.363478 django_tenant_users-1.3.0/tenant_users/permissions/migrations/__init__.py
+-rw-r--r--   0        0        0     4091 2023-09-13 14:11:01.837859 django_tenant_users-1.3.0/tenant_users/permissions/models.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:50:20.025905 django_tenant_users-1.3.0/tenant_users/tenants/__init__.py
+-rw-r--r--   0        0        0      246 2023-09-13 21:56:22.327540 django_tenant_users-1.3.0/tenant_users/tenants/apps.py
+-rw-r--r--   0        0        0        0 2021-12-17 15:19:01.364097 django_tenant_users-1.3.0/tenant_users/tenants/migrations/__init__.py
+-rw-r--r--   0        0        0    13402 2023-09-13 20:16:40.945358 django_tenant_users-1.3.0/tenant_users/tenants/models.py
+-rw-r--r--   0        0        0     4773 2023-09-13 14:11:01.838593 django_tenant_users-1.3.0/tenant_users/tenants/tasks.py
+-rw-r--r--   0        0        0     3420 2023-09-15 20:19:25.276605 django_tenant_users-1.3.0/tenant_users/tenants/utils.py
+-rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 django_tenant_users-1.3.0/PKG-INFO
```

### Comparing `django_tenant_users-1.2.0/LICENSE` & `django_tenant_users-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tenant_users-1.2.0/pyproject.toml` & `django_tenant_users-1.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 
 [tool.nitpick]
 style = "https://raw.githubusercontent.com/wemake-services/wemake-python-styleguide/master/styles/nitpick-style-wemake.toml"
 
 
 [tool.black]
 target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
-skip-string-normalization = true
 include = '\.pyi?$'
 
 
 [tool.poetry]
 name = "django-tenant-users"
 description = "A Django app to extend django-tenants to incorporate global multi-tenant users"
-version = "1.2.0"
+version = "1.3.0"
 license = "MIT License"
 
 packages = [
   { include = 'tenant_users' },
 ]
 
 authors = [
@@ -73,20 +72,32 @@
 
 safety = "^2.2"
 
 pytest = "^7.2.2"
 pytest-cov = "^4.0"
 pytest-randomly = "^3.12"
 
-sphinx = "^5.2"
-sphinx-autodoc-typehints = "^1.19"
-doc8 = "^1.0"
-m2r2 = "^0.3"
+doc8 = ">=0.11,<1.2"
+
 tomlkit = ">=0.11,<0.13"
 pytest-django = "^4.5.2"
 black = ">=22.8,<24.0"
 python-decouple = "^3.6"
 psycopg2-binary = "^2.9.6"
 pytest-deadfixtures = "^2.2.1"
 pytest-testmon = ">=1.3.3,<3.0.0"
 pytest-timeout = "^2.1.0"
 hypothesis = "^6.55.0"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+sphinx = ">=5.0,<8.0"
+sphinx-rtd-theme = "^1.3.0"
+sphinx-autodoc-typehints = "^1.19.5"
+m2r2 = "^0.3"
+psycopg2-binary = "^2.9.6"
+tomli = "^2.0.1"
+
+[tool.doc8]
+max-line-length = 88
```

### Comparing `django_tenant_users-1.2.0/tenant_users/permissions/backend.py` & `django_tenant_users-1.3.0/tenant_users/permissions/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,12 +11,12 @@
     The Facade classes handle the magic of passing
     requests to the right spot.
     """
 
     # We override this so that it looks for the 'groups' attribute on the
     # UserTenantPermissions rather than from get_user_model()
     def _get_group_permissions(self, user_obj):
-        user_groups_field = UserTenantPermissions._meta.get_field('groups')
-        user_groups_query = 'group__{0}'.format(
+        user_groups_field = UserTenantPermissions._meta.get_field("groups")
+        user_groups_query = "group__{0}".format(
             user_groups_field.related_query_name(),
         )
         return Permission.objects.filter(**{user_groups_query: user_obj})
```

### Comparing `django_tenant_users-1.2.0/tenant_users/permissions/functional.py` & `django_tenant_users-1.3.0/tenant_users/permissions/functional.py`

 * *Files identical despite different names*

### Comparing `django_tenant_users-1.2.0/tenant_users/permissions/migrations/0001_initial.py` & `django_tenant_users-1.3.0/tenant_users/permissions/migrations/0001_initial.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,79 +9,79 @@
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
-        ('auth', '0008_alter_user_username_max_length'),
+        ("auth", "0008_alter_user_username_max_length"),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='UserTenantPermissions',
+            name="UserTenantPermissions",
             fields=[
                 (
-                    'id',
+                    "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
-                        verbose_name='ID',
+                        verbose_name="ID",
                     ),
                 ),
                 (
-                    'is_superuser',
+                    "is_superuser",
                     models.BooleanField(
                         default=False,
-                        help_text='Designates that this user has all permissions without explicitly assigning them.',
-                        verbose_name='superuser status',
+                        help_text="Designates that this user has all permissions without explicitly assigning them.",
+                        verbose_name="superuser status",
                     ),
                 ),
                 (
-                    'is_staff',
+                    "is_staff",
                     models.BooleanField(
                         default=False,
-                        help_text='Designates whether the user can log into this tenants admin site.',
-                        verbose_name='staff status',
+                        help_text="Designates whether the user can log into this tenants admin site.",
+                        verbose_name="staff status",
                     ),
                 ),
                 (
-                    'groups',
+                    "groups",
                     models.ManyToManyField(
                         blank=True,
-                        help_text='The groups this user belongs to. A user will get all permissions granted to each of their groups.',
-                        related_name='user_set',
-                        related_query_name='user',
-                        to='auth.Group',
-                        verbose_name='groups',
+                        help_text="The groups this user belongs to. A user will get all permissions granted to each of their groups.",
+                        related_name="user_set",
+                        related_query_name="user",
+                        to="auth.Group",
+                        verbose_name="groups",
                     ),
                 ),
                 (
-                    'profile',
+                    "profile",
                     models.OneToOneField(
                         on_delete=django.db.models.deletion.CASCADE,
                         to=settings.AUTH_USER_MODEL,
                     ),
                 ),
                 (
-                    'user_permissions',
+                    "user_permissions",
                     models.ManyToManyField(
                         blank=True,
-                        help_text='Specific permissions for this user.',
-                        related_name='user_set',
-                        related_query_name='user',
-                        to='auth.Permission',
-                        verbose_name='user permissions',
+                        help_text="Specific permissions for this user.",
+                        related_name="user_set",
+                        related_query_name="user",
+                        to="auth.Permission",
+                        verbose_name="user permissions",
                     ),
                 ),
             ],
             options={
-                'abstract': False,
+                "abstract": False,
             },
             bases=(
                 models.Model,
                 tenant_users.permissions.models.AbstractBaseUserFacade,
             ),
         ),
     ]
```

### Comparing `django_tenant_users-1.2.0/tenant_users/permissions/models.py` & `django_tenant_users-1.3.0/tenant_users/permissions/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,28 +107,28 @@
     schema including authentication aspects. See UserProfile model.
     """
 
     id = models.AutoField(
         auto_created=True,
         primary_key=True,
         serialize=False,
-        verbose_name='ID',
+        verbose_name="ID",
     )
 
     # The profile stores all of the common information between
     # tenants for a user
     profile = models.OneToOneField(
         settings.AUTH_USER_MODEL,
         on_delete=models.CASCADE,
     )
 
     is_staff = models.BooleanField(
-        _('staff status'),
+        _("staff status"),
         default=False,
         help_text=_(
-            'Designates whether the user can log into this tenants admin site.',
+            "Designates whether the user can log into this tenants admin site.",
         ),
     )
 
     def __str__(self):
         """Return string representation."""
         return str(self.profile)
```

### Comparing `django_tenant_users-1.2.0/tenant_users/tenants/models.py` & `django_tenant_users-1.3.0/tenant_users/tenants/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     return inner
 
 
 class TenantBase(TenantMixin):
     """Contains global data and settings for the tenant model."""
 
-    slug = models.SlugField(_('Tenant URL Name'), blank=True)
+    slug = models.SlugField(_("Tenant URL Name"), blank=True)
 
     # The owner of the tenant. Only they can delete it. This can be changed,
     # but it can't be blank. There should always be an owner.
     owner = models.ForeignKey(
         settings.AUTH_USER_MODEL,
         on_delete=models.CASCADE,
     )
@@ -82,24 +82,24 @@
 
     def delete(self, force_drop=False, *args, **kwargs):
         """Override deleting of Tenant object."""
         if force_drop:
             super().delete(force_drop, *args, **kwargs)
         else:
             raise DeleteError(
-                'Not supported -- delete_tenant() should be used.',
+                "Not supported -- delete_tenant() should be used.",
             )
 
     @schema_required
     def add_user(self, user_obj, is_superuser=False, is_staff=False):
         """Add user to tenant."""
         # User already is linked here..
         if self.user_set.filter(id=user_obj.pk).exists():
             raise ExistsError(
-                'User already added to tenant: {0}'.format(
+                "User already added to tenant: {0}".format(
                     user_obj,
                 ),
             )
 
         # User not linked to this tenant, so we need to create
         # tenant permissions
         UserTenantPermissions.objects.create(
@@ -122,15 +122,15 @@
         # Test that user is already in the tenant
         self.user_set.get(pk=user_obj.pk)
 
         # Dont allow removing an owner from a tenant. This must be done
         # Through delete tenant or transfer_ownership
         if user_obj.pk == self.owner.pk:
             raise DeleteError(
-                'Cannot remove owner from tenant: {0}'.format(
+                "Cannot remove owner from tenant: {0}".format(
                     self.owner,
                 ),
             )
 
         user_tenant_perms = user_obj.usertenantpermissions
         # Remove all current groups from user..
         groups = user_tenant_perms.groups
@@ -154,26 +154,26 @@
         associate them with a the public schema user and change their url
         to reflect their delete datetime and previous owner
         The caller should verify that the user deleting the tenant owns
         the tenant.
         """
         # Prevent public tenant schema from being deleted
         if self.schema_name == get_public_schema_name():
-            raise ValueError('Cannot delete public tenant schema')
+            raise ValueError("Cannot delete public tenant schema")
 
         for user_obj in self.user_set.all():
             # Don't delete owner at this point
             if user_obj.pk == self.owner.pk:
                 continue
             self.remove_user(user_obj)
 
         # Seconds since epoch, time() returns a float, so we convert to
         # an int first to truncate the decimal portion
         time_string = str(int(time.time()))
-        new_url = '{0}-{1}-{2}'.format(
+        new_url = "{0}-{1}-{2}".format(
             time_string,
             str(self.owner.pk),
             self.domain_url,
         )
         self.domain_url = new_url
         # The schema generated each time (even with same url slug) will
         # be unique so we do not have to worry about a conflict with that
@@ -238,25 +238,25 @@
         # inside a tenant. Must create public tenant permissions during user
         # creation. This happens during assign role. This function cannot be
         # used until a public schema already exists
         UserModel = get_user_model()
 
         if connection.schema_name != get_public_schema_name():
             raise SchemaError(
-                'Schema must be public for UserProfileManager user creation',
+                "Schema must be public for UserProfileManager user creation",
             )
 
         if not email:
-            raise ValueError('Users must have an email address.')
+            raise ValueError("Users must have an email address.")
 
         email = self.normalize_email(email)
 
         profile = UserModel.objects.filter(email=email).first()
         if profile and profile.is_active:
-            raise ExistsError('User already exists!')
+            raise ExistsError("User already exists!")
 
         # Profile might exist but not be active. If a profile does exist
         # all previous history logs will still be associated with the user,
         # but will not be accessible because the user won't be linked to
         # any tenants from the user's previous membership. There are two
         # exceptions to this. 1) The user gets re-invited to a tenant it
         # previously had access to (this is good thing IMO). 2) The public
@@ -324,15 +324,15 @@
     def delete_user(self, user_obj):
         # Check to make sure we don't try to delete the public tenant owner
         # that would be bad....
         public_tenant = get_tenant_model().objects.get(
             schema_name=get_public_schema_name(),
         )
         if user_obj.pk == public_tenant.owner.pk:
-            raise DeleteError('Cannot delete the public tenant owner!')
+            raise DeleteError("Cannot delete the public tenant owner!")
 
         # This includes the linked public tenant 'tenant'. It will delete the
         # Tenant permissions and unlink when user is deleted
         for tenant in user_obj.tenants.all():
             # If user owns the tenant, we call delete on the tenant
             # which will delete the user from the tenant as well
             if tenant.owner.pk == user_obj.pk:
@@ -360,48 +360,48 @@
     where as to allow for one global profile (public schema) for each user
     but maintain permissions on a per tenant basis.
     To access permissions for a user, the request must come through the
     tenant that permissions are desired for.
     Requires use of the ModelBackend
     """
 
-    USERNAME_FIELD = 'email'
+    USERNAME_FIELD = "email"
     objects = UserProfileManager()
 
     tenants = models.ManyToManyField(
         settings.TENANT_MODEL,
-        verbose_name=_('tenants'),
+        verbose_name=_("tenants"),
         blank=True,
-        help_text=_('The tenants this user belongs to.'),
-        related_name='user_set',
+        help_text=_("The tenants this user belongs to."),
+        related_name="user_set",
     )
 
     email = models.EmailField(
-        _('Email Address'),
+        _("Email Address"),
         unique=True,
         db_index=True,
     )
 
-    is_active = models.BooleanField(_('active'), default=True)
+    is_active = models.BooleanField(_("active"), default=True)
 
     # Tracks whether the user's email has been verified
-    is_verified = models.BooleanField(_('verified'), default=False)
+    is_verified = models.BooleanField(_("verified"), default=False)
 
     class Meta(object):
         abstract = True
 
     def has_verified_email(self):
         return self.is_verified
 
     def delete(self, force_drop=False, *args, **kwargs):
         if force_drop:
             super().delete(*args, **kwargs)
         else:
             raise DeleteError(
-                'UserProfile.objects.delete_user() should be used.',
+                "UserProfile.objects.delete_user() should be used.",
             )
 
     def __str__(self):
         return self.email
 
     def get_short_name(self):
         return self.email
```

### Comparing `django_tenant_users-1.2.0/tenant_users/tenants/tasks.py` & `django_tenant_users-1.3.0/tenant_users/tenants/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,101 @@
-import time
-
-from django.conf import settings
 from django.contrib.auth import get_user_model
+from django.db import connection
 from django_tenants.utils import (
+    get_multi_type_database_field_name,
     get_public_schema_name,
     get_tenant_domain_model,
     get_tenant_model,
-    schema_context,
+    get_tenant_types,
+    has_multi_type_tenants,
 )
 
-from tenant_users.tenants.models import ExistsError, InactiveError
+from tenant_users.tenants.models import ExistsError, SchemaError
+
+
+def get_current_tenant():
+    current_schema = connection.schema_name
+    TenantModel = get_tenant_model()
+    tenant = TenantModel.objects.get(schema_name=current_schema)
+    return tenant
+
 
+def create_public_tenant(
+    domain_url,
+    owner_email,
+    is_superuser=False,
+    is_staff=False,
+    tenant_extra_data={},
+    **owner_extra,
+):
+    """Create a public tenant with an owner user.
+
+    `**Creates**` a public tenant in a multi-tenant architecture, `**assigns**` an owner user to it, and `**sets**` the owner's password as unusable if not provided.
+
+    **Args**
+    * `domain_url (str)`: The domain URL for the public tenant.
+    * `owner_email (str)`: The email address of the owner user.
+    * `is_staff`: Whether the user is  allowed to enter the admin panel. Defaults to `False`.
+    * `is_superuser`:Whether the user has all permissions in the respective tenant. Defaults to `True`.
+    * `tenant_extra_data`: Additional attributes for the tenant model (e.g., paid_until, on_trial,location,vision e.t.c).
+    * `owner_extra`: Additional attributes for the owner user (e.g., first_name, last_name).
 
-def provision_tenant(tenant_name, tenant_slug, user_email, is_staff=False):
-    """Create a tenant with default roles and permissions.
+    **Returns:**
 
-    Returns:
-    The FQDN for the tenant.
+    * `Tuple[YourTenantModel, YourDomainModel, YourUserModel]`: A tuple containing the created public tenant, its domain, and the owner user.
     """
-    tenant = None
 
     UserModel = get_user_model()
     TenantModel = get_tenant_model()
+    public_schema_name = get_public_schema_name()
 
-    user = UserModel.objects.get(email=user_email)
-    if not user.is_active:
-        raise InactiveError('Inactive user passed to provision tenant')
+    if TenantModel.objects.filter(schema_name=public_schema_name).first():
+        raise ExistsError("Public tenant already exists")
 
-    if hasattr(settings, 'TENANT_SUBFOLDER_PREFIX'):
-        tenant_domain = tenant_slug
-    else:
-        tenant_domain = '{0}.{1}'.format(tenant_slug, settings.TENANT_USERS_DOMAIN)
-
-    DomainModel = get_tenant_domain_model()
-    if DomainModel.objects.filter(domain=tenant_domain).exists():
-        raise ExistsError('Tenant URL already exists.')
-
-    time_string = str(int(time.time()))
-    # Must be valid postgres schema characters see:
-    # https://www.postgresql.org/docs/9.2/static/sql-syntax-lexical.html#SQL-SYNTAX-IDENTIFIERS
-    # We generate unique schema names each time so we can keep tenants around
-    # without taking up url/schema namespace.
-    schema_name = '{0}_{1}'.format(tenant_slug, time_string)
-    domain = None
-
-    # noinspection PyBroadException
-    try:
-        # Wrap it in public schema context so schema consistency is maintained
-        # if any error occurs
-        with schema_context(get_public_schema_name()):
-            tenant = TenantModel.objects.create(
-                name=tenant_name,
-                slug=tenant_slug,
-                schema_name=schema_name,
-                owner=user,
+    # Create public tenant user. This user doesn't go through object manager
+    # create_user function because public tenant does not exist yet
+    profile = UserModel.objects.create(
+        email=owner_email,
+        is_active=True,
+        **owner_extra,
+    )
+
+    # Create the public tenant
+    if has_multi_type_tenants():
+        valid_tenant_types = get_tenant_types()
+
+        # Check if the Public tenant type is defined
+        if public_schema_name not in valid_tenant_types:
+            error_message = "Please define a '{0}' tenant type.".format(
+                public_schema_name,
             )
+            raise SchemaError(error_message)
 
-            # Add one or more domains for the tenant
-            domain = get_tenant_domain_model().objects.create(
-                domain=tenant_domain,
-                tenant=tenant,
-                is_primary=True,
-            )
-            # Add user as a superuser inside the tenant
-            tenant.add_user(user, is_superuser=True, is_staff=is_staff)
-    except:
-        if domain is not None:
-            domain.delete()
-        if tenant is not None:
-            # Flag is set to auto-drop the schema for the tenant
-            tenant.delete(True)
-        raise
+        tenant_extra_data.update(
+            {get_multi_type_database_field_name(): public_schema_name}
+        )
+
+    public_tenant = TenantModel.objects.create(
+        schema_name=public_schema_name,
+        name="Public Tenant",
+        owner=profile,
+        **tenant_extra_data,
+    )
+
+    # Add one or more domains for the tenant
+    domain = get_tenant_domain_model().objects.create(
+        domain=domain_url,
+        tenant=public_tenant,
+        is_primary=True,
+    )
+
+    # Add system user to public tenant (no permissions)
+    public_tenant.add_user(profile, is_superuser=is_superuser, is_staff=is_staff)
+
+    # Handle setting the password for the user
+    if "password" in owner_extra:
+        profile.set_password(owner_extra["password"])
+    else:
+        profile.set_unusable_password()
+    profile.save()
 
-    return tenant_domain
+    return public_tenant, domain, profile
```

