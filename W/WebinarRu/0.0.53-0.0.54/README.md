# Comparing `tmp/webinarru-0.0.53.tar.gz` & `tmp/webinarru-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webinarru-0.0.53.tar", max compression
+gzip compressed data, was "webinarru-0.0.54.tar", max compression
```

## Comparing `webinarru-0.0.53.tar` & `webinarru-0.0.54.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      935 2023-09-23 05:40:20.990000 webinarru-0.0.53/README.md
--rw-r--r--   0        0        0       58 2023-09-23 09:37:15.780000 webinarru-0.0.53/WebinarRu/__init__.py
--rw-r--r--   0        0        0     5656 2024-03-22 08:25:55.281533 webinarru-0.0.53/WebinarRu/base_api.py
--rw-r--r--   0        0        0    31539 2024-03-25 18:43:37.167585 webinarru-0.0.53/WebinarRu/models.py
--rw-r--r--   0        0        0    60799 2024-04-08 16:00:36.071910 webinarru-0.0.53/WebinarRu/webinar_api.py
--rw-r--r--   0        0        0      515 2024-04-08 16:00:36.020706 webinarru-0.0.53/pyproject.toml
--rw-r--r--   0        0        0     1454 1970-01-01 00:00:00.000000 webinarru-0.0.53/PKG-INFO
+-rw-r--r--   0        0        0      935 2023-09-23 05:40:20.990000 webinarru-0.0.54/README.md
+-rw-r--r--   0        0        0       58 2023-09-23 09:37:15.780000 webinarru-0.0.54/WebinarRu/__init__.py
+-rw-r--r--   0        0        0     5656 2024-03-22 08:25:55.281533 webinarru-0.0.54/WebinarRu/base_api.py
+-rw-r--r--   0        0        0    31561 2024-05-06 09:40:32.544259 webinarru-0.0.54/WebinarRu/models.py
+-rw-r--r--   0        0        0    60799 2024-04-08 16:00:36.071910 webinarru-0.0.54/WebinarRu/webinar_api.py
+-rw-r--r--   0        0        0      515 2024-05-06 09:55:12.800722 webinarru-0.0.54/pyproject.toml
+-rw-r--r--   0        0        0     1454 1970-01-01 00:00:00.000000 webinarru-0.0.54/PKG-INFO
```

### Comparing `webinarru-0.0.53/README.md` & `webinarru-0.0.54/README.md`

 * *Files identical despite different names*

### Comparing `webinarru-0.0.53/WebinarRu/base_api.py` & `webinarru-0.0.54/WebinarRu/base_api.py`

 * *Files identical despite different names*

### Comparing `webinarru-0.0.53/WebinarRu/models.py` & `webinarru-0.0.54/WebinarRu/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     description: Optional[str] = None  # — описание;
     status: Optional[str] = None  # — текущее состояние вебинара;
     accessSettings: Optional[AccessSettings | dict] = None  #
     # - isPasswordRequired — доступ с паролем, или без него
     # - isRegistrationRequired — доступ с регистрацией, или без неё
     # - isModerationRequired — доступ с залом ожидания, или без него
     access: Optional[int] = None  # — (Архивный способ передачи данных) уровень доступа мероприятия;
-    additionalFields: Optional[str | dict] = None  # — информация о дополнительных регистрационных полях;
+    additionalFields: Optional[str | dict | list] = None  # — информация о дополнительных регистрационных полях;
     lang: Optional[str] = None  # — язык интерфейса мероприятия;
     startsAt: Optional[datetime.datetime] = None  # — дата начала мероприятия;
     timezoneId: Optional[int] = None  # — тайм-зона. Параметр в пользовательских сценариях не используется;
     timezone: Optional[str | dict] = None  # — часовой пояс, установленный при создании вебинара;
     endsAt: Optional[datetime.datetime] = None  # — дата завершения мероприятия;
     organizationId: Optional[int] = None  # — идентификатор организации, которой принадлежит мероприятие
     type: Optional[str] = None  # — тип мероприятия. Может быть вебинар, а может быть встречи. Разница в типах
@@ -279,15 +279,15 @@
     mimeType: Optional[str] = None  # — MIME тип файла. В пользовательских сценариях не используется;
     typeFile: Optional[
         Literal['video', 'presentation', 'slide', 'test', 'record', 'ConvertedRecord']
     ] = None  # — тип файла.
     uri: Optional[str] = None  # — uri файла. В пользовательских сценариях не используется;
     thumbnailUri: Optional[str] = None  # — ссылка на миниатюру картинки. В пользовательских сценариях не используется.
 
-    duration: Optional[int] = None  # — длительность видео или теста;
+    duration: Optional[int | float] = None  # — длительность видео или теста;
     description: Optional[str] = None  # — описание. Для видео Yotube/Vimeo:
     src: Optional[str] = None  # — ссылка на видео;
     author: Optional[str] = None  # — имя автора видео;
     authorUrl: Optional[str] = None  # — канал автора на Yotube/Vimeo;
     videoId: Optional[int] = None  # — id видео на Vimeo.
 
     slides: Optional[list | dict] = None  # Набор слайдов. Доступны после конвертации.
@@ -298,15 +298,15 @@
     minAnswers: Optional[int] = None  # минимальное количество ответов, для того чтобы пройти тест;
     minPoints: Optional[int] = None  # минимальное количество баллов;
     assessType: Optional[str] = None  # по какому критерию судить прохождение теста: minAnswers или minPoints;
     contextType: Optional[str] = None  # тест/голосование;
     questions: Optional[list] = None  # вопросы и ответы на них, либо голосование с вариантами ответа;
     testResult: Optional[int] = None  # файл результатов теста.
 
-    cuts: Optional[str] = None  # поле, которое показывает вырезанные отрезки видео в записи.
+    cuts: Optional[str | list] = None  # поле, которое показывает вырезанные отрезки видео в записи.
     # Определяются по полям start – end;
     password: Optional[str] = None  # пароль на запись;
     isViewable: Optional[bool] = None  # открыта ли запись для общего доступа;
     eventSession: Optional[EventSession] = None  # принадлежность вебинару;
     link: Optional[str] = None
     state: Optional[str] = None  # Состояние.
```

### Comparing `webinarru-0.0.53/WebinarRu/webinar_api.py` & `webinarru-0.0.54/WebinarRu/webinar_api.py`

 * *Files identical despite different names*

### Comparing `webinarru-0.0.53/pyproject.toml` & `webinarru-0.0.54/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "WebinarRu"
-version = "0.0.53"
+version = "0.0.54"
 description = "Python client for webinar.ru platform"
 authors = ["gulyaeve <gulyaev.e@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "WebinarRu"}]
 
 [tool.poetry.dependencies]
```

### Comparing `webinarru-0.0.53/PKG-INFO` & `webinarru-0.0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebinarRu
-Version: 0.0.53
+Version: 0.0.54
 Summary: Python client for webinar.ru platform
 License: MIT
 Author: gulyaeve
 Author-email: gulyaev.e@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

