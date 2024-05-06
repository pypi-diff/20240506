# Comparing `tmp/litestar-2.8.2.tar.gz` & `tmp/litestar-2.8.3.tar.gz`

## Comparing `litestar-2.8.2.tar` & `litestar-2.8.3.tar`

### file list

```diff
@@ -1,713 +1,730 @@
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 litestar-2.8.2/Makefile
--rw-r--r--   0        0        0    19851 2020-02-02 00:00:00.000000 litestar-2.8.2/docs/PYPI_README.md
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/__main__.py
--rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_multipart.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_parsers.py
--rw-r--r--   0        0        0    39586 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/app.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/background_tasks.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/concurrency.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/constants.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/controller.py
--rw-r--r--   0        0        0    17681 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/data_extractors.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/di.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/enums.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/file_system.py
--rw-r--r--   0        0        0    11029 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/pagination.py
--rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/py.typed
--rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/router.py
--rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/status_codes.py
--rw-r--r--   0        0        0    25972 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/typing.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_asgi/__init__.py
--rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_asgi/asgi_router.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_asgi/utils.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_asgi/routing_trie/validate.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_kwargs/__init__.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_kwargs/cleanup.py
--rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_kwargs/dependencies.py
--rw-r--r--   0        0        0    16651 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_kwargs/extractors.py
--rw-r--r--   0        0        0    20472 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_layers/__init__.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_layers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/__init__.py
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/datastructures.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/parameters.py
--rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/path_item.py
--rw-r--r--   0        0        0     7836 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/plugin.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/request_body.py
--rw-r--r--   0        0        0    13607 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/responses.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/utils.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/schema_generation/__init__.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/schema_generation/constrained_fields.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/schema_generation/examples.py
--rw-r--r--   0        0        0    25613 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/schema_generation/schema.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/schema_generation/utils.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/schema_generation/plugins/__init__.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/schema_generation/plugins/dataclass.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/schema_generation/plugins/pagination.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/schema_generation/plugins/struct.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/schema_generation/plugins/typed_dict.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_openapi/typescript_converter/types.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_signature/__init__.py
--rw-r--r--   0        0        0    11710 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_signature/model.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_signature/types.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/_signature/utils.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/channels/__init__.py
--rw-r--r--   0        0        0    15848 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/channels/plugin.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/channels/subscriber.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/channels/backends/__init__.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/channels/backends/_redis_flushall_streams.lua
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/channels/backends/_redis_pubsub_publish.lua
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/channels/backends/_redis_xadd_expire.lua
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/channels/backends/asyncpg.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/channels/backends/base.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/channels/backends/memory.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/channels/backends/psycopg.py
--rw-r--r--   0        0        0    11422 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/channels/backends/redis.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/cli/__init__.py
--rw-r--r--   0        0        0    20230 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/cli/_utils.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/cli/commands/__init__.py
--rw-r--r--   0        0        0    12215 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/cli/commands/core.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/cli/commands/schema.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/cli/commands/sessions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/config/__init__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/config/allowed_hosts.py
--rw-r--r--   0        0        0    12477 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/config/app.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/config/compression.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/config/cors.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/config/csrf.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/config/response_cache.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/connection/__init__.py
--rw-r--r--   0        0        0    11536 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/connection/base.py
--rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/connection/request.py
--rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/connection/websocket.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/__init__.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/jinja.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/mako.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/minijinja.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/minijnja.py
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/piccolo.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/attrs/__init__.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/attrs/attrs_schema_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/htmx/_utils.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/htmx/request.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/htmx/response.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/htmx/types.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/jwt/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/jwt/middleware.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/opentelemetry/_utils.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/prometheus/__init__.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/prometheus/config.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/prometheus/controller.py
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/prometheus/middleware.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/pydantic/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/pydantic/config.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/pydantic/pydantic_di_plugin.py
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/pydantic/pydantic_dto_factory.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/pydantic/pydantic_init_plugin.py
--rw-r--r--   0        0        0    13011 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/pydantic/pydantic_schema_plugin.py
--rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/pydantic/utils.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/repository/__init__.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/repository/exceptions.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/repository/filters.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/repository/handlers.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/repository/testing.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/repository/abc/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/base.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/dto.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/types.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/serialization.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/init/__init__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/init/plugin.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/init/config/common.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/init/config/compat.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/repository/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/repository/_async.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/repository/_sync.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/repository/_util.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/contrib/sqlalchemy/repository/types.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/datastructures/__init__.py
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/datastructures/cookie.py
--rw-r--r--   0        0        0    17475 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/datastructures/headers.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/datastructures/multi_dicts.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/datastructures/response_header.py
--rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/datastructures/state.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/datastructures/upload_file.py
--rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/datastructures/url.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/dto/__init__.py
--rw-r--r--   0        0        0    33807 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/dto/_backend.py
--rw-r--r--   0        0        0    22848 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/dto/_codegen_backend.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/dto/_types.py
--rw-r--r--   0        0        0    12845 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/dto/base_dto.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/dto/config.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/dto/data_structures.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/dto/dataclass_dto.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/dto/field.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/dto/msgspec_dto.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/dto/types.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/events/__init__.py
--rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/events/emitter.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/events/listener.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/exceptions/__init__.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/exceptions/base_exceptions.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/exceptions/dto_exceptions.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/handlers/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    23819 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/handlers/base.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    29363 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    65669 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/handlers/websocket_handlers/__init__.py
--rw-r--r--   0        0        0     6182 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/handlers/websocket_handlers/_utils.py
--rw-r--r--   0        0        0    18815 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/handlers/websocket_handlers/listener.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/handlers/websocket_handlers/route_handler.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/logging/__init__.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/logging/_utils.py
--rw-r--r--   0        0        0    18040 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/logging/config.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/logging/picologging.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/logging/standard.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/__init__.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/_utils.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/authentication.py
--rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/base.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/cors.py
--rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/csrf.py
--rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/logging.py
--rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/rate_limit.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/response_cache.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/compression/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/compression/brotli_facade.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/compression/facade.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/compression/gzip_facade.py
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/compression/middleware.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/exceptions/_debug_response.py
--rw-r--r--   0        0        0    11666 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/session/__init__.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/session/base.py
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/session/client_side.py
--rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/middleware/session/server_side.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/__init__.py
--rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/config.py
--rw-r--r--   0        0        0    23353 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/controller.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/datastructures.py
--rw-r--r--   0        0        0    23249 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/plugins.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/__init__.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/base.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/callback.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/components.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/contact.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/discriminator.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/encoding.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/enums.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/example.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/external_documentation.py
--rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/header.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/info.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/license.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/link.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/media_type.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/oauth_flow.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/oauth_flows.py
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/open_api.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/operation.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/parameter.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/path_item.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/paths.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/reference.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/request_body.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/response.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/responses.py
--rw-r--r--   0        0        0    33872 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/schema.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/security_requirement.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/security_scheme.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/server.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/server_variable.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/tag.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/openapi/spec/xml.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/plugins/__init__.py
--rw-r--r--   0        0        0    10975 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/plugins/base.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/plugins/core.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/plugins/flash.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/plugins/sqlalchemy.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/plugins/structlog.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/repository/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/repository/_exceptions.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/repository/_filters.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/repository/exceptions.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/repository/filters.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/repository/handlers.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/repository/abc/__init__.py
--rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/repository/abc/_async.py
--rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/repository/abc/_sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/repository/testing/__init__.py
--rw-r--r--   0        0        0    28346 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/repository/testing/generic_mock_repository.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/response/__init__.py
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/response/base.py
--rw-r--r--   0        0        0    15271 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/response/file.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/response/redirect.py
--rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/response/sse.py
--rw-r--r--   0        0        0     9650 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/response/streaming.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/response/template.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/routes/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/routes/asgi.py
--rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/routes/base.py
--rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/routes/http.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/routes/websocket.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/security/__init__.py
--rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/security/base.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/security/jwt/__init__.py
--rw-r--r--   0        0        0    30453 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/security/jwt/auth.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/security/jwt/middleware.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/security/jwt/token.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/security/session_auth/auth.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/security/session_auth/middleware.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/serialization/__init__.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/serialization/msgspec_hooks.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/static_files/__init__.py
--rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/static_files/base.py
--rw-r--r--   0        0        0     8666 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/static_files/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/stores/__init__.py
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/stores/base.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/stores/file.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/stores/memory.py
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/stores/redis.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/stores/registry.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/template/__init__.py
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/template/base.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/template/config.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/testing/__init__.py
--rw-r--r--   0        0        0    31457 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/testing/helpers.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/testing/life_span_handler.py
--rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/testing/request_factory.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/testing/transport.py
--rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/testing/websocket_test_session.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/testing/client/__init__.py
--rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/testing/client/async_client.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/testing/client/base.py
--rw-r--r--   0        0        0    19967 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/testing/client/sync_client.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/types/__init__.py
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/types/asgi_types.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/types/builtin_types.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/types/callable_types.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/types/composite_types.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/types/empty.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/types/file_types.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/types/helper_types.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/types/internal_types.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/types/protocols.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/types/serialization.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/__init__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/compat.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/dataclass.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/deprecation.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/empty.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/helpers.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/module_loader.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/path.py
--rw-r--r--   0        0        0     9211 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/predicates.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/sequence.py
--rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/signature.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/sync.py
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/typing.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/version.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/warnings.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/scope/__init__.py
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 litestar-2.8.2/litestar/utils/scope/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/__init__.py
--rw-r--r--   0        0        0    10120 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/conftest.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/docker-compose.yml
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/docker_service_fixtures.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/helpers.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/__init__.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_advanced_alchemy.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_exception_handlers.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_option_requests.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_pydantic.py
--rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_response_caching.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_router_registration.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_starlette_responses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_dependency_injection/__init__.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_dependency_injection/test_dependency_validation.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_dependency_injection/test_injection_of_classes.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_dependency_injection/test_inter_dependencies.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_dependency_injection/test_request_local_caching.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_life_cycle_hooks/__init__.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_life_cycle_hooks/test_after_request.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_life_cycle_hooks/test_after_response.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_life_cycle_hooks/test_before_request.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_routing/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_routing/conftest.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_routing/test_asset_url_path.py
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_routing/test_path_mounting.py
--rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_routing/test_path_resolution.py
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_routing/test_route_indexing.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_routing/test_route_reverse.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/e2e/test_routing/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/__init__.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/conftest.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_cache_control_headers.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_exceptions.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_hello_world.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_lifecycle_hooks.py
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_request_data.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_routing.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_signature_namespace.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_startup_and_shutdown.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_static_files.py
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_stores.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_todo_app.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_using_session_auth.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_application_hooks/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_application_hooks/test_application_after_exception_hook.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_application_hooks/test_application_before_send.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_application_hooks/test_lifespan_manager.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_application_hooks/test_on_app_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_application_state/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_application_state/test_passing_initial_state.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_application_state/test_using_application_state.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_application_state/test_using_custom_state.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_application_state/test_using_immutable_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_contrib/__init__.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_contrib/test_piccolo_orm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_contrib/prometheus/__init__.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_contrib/test_sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_contrib/test_sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_dependency_injection/__init__.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_dependency_injection/test_dependency_default_value_no_dependency_fn.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_dependency_injection/test_dependency_default_value_with_dependency_fn.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_dependency_injection/test_dependency_skip_validation.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_dependency_injection/test_dependency_validation_error.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_dependency_injection/tests_dependency_non_optional_not_provided.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_dto/__init__.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_dto/test_example_apps.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_dto/test_tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_middleware/__init__.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_middleware/test_abstract_middleware.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_middleware/test_call_order.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_middleware/test_logging_middleware.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_middleware/test_rate_limit_middleware.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_middleware/test_session_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_openapi/__init__.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_openapi/test_openapi.py
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_openapi/test_plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_pagination/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_pagination/test_using_classic_pagination.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_pagination/test_using_cursor_pagination.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_pagination/test_using_offset_pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_parameters/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_parameters/test_header_and_cookies_parameters.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_parameters/test_layered_parameters.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_parameters/test_path_parameters.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_parameters/test_query_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_plugins/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_plugins/test_di_plugin.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_plugins/test_example_apps.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_responses/__init__.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_responses/test_background_tasks.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_responses/test_custom_responses.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_responses/test_json_suffix_responses.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_responses/test_response_cookies.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_responses/test_response_headers.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_responses/test_returning_responses.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_responses/test_sse_responses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_security/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_security/test_jwt/__init__.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_security/test_jwt/test_using_jwt_auth.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_templating/__init__.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_templating/test_engine_instance.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_templating/test_returning_templates.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/examples/test_templating/test_template_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/__init__.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/conftest.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/piccolo_conf.py
--rw-r--r--   0        0        0    15242 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_app.py
--rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_asgi_router.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_background_tasks.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_concurrency.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_controller.py
--rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_data_extractors.py
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_deprecations.py
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_di.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_events.py
--rw-r--r--   0        0        0     8341 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_exceptions.py
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_file_system.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_guards.py
--rw-r--r--   0        0        0    11592 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_pagination.py
--rw-r--r--   0        0        0    11015 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_params.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_parsers.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_request_class_resolution.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_response_class_resolution.py
--rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_stores.py
--rw-r--r--   0        0        0    17322 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_typing.py
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_websocket_class_resolution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_channels/__init__.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_channels/conftest.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_channels/test_backends.py
--rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_channels/test_plugin.py
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_channels/test_subscriber.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_channels/util.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_cli/__init__.py
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_cli/conftest.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_cli/test_cli.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_cli/test_cli_plugin.py
--rw-r--r--   0        0        0    23147 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_cli/test_core_commands.py
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_cli/test_env_resolution.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_cli/test_schema_commands.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_cli/test_session_commands.py
--rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_cli/test_ssl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_connection/__init__.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_connection/test_base.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_connection/test_connection_caching.py
--rw-r--r--   0        0        0    19442 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_connection/test_request.py
--rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_connection/test_websocket.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/__init__.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/conftest.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_minijinja.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_msgspec.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_opentelemetry.py
--rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_prometheus.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_repository.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_attrs/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_attrs/test_schema_plugin.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_attrs/test_signature.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_htmx/__init__.py
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_htmx/test_htmx_request.py
--rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_htmx/test_htmx_response.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_piccolo_orm/__init__.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_piccolo_orm/endpoints.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_piccolo_orm/tables.py
--rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_pydantic/__init__.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_pydantic/conftest.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_pydantic/models.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_dto.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py
--rw-r--r--   0        0        0    11001 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_integration.py
--rw-r--r--   0        0        0    29005 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_openapi.py
--rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_datastructures/__init_.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_datastructures/test_cookie.py
--rw-r--r--   0        0        0    13358 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_datastructures/test_headers.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_datastructures/test_multi_dicts.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_datastructures/test_response_header.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_datastructures/test_state.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_datastructures/test_upload_file.py
--rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_datastructures/test_url.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/__init__.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/conftest.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_config.py
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_integration.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_interface.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_factory/__init__.py
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_factory/test_base_dto.py
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_factory/test_dataclass_dto.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_factory/test_field.py
--rw-r--r--   0        0        0    30290 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_factory/test_integration.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_factory/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_factory/test_backends/__init__.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_factory/test_backends/conftest.py
--rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_factory/test_backends/test_backends.py
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_dto/test_factory/test_backends/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_asgi_handlers/__init__.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_asgi_handlers/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_base_handlers/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_base_handlers/test_opt.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_base_handlers/test_resolution.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_base_handlers/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/__init__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_defaults.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_delete.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_head.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_media_type.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_sync.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_websocket_handlers/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py
--rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_handlers/test_websocket_handlers/test_validations.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/__init__.py
--rw-r--r--   0        0        0    72895 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/flower.jpeg
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_cleanup_group.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_cookie_params.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_defaults.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_dependency_batches.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_generator_dependencies.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_header_params.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_json_data.py
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_layered_params.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_msgpack_data.py
--rw-r--r--   0        0        0    21924 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_multipart_data.py
--rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_path_params.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_query_params.py
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_reserved_kwargs_injection.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_url_encoded_data.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_kwargs/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_logging/__init__.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_logging/test_logging_config.py
--rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_logging/test_structlog_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/__init__.py
--rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_allowed_hosts_middleware.py
--rw-r--r--   0        0        0     8644 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_base_authentication_middleware.py
--rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_base_middleware.py
--rw-r--r--   0        0        0    11412 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_compression_middleware.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_cors_middleware.py
--rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_csrf_middleware.py
--rw-r--r--   0        0        0    14919 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_exception_handler_middleware.py
--rw-r--r--   0        0        0    12163 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_logging_middleware.py
--rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_middleware_handling.py
--rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_rate_limit_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_session/__init__.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_session/conftest.py
--rw-r--r--   0        0        0     8354 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_session/test_client_side_backend.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_session/test_integration.py
--rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_session/test_middleware.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_middleware/test_session/test_server_side_backend.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/__init__.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/conftest.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_constrained_fields.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_datastructures.py
--rw-r--r--   0        0        0    20213 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_endpoints.py
--rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_integration.py
--rw-r--r--   0        0        0    13925 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_parameters.py
--rw-r--r--   0        0        0     9934 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_path_item.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_render_plugins.py
--rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_request_body.py
--rw-r--r--   0        0        0    20422 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_responses.py
--rw-r--r--   0        0        0    22306 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_schema.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_security_schemes.py
--rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_spec_generation.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_tags.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_typescript_converter/__init__.py
--rw-r--r--   0        0        0     8625 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_typescript_converter/test_converter.py
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_plugins/__init__.py
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_plugins/test_base.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_plugins/test_flash.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_plugins/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_repository/__init__.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_repository/models_bigint.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_repository/models_uuid.py
--rw-r--r--   0        0        0    18932 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_repository/test_generic_mock_repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_response/__init__.py
--rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_response/test_base_response.py
--rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_response/test_file_response.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_response/test_redirect_response.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_response/test_response_cookies.py
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_response/test_response_headers.py
--rw-r--r--   0        0        0    16365 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_response/test_response_to_asgi_response.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_response/test_serialization.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_response/test_sse.py
--rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_response/test_streaming_response.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_response/test_type_decoders.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_response/test_type_encoders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_security/__init__.py
--rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_security/test_security.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_security/test_session_auth.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_security/test_jwt/__init__.py
--rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_security/test_jwt/test_auth.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_security/test_jwt/test_integration.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_security/test_jwt/test_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_signature/__init__.py
--rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_signature/test_parsing.py
--rw-r--r--   0        0        0     9475 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_signature/test_validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_static_files/__init__.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_static_files/conftest.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_static_files/test_create_static_router.py
--rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_static_files/test_file_serving_resolution.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_static_files/test_html_mode.py
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_static_files/test_static_files_validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_template/__init__.py
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_template/test_built_in.py
--rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_template/test_builtin_functions.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_template/test_config.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_template/test_context.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_template/test_csrf_token.py
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_template/test_template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_testing/__init__.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_testing/test_lifespan_handler.py
--rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_testing/test_request_factory.py
--rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_testing/test_test_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_types/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_types/test_protocols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/test_compat.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/test_dataclass.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/test_deprecation.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/test_helpers.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/test_module_loader.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/test_path.py
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/test_predicates.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/test_scope.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/test_sequence.py
--rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/test_signature.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/test_sync.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/test_typing.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 litestar-2.8.2/tests/unit/test_utils/test_version.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 litestar-2.8.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 litestar-2.8.2/LICENSE
--rw-r--r--   0        0        0    92575 2020-02-02 00:00:00.000000 litestar-2.8.2/README.md
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 litestar-2.8.2/pyproject.toml
--rw-r--r--   0        0        0    97593 2020-02-02 00:00:00.000000 litestar-2.8.2/PKG-INFO
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 litestar-2.8.3/Makefile
+-rw-r--r--   0        0        0    19832 2020-02-02 00:00:00.000000 litestar-2.8.3/docs/PYPI_README.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/__main__.py
+-rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_multipart.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_parsers.py
+-rw-r--r--   0        0        0    39586 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/app.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/background_tasks.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/concurrency.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/constants.py
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/controller.py
+-rw-r--r--   0        0        0    17681 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/data_extractors.py
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/di.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/enums.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/file_system.py
+-rw-r--r--   0        0        0    11029 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/pagination.py
+-rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/py.typed
+-rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/router.py
+-rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/status_codes.py
+-rw-r--r--   0        0        0    25806 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/typing.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/__init__.py
+-rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/asgi_router.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/utils.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_kwargs/extractors.py
+-rw-r--r--   0        0        0    20472 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_layers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/__init__.py
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/datastructures.py
+-rw-r--r--   0        0        0    10822 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/parameters.py
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/path_item.py
+-rw-r--r--   0        0        0     7836 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/plugin.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/request_body.py
+-rw-r--r--   0        0        0    13607 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/responses.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/utils.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    25613 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/utils.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/plugins/__init__.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/plugins/dataclass.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/plugins/pagination.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/plugins/struct.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/schema_generation/plugins/typed_dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_signature/__init__.py
+-rw-r--r--   0        0        0    11710 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_signature/model.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_signature/types.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/_signature/utils.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/__init__.py
+-rw-r--r--   0        0        0    15848 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/plugin.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/subscriber.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/__init__.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/_redis_flushall_streams.lua
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/_redis_pubsub_publish.lua
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/_redis_xadd_expire.lua
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/asyncpg.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/base.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/memory.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/psycopg.py
+-rw-r--r--   0        0        0    11422 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/channels/backends/redis.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/__init__.py
+-rw-r--r--   0        0        0    20230 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/_utils.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/commands/__init__.py
+-rw-r--r--   0        0        0    12215 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/commands/core.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/commands/schema.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/cli/commands/sessions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/__init__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/allowed_hosts.py
+-rw-r--r--   0        0        0    12477 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/app.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/compression.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/cors.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/csrf.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/connection/__init__.py
+-rw-r--r--   0        0        0    11536 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/connection/base.py
+-rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/connection/request.py
+-rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/connection/websocket.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/__init__.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/jinja.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/mako.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/minijinja.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/minijnja.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/piccolo.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/attrs/__init__.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/attrs/attrs_schema_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/htmx/request.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/htmx/types.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/prometheus/__init__.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/prometheus/config.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/prometheus/controller.py
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/prometheus/middleware.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/config.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/pydantic_di_plugin.py
+-rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/pydantic_dto_factory.py
+-rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/pydantic_init_plugin.py
+-rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/pydantic_schema_plugin.py
+-rw-r--r--   0        0        0     8064 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/pydantic/utils.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/repository/__init__.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/repository/filters.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/repository/handlers.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/repository/testing.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/repository/abc/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/types.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/serialization.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/plugin.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/common.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/compat.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/repository/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/repository/_async.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/repository/_sync.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/repository/_util.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/contrib/sqlalchemy/repository/types.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/__init__.py
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/cookie.py
+-rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/headers.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/response_header.py
+-rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/state.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/datastructures/url.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/__init__.py
+-rw-r--r--   0        0        0    33807 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/_backend.py
+-rw-r--r--   0        0        0    22848 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/_codegen_backend.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/_types.py
+-rw-r--r--   0        0        0    14087 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/base_dto.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/config.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/data_structures.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/dataclass_dto.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/field.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/msgspec_dto.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/dto/types.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/events/__init__.py
+-rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/events/emitter.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/events/listener.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/exceptions/__init__.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/exceptions/dto_exceptions.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    23819 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/base.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    29363 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    65669 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     6182 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/websocket_handlers/_utils.py
+-rw-r--r--   0        0        0    18815 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/websocket_handlers/listener.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/handlers/websocket_handlers/route_handler.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/logging/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/logging/_utils.py
+-rw-r--r--   0        0        0    18153 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/logging/config.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/logging/picologging.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/logging/standard.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/__init__.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/_utils.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/authentication.py
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/base.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/cors.py
+-rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/csrf.py
+-rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/logging.py
+-rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/rate_limit.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/response_cache.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/compression/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/compression/brotli_facade.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/compression/facade.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/compression/gzip_facade.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/compression/middleware.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0    11666 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/templates/body.html
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/templates/frame.html
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/exceptions/templates/styles.css
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/session/__init__.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/session/base.py
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/session/client_side.py
+-rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/middleware/session/server_side.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/__init__.py
+-rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/config.py
+-rw-r--r--   0        0        0    23353 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/controller.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/datastructures.py
+-rw-r--r--   0        0        0    23249 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/plugins.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/info.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/responses.py
+-rw-r--r--   0        0        0    33872 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/openapi/spec/xml.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/plugins/__init__.py
+-rw-r--r--   0        0        0    10975 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/plugins/base.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/plugins/core.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/plugins/flash.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/plugins/sqlalchemy.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/plugins/structlog.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/_exceptions.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/_filters.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/exceptions.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/filters.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/handlers.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/abc/__init__.py
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/abc/_async.py
+-rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/abc/_sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/testing/__init__.py
+-rw-r--r--   0        0        0    28346 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/__init__.py
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/base.py
+-rw-r--r--   0        0        0    15271 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/file.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/redirect.py
+-rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/sse.py
+-rw-r--r--   0        0        0     9650 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/streaming.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/response/template.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/routes/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/routes/asgi.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/routes/base.py
+-rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/routes/http.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/routes/websocket.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/__init__.py
+-rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/base.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/jwt/__init__.py
+-rw-r--r--   0        0        0    30453 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/jwt/auth.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/jwt/middleware.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/jwt/token.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/session_auth/auth.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/security/session_auth/middleware.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/serialization/__init__.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/serialization/msgspec_hooks.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/static_files/__init__.py
+-rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/static_files/base.py
+-rw-r--r--   0        0        0     8666 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/static_files/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/stores/__init__.py
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/stores/base.py
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/stores/file.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/stores/memory.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/stores/redis.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/stores/registry.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/template/__init__.py
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/template/base.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/template/config.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/__init__.py
+-rw-r--r--   0        0        0    31457 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/helpers.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/life_span_handler.py
+-rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/request_factory.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/transport.py
+-rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/client/__init__.py
+-rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/client/async_client.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/client/base.py
+-rw-r--r--   0        0        0    19967 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/testing/client/sync_client.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/__init__.py
+-rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/asgi_types.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/builtin_types.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/callable_types.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/composite_types.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/empty.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/file_types.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/helper_types.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/internal_types.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/protocols.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/types/serialization.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/__init__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/compat.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/dataclass.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/deprecation.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/empty.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/helpers.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/module_loader.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/path.py
+-rw-r--r--   0        0        0     9211 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/predicates.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/sequence.py
+-rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/signature.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/sync.py
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/typing.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/version.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/warnings.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/scope/__init__.py
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 litestar-2.8.3/litestar/utils/scope/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/__init__.py
+-rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/conftest.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/docker-compose.yml
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/docker_service_fixtures.py
+-rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/helpers.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/__init__.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_advanced_alchemy.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_exception_handlers.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_option_requests.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_pydantic.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_regular_handler_under_asgi_mount_path.py
+-rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_response_caching.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_router_registration.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_starlette_responses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/__init__.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_dependency_validation.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_injection_of_classes.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_inter_dependencies.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_request_local_caching.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_life_cycle_hooks/__init__.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_life_cycle_hooks/test_after_request.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_life_cycle_hooks/test_after_response.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_life_cycle_hooks/test_before_request.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_logging/__init__.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_logging/test_structlog_to_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_middleware/__init__.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_middleware/test_middleware_send_wrapper_called_on_error.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_openapi/__init__.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_openapi/test_spec_headers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/conftest.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/test_asset_url_path.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/test_path_mounting.py
+-rw-r--r--   0        0        0    14279 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/test_path_resolution.py
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/test_route_indexing.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/test_route_reverse.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/e2e/test_routing/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/__init__.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/conftest.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_cache_control_headers.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_exceptions.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_hello_world.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_lifecycle_hooks.py
+-rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_request_data.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_routing.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_signature_namespace.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_startup_and_shutdown.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_static_files.py
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_stores.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_todo_app.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_using_session_auth.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_hooks/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_hooks/test_application_after_exception_hook.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_hooks/test_application_before_send.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_hooks/test_lifespan_manager.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_hooks/test_on_app_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_state/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_state/test_passing_initial_state.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_state/test_using_application_state.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_state/test_using_custom_state.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_application_state/test_using_immutable_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/__init__.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/test_piccolo_orm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/prometheus/__init__.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/test_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/test_sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/conftest.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_defining_dtos_on_layers.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_overriding_implicit_return_dto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/test_dto_data_problem_statement.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/test_dto_data_usage.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/test_leading_underscore_private.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/test_leading_underscore_private_override.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_data_transfer_objects/test_factory/test_type_checking.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dependency_injection/__init__.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dependency_injection/test_dependency_default_value_no_dependency_fn.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dependency_injection/test_dependency_default_value_with_dependency_fn.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dependency_injection/test_dependency_skip_validation.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dependency_injection/test_dependency_validation_error.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dependency_injection/tests_dependency_non_optional_not_provided.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dto/__init__.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dto/test_example_apps.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_dto/test_tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_middleware/__init__.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_middleware/test_abstract_middleware.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_middleware/test_call_order.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_middleware/test_logging_middleware.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_middleware/test_rate_limit_middleware.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_middleware/test_session_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_openapi/__init__.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_openapi/test_openapi.py
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_openapi/test_plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_pagination/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_pagination/test_using_classic_pagination.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_pagination/test_using_cursor_pagination.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_pagination/test_using_offset_pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_parameters/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_parameters/test_header_and_cookies_parameters.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_parameters/test_layered_parameters.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_parameters/test_path_parameters.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_parameters/test_query_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_plugins/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_plugins/test_di_plugin.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_plugins/test_example_apps.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/__init__.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_background_tasks.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_custom_responses.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_json_suffix_responses.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_response_cookies.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_response_headers.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_returning_responses.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_responses/test_sse_responses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_security/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_security/test_jwt/__init__.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_security/test_jwt/test_using_jwt_auth.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_templating/__init__.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_templating/test_engine_instance.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_templating/test_returning_templates.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/examples/test_templating/test_template_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/conftest.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/piccolo_conf.py
+-rw-r--r--   0        0        0    15242 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_app.py
+-rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_asgi_router.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_background_tasks.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_concurrency.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_controller.py
+-rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_data_extractors.py
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_deprecations.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_di.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_events.py
+-rw-r--r--   0        0        0     8341 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_exceptions.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_file_system.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_guards.py
+-rw-r--r--   0        0        0    11592 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_pagination.py
+-rw-r--r--   0        0        0    11015 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_params.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_parsers.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_request_class_resolution.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response_class_resolution.py
+-rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_stores.py
+-rw-r--r--   0        0        0    17777 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_typing.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_websocket_class_resolution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_channels/__init__.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_channels/conftest.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_channels/test_backends.py
+-rw-r--r--   0        0        0    16494 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_channels/test_plugin.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_channels/test_subscriber.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_channels/util.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/__init__.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/conftest.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_cli.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_cli_plugin.py
+-rw-r--r--   0        0        0    23082 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_core_commands.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_env_resolution.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_schema_commands.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_session_commands.py
+-rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_cli/test_ssl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_connection/__init__.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_connection/test_base.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_connection/test_connection_caching.py
+-rw-r--r--   0        0        0    19442 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_connection/test_request.py
+-rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_connection/test_websocket.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/__init__.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/conftest.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_minijinja.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_msgspec.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_opentelemetry.py
+-rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_prometheus.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_repository.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_attrs/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_schema_plugin.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_signature.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_htmx/__init__.py
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_htmx/test_htmx_request.py
+-rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_htmx/test_htmx_response.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/__init__.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/endpoints.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/tables.py
+-rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/conftest.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/models.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_dto.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py
+-rw-r--r--   0        0        0    11001 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_integration.py
+-rw-r--r--   0        0        0    29635 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_openapi.py
+-rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/__init_.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_cookie.py
+-rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_headers.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_multi_dicts.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_response_header.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_state.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_upload_file.py
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_datastructures/test_url.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/__init__.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/conftest.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_config.py
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_integration.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_interface.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/__init__.py
+-rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_base_dto.py
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_dataclass_dto.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_field.py
+-rw-r--r--   0        0        0    33747 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_integration.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/__init__.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/conftest.py
+-rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/test_backends.py
+-rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/__init__.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/test_opt.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/test_resolution.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/__init__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_defaults.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_delete.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_head.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_media_type.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_sync.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py
+-rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_validations.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/__init__.py
+-rw-r--r--   0        0        0    72895 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/flower.jpeg
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_cleanup_group.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_cookie_params.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_defaults.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_dependency_batches.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_generator_dependencies.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_header_params.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_json_data.py
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_layered_params.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_msgpack_data.py
+-rw-r--r--   0        0        0    22582 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_multipart_data.py
+-rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_path_params.py
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_query_params.py
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_reserved_kwargs_injection.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_url_encoded_data.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_kwargs/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_logging/__init__.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_logging/test_logging_config.py
+-rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_logging/test_structlog_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/__init__.py
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_allowed_hosts_middleware.py
+-rw-r--r--   0        0        0     8644 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_base_authentication_middleware.py
+-rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_base_middleware.py
+-rw-r--r--   0        0        0    11412 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_compression_middleware.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_cors_middleware.py
+-rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_csrf_middleware.py
+-rw-r--r--   0        0        0    14919 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_exception_handler_middleware.py
+-rw-r--r--   0        0        0    12163 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_logging_middleware.py
+-rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_middleware_handling.py
+-rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_rate_limit_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_session/__init__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_session/conftest.py
+-rw-r--r--   0        0        0     9883 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_session/test_client_side_backend.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_session/test_integration.py
+-rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_session/test_middleware.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_middleware/test_session/test_server_side_backend.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/__init__.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/conftest.py
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_constrained_fields.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_datastructures.py
+-rw-r--r--   0        0        0    20213 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_endpoints.py
+-rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_integration.py
+-rw-r--r--   0        0        0    13925 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_parameters.py
+-rw-r--r--   0        0        0     9934 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_path_item.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_render_plugins.py
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_request_body.py
+-rw-r--r--   0        0        0    20422 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_responses.py
+-rw-r--r--   0        0        0    22895 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_schema.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_security_schemes.py
+-rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_spec_generation.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_tags.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/__init__.py
+-rw-r--r--   0        0        0     8625 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/test_converter.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_plugins/__init__.py
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_plugins/test_base.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_plugins/test_flash.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_plugins/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_repository/__init__.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_repository/models_bigint.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_repository/models_uuid.py
+-rw-r--r--   0        0        0    18932 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_repository/test_generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/__init__.py
+-rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_base_response.py
+-rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_file_response.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_redirect_response.py
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_response_cookies.py
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_response_headers.py
+-rw-r--r--   0        0        0    16365 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_response_to_asgi_response.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_serialization.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_sse.py
+-rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_streaming_response.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_type_decoders.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_response/test_type_encoders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/__init__.py
+-rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/test_security.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/test_session_auth.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/test_jwt/__init__.py
+-rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/test_jwt/test_auth.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/test_jwt/test_integration.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_security/test_jwt/test_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_signature/__init__.py
+-rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_signature/test_parsing.py
+-rw-r--r--   0        0        0     9475 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_signature/test_validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_static_files/__init__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_static_files/conftest.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_static_files/test_create_static_router.py
+-rw-r--r--   0        0        0    12804 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_static_files/test_file_serving_resolution.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_static_files/test_html_mode.py
+-rw-r--r--   0        0        0     5932 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_static_files/test_static_files_validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/__init__.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/test_built_in.py
+-rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/test_builtin_functions.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/test_config.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/test_context.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/test_csrf_token.py
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_template/test_template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_testing/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_testing/test_lifespan_handler.py
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_testing/test_request_factory.py
+-rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_testing/test_test_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_types/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_types/test_protocols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_compat.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_dataclass.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_deprecation.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_helpers.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_module_loader.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_path.py
+-rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_predicates.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_scope.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_sequence.py
+-rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_signature.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_sync.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_typing.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 litestar-2.8.3/tests/unit/test_utils/test_version.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 litestar-2.8.3/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 litestar-2.8.3/LICENSE
+-rw-r--r--   0        0        0    93354 2020-02-02 00:00:00.000000 litestar-2.8.3/README.md
+-rw-r--r--   0        0        0    12992 2020-02-02 00:00:00.000000 litestar-2.8.3/pyproject.toml
+-rw-r--r--   0        0        0    99274 2020-02-02 00:00:00.000000 litestar-2.8.3/PKG-INFO
```

### Comparing `litestar-2.8.2/Makefile` & `litestar-2.8.3/Makefile`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/docs/PYPI_README.md` & `litestar-2.8.3/docs/PYPI_README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 <!-- prettier-ignore-start -->
 
 | Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 |-----------|:----|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | CI/CD     |     | [![Latest Release](https://github.com/litestar-org/litestar/actions/workflows/publish.yml/badge.svg)](https://github.com/litestar-org/litestar/actions/workflows/publish.yml) [![ci](https://github.com/litestar-org/litestar/actions/workflows/ci.yml/badge.svg)](https://github.com/litestar-org/litestar/actions/workflows/ci.yml) [![Documentation Building](https://github.com/litestar-org/litestar/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/litestar-org/litestar/actions/workflows/docs.yml)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 | Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/litestar/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/litestar) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)                                                                                                                                                                                                                                                                                                                               |
 | Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/litestar?labelColor=202235&color=edb641&logo=python&logoColor=edb641)](https://badge.fury.io/py/litestar) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/litestar?labelColor=202235&color=edb641&logo=python&logoColor=edb641) ![Starlite PyPI - Downloads](https://img.shields.io/pypi/dm/starlite?logo=python&label=starlite%20downloads&labelColor=202235&color=edb641&logoColor=edb641) ![Litestar PyPI - Downloads](https://img.shields.io/pypi/dm/litestar?logo=python&label=litestar%20downloads&labelColor=202235&color=edb641&logoColor=edb641)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
-| Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar-919193495116337154) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
+| Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
 | Meta      |     | [![Litestar Project](https://img.shields.io/badge/Litestar%20Org-%E2%AD%90%20Litestar-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/litestar-org/litestar) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://spdx.org/licenses/) [![Litestar Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23edb641.svg?&logo=github&logoColor=edb641&labelColor=202235)](https://github.com/sponsors/litestar-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=202235)](https://github.com/astral-sh/ruff) [![code style - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/format.json&labelColor=202235)](https://github.com/psf/black) [![All Contributors](https://img.shields.io/github/all-contributors/litestar-org/litestar?labelColor=202235&color=edb641&logoColor=edb641)](#contributors-) |
 
 <!-- prettier-ignore-end -->
 </div>
 
 <hr>
```

### Comparing `litestar-2.8.2/litestar/__init__.py` & `litestar-2.8.3/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_multipart.py` & `litestar-2.8.3/litestar/_multipart.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_parsers.py` & `litestar-2.8.3/litestar/_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/app.py` & `litestar-2.8.3/litestar/app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/background_tasks.py` & `litestar-2.8.3/litestar/background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/concurrency.py` & `litestar-2.8.3/litestar/concurrency.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/constants.py` & `litestar-2.8.3/litestar/constants.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/controller.py` & `litestar-2.8.3/litestar/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/data_extractors.py` & `litestar-2.8.3/litestar/data_extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/di.py` & `litestar-2.8.3/litestar/di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/enums.py` & `litestar-2.8.3/litestar/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/file_system.py` & `litestar-2.8.3/litestar/file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/pagination.py` & `litestar-2.8.3/litestar/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/params.py` & `litestar-2.8.3/litestar/params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/router.py` & `litestar-2.8.3/litestar/router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/status_codes.py` & `litestar-2.8.3/litestar/status_codes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/typing.py` & `litestar-2.8.3/litestar/typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,32 +508,30 @@
         origin = get_origin(unwrapped)
 
         args = () if origin is abc.Callable else get_args(unwrapped)
 
         if not kwargs.get("kwarg_definition"):
             if isinstance(kwargs.get("default"), (KwargDefinition, DependencyKwarg)):
                 kwargs["kwarg_definition"] = kwargs.pop("default")
-            elif any(isinstance(v, (KwargDefinition, DependencyKwarg)) for v in metadata):
-                kwarg_definition = kwargs["kwarg_definition"] = next(  # pragma: no cover
-                    # see https://github.com/nedbat/coveragepy/issues/475
-                    v
-                    for v in metadata
-                    if isinstance(v, (KwargDefinition, DependencyKwarg))
-                )
+            elif kwarg_definition := next(
+                (v for v in metadata if isinstance(v, (KwargDefinition, DependencyKwarg))), None
+            ):
+                kwargs["kwarg_definition"] = kwarg_definition
+
                 if kwarg_definition.default is not Empty:
                     warnings.warn(
                         f"Deprecated default value specification for annotation '{annotation}'. Setting defaults "
                         f"inside 'typing.Annotated' is discouraged and support for this will be removed in a future "
                         f"version. Defaults should be set with regular parameter default values. Use "
                         "'param: Annotated[<type>, Parameter(...)] = <default>' instead of "
                         "'param: Annotated[<type>, Parameter(..., default=<default>)].",
                         category=DeprecationWarning,
                         stacklevel=2,
                     )
-                    if "default" in kwargs and kwarg_definition.default != kwargs["default"]:
+                    if kwargs.get("default", Empty) is not Empty and kwarg_definition.default != kwargs["default"]:
                         warnings.warn(
                             f"Ambiguous default values for annotation '{annotation}'. The default value "
                             f"'{kwarg_definition.default!r}' set inside the parameter annotation differs from the "
                             f"parameter default value '{kwargs['default']!r}'",
                             category=LitestarWarning,
                             stacklevel=2,
                         )
```

### Comparing `litestar-2.8.2/litestar/_asgi/asgi_router.py` & `litestar-2.8.3/litestar/_asgi/asgi_router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_asgi/utils.py` & `litestar-2.8.3/litestar/_asgi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_asgi/routing_trie/mapping.py` & `litestar-2.8.3/litestar/_asgi/routing_trie/mapping.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_asgi/routing_trie/traversal.py` & `litestar-2.8.3/litestar/_asgi/routing_trie/traversal.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,16 +138,20 @@
 
         if mount_paths_regex and (match := mount_paths_regex.search(path)):
             mount_path = path[match.start() : match.end()]
             mount_node = mount_routes[mount_path]
             remaining_path = path[match.end() :]
             # since we allow regular handlers under static paths, we must validate that the request does not match
             # any such handler.
-            children = [sub_route for sub_route in mount_node.children or [] if sub_route != mount_path]
-            if not children or all(sub_route not in path for sub_route in children):  # type: ignore[operator]
+            children = (
+                normalize_path(sub_route)
+                for sub_route in mount_node.children or []
+                if sub_route != mount_path and isinstance(sub_route, str)
+            )
+            if not any(remaining_path.startswith(f"{sub_route}/") for sub_route in children):
                 asgi_app, handler = parse_node_handlers(node=mount_node, method=method)
                 remaining_path = remaining_path or "/"
                 if not mount_node.is_static:
                     remaining_path = remaining_path if remaining_path.endswith("/") else f"{remaining_path}/"
                 return asgi_app, handler, remaining_path, {}
 
         node, path_parameters, path = traverse_route_map(
```

### Comparing `litestar-2.8.2/litestar/_asgi/routing_trie/types.py` & `litestar-2.8.3/litestar/_asgi/routing_trie/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_asgi/routing_trie/validate.py` & `litestar-2.8.3/litestar/_asgi/routing_trie/validate.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_kwargs/cleanup.py` & `litestar-2.8.3/litestar/_kwargs/cleanup.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_kwargs/dependencies.py` & `litestar-2.8.3/litestar/_kwargs/dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_kwargs/extractors.py` & `litestar-2.8.3/litestar/_kwargs/extractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from litestar.datastructures import Headers
 from litestar.datastructures.upload_file import UploadFile
 from litestar.datastructures.url import URL
 from litestar.enums import ParamType, RequestEncodingType
 from litestar.exceptions import ValidationException
 from litestar.params import BodyKwarg
 from litestar.types import Empty
-from litestar.utils.predicates import is_non_string_sequence
+from litestar.utils import make_non_optional_union
+from litestar.utils.predicates import is_non_string_sequence, is_optional_union
 from litestar.utils.scope.state import ScopeState
 
 if TYPE_CHECKING:
     from litestar._kwargs import KwargsModel
     from litestar._kwargs.parameter_definition import ParameterDefinition
     from litestar.connection import ASGIConnection, Request
     from litestar.dto import AbstractDTO
@@ -344,15 +345,18 @@
             multipart_form_part_limit=multipart_form_part_limit,
             type_decoders=connection.route_handler.resolve_type_decoders(),
         )
     )
 
     if field_definition.is_non_string_sequence:
         values = list(form_values.values())
-        if field_definition.has_inner_subclass_of(UploadFile) and isinstance(values[0], list):
+        if isinstance(values[0], list) and (
+            field_definition.has_inner_subclass_of(UploadFile)
+            or (field_definition.is_optional and field_definition.inner_types[0].is_non_string_sequence)
+        ):
             return values[0]
 
         return values
 
     if field_definition.is_simple_type and field_definition.annotation is UploadFile and form_values:
         return next(v for v in form_values.values() if isinstance(v, UploadFile))
 
@@ -360,15 +364,22 @@
         return None
 
     if data_dto:
         return data_dto(connection).decode_builtins(form_values)
 
     for name, tp in field_definition.get_type_hints().items():
         value = form_values.get(name)
-        if value is not None and is_non_string_sequence(tp) and not isinstance(value, list):
+        if (
+            value is not None
+            and not isinstance(value, list)
+            and (
+                is_non_string_sequence(tp)
+                or (is_optional_union(tp) and is_non_string_sequence(make_non_optional_union(tp)))
+            )
+        ):
             form_values[name] = [value]
 
     return form_values
 
 
 def create_multipart_extractor(
     field_definition: FieldDefinition, is_data_optional: bool, data_dto: type[AbstractDTO] | None
```

### Comparing `litestar-2.8.2/litestar/_kwargs/kwargs_model.py` & `litestar-2.8.3/litestar/_kwargs/kwargs_model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_kwargs/parameter_definition.py` & `litestar-2.8.3/litestar/_kwargs/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_layers/utils.py` & `litestar-2.8.3/litestar/_layers/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/datastructures.py` & `litestar-2.8.3/litestar/_openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/parameters.py` & `litestar-2.8.3/litestar/_openapi/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,19 +214,23 @@
 
     def create_parameters_for_handler(self) -> list[Parameter]:
         """Create a list of path/query/header Parameter models for the given PathHandler."""
         handler_fields = self.route_handler.parsed_fn_signature.parameters
         # not all path parameters have to be consumed by the handler. Because even not
         # consumed path parameters must still be specified, we create stub parameters
         # for the unconsumed ones so a correct OpenAPI schema can be generated
+        dependency_fields = {
+            name for dep in self.dependency_providers.values() for name in dep.parsed_fn_signature.parameters
+        }
         params_not_consumed_by_handler = set(self.path_parameters) - handler_fields.keys()
+        unconsumed_path_parameters = params_not_consumed_by_handler - dependency_fields
         handler_fields.update(
             {
                 param_name: FieldDefinition.from_kwarg(self.path_parameters[param_name].type, name=param_name)
-                for param_name in params_not_consumed_by_handler
+                for param_name in unconsumed_path_parameters
             }
         )
 
         self.create_parameters_for_field_definitions(handler_fields)
         return self.parameters.list()
```

### Comparing `litestar-2.8.2/litestar/_openapi/path_item.py` & `litestar-2.8.3/litestar/_openapi/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/plugin.py` & `litestar-2.8.3/litestar/_openapi/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/request_body.py` & `litestar-2.8.3/litestar/_openapi/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/responses.py` & `litestar-2.8.3/litestar/_openapi/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/utils.py` & `litestar-2.8.3/litestar/_openapi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/schema_generation/constrained_fields.py` & `litestar-2.8.3/litestar/_openapi/schema_generation/constrained_fields.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/schema_generation/examples.py` & `litestar-2.8.3/litestar/_openapi/schema_generation/examples.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/schema_generation/schema.py` & `litestar-2.8.3/litestar/_openapi/schema_generation/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/schema_generation/utils.py` & `litestar-2.8.3/litestar/_openapi/schema_generation/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/schema_generation/plugins/__init__.py` & `litestar-2.8.3/litestar/_openapi/schema_generation/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/schema_generation/plugins/dataclass.py` & `litestar-2.8.3/litestar/_openapi/schema_generation/plugins/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/schema_generation/plugins/pagination.py` & `litestar-2.8.3/litestar/_openapi/schema_generation/plugins/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/schema_generation/plugins/struct.py` & `litestar-2.8.3/litestar/_openapi/schema_generation/plugins/struct.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/schema_generation/plugins/typed_dict.py` & `litestar-2.8.3/litestar/_openapi/schema_generation/plugins/typed_dict.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/typescript_converter/converter.py` & `litestar-2.8.3/litestar/_openapi/typescript_converter/converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/typescript_converter/schema_parsing.py` & `litestar-2.8.3/litestar/_openapi/typescript_converter/schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_openapi/typescript_converter/types.py` & `litestar-2.8.3/litestar/_openapi/typescript_converter/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_signature/model.py` & `litestar-2.8.3/litestar/_signature/model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/_signature/utils.py` & `litestar-2.8.3/litestar/_signature/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/channels/plugin.py` & `litestar-2.8.3/litestar/channels/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/channels/subscriber.py` & `litestar-2.8.3/litestar/channels/subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/channels/backends/asyncpg.py` & `litestar-2.8.3/litestar/channels/backends/asyncpg.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/channels/backends/base.py` & `litestar-2.8.3/litestar/channels/backends/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/channels/backends/memory.py` & `litestar-2.8.3/litestar/channels/backends/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/channels/backends/psycopg.py` & `litestar-2.8.3/litestar/channels/backends/psycopg.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/channels/backends/redis.py` & `litestar-2.8.3/litestar/channels/backends/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/cli/__init__.py` & `litestar-2.8.3/litestar/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/cli/_utils.py` & `litestar-2.8.3/litestar/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/cli/main.py` & `litestar-2.8.3/litestar/cli/main.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/cli/commands/core.py` & `litestar-2.8.3/litestar/cli/commands/core.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/cli/commands/schema.py` & `litestar-2.8.3/litestar/cli/commands/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/cli/commands/sessions.py` & `litestar-2.8.3/litestar/cli/commands/sessions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/config/allowed_hosts.py` & `litestar-2.8.3/litestar/config/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/config/app.py` & `litestar-2.8.3/litestar/config/app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/config/compression.py` & `litestar-2.8.3/litestar/config/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/config/cors.py` & `litestar-2.8.3/litestar/config/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/config/csrf.py` & `litestar-2.8.3/litestar/config/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/config/response_cache.py` & `litestar-2.8.3/litestar/config/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/connection/__init__.py` & `litestar-2.8.3/litestar/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/connection/base.py` & `litestar-2.8.3/litestar/connection/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/connection/request.py` & `litestar-2.8.3/litestar/connection/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/connection/websocket.py` & `litestar-2.8.3/litestar/connection/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/jinja.py` & `litestar-2.8.3/litestar/contrib/jinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/mako.py` & `litestar-2.8.3/litestar/contrib/mako.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/minijinja.py` & `litestar-2.8.3/litestar/contrib/minijinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/piccolo.py` & `litestar-2.8.3/litestar/contrib/piccolo.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/attrs/attrs_schema_plugin.py` & `litestar-2.8.3/litestar/contrib/attrs/attrs_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/htmx/_utils.py` & `litestar-2.8.3/litestar/contrib/htmx/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/htmx/request.py` & `litestar-2.8.3/litestar/contrib/htmx/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/htmx/response.py` & `litestar-2.8.3/litestar/contrib/htmx/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/htmx/types.py` & `litestar-2.8.3/litestar/contrib/htmx/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/jwt/__init__.py` & `litestar-2.8.3/litestar/contrib/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/opentelemetry/_utils.py` & `litestar-2.8.3/litestar/contrib/opentelemetry/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/opentelemetry/config.py` & `litestar-2.8.3/litestar/contrib/opentelemetry/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/opentelemetry/middleware.py` & `litestar-2.8.3/litestar/contrib/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/prometheus/config.py` & `litestar-2.8.3/litestar/contrib/prometheus/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/prometheus/controller.py` & `litestar-2.8.3/litestar/contrib/prometheus/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/prometheus/middleware.py` & `litestar-2.8.3/litestar/contrib/prometheus/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/pydantic/__init__.py` & `litestar-2.8.3/litestar/contrib/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/pydantic/pydantic_di_plugin.py` & `litestar-2.8.3/litestar/contrib/pydantic/pydantic_di_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/pydantic/pydantic_dto_factory.py` & `litestar-2.8.3/litestar/contrib/pydantic/pydantic_dto_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dataclasses import replace
 from typing import TYPE_CHECKING, Any, Collection, Generic, TypeVar
 from warnings import warn
 
 from typing_extensions import Annotated, TypeAlias, override
 
-from litestar.contrib.pydantic.utils import is_pydantic_undefined
+from litestar.contrib.pydantic.utils import is_pydantic_undefined, is_pydantic_v2
 from litestar.dto.base_dto import AbstractDTO
 from litestar.dto.data_structures import DTOFieldDefinition
 from litestar.dto.field import DTO_FIELD_META_KEY, extract_dto_field
 from litestar.exceptions import MissingDependencyException, ValidationException
 from litestar.types.empty import Empty
 from litestar.typing import FieldDefinition
 
@@ -22,23 +22,24 @@
 except ImportError as e:
     raise MissingDependencyException("pydantic") from e
 
 
 try:
     import pydantic as pydantic_v2
 
-    assert pydantic_v2.__version__.startswith("2.")  # noqa: S101
+    if not is_pydantic_v2(pydantic_v2):
+        raise ImportError
 
     from pydantic import ValidationError as ValidationErrorV2
     from pydantic import v1 as pydantic_v1
     from pydantic.v1 import ValidationError as ValidationErrorV1
 
     ModelType: TypeAlias = "pydantic_v1.BaseModel | pydantic_v2.BaseModel"
 
-except AssertionError:
+except ImportError:
     import pydantic as pydantic_v1  # type: ignore[no-redef]
 
     pydantic_v2 = Empty  # type: ignore[assignment]
     from pydantic import ValidationError as ValidationErrorV1  # type: ignore[assignment]
 
     ValidationErrorV2 = ValidationErrorV1  # type: ignore[assignment, misc]
     ModelType = "pydantic_v1.BaseModel"  # type: ignore[misc]
```

### Comparing `litestar-2.8.2/litestar/contrib/pydantic/pydantic_init_plugin.py` & `litestar-2.8.3/litestar/contrib/pydantic/pydantic_init_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 from typing import TYPE_CHECKING, Any, Callable, TypeVar, cast
 from uuid import UUID
 
 from msgspec import ValidationError
 from typing_extensions import Buffer, TypeGuard
 
 from litestar._signature.types import ExtendedMsgSpecValidationError
-from litestar.contrib.pydantic.utils import is_pydantic_constrained_field
+from litestar.contrib.pydantic.utils import is_pydantic_constrained_field, is_pydantic_v2
 from litestar.exceptions import MissingDependencyException
 from litestar.plugins import InitPluginProtocol
 from litestar.typing import _KWARG_META_EXTRACTORS
 from litestar.utils import is_class_and_subclass
 
 try:
     import pydantic as _  # noqa: F401
 except ImportError as e:
     raise MissingDependencyException("pydantic") from e
 
 try:
     import pydantic as pydantic_v2
 
-    assert pydantic_v2.__version__.startswith("2.")  # noqa: S101
+    if not is_pydantic_v2(pydantic_v2):
+        raise ImportError
 
     from pydantic import v1 as pydantic_v1
-except AssertionError:
+except ImportError:
     import pydantic as pydantic_v1  # type: ignore[no-redef]
 
     pydantic_v2 = None  # type: ignore[assignment]
 
 
 if TYPE_CHECKING:
     from litestar.config.app import AppConfig
```

### Comparing `litestar-2.8.2/litestar/contrib/pydantic/pydantic_schema_plugin.py` & `litestar-2.8.3/litestar/contrib/pydantic/pydantic_schema_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from litestar.contrib.pydantic.utils import (
     create_field_definitions_for_computed_fields,
     is_pydantic_2_model,
     is_pydantic_constrained_field,
     is_pydantic_model_class,
     is_pydantic_undefined,
+    is_pydantic_v2,
     pydantic_get_type_hints_with_generics_resolved,
     pydantic_unwrap_and_get_origin,
 )
 from litestar.exceptions import MissingDependencyException
 from litestar.openapi.spec import OpenAPIFormat, OpenAPIType, Schema
 from litestar.plugins import OpenAPISchemaPlugin
 from litestar.types import Empty
@@ -24,18 +25,19 @@
     import pydantic as _  # noqa: F401
 except ImportError as e:
     raise MissingDependencyException("pydantic") from e
 
 try:
     import pydantic as pydantic_v2
 
-    assert pydantic_v2.__version__.startswith("2.")  # noqa: S101
+    if not is_pydantic_v2(pydantic_v2):
+        raise ImportError
 
     from pydantic import v1 as pydantic_v1
-except AssertionError:
+except ImportError:
     import pydantic as pydantic_v1  # type: ignore[no-redef]
 
     pydantic_v2 = None  # type: ignore[assignment]
 
 if TYPE_CHECKING:
     from litestar._openapi.schema_generation.schema import SchemaCreator
```

### Comparing `litestar-2.8.2/litestar/contrib/pydantic/utils.py` & `litestar-2.8.3/litestar/contrib/pydantic/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         pydantic_v1 = Empty  # type: ignore[assignment]
         pydantic_v2 = Empty  # type: ignore[assignment]
         PYDANTIC_UNDEFINED_SENTINELS = set()
 # isort: on
 
 
 if TYPE_CHECKING:
+    from types import ModuleType
+
     from typing_extensions import TypeGuard
 
 
 def is_pydantic_model_class(
     annotation: Any,
 ) -> TypeGuard[type[pydantic_v1.BaseModel | pydantic_v2.BaseModel]]:  # pyright: ignore
     """Given a type annotation determine if the annotation is a subclass of pydantic's BaseModel.
@@ -208,7 +210,21 @@
                 dec.info.return_type,
                 KwargDefinition(title=dec.info.title, description=dec.info.description, read_only=True),
             ],
             name=name,
         )
         for k, dec in pydantic_decorators.computed_fields.items()
     }
+
+
+def is_pydantic_v2(module: ModuleType) -> bool:
+    """Determine if the given module is pydantic v2.
+
+    Given a module we expect to be a pydantic version, determine if it is pydantic v2.
+
+    Args:
+        module: A module.
+
+    Returns:
+        True if the module is pydantic v2, otherwise False.
+    """
+    return bool(module.__version__.startswith("2."))
```

### Comparing `litestar-2.8.2/litestar/contrib/repository/__init__.py` & `litestar-2.8.3/litestar/contrib/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/repository/exceptions.py` & `litestar-2.8.3/litestar/contrib/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/repository/filters.py` & `litestar-2.8.3/litestar/contrib/repository/filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/repository/handlers.py` & `litestar-2.8.3/litestar/contrib/repository/handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/repository/testing.py` & `litestar-2.8.3/litestar/contrib/repository/testing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/repository/abc/__init__.py` & `litestar-2.8.3/litestar/contrib/repository/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/sqlalchemy/base.py` & `litestar-2.8.3/litestar/contrib/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/__init__.py` & `litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py` & `litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/init/config/compat.py` & `litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/contrib/sqlalchemy/plugins/init/config/sync.py` & `litestar-2.8.3/litestar/contrib/sqlalchemy/plugins/init/config/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/datastructures/__init__.py` & `litestar-2.8.3/litestar/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/datastructures/cookie.py` & `litestar-2.8.3/litestar/datastructures/cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/datastructures/headers.py` & `litestar-2.8.3/litestar/datastructures/headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 from abc import ABC, abstractmethod
 from contextlib import suppress
 from copy import copy
 from dataclasses import dataclass, fields
 from typing import (
     TYPE_CHECKING,
-    AbstractSet,
     Any,
     ClassVar,
     Dict,
     Iterable,
     Iterator,
     List,
     Mapping,
@@ -298,16 +297,14 @@
     must_understand: Optional[bool] = None
     """Accessor for the ``must-understand`` directive."""
     immutable: Optional[bool] = None
     """Accessor for the ``immutable`` directive."""
     stale_while_revalidate: Optional[int] = None
     """Accessor for the ``stale-while-revalidate`` directive."""
 
-    _field_names: ClassVar[AbstractSet[str]]
-
     def _get_header_value(self) -> str:
         """Get the header value as string."""
 
         cc_items = [
             key.replace("_", "-") if isinstance(value, bool) else f"{key.replace('_', '-')}={value}"
             for key, value in simple_asdict(self, exclude_none=True, exclude={"documentation_only"}).items()
         ]
@@ -321,15 +318,15 @@
             header_value: the header value as string
 
         Returns:
             An instance of ``CacheControlHeader``
         """
 
         kwargs: Dict[str, Any] = {}
-        field_names = cls._get_field_names()
+        field_names = {f.name for f in fields(cls)}
         for cc_item in (stripped for v in header_value.split(",") if (stripped := v.strip())):
             key, *value = cc_item.split("=", maxsplit=1)
             key = key.replace("-", "_")
             if key not in field_names:
                 raise ImproperlyConfiguredException("Invalid cache-control header")
             if not value:
                 kwargs[key] = True
@@ -345,31 +342,14 @@
     def prevent_storing(cls) -> "CacheControlHeader":
         """Create a ``cache-control`` header with the ``no-store`` directive which indicates that any caches of any kind
         (private or shared) should not store this response.
         """
 
         return cls(no_store=True)
 
-    @classmethod
-    def _get_field_names(cls) -> AbstractSet[str]:
-        """Get the type annotations for the ``CacheControlHeader`` class properties.
-
-        This is needed due to the conversion from pydantic models to dataclasses. Dataclasses do not support
-        automatic conversion of types like pydantic models do.
-
-        Returns:
-            A dictionary of type annotations
-
-        """
-        try:
-            names = cls._field_names
-        except AttributeError:
-            names = cls._field_names = {f.name for f in fields(cls)}
-        return names
-
 
 @dataclass
 class ETag(Header):
     """An ``etag`` header."""
 
     HEADER_NAME: ClassVar[str] = "etag"
```

### Comparing `litestar-2.8.2/litestar/datastructures/multi_dicts.py` & `litestar-2.8.3/litestar/datastructures/multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/datastructures/response_header.py` & `litestar-2.8.3/litestar/datastructures/response_header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/datastructures/state.py` & `litestar-2.8.3/litestar/datastructures/state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/datastructures/upload_file.py` & `litestar-2.8.3/litestar/datastructures/upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/datastructures/url.py` & `litestar-2.8.3/litestar/datastructures/url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/dto/_backend.py` & `litestar-2.8.3/litestar/dto/_backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/dto/_codegen_backend.py` & `litestar-2.8.3/litestar/dto/_codegen_backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/dto/_types.py` & `litestar-2.8.3/litestar/dto/_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/dto/base_dto.py` & `litestar-2.8.3/litestar/dto/base_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -191,19 +191,39 @@
 
     @classmethod
     def create_openapi_schema(
         cls, field_definition: FieldDefinition, handler_id: str, schema_creator: SchemaCreator
     ) -> Reference | Schema:
         """Create an OpenAPI request body.
 
+        Args:
+            field_definition: A parsed type annotation that represents the annotation used on the handler.
+            handler_id: ID of the route handler for which to create a DTO instance.
+            schema_creator: A factory for creating schemas. Has a ``for_field_definition()`` method that accepts a
+                :class:`~litestar.typing.FieldDefinition` instance.
+
         Returns:
             OpenAPI request body.
         """
         key = "data_backend" if field_definition.name == "data" else "return_backend"
         backend = cls._dto_backends[handler_id][key]  # type: ignore[literal-required]
+
+        if backend.wrapper_attribute_name:
+            # The DTO has been built for a handler that has a DTO supported type wrapped in a generic type.
+            #
+            # The backend doesn't receive the full annotation, only the type of the attribute on the outer type that
+            # holds the DTO supported type.
+            #
+            # This special casing rebuilds the outer generic type annotation with the original model replaced by the DTO
+            # generated transfer model type in the type arguments.
+            transfer_model = backend.transfer_model_type
+            generic_args = tuple(transfer_model if a is cls.model_type else a for a in field_definition.args)
+            return schema_creator.for_field_definition(
+                FieldDefinition.from_annotation(field_definition.origin[generic_args])
+            )
         return schema_creator.for_field_definition(FieldDefinition.from_annotation(backend.annotation))
 
     @classmethod
     def resolve_generic_wrapper_type(
         cls, field_definition: FieldDefinition
     ) -> tuple[FieldDefinition, FieldDefinition, str] | None:
         """Handle where DTO supported data is wrapped in a generic container type.
```

### Comparing `litestar-2.8.2/litestar/dto/config.py` & `litestar-2.8.3/litestar/dto/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/dto/data_structures.py` & `litestar-2.8.3/litestar/dto/data_structures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/dto/dataclass_dto.py` & `litestar-2.8.3/litestar/dto/dataclass_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/dto/field.py` & `litestar-2.8.3/litestar/dto/field.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/dto/msgspec_dto.py` & `litestar-2.8.3/litestar/dto/msgspec_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/events/emitter.py` & `litestar-2.8.3/litestar/events/emitter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/events/listener.py` & `litestar-2.8.3/litestar/events/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/exceptions/__init__.py` & `litestar-2.8.3/litestar/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/exceptions/base_exceptions.py` & `litestar-2.8.3/litestar/exceptions/base_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/exceptions/http_exceptions.py` & `litestar-2.8.3/litestar/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/exceptions/websocket_exceptions.py` & `litestar-2.8.3/litestar/exceptions/websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/handlers/__init__.py` & `litestar-2.8.3/litestar/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/handlers/asgi_handlers.py` & `litestar-2.8.3/litestar/handlers/asgi_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/handlers/base.py` & `litestar-2.8.3/litestar/handlers/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/handlers/http_handlers/_utils.py` & `litestar-2.8.3/litestar/handlers/http_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/handlers/http_handlers/base.py` & `litestar-2.8.3/litestar/handlers/http_handlers/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/handlers/http_handlers/decorators.py` & `litestar-2.8.3/litestar/handlers/http_handlers/decorators.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/handlers/websocket_handlers/_utils.py` & `litestar-2.8.3/litestar/handlers/websocket_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/handlers/websocket_handlers/listener.py` & `litestar-2.8.3/litestar/handlers/websocket_handlers/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/handlers/websocket_handlers/route_handler.py` & `litestar-2.8.3/litestar/handlers/websocket_handlers/route_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/logging/_utils.py` & `litestar-2.8.3/litestar/logging/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/logging/config.py` & `litestar-2.8.3/litestar/logging/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import sys
 from abc import ABC, abstractmethod
-from dataclasses import asdict, dataclass, field, fields
+from dataclasses import dataclass, field, fields
 from importlib.util import find_spec
 from logging import INFO
 from typing import TYPE_CHECKING, Any, Callable, Literal, cast
 
 from litestar.exceptions import ImproperlyConfiguredException, MissingDependencyException
 from litestar.serialization.msgspec_hooks import _msgspec_json_encoder
+from litestar.utils.dataclass import simple_asdict
 from litestar.utils.deprecation import deprecated
 
 __all__ = ("BaseLoggingConfig", "LoggingConfig", "StructLoggingConfig")
 
 
 if TYPE_CHECKING:
     from collections.abc import Iterable
@@ -309,15 +310,17 @@
     return _msgspec_json_encoder.encode(value)
 
 
 def stdlib_json_serializer(value: EventDict, **_: Any) -> str:  # pragma: no cover
     return _msgspec_json_encoder.encode(value).decode("utf-8")
 
 
-def default_structlog_processors(as_json: bool = True) -> list[Processor]:  # pyright: ignore
+def default_structlog_processors(
+    as_json: bool = True, json_serializer: Callable[[Any], Any] = default_json_serializer
+) -> list[Processor]:  # pyright: ignore
     """Set the default processors for structlog.
 
     Returns:
         An optional list of processors.
     """
     try:
         import structlog
@@ -325,15 +328,15 @@
 
         if as_json:
             return [
                 structlog.contextvars.merge_contextvars,
                 structlog.processors.add_log_level,
                 structlog.processors.format_exc_info,
                 structlog.processors.TimeStamper(fmt="iso"),
-                structlog.processors.JSONRenderer(serializer=default_json_serializer),
+                structlog.processors.JSONRenderer(serializer=json_serializer),
             ]
         return [
             structlog.contextvars.merge_contextvars,
             structlog.processors.add_log_level,
             structlog.processors.TimeStamper(fmt="iso"),
             structlog.dev.ConsoleRenderer(
                 colors=True, exception_formatter=RichTracebackFormatter(max_frames=1, show_locals=False, width=80)
@@ -461,15 +464,15 @@
             import structlog
         except ImportError as e:
             raise MissingDependencyException("structlog") from e
 
         structlog.configure(
             **{
                 k: v
-                for k, v in asdict(self).items()
+                for k, v in simple_asdict(self).items()
                 if k
                 not in (
                     "standard_lib_logging_config",
                     "log_exceptions",
                     "traceback_line_limit",
                     "exception_logging_handler",
                     "pretty_print_tty",
```

### Comparing `litestar-2.8.2/litestar/logging/picologging.py` & `litestar-2.8.3/litestar/logging/picologging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/logging/standard.py` & `litestar-2.8.3/litestar/logging/standard.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/_utils.py` & `litestar-2.8.3/litestar/middleware/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/allowed_hosts.py` & `litestar-2.8.3/litestar/middleware/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/authentication.py` & `litestar-2.8.3/litestar/middleware/authentication.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 if TYPE_CHECKING:
     from litestar.types import ASGIApp, Method, Receive, Scope, Scopes, Send
 
 
 @dataclass
 class AuthenticationResult:
-    """Pydantic model for authentication data."""
+    """Dataclass for authentication result."""
 
     __slots__ = ("user", "auth")
 
     user: Any
     """The user model, this can be any value corresponding to a user of the API."""
     auth: Any
     """The auth value, this can for example be a JWT token."""
```

### Comparing `litestar-2.8.2/litestar/middleware/base.py` & `litestar-2.8.3/litestar/middleware/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/cors.py` & `litestar-2.8.3/litestar/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/csrf.py` & `litestar-2.8.3/litestar/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/logging.py` & `litestar-2.8.3/litestar/middleware/logging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/rate_limit.py` & `litestar-2.8.3/litestar/middleware/rate_limit.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/response_cache.py` & `litestar-2.8.3/litestar/middleware/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/compression/brotli_facade.py` & `litestar-2.8.3/litestar/middleware/compression/brotli_facade.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/compression/facade.py` & `litestar-2.8.3/litestar/middleware/compression/facade.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/compression/gzip_facade.py` & `litestar-2.8.3/litestar/middleware/compression/gzip_facade.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/compression/middleware.py` & `litestar-2.8.3/litestar/middleware/compression/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/exceptions/_debug_response.py` & `litestar-2.8.3/litestar/middleware/exceptions/_debug_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/exceptions/middleware.py` & `litestar-2.8.3/litestar/middleware/exceptions/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/exceptions/templates/scripts.js` & `litestar-2.8.3/litestar/middleware/exceptions/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/exceptions/templates/styles.css` & `litestar-2.8.3/litestar/middleware/exceptions/templates/styles.css`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/session/base.py` & `litestar-2.8.3/litestar/middleware/session/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/middleware/session/client_side.py` & `litestar-2.8.3/litestar/middleware/session/client_side.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import binascii
 import contextlib
 import re
 import time
 from base64 import b64decode, b64encode
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, fields
 from os import urandom
-from typing import TYPE_CHECKING, Any, Literal
+from typing import TYPE_CHECKING, Any, Final, Literal, Mapping
 
 from litestar.datastructures import MutableScopeHeaders
 from litestar.datastructures.cookie import Cookie
 from litestar.enums import ScopeType
 from litestar.exceptions import (
     ImproperlyConfiguredException,
     MissingDependencyException,
@@ -34,30 +34,43 @@
 if TYPE_CHECKING:
     from litestar.connection import ASGIConnection
     from litestar.types import Message, Scope, ScopeSession
 
 NONCE_SIZE = 12
 CHUNK_SIZE = 4096 - 64
 AAD = b"additional_authenticated_data="
+SET_COOKIE_INCLUDE = {f.name for f in fields(Cookie) if f.name not in {"key", "secret"}}
+CLEAR_COOKIE_INCLUDE = {f.name for f in fields(Cookie) if f.name not in {"key", "secret", "max_age"}}
 
 
 class ClientSideSessionBackend(BaseSessionBackend["CookieBackendConfig"]):
     """Cookie backend for SessionMiddleware."""
 
-    __slots__ = ("aesgcm", "cookie_re")
+    __slots__ = (
+        "_clear_cookie_params",
+        "_set_cookie_params",
+        "aesgcm",
+        "cookie_re",
+    )
 
     def __init__(self, config: CookieBackendConfig) -> None:
         """Initialize ``ClientSideSessionBackend``.
 
         Args:
             config: SessionCookieConfig instance.
         """
         super().__init__(config)
         self.aesgcm = AESGCM(config.secret)
         self.cookie_re = re.compile(rf"{self.config.key}(?:-\d+)?")
+        self._set_cookie_params: Final[Mapping[str, Any]] = dict(
+            extract_dataclass_items(config, exclude_none=True, include=SET_COOKIE_INCLUDE)
+        )
+        self._clear_cookie_params: Final[Mapping[str, Any]] = dict(
+            extract_dataclass_items(config, exclude_none=True, include=CLEAR_COOKIE_INCLUDE)
+        )
 
     def dump_data(self, data: Any, scope: Scope | None = None) -> list[bytes]:
         """Given serializable data, including pydantic models and numpy types, dump it into a bytes string, encrypt,
         encode and split it into chunks of the desirable size.
 
         Args:
             data: Data to serialize, encrypt, encode and chunk.
@@ -103,27 +116,33 @@
             connection: An ASGIConnection instance
 
         Returns:
             A list of session-cookie keys
         """
         return sorted(key for key in connection.cookies if self.cookie_re.fullmatch(key))
 
-    def _create_session_cookies(self, data: list[bytes], cookie_params: dict[str, Any] | None = None) -> list[Cookie]:
+    def get_cookie_key_set(self, connection: ASGIConnection) -> set[str]:
+        """Return a set of cookie-keys from the connection if they match the session-cookie pattern.
+
+        .. versionadded:: 2.8.3
+
+        Args:
+            connection: An ASGIConnection instance
+
+        Returns:
+            A set of session-cookie keys
+        """
+        return {key for key in connection.cookies if self.cookie_re.fullmatch(key)}
+
+    def _create_session_cookies(self, data: list[bytes]) -> list[Cookie]:
         """Create a list of cookies containing the session data.
         If the data is split into multiple cookies, the key will be of the format ``session-{segment number}``,
         however if only one cookie is needed, the key will be ``session``.
         """
-        if cookie_params is None:
-            cookie_params = dict(
-                extract_dataclass_items(
-                    self.config,
-                    exclude_none=True,
-                    include={f for f in Cookie.__dict__ if f not in ("key", "secret")},
-                )
-            )
+        cookie_params = self._set_cookie_params
 
         if len(data) == 1:
             return [
                 Cookie(
                     value=data[0].decode("utf-8"),
                     key=self.config.key,
                     **cookie_params,
@@ -152,46 +171,31 @@
 
         Returns:
             None
         """
 
         scope = connection.scope
         headers = MutableScopeHeaders.from_message(message)
-        cookie_keys = self.get_cookie_keys(connection)
+        connection_cookies = self.get_cookie_key_set(connection)
+        response_cookies: set[str] = set()
 
         if scope_session and scope_session is not Empty:
             data = self.dump_data(scope_session, scope=scope)
-            cookie_params = dict(
-                extract_dataclass_items(
-                    self.config,
-                    exclude_none=True,
-                    include={f for f in Cookie.__dict__ if f not in ("key", "secret")},
-                )
-            )
-            for cookie in self._create_session_cookies(data, cookie_params):
+            for cookie in self._create_session_cookies(data):
                 headers.add("Set-Cookie", cookie.to_header(header=""))
-            # Cookies with the same key overwrite the earlier cookie with that key. To expire earlier session
-            # cookies, first check how many session cookies will not be overwritten in this upcoming response.
-            # If leftover cookies are greater than or equal to 1, that means older session cookies have to be
-            # expired and their names are in cookie_keys.
-            cookies_to_clear = cookie_keys[len(data) :] if len(cookie_keys) - len(data) > 0 else []
+                response_cookies.add(cookie.key)
+
+            cookies_to_clear = connection_cookies - response_cookies
         else:
-            cookies_to_clear = cookie_keys
+            cookies_to_clear = connection_cookies
 
         for cookie_key in cookies_to_clear:
-            cookie_params = dict(
-                extract_dataclass_items(
-                    self.config,
-                    exclude_none=True,
-                    include={f for f in Cookie.__dict__ if f not in ("key", "secret", "max_age")},
-                )
-            )
             headers.add(
                 "Set-Cookie",
-                Cookie(value="null", key=cookie_key, expires=0, **cookie_params).to_header(header=""),
+                Cookie(value="null", key=cookie_key, expires=0, **self._clear_cookie_params).to_header(header=""),
             )
 
     async def load_from_connection(self, connection: ASGIConnection) -> dict[str, Any]:
         """Load session data from a connection's session-cookies and return it as a dictionary.
 
         Args:
             connection: Originating ASGIConnection
```

### Comparing `litestar-2.8.2/litestar/middleware/session/server_side.py` & `litestar-2.8.3/litestar/middleware/session/server_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/config.py` & `litestar-2.8.3/litestar/openapi/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/controller.py` & `litestar-2.8.3/litestar/openapi/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/datastructures.py` & `litestar-2.8.3/litestar/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/plugins.py` & `litestar-2.8.3/litestar/openapi/plugins.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/__init__.py` & `litestar-2.8.3/litestar/openapi/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/base.py` & `litestar-2.8.3/litestar/openapi/spec/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass, fields, is_dataclass
 from enum import Enum
-from typing import Any
+from typing import TYPE_CHECKING, Any
+
+if TYPE_CHECKING:
+    from collections.abc import Iterator
+    from dataclasses import Field
 
 __all__ = ("BaseSchemaObject",)
 
 
 def _normalize_key(key: str) -> str:
     if key.endswith("_in"):
         return "in"
@@ -30,21 +34,24 @@
     return value.value if isinstance(value, Enum) else value
 
 
 @dataclass
 class BaseSchemaObject:
     """Base class for schema spec objects"""
 
+    def _iter_fields(self) -> Iterator[Field[Any]]:
+        yield from fields(self)
+
     def to_schema(self) -> dict[str, Any]:
         """Transform the spec dataclass object into a string keyed dictionary. This method traverses all nested values
         recursively.
         """
         result: dict[str, Any] = {}
 
-        for field in fields(self):
+        for field in self._iter_fields():
             value = _normalize_value(getattr(self, field.name, None))
 
             if value is not None:
                 if "alias" in field.metadata:
                     if not isinstance(field.metadata["alias"], str):
                         raise TypeError('metadata["alias"] must be a str')
                     key = field.metadata["alias"]
```

### Comparing `litestar-2.8.2/litestar/openapi/spec/callback.py` & `litestar-2.8.3/litestar/openapi/spec/callback.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/components.py` & `litestar-2.8.3/litestar/openapi/spec/components.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/contact.py` & `litestar-2.8.3/litestar/openapi/spec/contact.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/discriminator.py` & `litestar-2.8.3/litestar/openapi/spec/discriminator.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/encoding.py` & `litestar-2.8.3/litestar/openapi/spec/encoding.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/enums.py` & `litestar-2.8.3/litestar/openapi/spec/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/example.py` & `litestar-2.8.3/litestar/openapi/spec/example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/external_documentation.py` & `litestar-2.8.3/litestar/openapi/spec/external_documentation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/header.py` & `litestar-2.8.3/litestar/openapi/spec/header.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Literal
+from dataclasses import Field, dataclass
+from typing import TYPE_CHECKING, Any, Iterator, Literal
+
+from typing_extensions import override
 
 from litestar.openapi.spec.base import BaseSchemaObject
 
 if TYPE_CHECKING:
     from litestar.openapi.spec.example import Example
     from litestar.openapi.spec.media_type import OpenAPIMediaType
     from litestar.openapi.spec.reference import Reference
@@ -115,7 +117,11 @@
     """
 
     content: dict[str, OpenAPIMediaType] | None = None
     """A map containing the representations for the parameter.
 
     The key is the media type and the value describes it. The map MUST only contain one entry.
     """
+
+    @override
+    def _iter_fields(self) -> Iterator[Field[Any]]:
+        yield from (f for f in super()._iter_fields() if f.name not in {"name", "param_in"})
```

### Comparing `litestar-2.8.2/litestar/openapi/spec/info.py` & `litestar-2.8.3/litestar/openapi/spec/info.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/license.py` & `litestar-2.8.3/litestar/openapi/spec/license.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/link.py` & `litestar-2.8.3/litestar/openapi/spec/link.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/media_type.py` & `litestar-2.8.3/litestar/openapi/spec/media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/oauth_flow.py` & `litestar-2.8.3/litestar/openapi/spec/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/oauth_flows.py` & `litestar-2.8.3/litestar/openapi/spec/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/open_api.py` & `litestar-2.8.3/litestar/openapi/spec/open_api.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/operation.py` & `litestar-2.8.3/litestar/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/parameter.py` & `litestar-2.8.3/litestar/openapi/spec/parameter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/path_item.py` & `litestar-2.8.3/litestar/openapi/spec/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/paths.py` & `litestar-2.8.3/litestar/openapi/spec/paths.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/reference.py` & `litestar-2.8.3/litestar/openapi/spec/reference.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/request_body.py` & `litestar-2.8.3/litestar/openapi/spec/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/response.py` & `litestar-2.8.3/litestar/openapi/spec/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/responses.py` & `litestar-2.8.3/litestar/openapi/spec/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/schema.py` & `litestar-2.8.3/litestar/openapi/spec/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/security_requirement.py` & `litestar-2.8.3/litestar/openapi/spec/security_requirement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/security_scheme.py` & `litestar-2.8.3/litestar/openapi/spec/security_scheme.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/server.py` & `litestar-2.8.3/litestar/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/server_variable.py` & `litestar-2.8.3/litestar/openapi/spec/server_variable.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/tag.py` & `litestar-2.8.3/litestar/openapi/spec/tag.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/openapi/spec/xml.py` & `litestar-2.8.3/litestar/openapi/spec/xml.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/plugins/base.py` & `litestar-2.8.3/litestar/plugins/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/plugins/core.py` & `litestar-2.8.3/litestar/plugins/core.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/plugins/flash.py` & `litestar-2.8.3/litestar/plugins/flash.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 """Plugin for creating and retrieving flash messages."""
 
+from __future__ import annotations
+
+from contextlib import suppress
 from dataclasses import dataclass
-from typing import Any, Mapping
+from typing import TYPE_CHECKING, Any, Mapping
 
-from litestar.config.app import AppConfig
-from litestar.connection import ASGIConnection
-from litestar.contrib.minijinja import MiniJinjaTemplateEngine
+import litestar.exceptions
+from litestar import Request
+from litestar.exceptions import MissingDependencyException
+from litestar.middleware import DefineMiddleware
+from litestar.middleware.session import SessionMiddleware
 from litestar.plugins import InitPluginProtocol
-from litestar.template import TemplateConfig
+from litestar.security.session_auth.middleware import MiddlewareWrapper
 from litestar.template.base import _get_request_from_context
-from litestar.utils.scope.state import ScopeState
+from litestar.utils.predicates import is_class_and_subclass
+
+if TYPE_CHECKING:
+    from collections.abc import Callable
+
+    from litestar.config.app import AppConfig
+    from litestar.template import TemplateConfig
 
 
 @dataclass
 class FlashConfig:
     """Configuration for Flash messages."""
 
     template_config: TemplateConfig
@@ -35,41 +46,35 @@
 
         Args:
             app_config: The application configuration.
 
         Returns:
             The application configuration with the message callable registered.
         """
-        if isinstance(self.config.template_config.engine_instance, MiniJinjaTemplateEngine):
-            from litestar.contrib.minijinja import _transform_state
-
-            self.config.template_config.engine_instance.register_template_callable(
-                "get_flashes", _transform_state(get_flashes)
-            )
+        for mw in app_config.middleware:
+            if isinstance(mw, DefineMiddleware) and is_class_and_subclass(
+                mw.middleware, (MiddlewareWrapper, SessionMiddleware)
+            ):
+                break
         else:
-            self.config.template_config.engine_instance.register_template_callable("get_flashes", get_flashes)
-        return app_config
+            raise litestar.exceptions.ImproperlyConfiguredException("Flash messages require a session middleware.")
+        template_callable: Callable[[Any], Any] = get_flashes
+        with suppress(MissingDependencyException):
+            from litestar.contrib.minijinja import MiniJinjaTemplateEngine, _transform_state
 
+            if isinstance(self.config.template_config.engine_instance, MiniJinjaTemplateEngine):
+                template_callable = _transform_state(get_flashes)
 
-def flash(connection: ASGIConnection, message: str, category: str) -> None:
-    """Add a flash message to the request scope.
-
-    Args:
-        connection: The connection instance.
-        message: The message to flash.
-        category: The category of the message.
-    """
-    scope_state = ScopeState.from_scope(connection.scope)
-    scope_state.flash_messages.append({"message": message, "category": category})
+        self.config.template_config.engine_instance.register_template_callable("get_flashes", template_callable)  # pyright: ignore[reportGeneralTypeIssues]
+        return app_config
 
 
-def get_flashes(context: Mapping[str, Any]) -> Any:
-    """Get flash messages from the request scope, if any.
+def flash(
+    request: Request,
+    message: Any,
+    category: str,
+) -> None:
+    request.session.setdefault("_messages", []).append({"message": message, "category": category})
 
-    Args:
-        context: The context dictionary.
 
-    Returns:
-        The flash messages, if any.
-    """
-    scope_state = ScopeState.from_scope(_get_request_from_context(context).scope)
-    return scope_state.flash_messages
+def get_flashes(context: Mapping[str, Any]) -> Any:
+    return _get_request_from_context(context).session.pop("_messages", [])
```

### Comparing `litestar-2.8.2/litestar/plugins/sqlalchemy.py` & `litestar-2.8.3/litestar/plugins/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/plugins/structlog.py` & `litestar-2.8.3/litestar/plugins/structlog.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/repository/_filters.py` & `litestar-2.8.3/litestar/repository/_filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/repository/filters.py` & `litestar-2.8.3/litestar/repository/filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/repository/handlers.py` & `litestar-2.8.3/litestar/repository/handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/repository/abc/_async.py` & `litestar-2.8.3/litestar/repository/abc/_async.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/repository/abc/_sync.py` & `litestar-2.8.3/litestar/repository/abc/_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/repository/testing/generic_mock_repository.py` & `litestar-2.8.3/litestar/repository/testing/generic_mock_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/response/base.py` & `litestar-2.8.3/litestar/response/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/response/file.py` & `litestar-2.8.3/litestar/response/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/response/redirect.py` & `litestar-2.8.3/litestar/response/redirect.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/response/sse.py` & `litestar-2.8.3/litestar/response/sse.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/response/streaming.py` & `litestar-2.8.3/litestar/response/streaming.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/response/template.py` & `litestar-2.8.3/litestar/response/template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/routes/asgi.py` & `litestar-2.8.3/litestar/routes/asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/routes/base.py` & `litestar-2.8.3/litestar/routes/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/routes/http.py` & `litestar-2.8.3/litestar/routes/http.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/routes/websocket.py` & `litestar-2.8.3/litestar/routes/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/security/base.py` & `litestar-2.8.3/litestar/security/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/security/jwt/__init__.py` & `litestar-2.8.3/litestar/security/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/security/jwt/auth.py` & `litestar-2.8.3/litestar/security/jwt/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/security/jwt/middleware.py` & `litestar-2.8.3/litestar/security/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/security/jwt/token.py` & `litestar-2.8.3/litestar/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/security/session_auth/auth.py` & `litestar-2.8.3/litestar/security/session_auth/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/security/session_auth/middleware.py` & `litestar-2.8.3/litestar/security/session_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/serialization/msgspec_hooks.py` & `litestar-2.8.3/litestar/serialization/msgspec_hooks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/static_files/base.py` & `litestar-2.8.3/litestar/static_files/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+# ruff: noqa: PTH118
 from __future__ import annotations
 
-from os.path import commonpath
+import os.path
 from pathlib import Path
 from typing import TYPE_CHECKING, Literal, Sequence
 
 from litestar.enums import ScopeType
 from litestar.exceptions import MethodNotAllowedException, NotFoundException
 from litestar.file_system import FileSystemAdapter
 from litestar.response.file import ASGIFileResponse
 from litestar.status_codes import HTTP_404_NOT_FOUND
 
 __all__ = ("StaticFiles",)
 
-
 if TYPE_CHECKING:
     from litestar.types import Receive, Scope, Send
     from litestar.types.composite_types import PathType
     from litestar.types.file_types import FileInfo, FileSystemProtocol
 
 
 class StaticFiles:
@@ -41,37 +41,47 @@
             file_system: The file_system spec to use for serving files.
             send_as_attachment: Whether to send the file with a ``content-disposition`` header of
              ``attachment`` or ``inline``
             resolve_symlinks: Resolve symlinks to the directories
             headers: Headers that will be sent with every response.
         """
         self.adapter = FileSystemAdapter(file_system)
-        self.directories = tuple(Path(p).resolve() if resolve_symlinks else Path(p) for p in directories)
+        self.directories = tuple(
+            os.path.normpath(Path(p).resolve() if resolve_symlinks else Path(p)) for p in directories
+        )
         self.is_html_mode = is_html_mode
         self.send_as_attachment = send_as_attachment
         self.headers = headers
 
     async def get_fs_info(
         self, directories: Sequence[PathType], file_path: PathType
     ) -> tuple[Path, FileInfo] | tuple[None, None]:
         """Return the resolved path and a :class:`stat_result <os.stat_result>`.
 
+        .. versionchanged:: 2.8.3
+
+            Prevent `CVE-2024-32982 <https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2024-32982>`_
+            by ensuring that the resolved path is within the configured directory as part of `advisory
+            GHSA-83pv-qr33-2vcf <https://github.com/advisories/GHSA-83pv-qr33-2vcf>`_.
+
         Args:
             directories: A list of directory paths.
             file_path: A file path to resolve
 
         Returns:
             A tuple with an optional resolved :class:`Path <anyio.Path>` instance and an optional
             :class:`stat_result <os.stat_result>`.
         """
         for directory in directories:
             try:
                 joined_path = Path(directory, file_path)
-                file_info = await self.adapter.info(joined_path)
-                if file_info and commonpath([str(directory), file_info["name"], joined_path]) == str(directory):
+                normalized_file_path = os.path.normpath(joined_path)
+                if os.path.commonpath([directory, normalized_file_path]) == str(directory) and (
+                    file_info := await self.adapter.info(joined_path)
+                ):
                     return joined_path, file_info
             except FileNotFoundError:
                 continue
         return None, None
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI callable.
```

### Comparing `litestar-2.8.2/litestar/static_files/config.py` & `litestar-2.8.3/litestar/static_files/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/stores/base.py` & `litestar-2.8.3/litestar/stores/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/stores/file.py` & `litestar-2.8.3/litestar/stores/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/stores/memory.py` & `litestar-2.8.3/litestar/stores/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/stores/redis.py` & `litestar-2.8.3/litestar/stores/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types import Empty, EmptyType
 from litestar.utils.empty import value_or_default
 
 from .base import NamespacedStore
 
-__all__ = ("RedisStore",)
-
 if TYPE_CHECKING:
     from types import TracebackType
 
+    from redis.asyncio.connection import Connection
+
+__all__ = ("RedisStore",)
+
 
 class RedisStore(NamespacedStore):
     """Redis based, thread and process safe asynchronous key/value store."""
 
     __slots__ = (
         "_delete_all_script",
         "_get_and_renew_script",
@@ -105,15 +107,15 @@
             url: Redis URL to connect to
             db: Redis database to use
             port: Redis port to use
             username: Redis username to use
             password: Redis password to use
             namespace: Virtual key namespace to use
         """
-        pool = ConnectionPool.from_url(
+        pool: ConnectionPool[Connection] = ConnectionPool.from_url(
             url=url,
             db=db,
             decode_responses=False,
             port=port,
             username=username,
             password=password,
         )
```

### Comparing `litestar-2.8.2/litestar/stores/registry.py` & `litestar-2.8.3/litestar/stores/registry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/template/base.py` & `litestar-2.8.3/litestar/template/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/template/config.py` & `litestar-2.8.3/litestar/template/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/testing/__init__.py` & `litestar-2.8.3/litestar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/testing/helpers.py` & `litestar-2.8.3/litestar/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/testing/life_span_handler.py` & `litestar-2.8.3/litestar/testing/life_span_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/testing/request_factory.py` & `litestar-2.8.3/litestar/testing/request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/testing/transport.py` & `litestar-2.8.3/litestar/testing/transport.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/testing/websocket_test_session.py` & `litestar-2.8.3/litestar/testing/websocket_test_session.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/testing/client/__init__.py` & `litestar-2.8.3/litestar/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/testing/client/async_client.py` & `litestar-2.8.3/litestar/testing/client/async_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/testing/client/base.py` & `litestar-2.8.3/litestar/testing/client/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/testing/client/sync_client.py` & `litestar-2.8.3/litestar/testing/client/sync_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/types/__init__.py` & `litestar-2.8.3/litestar/types/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/types/asgi_types.py` & `litestar-2.8.3/litestar/types/asgi_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/types/builtin_types.py` & `litestar-2.8.3/litestar/types/builtin_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/types/callable_types.py` & `litestar-2.8.3/litestar/types/callable_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/types/composite_types.py` & `litestar-2.8.3/litestar/types/composite_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/types/file_types.py` & `litestar-2.8.3/litestar/types/file_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/types/helper_types.py` & `litestar-2.8.3/litestar/types/helper_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/types/internal_types.py` & `litestar-2.8.3/litestar/types/internal_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/types/protocols.py` & `litestar-2.8.3/litestar/types/protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/types/serialization.py` & `litestar-2.8.3/litestar/types/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/__init__.py` & `litestar-2.8.3/litestar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/compat.py` & `litestar-2.8.3/litestar/utils/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/dataclass.py` & `litestar-2.8.3/litestar/utils/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/deprecation.py` & `litestar-2.8.3/litestar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/empty.py` & `litestar-2.8.3/litestar/utils/empty.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/helpers.py` & `litestar-2.8.3/litestar/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/module_loader.py` & `litestar-2.8.3/litestar/utils/module_loader.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/path.py` & `litestar-2.8.3/litestar/utils/path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/predicates.py` & `litestar-2.8.3/litestar/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/sequence.py` & `litestar-2.8.3/litestar/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/signature.py` & `litestar-2.8.3/litestar/utils/signature.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/sync.py` & `litestar-2.8.3/litestar/utils/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/typing.py` & `litestar-2.8.3/litestar/utils/typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/version.py` & `litestar-2.8.3/litestar/utils/version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/warnings.py` & `litestar-2.8.3/litestar/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/scope/__init__.py` & `litestar-2.8.3/litestar/utils/scope/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/litestar/utils/scope/state.py` & `litestar-2.8.3/litestar/utils/scope/state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/conftest.py` & `litestar-2.8.3/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import random
 import string
 import sys
 from datetime import datetime
 from os import urandom
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable, Generator, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable, Generator, Union, cast
 from unittest.mock import AsyncMock, MagicMock
 
 import pytest
 from pytest_lazy_fixtures import lf
 from redis.asyncio import Redis as AsyncRedis
 from redis.client import Redis
 from time_machine import travel
@@ -26,14 +26,15 @@
 from litestar.middleware.session.server_side import ServerSideSessionBackend, ServerSideSessionConfig
 from litestar.openapi.config import OpenAPIConfig
 from litestar.stores.base import Store
 from litestar.stores.file import FileStore
 from litestar.stores.memory import MemoryStore
 from litestar.stores.redis import RedisStore
 from litestar.testing import RequestFactory
+from tests.helpers import not_none
 
 if TYPE_CHECKING:
     from types import ModuleType
 
     from pytest import FixtureRequest, MonkeyPatch
     from time_machine import Coordinates
 
@@ -224,19 +225,14 @@
 
         Args:
             source: Source code as a string.
 
         Returns:
             An imported module.
         """
-        T = TypeVar("T")
-
-        def not_none(val: T | T | None) -> T:
-            assert val is not None
-            return val
 
         def module_name_generator() -> str:
             letters = string.ascii_lowercase
             return "".join(random.choice(letters) for _ in range(10))
 
         module_name = module_name_generator()
         path = tmp_path / f"{module_name}.py"
```

### Comparing `litestar-2.8.2/tests/docker_service_fixtures.py` & `litestar-2.8.3/tests/docker_service_fixtures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/helpers.py` & `litestar-2.8.3/tests/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,7 +102,12 @@
     # else the test suite would hang on at the end of the tests and some tests would fail)
     queue_listener_handler = getHandlerByName("queue_listener")
     if queue_listener_handler and hasattr(queue_listener_handler, "listener"):
         atexit.unregister(queue_listener_handler.listener.stop)
         queue_listener_handler.listener.stop()
         queue_listener_handler.close()
         del queue_listener_handler
+
+
+def not_none(val: T | None) -> T:
+    assert val is not None
+    return val
```

### Comparing `litestar-2.8.2/tests/models.py` & `litestar-2.8.3/tests/models.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_advanced_alchemy.py` & `litestar-2.8.3/tests/e2e/test_advanced_alchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_exception_handlers.py` & `litestar-2.8.3/tests/e2e/test_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_option_requests.py` & `litestar-2.8.3/tests/e2e/test_option_requests.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_pydantic.py` & `litestar-2.8.3/tests/e2e/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_response_caching.py` & `litestar-2.8.3/tests/e2e/test_response_caching.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_router_registration.py` & `litestar-2.8.3/tests/e2e/test_router_registration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_starlette_responses.py` & `litestar-2.8.3/tests/e2e/test_starlette_responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_dependency_injection/test_dependency_validation.py` & `litestar-2.8.3/tests/e2e/test_dependency_injection/test_dependency_validation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py` & `litestar-2.8.3/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_dependency_injection/test_injection_of_classes.py` & `litestar-2.8.3/tests/e2e/test_dependency_injection/test_injection_of_classes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py` & `litestar-2.8.3/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_dependency_injection/test_inter_dependencies.py` & `litestar-2.8.3/tests/e2e/test_dependency_injection/test_inter_dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_dependency_injection/test_request_local_caching.py` & `litestar-2.8.3/tests/e2e/test_dependency_injection/test_request_local_caching.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py` & `litestar-2.8.3/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_life_cycle_hooks/test_after_request.py` & `litestar-2.8.3/tests/e2e/test_life_cycle_hooks/test_after_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_life_cycle_hooks/test_after_response.py` & `litestar-2.8.3/tests/e2e/test_life_cycle_hooks/test_after_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_life_cycle_hooks/test_before_request.py` & `litestar-2.8.3/tests/e2e/test_life_cycle_hooks/test_before_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_routing/conftest.py` & `litestar-2.8.3/tests/e2e/test_routing/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_routing/test_asset_url_path.py` & `litestar-2.8.3/tests/e2e/test_routing/test_asset_url_path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_routing/test_path_mounting.py` & `litestar-2.8.3/tests/e2e/test_routing/test_path_mounting.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_routing/test_path_resolution.py` & `litestar-2.8.3/tests/e2e/test_routing/test_path_resolution.py`

 * *Files 7% similar despite different names*

```diff
@@ -356,7 +356,55 @@
 app = Litestar(route_handlers=[pathfinder], debug=True)
     """
 
     run_server(app, server_command)
 
     assert httpx.get("http://127.0.0.1:9999/").text == "None"
     assert httpx.get("http://127.0.0.1:9999/something").text == "/something"
+
+
+@pytest.mark.parametrize(
+    "server_command",
+    [
+        pytest.param(["uvicorn", "app:app", "--port", "9999", "--root-path", "/test"], id="uvicorn"),
+        pytest.param(["hypercorn", "app:app", "--bind", "127.0.0.1:9999", "--root-path", "/test"], id="hypercorn"),
+        pytest.param(["daphne", "app:app", "--port", "9999", "--root-path", "/test"], id="daphne"),
+    ],
+)
+@pytest.mark.xdist_group("live_server_test")
+@pytest.mark.server_integration
+def test_no_path_traversal_from_static_directory(
+    tmp_path: Path, monkeypatch: MonkeyPatch, server_command: List[str], run_server: Callable[[str, List[str]], None]
+) -> None:
+    import http.client
+
+    static = tmp_path / "static"
+    static.mkdir()
+    (static / "index.html").write_text("Hello, World!")
+
+    app = """
+from pathlib import Path
+from litestar import Litestar
+from litestar.static_files import create_static_files_router
+import uvicorn
+
+app = Litestar(
+    route_handlers=[
+        create_static_files_router(path="/static", directories=["static"]),
+    ],
+)
+    """
+
+    def send_request(host: str, port: int, path: str) -> http.client.HTTPResponse:
+        connection = http.client.HTTPConnection(host, port)
+        connection.request("GET", path)
+        resp = connection.getresponse()
+        connection.close()
+        return resp
+
+    run_server(app, server_command)
+
+    response = send_request("127.0.0.1", 9999, "/static/index.html")
+    assert response.status == 200
+
+    response = send_request("127.0.0.1", 9999, "/static/../app.py")
+    assert response.status == 404
```

### Comparing `litestar-2.8.2/tests/e2e/test_routing/test_route_indexing.py` & `litestar-2.8.3/tests/e2e/test_routing/test_route_indexing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_routing/test_route_reverse.py` & `litestar-2.8.3/tests/e2e/test_routing/test_route_reverse.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/e2e/test_routing/test_validations.py` & `litestar-2.8.3/tests/e2e/test_routing/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_cache_control_headers.py` & `litestar-2.8.3/tests/examples/test_cache_control_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_exceptions.py` & `litestar-2.8.3/tests/examples/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_lifecycle_hooks.py` & `litestar-2.8.3/tests/examples/test_lifecycle_hooks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_request_data.py` & `litestar-2.8.3/tests/examples/test_request_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_routing.py` & `litestar-2.8.3/tests/examples/test_routing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_startup_and_shutdown.py` & `litestar-2.8.3/tests/examples/test_startup_and_shutdown.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_static_files.py` & `litestar-2.8.3/tests/examples/test_static_files.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_stores.py` & `litestar-2.8.3/tests/examples/test_stores.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_todo_app.py` & `litestar-2.8.3/tests/examples/test_todo_app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_using_session_auth.py` & `litestar-2.8.3/tests/examples/test_using_session_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_application_hooks/test_application_after_exception_hook.py` & `litestar-2.8.3/tests/examples/test_application_hooks/test_application_after_exception_hook.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_application_hooks/test_lifespan_manager.py` & `litestar-2.8.3/tests/examples/test_application_hooks/test_lifespan_manager.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_application_state/test_using_application_state.py` & `litestar-2.8.3/tests/examples/test_application_state/test_using_application_state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_contrib/test_piccolo_orm.py` & `litestar-2.8.3/tests/examples/test_contrib/test_piccolo_orm.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py` & `litestar-2.8.3/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py` & `litestar-2.8.3/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py` & `litestar-2.8.3/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py` & `litestar-2.8.3/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_dto/test_example_apps.py` & `litestar-2.8.3/tests/examples/test_dto/test_example_apps.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,12 @@
 from __future__ import annotations
 
-from unittest.mock import ANY
-
 from litestar.testing import TestClient
 
 
-def test_dto_data_problem_statement_app() -> None:
-    from docs.examples.data_transfer_objects.factory.dto_data_problem_statement import app
-
-    with TestClient(app) as client:
-        response = client.post("/person", json={"name": "John", "age": 30})
-        assert response.status_code == 500
-
-
-def test_dto_data_usage_app() -> None:
-    from docs.examples.data_transfer_objects.factory.dto_data_usage import app
-
-    with TestClient(app) as client:
-        response = client.post("/person", json={"name": "John", "age": 30})
-        assert response.status_code == 201
-        assert response.json() == {"id": ANY, "name": "John", "age": 30}
-
-
 def test_dto_data_nested_data_create_instance_app() -> None:
     from docs.examples.data_transfer_objects.factory.providing_values_for_nested_data import app
 
     with TestClient(app) as client:
         response = client.post(
             "/person",
             json={
```

### Comparing `litestar-2.8.2/tests/examples/test_dto/test_tutorial.py` & `litestar-2.8.3/tests/examples/test_dto/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_middleware/test_abstract_middleware.py` & `litestar-2.8.3/tests/examples/test_middleware/test_abstract_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_middleware/test_logging_middleware.py` & `litestar-2.8.3/tests/examples/test_middleware/test_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_middleware/test_session_middleware.py` & `litestar-2.8.3/tests/examples/test_middleware/test_session_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_openapi/test_openapi.py` & `litestar-2.8.3/tests/examples/test_openapi/test_openapi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_openapi/test_plugins.py` & `litestar-2.8.3/tests/examples/test_openapi/test_plugins.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_pagination/test_using_classic_pagination.py` & `litestar-2.8.3/tests/examples/test_pagination/test_using_classic_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_pagination/test_using_cursor_pagination.py` & `litestar-2.8.3/tests/examples/test_pagination/test_using_cursor_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_pagination/test_using_offset_pagination.py` & `litestar-2.8.3/tests/examples/test_pagination/test_using_offset_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_parameters/test_header_and_cookies_parameters.py` & `litestar-2.8.3/tests/examples/test_parameters/test_header_and_cookies_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_parameters/test_layered_parameters.py` & `litestar-2.8.3/tests/examples/test_parameters/test_layered_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_parameters/test_path_parameters.py` & `litestar-2.8.3/tests/examples/test_parameters/test_path_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_parameters/test_query_parameters.py` & `litestar-2.8.3/tests/examples/test_parameters/test_query_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py` & `litestar-2.8.3/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_responses/test_background_tasks.py` & `litestar-2.8.3/tests/examples/test_responses/test_background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_responses/test_response_cookies.py` & `litestar-2.8.3/tests/examples/test_responses/test_response_cookies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_responses/test_response_headers.py` & `litestar-2.8.3/tests/examples/test_responses/test_response_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_security/test_jwt/test_using_jwt_auth.py` & `litestar-2.8.3/tests/examples/test_security/test_jwt/test_using_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py` & `litestar-2.8.3/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py` & `litestar-2.8.3/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_templating/test_engine_instance.py` & `litestar-2.8.3/tests/examples/test_templating/test_engine_instance.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_templating/test_returning_templates.py` & `litestar-2.8.3/tests/examples/test_templating/test_returning_templates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/examples/test_templating/test_template_functions.py` & `litestar-2.8.3/tests/examples/test_templating/test_template_functions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/conftest.py` & `litestar-2.8.3/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_app.py` & `litestar-2.8.3/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_asgi_router.py` & `litestar-2.8.3/tests/unit/test_asgi_router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_background_tasks.py` & `litestar-2.8.3/tests/unit/test_background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_concurrency.py` & `litestar-2.8.3/tests/unit/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_controller.py` & `litestar-2.8.3/tests/unit/test_controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_data_extractors.py` & `litestar-2.8.3/tests/unit/test_data_extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_deprecations.py` & `litestar-2.8.3/tests/unit/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_di.py` & `litestar-2.8.3/tests/unit/test_di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_events.py` & `litestar-2.8.3/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_exceptions.py` & `litestar-2.8.3/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_file_system.py` & `litestar-2.8.3/tests/unit/test_file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_guards.py` & `litestar-2.8.3/tests/unit/test_guards.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_pagination.py` & `litestar-2.8.3/tests/unit/test_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_params.py` & `litestar-2.8.3/tests/unit/test_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_parsers.py` & `litestar-2.8.3/tests/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_request_class_resolution.py` & `litestar-2.8.3/tests/unit/test_request_class_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_response_class_resolution.py` & `litestar-2.8.3/tests/unit/test_response_class_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_stores.py` & `litestar-2.8.3/tests/unit/test_stores.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_typing.py` & `litestar-2.8.3/tests/unit/test_typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any, ForwardRef, Generic, List, Optional, Tuple, TypeVar, Union
 
 import annotated_types
 import msgspec
 import pytest
 from typing_extensions import Annotated, NotRequired, Required, TypedDict, get_type_hints
 
+from litestar import get
 from litestar.exceptions import LitestarWarning
 from litestar.params import DependencyKwarg, KwargDefinition, Parameter, ParameterKwarg
 from litestar.typing import FieldDefinition, _unpack_predicate
 
 from .test_utils.test_signature import T, _check_field_definition, field_definition_int, test_type_hints
 
 
@@ -457,7 +458,21 @@
     with pytest.warns(LitestarWarning, match="Ambiguous default values"):
         FieldDefinition.from_annotation(Annotated[int, Parameter(default=1)], default=2)
 
 
 def test_warn_defaults_inside_parameter_definition() -> None:
     with pytest.warns(DeprecationWarning, match="Deprecated default value specification"):
         FieldDefinition.from_annotation(Annotated[int, Parameter(default=1)], default=1)
+
+
+def test_warn_default_inside_kwarg_definition_and_default_empty() -> None:
+    with pytest.warns() as warnings:
+
+        @get(sync_to_thread=False)
+        def handler(foo: Annotated[int, Parameter(default=1)]) -> None:
+            pass
+
+        _ = handler.parsed_fn_signature
+
+    (record,) = warnings
+    assert record.category == DeprecationWarning
+    assert "Deprecated default value specification" in str(record.message)
```

### Comparing `litestar-2.8.2/tests/unit/test_websocket_class_resolution.py` & `litestar-2.8.3/tests/unit/test_websocket_class_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_channels/conftest.py` & `litestar-2.8.3/tests/unit/test_channels/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_channels/test_backends.py` & `litestar-2.8.3/tests/unit/test_channels/test_backends.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_channels/test_plugin.py` & `litestar-2.8.3/tests/unit/test_channels/test_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         channels_plugin.publish(["foo"], "something")
         # send some arbitrary message
         ws.send("bar")
         # the subscription should still be alive
         assert ws.receive_json(timeout=2) == ["foo"]
 
 
-@pytest.mark.flaky(reruns=5)
+@pytest.mark.flaky(reruns=15)
 def test_create_ws_route_handlers_arbitrary_channels_allowed(channels_backend: ChannelsBackend) -> None:
     channels_plugin = ChannelsPlugin(
         backend=channels_backend,
         arbitrary_channels_allowed=True,
         create_ws_route_handlers=True,
         ws_handler_base_path="/ws",
     )
```

### Comparing `litestar-2.8.2/tests/unit/test_channels/test_subscriber.py` & `litestar-2.8.3/tests/unit/test_channels/test_subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_cli/__init__.py` & `litestar-2.8.3/tests/unit/test_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_cli/conftest.py` & `litestar-2.8.3/tests/unit/test_cli/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_cli/test_cli.py` & `litestar-2.8.3/tests/unit/test_cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_cli/test_cli_plugin.py` & `litestar-2.8.3/tests/unit/test_cli/test_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_cli/test_core_commands.py` & `litestar-2.8.3/tests/unit/test_cli/test_core_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,15 @@
     env_name, env_value = env
     cli_name, cli_value = cli
 
     if env_name:
         if isinstance(env_value, list):
             monkeypatch.setenv(env_name, "".join(env_value))
         else:
-            monkeypatch.setenv(env_name, env_value)  # type: ignore[arg-type] # pyright: ignore (reportGeneralTypeIssues)
+            monkeypatch.setenv(env_name, str(env_value))
 
     if cli_name:
         if cli_value is True:
             args.append(cli_name)
         elif isinstance(cli_value, list):
             for value in cli_value:
                 args.extend([cli_name, value])
```

### Comparing `litestar-2.8.2/tests/unit/test_cli/test_env_resolution.py` & `litestar-2.8.3/tests/unit/test_cli/test_env_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_cli/test_schema_commands.py` & `litestar-2.8.3/tests/unit/test_cli/test_schema_commands.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_cli/test_session_commands.py` & `litestar-2.8.3/tests/unit/test_cli/test_session_commands.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_cli/test_ssl.py` & `litestar-2.8.3/tests/unit/test_cli/test_ssl.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_connection/test_base.py` & `litestar-2.8.3/tests/unit/test_connection/test_base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_connection/test_connection_caching.py` & `litestar-2.8.3/tests/unit/test_connection/test_connection_caching.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_connection/test_request.py` & `litestar-2.8.3/tests/unit/test_connection/test_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_connection/test_websocket.py` & `litestar-2.8.3/tests/unit/test_connection/test_websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/conftest.py` & `litestar-2.8.3/tests/unit/test_contrib/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_minijinja.py` & `litestar-2.8.3/tests/unit/test_contrib/test_minijinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_msgspec.py` & `litestar-2.8.3/tests/unit/test_contrib/test_msgspec.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_opentelemetry.py` & `litestar-2.8.3/tests/unit/test_contrib/test_opentelemetry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_prometheus.py` & `litestar-2.8.3/tests/unit/test_contrib/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_repository.py` & `litestar-2.8.3/tests/unit/test_contrib/test_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_sqlalchemy.py` & `litestar-2.8.3/tests/unit/test_contrib/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py` & `litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_attrs/test_schema_plugin.py` & `litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py` & `litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_attrs/test_signature.py` & `litestar-2.8.3/tests/unit/test_contrib/test_attrs/test_signature.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_htmx/test_htmx_request.py` & `litestar-2.8.3/tests/unit/test_contrib/test_htmx/test_htmx_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_htmx/test_htmx_response.py` & `litestar-2.8.3/tests/unit/test_contrib/test_htmx/test_htmx_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_piccolo_orm/endpoints.py` & `litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/endpoints.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py` & `litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_piccolo_orm/tables.py` & `litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/tables.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py` & `litestar-2.8.3/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_pydantic/models.py` & `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/models.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py` & `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_dto.py` & `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py` & `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_integration.py` & `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_openapi.py` & `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_openapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import date, datetime, timedelta
+from datetime import date, datetime, timedelta, timezone
 from decimal import Decimal
 from types import ModuleType
 from typing import Any, Callable, Pattern, Type, Union, cast
 
 import pydantic as pydantic_v2
 import pytest
 from pydantic import v1 as pydantic_v1
@@ -253,57 +253,85 @@
 def test_create_date_constrained_field_schema_pydantic_v1(annotation: Any) -> None:
     field_definition = FieldDefinition.from_annotation(annotation)
 
     assert isinstance(field_definition.kwarg_definition, KwargDefinition)
     schema = create_date_constrained_field_schema(field_definition.annotation, field_definition.kwarg_definition)
     assert schema.type == OpenAPIType.STRING
     assert schema.format == OpenAPIFormat.DATE
-    assert (datetime.utcfromtimestamp(schema.exclusive_minimum) if schema.exclusive_minimum else None) == (
-        datetime.fromordinal(annotation.gt.toordinal()) if annotation.gt is not None else None
+    assert (
+        datetime.fromtimestamp(schema.exclusive_minimum, tz=timezone.utc) if schema.exclusive_minimum else None
+    ) == (
+        datetime.fromordinal(annotation.gt.toordinal()).replace(tzinfo=timezone.utc)
+        if annotation.gt is not None
+        else None
     )
-    assert (datetime.utcfromtimestamp(schema.minimum) if schema.minimum else None) == (
-        datetime.fromordinal(annotation.ge.toordinal()) if annotation.ge is not None else None
+    assert (datetime.fromtimestamp(schema.minimum, tz=timezone.utc) if schema.minimum else None) == (
+        datetime.fromordinal(annotation.ge.toordinal()).replace(tzinfo=timezone.utc)
+        if annotation.ge is not None
+        else None
     )
-    assert (datetime.utcfromtimestamp(schema.exclusive_maximum) if schema.exclusive_maximum else None) == (
-        datetime.fromordinal(annotation.lt.toordinal()) if annotation.lt is not None else None
+    assert (
+        datetime.fromtimestamp(schema.exclusive_maximum, tz=timezone.utc) if schema.exclusive_maximum else None
+    ) == (
+        datetime.fromordinal(annotation.lt.toordinal()).replace(tzinfo=timezone.utc)
+        if annotation.lt is not None
+        else None
     )
-    assert (datetime.utcfromtimestamp(schema.maximum) if schema.maximum else None) == (
-        datetime.fromordinal(annotation.le.toordinal()) if annotation.le is not None else None
+    assert (datetime.fromtimestamp(schema.maximum, tz=timezone.utc) if schema.maximum else None) == (
+        datetime.fromordinal(annotation.le.toordinal()).replace(tzinfo=timezone.utc)
+        if annotation.le is not None
+        else None
     )
 
 
 @pytest.mark.parametrize("annotation", constrained_dates_v2)
 def test_create_date_constrained_field_schema_pydantic_v2(annotation: Any) -> None:
     field_definition = FieldDefinition.from_annotation(annotation)
 
     assert isinstance(field_definition.kwarg_definition, KwargDefinition)
     schema = create_date_constrained_field_schema(field_definition.annotation, field_definition.kwarg_definition)
     assert schema.type == OpenAPIType.STRING
     assert schema.format == OpenAPIFormat.DATE
     assert any(
-        (datetime.fromordinal(getattr(m, "gt", None).toordinal()) if getattr(m, "gt", None) is not None else None)  # type: ignore[union-attr]
-        == (datetime.utcfromtimestamp(schema.exclusive_minimum) if schema.exclusive_minimum else None)
+        (
+            datetime.fromordinal(getattr(m, "gt", None).toordinal()).replace(tzinfo=timezone.utc)  # type: ignore[union-attr]
+            if getattr(m, "gt", None) is not None
+            else None
+        )
+        == (datetime.fromtimestamp(schema.exclusive_minimum, tz=timezone.utc) if schema.exclusive_minimum else None)
         for m in field_definition.metadata
         if m
     )
     assert any(
-        (datetime.fromordinal(getattr(m, "ge", None).toordinal()) if getattr(m, "ge", None) is not None else None)  # type: ignore[union-attr]
-        == (datetime.utcfromtimestamp(schema.minimum) if schema.minimum else None)
+        (
+            datetime.fromordinal(getattr(m, "ge", None).toordinal()).replace(tzinfo=timezone.utc)  # type: ignore[union-attr]
+            if getattr(m, "ge", None) is not None
+            else None
+        )
+        == (datetime.fromtimestamp(schema.minimum, tz=timezone.utc) if schema.minimum else None)
         for m in field_definition.metadata
         if m
     )
     assert any(
-        (datetime.fromordinal(getattr(m, "lt", None).toordinal()) if getattr(m, "lt", None) is not None else None)  # type: ignore[union-attr]
-        == (datetime.utcfromtimestamp(schema.exclusive_maximum) if schema.exclusive_maximum else None)
+        (
+            datetime.fromordinal(getattr(m, "lt", None).toordinal()).replace(tzinfo=timezone.utc)  # type: ignore[union-attr]
+            if getattr(m, "lt", None) is not None
+            else None
+        )
+        == (datetime.fromtimestamp(schema.exclusive_maximum, tz=timezone.utc) if schema.exclusive_maximum else None)
         for m in field_definition.metadata
         if m
     )
     assert any(
-        (datetime.fromordinal(getattr(m, "le", None).toordinal()) if getattr(m, "le", None) is not None else None)  # type: ignore[union-attr]
-        == (datetime.utcfromtimestamp(schema.maximum) if schema.maximum else None)
+        (
+            datetime.fromordinal(getattr(m, "le", None).toordinal()).replace(tzinfo=timezone.utc)  # type: ignore[union-attr]
+            if getattr(m, "le", None) is not None
+            else None
+        )
+        == (datetime.fromtimestamp(schema.maximum, tz=timezone.utc) if schema.maximum else None)
         for m in field_definition.metadata
         if m
     )
 
 
 @pytest.mark.parametrize(
     "annotation",
```

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py` & `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py` & `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py` & `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_contrib/test_pydantic/test_utils.py` & `litestar-2.8.3/tests/unit/test_contrib/test_pydantic/test_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_datastructures/test_cookie.py` & `litestar-2.8.3/tests/unit/test_datastructures/test_cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_datastructures/test_headers.py` & `litestar-2.8.3/tests/unit/test_datastructures/test_headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
     header_dict = simple_asdict(header, exclude_none=True)
     assert header_dict == {"no_store": True, "documentation_only": False}
 
 
 def test_cache_control_header_unsupported_type_annotation() -> None:
     @dataclass
     class InvalidCacheControlHeader(CacheControlHeader):
-        unsupported_type: Union[int, str] = "foo"
+        foo_field: Union[int, str] = "foo"
 
     with pytest.raises(ImproperlyConfiguredException):
         InvalidCacheControlHeader.from_header("unsupported_type")
 
 
 def test_etag_documentation_only() -> None:
     assert ETag(documentation_only=True).value is None
```

### Comparing `litestar-2.8.2/tests/unit/test_datastructures/test_multi_dicts.py` & `litestar-2.8.3/tests/unit/test_datastructures/test_multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_datastructures/test_state.py` & `litestar-2.8.3/tests/unit/test_datastructures/test_state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_datastructures/test_upload_file.py` & `litestar-2.8.3/tests/unit/test_datastructures/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_datastructures/test_url.py` & `litestar-2.8.3/tests/unit/test_datastructures/test_url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_dto/conftest.py` & `litestar-2.8.3/tests/unit/test_dto/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 
 from typing import Any, Collection, Generator, TypeVar, get_type_hints
 
 import pytest
 
 from litestar import Request, get
 from litestar._openapi.schema_generation import SchemaCreator
-from litestar.dto import AbstractDTO, DTOField, DTOFieldDefinition
+from litestar.dto import AbstractDTO, DTOConfig, DTOField, DTOFieldDefinition
 from litestar.enums import MediaType
 from litestar.openapi.spec import Reference, Schema
 from litestar.testing import RequestFactory
 from litestar.types.serialization import LitestarEncodableType
 from litestar.typing import FieldDefinition
 
 from . import Model
 
 T = TypeVar("T", bound=Model)
 
 
 @pytest.fixture
-def ModelDataDTO() -> type[AbstractDTO]:
+def ModelDataDTO(use_experimental_dto_backend: bool) -> type[AbstractDTO]:
     class DTOCls(AbstractDTO[Model]):
+        config = DTOConfig(experimental_codegen_backend=use_experimental_dto_backend)
+
         def decode_builtins(self, value: Any) -> Model:
             return Model(a=1, b="2")
 
         def decode_bytes(self, value: bytes) -> Model:
             return Model(a=1, b="2")
 
         def data_to_encodable_type(self, data: Model | Collection[Model]) -> bytes | LitestarEncodableType:
```

### Comparing `litestar-2.8.2/tests/unit/test_dto/test_factory/test_base_dto.py` & `litestar-2.8.3/tests/unit/test_dto/test_factory/test_base_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_dto/test_factory/test_dataclass_dto.py` & `litestar-2.8.3/tests/unit/test_dto/test_factory/test_dataclass_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_dto/test_factory/test_integration.py` & `litestar-2.8.3/tests/unit/test_dto/test_factory/test_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,27 @@
 
 from litestar import Controller, Response, get, patch, post
 from litestar.connection.request import Request
 from litestar.datastructures import UploadFile
 from litestar.dto import DataclassDTO, DTOConfig, DTOData, MsgspecDTO, dto_field
 from litestar.dto.types import RenameStrategy
 from litestar.enums import MediaType, RequestEncodingType
+from litestar.openapi.spec.response import OpenAPIResponse
+from litestar.openapi.spec.schema import Schema
 from litestar.pagination import ClassicPagination, CursorPagination, OffsetPagination
 from litestar.params import Body
 from litestar.serialization import encode_json
 from litestar.testing import create_test_client
+from tests.helpers import not_none
 
 if TYPE_CHECKING:
     from typing import Any
 
+    from litestar import Litestar
+
 
 def test_url_encoded_form_data(use_experimental_dto_backend: bool) -> None:
     @dataclass()
     class User:
         name: str
         age: int
         read_only: str = field(default="read-only", metadata=dto_field("read-only"))
@@ -894,7 +899,107 @@
 
     @post("/", dto=FooDTO, signature_types={Foo})
     def handler(data: Foo) -> None:
         pass
 
     with create_test_client([handler]) as client:
         assert client.post("/", json={"bar": "1", "baz": "123"}).status_code == 201
+
+
+def test_openapi_schema_for_type_with_generic_pagination_type(
+    create_module: Callable[[str], ModuleType], use_experimental_dto_backend: bool
+) -> None:
+    module = create_module(
+        """
+from dataclasses import dataclass
+
+from litestar import Litestar, get
+from litestar.dto import DataclassDTO
+from litestar.pagination import ClassicPagination
+
+@dataclass
+class Test:
+    name: str
+    age: int
+
+@get("/without-dto", sync_to_thread=False)
+def without_dto() -> ClassicPagination[Test]:
+    return ClassicPagination(
+        items=[Test("John", 25), Test("Jane", 30)],
+        page_size=1,
+        current_page=2,
+        total_pages=2,
+    )
+
+@get("/with-dto", return_dto=DataclassDTO[Test], sync_to_thread=False)
+def with_dto() -> ClassicPagination[Test]:
+    return ClassicPagination(
+        items=[Test("John", 25), Test("Jane", 30)],
+        page_size=1,
+        current_page=2,
+        total_pages=2,
+    )
+
+app = Litestar([without_dto, with_dto])
+"""
+    )
+    openapi = cast("Litestar", module.app).openapi_schema
+    paths = not_none(openapi.paths)
+    without_dto_response = not_none(not_none(paths["/without-dto"].get).responses)["200"]
+    with_dto_response = not_none(not_none(paths["/with-dto"].get).responses)["200"]
+    assert isinstance(without_dto_response, OpenAPIResponse)
+    assert isinstance(with_dto_response, OpenAPIResponse)
+    without_dto_schema = not_none(without_dto_response.content)["application/json"].schema
+    with_dto_schema = not_none(with_dto_response.content)["application/json"].schema
+    assert isinstance(without_dto_schema, Schema)
+    assert isinstance(with_dto_schema, Schema)
+    assert not_none(without_dto_schema.properties).keys() == not_none(with_dto_schema.properties).keys()
+
+
+def test_openapi_schema_for_type_with_custom_generic_type(
+    create_module: Callable[[str], ModuleType], use_experimental_dto_backend: bool
+) -> None:
+    module = create_module(
+        """
+from dataclasses import dataclass
+from datetime import datetime
+from typing import Generic, List, TypeVar
+
+from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column
+
+from litestar import Litestar, get
+from litestar.contrib.sqlalchemy.dto import SQLAlchemyDTO
+from litestar.dto import DTOConfig
+
+T = TypeVar("T")
+
+@dataclass
+class WithCount(Generic[T]):
+    count: int
+    data: List[T]
+
+class Base(DeclarativeBase): ...
+
+class User(Base):
+    __tablename__ = "user"
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+    password: Mapped[str]
+    created_at: Mapped[datetime]
+
+class UserDTO(SQLAlchemyDTO[User]):
+    config = DTOConfig(exclude={"password", "created_at"})
+
+@get("/users", dto=UserDTO, sync_to_thread=False)
+def get_users() -> WithCount[User]:
+    return WithCount(
+        count=1, data=[User(id=1, name="Litestar User", password="xyz", created_at=datetime.now())]
+    )
+
+app = Litestar(route_handlers=[get_users])
+"""
+    )
+    openapi = cast("Litestar", module.app).openapi_schema
+    schema = openapi.components.schemas["WithCount[litestar.dto._backend.GetUsersUserResponseBody]"]
+    assert not_none(schema.properties).keys() == {"count", "data"}
+    model_schema = openapi.components.schemas["GetUsersUserResponseBody"]
+    assert not_none(model_schema.properties).keys() == {"id", "name"}
```

### Comparing `litestar-2.8.2/tests/unit/test_dto/test_factory/test_utils.py` & `litestar-2.8.3/tests/unit/test_dto/test_factory/test_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_dto/test_factory/test_backends/test_backends.py` & `litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/test_backends.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py` & `litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_dto/test_factory/test_backends/test_utils.py` & `litestar-2.8.3/tests/unit/test_dto/test_factory/test_backends/test_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py` & `litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py` & `litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_asgi_handlers/test_validations.py` & `litestar-2.8.3/tests/unit/test_handlers/test_asgi_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_base_handlers/test_opt.py` & `litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/test_opt.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_base_handlers/test_resolution.py` & `litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/test_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_base_handlers/test_validations.py` & `litestar-2.8.3/tests/unit/test_handlers/test_base_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_defaults.py` & `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_defaults.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_head.py` & `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_head.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py` & `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_media_type.py` & `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py` & `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_sync.py` & `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_http_handlers/test_validations.py` & `litestar-2.8.3/tests/unit/test_handlers/test_http_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py` & `litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py` & `litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py` & `litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py` & `litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_handlers/test_websocket_handlers/test_validations.py` & `litestar-2.8.3/tests/unit/test_handlers/test_websocket_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/flower.jpeg` & `litestar-2.8.3/tests/unit/test_kwargs/flower.jpeg`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_cleanup_group.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_cleanup_group.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_cookie_params.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_cookie_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_defaults.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_defaults.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_dependency_batches.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_dependency_batches.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_generator_dependencies.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_generator_dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_header_params.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_header_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_json_data.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_json_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_layered_params.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_layered_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_msgpack_data.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_msgpack_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_multipart_data.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_multipart_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -390,18 +390,23 @@
         route_handlers=[hello_world]
     ) as client:
         data = f.read()
         response = client.post("/", files={"data": data})
         assert response.status_code == HTTP_201_CREATED
 
 
+@pytest.mark.parametrize("optional", [True, False])
 @pytest.mark.parametrize("file_count", (1, 2))
-def test_upload_multiple_files(file_count: int) -> None:
-    @post("/")
-    async def handler(data: List[UploadFile] = Body(media_type=RequestEncodingType.MULTI_PART)) -> None:
+def test_upload_multiple_files(file_count: int, optional: bool) -> None:
+    annotation = List[UploadFile]
+    if optional:
+        annotation = Optional[annotation]  # type: ignore[misc, assignment]
+
+    @post("/", signature_namespace={"annotation": annotation})
+    async def handler(data: annotation = Body(media_type=RequestEncodingType.MULTI_PART)) -> None:  # pyright: ignore[reportGeneralTypeIssues]
         assert len(data) == file_count
 
         for file in data:
             assert await file.read() == b"1"
 
     with create_test_client([handler]) as client:
         files_to_upload = [("file", b"1") for _ in range(file_count)]
@@ -411,21 +416,28 @@
 
 
 @dataclass
 class Files:
     file_list: List[UploadFile]
 
 
+# https://github.com/litestar-org/litestar/issues/3407
+@dataclass
+class OptionalFiles:
+    file_list: Optional[List[UploadFile]]
+
+
+@pytest.mark.parametrize("file_model", (Files, OptionalFiles))
 @pytest.mark.parametrize("file_count", (1, 2))
-def test_upload_multiple_files_in_model(file_count: int) -> None:
-    @post("/")
-    async def handler(data: Files = Body(media_type=RequestEncodingType.MULTI_PART)) -> None:
-        assert len(data.file_list) == file_count
+def test_upload_multiple_files_in_model(file_count: int, file_model: type[Files | OptionalFiles]) -> None:
+    @post("/", signature_namespace={"file_model": file_model})
+    async def handler(data: file_model = Body(media_type=RequestEncodingType.MULTI_PART)) -> None:  # type: ignore[valid-type]
+        assert len(data.file_list) == file_count  # type: ignore[attr-defined]
 
-        for file in data.file_list:
+        for file in data.file_list:  # type: ignore[attr-defined]
             assert await file.read() == b"1"
 
     with create_test_client([handler]) as client:
         files_to_upload = [("file_list", b"1") for _ in range(file_count)]
         response = client.post("/", files=files_to_upload)
 
         assert response.status_code == HTTP_201_CREATED
```

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_path_params.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_path_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_query_params.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_query_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_reserved_kwargs_injection.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_reserved_kwargs_injection.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_url_encoded_data.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_url_encoded_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_kwargs/test_validations.py` & `litestar-2.8.3/tests/unit/test_kwargs/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_logging/test_logging_config.py` & `litestar-2.8.3/tests/unit/test_logging/test_logging_config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_logging/test_structlog_config.py` & `litestar-2.8.3/tests/unit/test_logging/test_structlog_config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_allowed_hosts_middleware.py` & `litestar-2.8.3/tests/unit/test_middleware/test_allowed_hosts_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_base_authentication_middleware.py` & `litestar-2.8.3/tests/unit/test_middleware/test_base_authentication_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_base_middleware.py` & `litestar-2.8.3/tests/unit/test_middleware/test_base_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_compression_middleware.py` & `litestar-2.8.3/tests/unit/test_middleware/test_compression_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_cors_middleware.py` & `litestar-2.8.3/tests/unit/test_middleware/test_cors_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_csrf_middleware.py` & `litestar-2.8.3/tests/unit/test_middleware/test_csrf_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_exception_handler_middleware.py` & `litestar-2.8.3/tests/unit/test_middleware/test_exception_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_logging_middleware.py` & `litestar-2.8.3/tests/unit/test_middleware/test_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_middleware_handling.py` & `litestar-2.8.3/tests/unit/test_middleware/test_middleware_handling.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_rate_limit_middleware.py` & `litestar-2.8.3/tests/unit/test_middleware/test_rate_limit_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_session/conftest.py` & `litestar-2.8.3/tests/unit/test_middleware/test_session/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_session/test_client_side_backend.py` & `litestar-2.8.3/tests/unit/test_middleware/test_session/test_client_side_backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 from typing import Any, Dict
 from unittest import mock
 
 import pytest
 from cryptography.exceptions import InvalidTag
 
 from litestar import Request, get, post
+from litestar.datastructures.headers import MutableScopeHeaders
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.middleware.session import SessionMiddleware
 from litestar.middleware.session.client_side import (
     AAD,
     CHUNK_SIZE,
     ClientSideSessionBackend,
     CookieBackendConfig,
 )
 from litestar.serialization import encode_json
-from litestar.testing import create_test_client
+from litestar.testing import RequestFactory, create_test_client
+from litestar.types.asgi_types import HTTPResponseStartEvent
 from tests.helpers import randbytes
 
 
 @pytest.mark.parametrize(
     "secret, should_raise",
     [
         [randbytes(16), False],
@@ -216,7 +218,29 @@
     # The attacker removes the original AAD and attaches its own.
     ciphertext = b64encode(decoded[:aad_starts_from] + AAD + fraudulent_associated_data)
     # The attacker puts the data back to its original form.
     encoded = [ciphertext[i : i + CHUNK_SIZE] for i in range(0, len(ciphertext), CHUNK_SIZE)]
 
     with pytest.raises(InvalidTag):
         cookie_session_backend.load_data(encoded)
+
+
+async def test_store_in_message_clears_cookies_when_session_grows_gt_chunk_size(
+    cookie_session_backend: ClientSideSessionBackend,
+) -> None:
+    """Should clear the cookies when the session grows larger than the chunk size."""
+    # we have a connection that already contains a cookie header with the "session" key in it
+    connection = RequestFactory().get("/", headers={"Cookie": "session=foo"})
+    # we want to persist a new session that is larger than the chunk size
+    # by the time the encrypted data, nonce and associated data are b64 encoded, the size of
+    # this session will be > 2x larger than the chunk size
+    session = create_session(size=CHUNK_SIZE)
+    message: HTTPResponseStartEvent = {"type": "http.response.start", "status": 200, "headers": []}
+    await cookie_session_backend.store_in_message(session, message, connection)
+    # due to the large session stored in multiple chunks, we now enumerate the name of the cookies
+    # e.g., session-0, session-1, session-2, etc. This means we need to have a cookie with the name
+    # "session" in the response headers that is set to null to clear the original cookie.
+    headers = MutableScopeHeaders.from_message(message)
+    assert len(headers.headers) > 1
+    header_name, header_content = headers.headers[-1]
+    assert header_name == b"set-cookie"
+    assert header_content.startswith(b"session=null;")
```

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_session/test_integration.py` & `litestar-2.8.3/tests/unit/test_middleware/test_session/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_session/test_middleware.py` & `litestar-2.8.3/tests/unit/test_middleware/test_session/test_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_middleware/test_session/test_server_side_backend.py` & `litestar-2.8.3/tests/unit/test_middleware/test_session/test_server_side_backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/conftest.py` & `litestar-2.8.3/tests/unit/test_openapi/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_config.py` & `litestar-2.8.3/tests/unit/test_openapi/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,24 +24,20 @@
     openapi = config.to_openapi_schema()
     assert openapi.components
     assert openapi.components.to_schema() == {
         "schemas": {"test": {"type": "string"}},
         "examples": {"example-one": {"summary": "an example"}},
         "headers": {
             "one": {
-                "name": "",
-                "in": "header",
                 "required": False,
                 "deprecated": False,
                 "allowEmptyValue": False,
                 "allowReserved": False,
             },
             "two": {
-                "name": "",
-                "in": "header",
                 "required": False,
                 "deprecated": False,
                 "allowEmptyValue": False,
                 "allowReserved": False,
             },
         },
     }
```

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_datastructures.py` & `litestar-2.8.3/tests/unit/test_openapi/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_endpoints.py` & `litestar-2.8.3/tests/unit/test_openapi/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_integration.py` & `litestar-2.8.3/tests/unit/test_openapi/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_parameters.py` & `litestar-2.8.3/tests/unit/test_openapi/test_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_path_item.py` & `litestar-2.8.3/tests/unit/test_openapi/test_path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_request_body.py` & `litestar-2.8.3/tests/unit/test_openapi/test_request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_responses.py` & `litestar-2.8.3/tests/unit/test_openapi/test_responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_schema.py` & `litestar-2.8.3/tests/unit/test_openapi/test_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 from dataclasses import dataclass
-from datetime import date, datetime
+from datetime import date, datetime, timezone
 from enum import Enum, auto
 from typing import (  # type: ignore[attr-defined]
     TYPE_CHECKING,
     Any,
     Dict,
     Generic,
     List,
@@ -313,20 +313,22 @@
 
     schema = get_schema_for_field_definition(FieldDefinition.from_kwarg(name="MyDataclass", annotation=MyDataclass))
 
     assert schema.properties["constrained_int"].exclusive_minimum == 1  # type: ignore[index, union-attr]
     assert schema.properties["constrained_int"].exclusive_maximum == 10  # type: ignore[index, union-attr]
     assert schema.properties["constrained_float"].minimum == 1  # type: ignore[index, union-attr]
     assert schema.properties["constrained_float"].maximum == 10  # type: ignore[index, union-attr]
-    assert datetime.utcfromtimestamp(schema.properties["constrained_date"].exclusive_minimum) == datetime.fromordinal(  # type: ignore[arg-type, index, union-attr]
-        historical_date.toordinal()
-    )
-    assert datetime.utcfromtimestamp(schema.properties["constrained_date"].exclusive_maximum) == datetime.fromordinal(  # type: ignore[arg-type, index, union-attr]
-        today.toordinal()
-    )
+    assert datetime.fromtimestamp(
+        schema.properties["constrained_date"].exclusive_minimum,  # type: ignore[arg-type, index, union-attr]
+        tz=timezone.utc,
+    ) == datetime.fromordinal(historical_date.toordinal()).replace(tzinfo=timezone.utc)
+    assert datetime.fromtimestamp(
+        schema.properties["constrained_date"].exclusive_maximum,  # type: ignore[arg-type, index, union-attr]
+        tz=timezone.utc,
+    ) == datetime.fromordinal(today.toordinal()).replace(tzinfo=timezone.utc)
     assert schema.properties["constrained_lower_case"].description == "must be in lower case"  # type: ignore[index]
     assert schema.properties["constrained_upper_case"].description == "must be in upper case"  # type: ignore[index]
     assert schema.properties["constrained_is_ascii"].pattern == "[[:ascii:]]"  # type: ignore[index, union-attr]
     assert schema.properties["constrained_is_digit"].pattern == "[[:digit:]]"  # type: ignore[index, union-attr]
 
 
 def test_literal_enums() -> None:
@@ -588,20 +590,28 @@
     paths = app.openapi_schema.paths["/{param}"]
     assert paths.get is not None
     assert paths.post is not None
 
 
 def test_unconsumed_path_parameters_are_documented() -> None:
     # https://github.com/litestar-org/litestar/issues/3290
-    @get("/{param:str}")
-    async def handler() -> None:
+    # https://github.com/litestar-org/litestar/issues/3369
+
+    async def dd(param3: Annotated[str, Parameter(description="123")]) -> str:
+        return param3
+
+    async def d(dep_dep: str, param2: Annotated[str, Parameter(description="abc")]) -> str:
+        return f"{dep_dep}_{param2}"
+
+    @get("/{param1:str}/{param2:str}/{param3:str}", dependencies={"dep": d, "dep_dep": dd})
+    async def handler(dep: str) -> None:
         pass
 
     app = Litestar([handler])
-    params = app.openapi_schema.paths["/{param}"].get.parameters  # type: ignore[index, union-attr]
+    params = app.openapi_schema.paths["/{param1}/{param2}/{param3}"].get.parameters  # type: ignore[index, union-attr]
     assert params
-    assert len(params) == 1
-    param = params[0]
-    assert isinstance(param, OpenAPIParameter)
-    assert param.name == "param"
-    assert param.required is True
-    assert param.param_in is ParamType.PATH
+    assert len(params) == 3
+    for i, param in enumerate(sorted(params, key=lambda p: p.name), 1):  # pyright: ignore
+        assert isinstance(param, OpenAPIParameter)
+        assert param.name == f"param{i}"
+        assert param.required is True
+        assert param.param_in is ParamType.PATH
```

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_security_schemes.py` & `litestar-2.8.3/tests/unit/test_openapi/test_security_schemes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_spec_generation.py` & `litestar-2.8.3/tests/unit/test_openapi/test_spec_generation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_tags.py` & `litestar-2.8.3/tests/unit/test_openapi/test_tags.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_typescript_converter/test_converter.py` & `litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/test_converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py` & `litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py` & `litestar-2.8.3/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_plugins/test_base.py` & `litestar-2.8.3/tests/unit/test_plugins/test_base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_plugins/test_flash.py` & `litestar-2.8.3/tests/unit/test_plugins/test_flash.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 from enum import Enum
 from pathlib import Path
 
 import pytest
 
-from litestar import Request, get
+from litestar import Litestar, Request, get, post
 from litestar.contrib.jinja import JinjaTemplateEngine
 from litestar.contrib.mako import MakoTemplateEngine
 from litestar.contrib.minijinja import MiniJinjaTemplateEngine
+from litestar.exceptions import ImproperlyConfiguredException
+from litestar.middleware.rate_limit import RateLimitConfig
+from litestar.middleware.session.server_side import ServerSideSessionConfig
 from litestar.plugins.flash import FlashConfig, FlashPlugin, flash
-from litestar.response import Template
+from litestar.response import Redirect, Template
 from litestar.template import TemplateConfig, TemplateEngineProtocol
 from litestar.testing import create_test_client
 
 text_html_jinja = """{% for message in get_flashes() %}<span class="{{ message.category }}">{{ message.message }}</span>{% endfor %}"""
 text_html_mako = """<% messages = get_flashes() %>\\
 % for m in messages:
 <span class="${m['category']}">${m['message']}</span>\\
@@ -52,29 +55,59 @@
 def test_flash_plugin(
     tmp_path: Path,
     engine: type[TemplateEngineProtocol],
     template_str: str,
     category_enum: Enum,
 ) -> None:
     Path(tmp_path / "flash.html").write_text(template_str)
-    text_expected = "".join(
-        [f'<span class="{category.value}">message {category.value}</span>' for category in category_enum]  # type: ignore[attr-defined]
-    )
 
-    @get("/flash")
-    def flash_handler(request: Request) -> Template:
-        for category in category_enum:  # type: ignore[attr-defined]
-            flash(request, f"message {category.value}", category=category.value)
+    @get("/")
+    async def index() -> Redirect:
+        return Redirect("/login")
+
+    @get("/login")
+    async def login(request: Request) -> Template:
+        flash(request, "Flash Test!", category="info")
         return Template("flash.html")
 
+    @post("/check")
+    async def check(request: Request) -> Redirect:
+        flash(request, "User not Found!", category="warning")
+        return Redirect("/login")
+
     template_config: TemplateConfig = TemplateConfig(
         directory=Path(tmp_path),
         engine=engine,
     )
+    session_config = ServerSideSessionConfig()
+    flash_config = FlashConfig(template_config=template_config)
     with create_test_client(
-        [flash_handler],
+        plugins=[FlashPlugin(config=flash_config)],
+        route_handlers=[index, login, check],
         template_config=template_config,
-        plugins=[FlashPlugin(config=FlashConfig(template_config=template_config))],
+        middleware=[session_config.middleware],
     ) as client:
-        r = client.get("/flash")
+        r = client.get("/")
+        assert r.status_code == 200
+        assert "Flash Test!" in r.text
+        r = client.get("/login")
         assert r.status_code == 200
-        assert r.text == text_expected
+        assert "Flash Test!" in r.text
+        r = client.post("/check")
+        assert r.status_code == 200
+        assert "User not Found!" in r.text
+        assert "Flash Test!" in r.text
+
+
+def test_flash_config_doesnt_have_session() -> None:
+    template_config = TemplateConfig(directory=Path("tests/templates"), engine=JinjaTemplateEngine)
+    flash_config = FlashConfig(template_config=template_config)
+    with pytest.raises(ImproperlyConfiguredException):
+        Litestar(plugins=[FlashPlugin(config=flash_config)])
+
+
+def test_flash_config_has_wrong_middleware_type() -> None:
+    template_config = TemplateConfig(directory=Path("tests/templates"), engine=JinjaTemplateEngine)
+    flash_config = FlashConfig(template_config=template_config)
+    rate_limit_config = RateLimitConfig(rate_limit=("minute", 1), exclude=["/schema"])
+    with pytest.raises(ImproperlyConfiguredException):
+        Litestar(plugins=[FlashPlugin(config=flash_config)], middleware=[rate_limit_config.middleware])
```

### Comparing `litestar-2.8.2/tests/unit/test_plugins/test_sqlalchemy.py` & `litestar-2.8.3/tests/unit/test_plugins/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_repository/models_bigint.py` & `litestar-2.8.3/tests/unit/test_repository/models_bigint.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_repository/models_uuid.py` & `litestar-2.8.3/tests/unit/test_repository/models_uuid.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_repository/test_generic_mock_repository.py` & `litestar-2.8.3/tests/unit/test_repository/test_generic_mock_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_response/test_base_response.py` & `litestar-2.8.3/tests/unit/test_response/test_base_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_response/test_file_response.py` & `litestar-2.8.3/tests/unit/test_response/test_file_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_response/test_redirect_response.py` & `litestar-2.8.3/tests/unit/test_response/test_redirect_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_response/test_response_cookies.py` & `litestar-2.8.3/tests/unit/test_response/test_response_cookies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_response/test_response_headers.py` & `litestar-2.8.3/tests/unit/test_response/test_response_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_response/test_response_to_asgi_response.py` & `litestar-2.8.3/tests/unit/test_response/test_response_to_asgi_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_response/test_serialization.py` & `litestar-2.8.3/tests/unit/test_response/test_serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_response/test_sse.py` & `litestar-2.8.3/tests/unit/test_response/test_sse.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_response/test_streaming_response.py` & `litestar-2.8.3/tests/unit/test_response/test_streaming_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_response/test_type_decoders.py` & `litestar-2.8.3/tests/unit/test_response/test_type_decoders.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_response/test_type_encoders.py` & `litestar-2.8.3/tests/unit/test_response/test_type_encoders.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_security/test_security.py` & `litestar-2.8.3/tests/unit/test_security/test_security.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_security/test_session_auth.py` & `litestar-2.8.3/tests/unit/test_security/test_session_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_security/test_jwt/test_auth.py` & `litestar-2.8.3/tests/unit/test_security/test_jwt/test_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_security/test_jwt/test_integration.py` & `litestar-2.8.3/tests/unit/test_security/test_jwt/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_security/test_jwt/test_token.py` & `litestar-2.8.3/tests/unit/test_security/test_jwt/test_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_signature/test_parsing.py` & `litestar-2.8.3/tests/unit/test_signature/test_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_signature/test_validation.py` & `litestar-2.8.3/tests/unit/test_signature/test_validation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_static_files/conftest.py` & `litestar-2.8.3/tests/unit/test_static_files/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_static_files/test_create_static_router.py` & `litestar-2.8.3/tests/unit/test_static_files/test_create_static_router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_static_files/test_file_serving_resolution.py` & `litestar-2.8.3/tests/unit/test_static_files/test_file_serving_resolution.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import TYPE_CHECKING, Callable
 
 import brotli
 import pytest
 from typing_extensions import TypeAlias
 
 from litestar import MediaType, Router, get
-from litestar.static_files import StaticFilesConfig, create_static_files_router
+from litestar.static_files import StaticFiles, StaticFilesConfig, create_static_files_router
 from litestar.status_codes import HTTP_200_OK
 from litestar.testing import create_test_client
 from tests.unit.test_static_files.conftest import MakeConfig
 
 if TYPE_CHECKING:
     from litestar.types import FileSystemProtocol
 
@@ -291,7 +291,35 @@
 
     with create_test_client(router) as client:
         if not resolve:
             linked_dir.unlink()
             assert client.get("/test.txt").status_code == 404
         else:
             assert client.get("/test.txt").status_code == 200
+
+
+async def test_staticfiles_get_fs_info_no_access_to_non_static_directory(
+    tmp_path: Path,
+    file_system: FileSystemProtocol,
+) -> None:
+    assets = tmp_path / "assets"
+    assets.mkdir()
+    index = tmp_path / "index.html"
+    index.write_text("content", "utf-8")
+    static_files = StaticFiles(is_html_mode=False, directories=[assets], file_system=file_system)
+    path, info = await static_files.get_fs_info([assets], "../index.html")
+    assert path is None
+    assert info is None
+
+
+async def test_staticfiles_get_fs_info_no_access_to_non_static_file_with_prefix(
+    tmp_path: Path,
+    file_system: FileSystemProtocol,
+) -> None:
+    static = tmp_path / "static"
+    static.mkdir()
+    private_file = tmp_path / "staticsecrets.env"
+    private_file.write_text("content", "utf-8")
+    static_files = StaticFiles(is_html_mode=False, directories=[static], file_system=file_system)
+    path, info = await static_files.get_fs_info([static], "../staticsecrets.env")
+    assert path is None
+    assert info is None
```

### Comparing `litestar-2.8.2/tests/unit/test_static_files/test_html_mode.py` & `litestar-2.8.3/tests/unit/test_static_files/test_html_mode.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_template/test_built_in.py` & `litestar-2.8.3/tests/unit/test_template/test_built_in.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_template/test_builtin_functions.py` & `litestar-2.8.3/tests/unit/test_template/test_builtin_functions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_template/test_context.py` & `litestar-2.8.3/tests/unit/test_template/test_context.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_template/test_csrf_token.py` & `litestar-2.8.3/tests/unit/test_template/test_csrf_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_template/test_template.py` & `litestar-2.8.3/tests/unit/test_template/test_template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_testing/test_lifespan_handler.py` & `litestar-2.8.3/tests/unit/test_testing/test_lifespan_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_testing/test_request_factory.py` & `litestar-2.8.3/tests/unit/test_testing/test_request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_testing/test_test_client.py` & `litestar-2.8.3/tests/unit/test_testing/test_test_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_types/test_protocols.py` & `litestar-2.8.3/tests/unit/test_types/test_protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_utils/test_dataclass.py` & `litestar-2.8.3/tests/unit/test_utils/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_utils/test_deprecation.py` & `litestar-2.8.3/tests/unit/test_utils/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_utils/test_helpers.py` & `litestar-2.8.3/tests/unit/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_utils/test_module_loader.py` & `litestar-2.8.3/tests/unit/test_utils/test_module_loader.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_utils/test_path.py` & `litestar-2.8.3/tests/unit/test_utils/test_path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_utils/test_predicates.py` & `litestar-2.8.3/tests/unit/test_utils/test_predicates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_utils/test_scope.py` & `litestar-2.8.3/tests/unit/test_utils/test_scope.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_utils/test_sequence.py` & `litestar-2.8.3/tests/unit/test_utils/test_sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_utils/test_signature.py` & `litestar-2.8.3/tests/unit/test_utils/test_signature.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_utils/test_sync.py` & `litestar-2.8.3/tests/unit/test_utils/test_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_utils/test_typing.py` & `litestar-2.8.3/tests/unit/test_utils/test_typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/tests/unit/test_utils/test_version.py` & `litestar-2.8.3/tests/unit/test_utils/test_version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/LICENSE` & `litestar-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar-2.8.2/README.md` & `litestar-2.8.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 <!-- prettier-ignore-start -->
 
 | Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 |-----------|:----|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | CI/CD     |     | [![Latest Release](https://github.com/litestar-org/litestar/actions/workflows/publish.yml/badge.svg)](https://github.com/litestar-org/litestar/actions/workflows/publish.yml) [![ci](https://github.com/litestar-org/litestar/actions/workflows/ci.yml/badge.svg)](https://github.com/litestar-org/litestar/actions/workflows/ci.yml) [![Documentation Building](https://github.com/litestar-org/litestar/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/litestar-org/litestar/actions/workflows/docs.yml)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 | Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/litestar/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/litestar) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)                                                                                                                                                                                                                                                                                                                               |
 | Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/litestar?labelColor=202235&color=edb641&logo=python&logoColor=edb641)](https://badge.fury.io/py/litestar) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/litestar?labelColor=202235&color=edb641&logo=python&logoColor=edb641) ![Starlite PyPI - Downloads](https://img.shields.io/pypi/dm/starlite?logo=python&label=starlite%20downloads&labelColor=202235&color=edb641&logoColor=edb641) ![Litestar PyPI - Downloads](https://img.shields.io/pypi/dm/litestar?logo=python&label=litestar%20downloads&labelColor=202235&color=edb641&logoColor=edb641)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
-| Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar-919193495116337154) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
+| Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
 | Meta      |     | [![Litestar Project](https://img.shields.io/badge/Litestar%20Org-%E2%AD%90%20Litestar-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/litestar-org/litestar) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://spdx.org/licenses/) [![Litestar Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23edb641.svg?&logo=github&logoColor=edb641&labelColor=202235)](https://github.com/sponsors/litestar-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=202235)](https://github.com/astral-sh/ruff) [![code style - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/format.json&labelColor=202235)](https://github.com/psf/black) [![All Contributors](https://img.shields.io/github/all-contributors/litestar-org/litestar?labelColor=202235&color=edb641&logoColor=edb641)](#contributors-) |
 
 <!-- prettier-ignore-end -->
 </div>
 
 <hr>
 
@@ -405,15 +405,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/scott2b"><img src="https://avatars.githubusercontent.com/u/307713?v=4?s=100" width="100px;" alt="Scott Bradley"/><br /><sub><b>Scott Bradley</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Ascott2b" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/srikanthccv/"><img src="https://avatars.githubusercontent.com/u/22846633?v=4?s=100" width="100px;" alt="Srikanth Chekuri"/><br /><sub><b>Srikanth Chekuri</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=srikanthccv" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/litestar/commits?author=srikanthccv" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://lonelyviking.com"><img src="https://avatars.githubusercontent.com/u/78952809?v=4?s=100" width="100px;" alt="Michael Bosch"/><br /><sub><b>Michael Bosch</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=LonelyVikingMichael" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sssssss340"><img src="https://avatars.githubusercontent.com/u/8406195?v=4?s=100" width="100px;" alt="sssssss340"/><br /><sub><b>sssssss340</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Asssssss340" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ste-pool"><img src="https://avatars.githubusercontent.com/u/17198460?v=4?s=100" width="100px;" alt="ste-pool"/><br /><sub><b>ste-pool</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=ste-pool" title="Code">💻</a> <a href="#infra-ste-pool" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
     </tr>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Alc-Alc"><img src="https://avatars.githubusercontent.com/u/45509143?v=4?s=100" width="100px;" alt="Alc-Alc"/><br /><sub><b>Alc-Alc</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=Alc-Alc" title="Documentation">📖</a> <a href="https://github.com/litestar-org/litestar/commits?author=Alc-Alc" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=Alc-Alc" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Alc-Alc"><img src="https://avatars.githubusercontent.com/u/45509143?v=4?s=100" width="100px;" alt="Alc-Alc"/><br /><sub><b>Alc-Alc</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=Alc-Alc" title="Documentation">📖</a> <a href="https://github.com/litestar-org/litestar/commits?author=Alc-Alc" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=Alc-Alc" title="Tests">⚠️</a> <a href="#infra-Alc-Alc" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://asomethings.com"><img src="https://avatars.githubusercontent.com/u/16171942?v=4?s=100" width="100px;" alt="asomethings"/><br /><sub><b>asomethings</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=asomethings" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/garburator"><img src="https://avatars.githubusercontent.com/u/14207857?v=4?s=100" width="100px;" alt="Garry Bullock"/><br /><sub><b>Garry Bullock</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=garburator" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/NiclasHaderer"><img src="https://avatars.githubusercontent.com/u/109728711?v=4?s=100" width="100px;" alt="Niclas Haderer"/><br /><sub><b>Niclas Haderer</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=NiclasHaderer" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dialvarezs"><img src="https://avatars.githubusercontent.com/u/13831919?v=4?s=100" width="100px;" alt="Diego Alvarez"/><br /><sub><b>Diego Alvarez</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=dialvarezs" title="Documentation">📖</a> <a href="https://github.com/litestar-org/litestar/commits?author=dialvarezs" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=dialvarezs" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.rgare.com"><img src="https://avatars.githubusercontent.com/u/51208317?v=4?s=100" width="100px;" alt="Jason Nance"/><br /><sub><b>Jason Nance</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=rgajason" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/spikenn"><img src="https://avatars.githubusercontent.com/u/32995595?v=4?s=100" width="100px;" alt="Igor Kapadze"/><br /><sub><b>Igor Kapadze</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=spikenn" title="Documentation">📖</a></td>
     </tr>
@@ -552,14 +552,16 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/crisog"><img src="https://avatars.githubusercontent.com/u/40803711?v=4?s=100" width="100px;" alt="CrisOG"/><br /><sub><b>CrisOG</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Acrisog" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/litestar/commits?author=crisog" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=crisog" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/haryle"><img src="https://avatars.githubusercontent.com/u/64817481?v=4?s=100" width="100px;" alt="harryle"/><br /><sub><b>harryle</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=haryle" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=haryle" title="Tests">⚠️</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://www.b-list.org/"><img src="https://avatars.githubusercontent.com/u/12384?v=4?s=100" width="100px;" alt="James Bennett"/><br /><sub><b>James Bennett</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Aubernostrum" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sherbang"><img src="https://avatars.githubusercontent.com/u/275015?v=4?s=100" width="100px;" alt="sherbang"/><br /><sub><b>sherbang</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sherbang" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/carlsmedstad"><img src="https://avatars.githubusercontent.com/u/6952324?v=4?s=100" width="100px;" alt="Carl Smedstad"/><br /><sub><b>Carl Smedstad</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=carlsmedstad" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/maintain0404"><img src="https://avatars.githubusercontent.com/u/50428534?v=4?s=100" width="100px;" alt="Taein Min"/><br /><sub><b>Taein Min</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=maintain0404" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/wallseat"><img src="https://avatars.githubusercontent.com/u/26143672?v=4?s=100" width="100px;" alt="Stanislav Lyu."/><br /><sub><b>Stanislav Lyu.</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Awallseat" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `litestar-2.8.2/pyproject.toml` & `litestar-2.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -56,20 +56,20 @@
   {name = "Peter Schutt", email = "peter@litestar.dev"},
   {name = "Visakh Unnikrishnan", email = "guacs@litestar.dev"},
   {name = "Alc", email = "alc@litestar.dev"}
 ]
 name = "litestar"
 readme = "README.md"
 requires-python = ">=3.8,<4.0"
-version = "2.8.2"
+version = "2.8.3"
 
 [project.urls]
 Blog = "https://blog.litestar.dev"
 Changelog = "https://github.com/litestar-org/litestar/releases/"
-Discord = "https://discord.gg/litestar-919193495116337154"
+Discord = "https://discord.gg/litestar"
 Documentation = "https://docs.litestar.dev/"
 Homepage = "https://litestar.dev/"
 "Issue Tracker" = "https://github.com/litestar-org/litestar/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc"
 Reddit = "https://www.reddit.com/r/LitestarAPI"
 Repository = "https://github.com/litestar-org/litestar"
 Twitter = "https://twitter.com/LitestarAPI"
 
@@ -195,15 +195,15 @@
 
 [tool.coverage.report]
 exclude_lines = [
   'except ImportError\b',
   'if VERSION.startswith("1"):',
   'if pydantic.VERSION.startswith("1"):',
 ]
-fail_under = 96
+fail_under = 50
 
 [tool.pytest.ini_options]
 addopts = "--strict-markers --strict-config --dist=loadgroup -m 'not server_integration'"
 asyncio_mode = "auto"
 filterwarnings = [
   "ignore::trio.TrioDeprecationWarning:anyio._backends._trio*:",
   "ignore::DeprecationWarning:pkg_resources.*",
@@ -212,14 +212,18 @@
   "ignore::DeprecationWarning:google.iam",
   "ignore::DeprecationWarning:google",
   "ignore::DeprecationWarning:sphinxcontrib",
   "ignore::DeprecationWarning:litestar.*",
   "ignore::pydantic.PydanticDeprecatedSince20::",
   "ignore:`general_plain_validator_function`:DeprecationWarning::",
   "ignore: 'RichMultiCommand':DeprecationWarning::", # this is coming from rich_click itself, nothing we can do about # that for now
+  "ignore: Dropping max_length:litestar.exceptions.LitestarWarning:litestar.contrib.piccolo",
+  "ignore: Python Debugger on exception enabled:litestar.exceptions.LitestarWarning:",
+  "ignore: datetime.datetime.utcnow:DeprecationWarning:time_machine",
+  "ignore: datetime.datetime.utcnow:DeprecationWarning:jose",
 ]
 markers = [
   "sqlalchemy_integration: SQLAlchemy integration tests",
   "server_integration: Test integration with ASGI server",
 ]
 testpaths = ["tests", "docs/examples/testing"]
 xfail_strict = true
```

### Comparing `litestar-2.8.2/PKG-INFO` & `litestar-2.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: litestar
-Version: 2.8.2
+Version: 2.8.3
 Summary: Litestar - A production-ready, highly performant, extensible ASGI API Framework
 Project-URL: Blog, https://blog.litestar.dev
 Project-URL: Changelog, https://github.com/litestar-org/litestar/releases/
-Project-URL: Discord, https://discord.gg/litestar-919193495116337154
+Project-URL: Discord, https://discord.gg/litestar
 Project-URL: Documentation, https://docs.litestar.dev/
 Project-URL: Homepage, https://litestar.dev/
 Project-URL: Issue Tracker, https://github.com/litestar-org/litestar/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc
 Project-URL: Reddit, https://www.reddit.com/r/LitestarAPI
 Project-URL: Repository, https://github.com/litestar-org/litestar
 Project-URL: Twitter, https://twitter.com/LitestarAPI
 Author-email: Cody Fincher <cody.fincher@gmail.com>, Jacob Coffee <jacob@z7x.org>, Janek Nouvertné <provinzkraut@posteo.de>, Na'aman Hirschfeld <nhirschfeld@gmail.com>, Peter Schutt <peter.github@proton.me>
@@ -61,15 +61,37 @@
 Provides-Extra: cli
 Requires-Dist: jsbeautifier; extra == 'cli'
 Requires-Dist: uvicorn[standard]; extra == 'cli'
 Requires-Dist: uvloop>=0.18.0; (sys_platform != 'win32') and extra == 'cli'
 Provides-Extra: cryptography
 Requires-Dist: cryptography; extra == 'cryptography'
 Provides-Extra: full
-Requires-Dist: litestar[annotated-types,attrs,brotli,cli,cryptography,jinja,jwt,mako,minijinja,opentelemetry,piccolo,picologging,prometheus,pydantic,redis,sqlalchemy,standard,structlog]; extra == 'full'
+Requires-Dist: advanced-alchemy<0.9.0,>=0.2.2; extra == 'full'
+Requires-Dist: annotated-types; extra == 'full'
+Requires-Dist: attrs; extra == 'full'
+Requires-Dist: brotli; extra == 'full'
+Requires-Dist: cryptography; extra == 'full'
+Requires-Dist: email-validator; extra == 'full'
+Requires-Dist: fast-query-parsers>=1.0.2; extra == 'full'
+Requires-Dist: jinja2; extra == 'full'
+Requires-Dist: jinja2>=3.1.2; extra == 'full'
+Requires-Dist: jsbeautifier; extra == 'full'
+Requires-Dist: mako>=1.2.4; extra == 'full'
+Requires-Dist: minijinja>=1.0.0; extra == 'full'
+Requires-Dist: opentelemetry-instrumentation-asgi; extra == 'full'
+Requires-Dist: piccolo; extra == 'full'
+Requires-Dist: picologging; extra == 'full'
+Requires-Dist: prometheus-client; extra == 'full'
+Requires-Dist: pydantic; extra == 'full'
+Requires-Dist: pydantic-extra-types; extra == 'full'
+Requires-Dist: python-jose; extra == 'full'
+Requires-Dist: redis[hiredis]>=4.4.4; extra == 'full'
+Requires-Dist: structlog; extra == 'full'
+Requires-Dist: uvicorn[standard]; extra == 'full'
+Requires-Dist: uvloop>=0.18.0; (sys_platform != 'win32') and extra == 'full'
 Provides-Extra: jinja
 Requires-Dist: jinja2>=3.1.2; extra == 'jinja'
 Provides-Extra: jwt
 Requires-Dist: cryptography; extra == 'jwt'
 Requires-Dist: python-jose; extra == 'jwt'
 Provides-Extra: mako
 Requires-Dist: mako>=1.2.4; extra == 'mako'
@@ -115,15 +137,15 @@
 <!-- prettier-ignore-start -->
 
 | Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 |-----------|:----|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | CI/CD     |     | [![Latest Release](https://github.com/litestar-org/litestar/actions/workflows/publish.yml/badge.svg)](https://github.com/litestar-org/litestar/actions/workflows/publish.yml) [![ci](https://github.com/litestar-org/litestar/actions/workflows/ci.yml/badge.svg)](https://github.com/litestar-org/litestar/actions/workflows/ci.yml) [![Documentation Building](https://github.com/litestar-org/litestar/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/litestar-org/litestar/actions/workflows/docs.yml)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 | Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/litestar/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/litestar) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)                                                                                                                                                                                                                                                                                                                               |
 | Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/litestar?labelColor=202235&color=edb641&logo=python&logoColor=edb641)](https://badge.fury.io/py/litestar) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/litestar?labelColor=202235&color=edb641&logo=python&logoColor=edb641) ![Starlite PyPI - Downloads](https://img.shields.io/pypi/dm/starlite?logo=python&label=starlite%20downloads&labelColor=202235&color=edb641&logoColor=edb641) ![Litestar PyPI - Downloads](https://img.shields.io/pypi/dm/litestar?logo=python&label=litestar%20downloads&labelColor=202235&color=edb641&logoColor=edb641)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
-| Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar-919193495116337154) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
+| Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
 | Meta      |     | [![Litestar Project](https://img.shields.io/badge/Litestar%20Org-%E2%AD%90%20Litestar-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/litestar-org/litestar) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://spdx.org/licenses/) [![Litestar Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23edb641.svg?&logo=github&logoColor=edb641&labelColor=202235)](https://github.com/sponsors/litestar-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=202235)](https://github.com/astral-sh/ruff) [![code style - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/format.json&labelColor=202235)](https://github.com/psf/black) [![All Contributors](https://img.shields.io/github/all-contributors/litestar-org/litestar?labelColor=202235&color=edb641&logoColor=edb641)](#contributors-) |
 
 <!-- prettier-ignore-end -->
 </div>
 
 <hr>
 
@@ -508,15 +530,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/scott2b"><img src="https://avatars.githubusercontent.com/u/307713?v=4?s=100" width="100px;" alt="Scott Bradley"/><br /><sub><b>Scott Bradley</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Ascott2b" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/srikanthccv/"><img src="https://avatars.githubusercontent.com/u/22846633?v=4?s=100" width="100px;" alt="Srikanth Chekuri"/><br /><sub><b>Srikanth Chekuri</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=srikanthccv" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/litestar/commits?author=srikanthccv" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://lonelyviking.com"><img src="https://avatars.githubusercontent.com/u/78952809?v=4?s=100" width="100px;" alt="Michael Bosch"/><br /><sub><b>Michael Bosch</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=LonelyVikingMichael" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sssssss340"><img src="https://avatars.githubusercontent.com/u/8406195?v=4?s=100" width="100px;" alt="sssssss340"/><br /><sub><b>sssssss340</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Asssssss340" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ste-pool"><img src="https://avatars.githubusercontent.com/u/17198460?v=4?s=100" width="100px;" alt="ste-pool"/><br /><sub><b>ste-pool</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=ste-pool" title="Code">💻</a> <a href="#infra-ste-pool" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
     </tr>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Alc-Alc"><img src="https://avatars.githubusercontent.com/u/45509143?v=4?s=100" width="100px;" alt="Alc-Alc"/><br /><sub><b>Alc-Alc</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=Alc-Alc" title="Documentation">📖</a> <a href="https://github.com/litestar-org/litestar/commits?author=Alc-Alc" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=Alc-Alc" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Alc-Alc"><img src="https://avatars.githubusercontent.com/u/45509143?v=4?s=100" width="100px;" alt="Alc-Alc"/><br /><sub><b>Alc-Alc</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=Alc-Alc" title="Documentation">📖</a> <a href="https://github.com/litestar-org/litestar/commits?author=Alc-Alc" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=Alc-Alc" title="Tests">⚠️</a> <a href="#infra-Alc-Alc" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://asomethings.com"><img src="https://avatars.githubusercontent.com/u/16171942?v=4?s=100" width="100px;" alt="asomethings"/><br /><sub><b>asomethings</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=asomethings" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/garburator"><img src="https://avatars.githubusercontent.com/u/14207857?v=4?s=100" width="100px;" alt="Garry Bullock"/><br /><sub><b>Garry Bullock</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=garburator" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/NiclasHaderer"><img src="https://avatars.githubusercontent.com/u/109728711?v=4?s=100" width="100px;" alt="Niclas Haderer"/><br /><sub><b>Niclas Haderer</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=NiclasHaderer" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dialvarezs"><img src="https://avatars.githubusercontent.com/u/13831919?v=4?s=100" width="100px;" alt="Diego Alvarez"/><br /><sub><b>Diego Alvarez</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=dialvarezs" title="Documentation">📖</a> <a href="https://github.com/litestar-org/litestar/commits?author=dialvarezs" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=dialvarezs" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.rgare.com"><img src="https://avatars.githubusercontent.com/u/51208317?v=4?s=100" width="100px;" alt="Jason Nance"/><br /><sub><b>Jason Nance</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=rgajason" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/spikenn"><img src="https://avatars.githubusercontent.com/u/32995595?v=4?s=100" width="100px;" alt="Igor Kapadze"/><br /><sub><b>Igor Kapadze</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=spikenn" title="Documentation">📖</a></td>
     </tr>
@@ -655,14 +677,16 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/crisog"><img src="https://avatars.githubusercontent.com/u/40803711?v=4?s=100" width="100px;" alt="CrisOG"/><br /><sub><b>CrisOG</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Acrisog" title="Bug reports">🐛</a> <a href="https://github.com/litestar-org/litestar/commits?author=crisog" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=crisog" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/haryle"><img src="https://avatars.githubusercontent.com/u/64817481?v=4?s=100" width="100px;" alt="harryle"/><br /><sub><b>harryle</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=haryle" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=haryle" title="Tests">⚠️</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://www.b-list.org/"><img src="https://avatars.githubusercontent.com/u/12384?v=4?s=100" width="100px;" alt="James Bennett"/><br /><sub><b>James Bennett</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Aubernostrum" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sherbang"><img src="https://avatars.githubusercontent.com/u/275015?v=4?s=100" width="100px;" alt="sherbang"/><br /><sub><b>sherbang</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sherbang" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/carlsmedstad"><img src="https://avatars.githubusercontent.com/u/6952324?v=4?s=100" width="100px;" alt="Carl Smedstad"/><br /><sub><b>Carl Smedstad</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=carlsmedstad" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/maintain0404"><img src="https://avatars.githubusercontent.com/u/50428534?v=4?s=100" width="100px;" alt="Taein Min"/><br /><sub><b>Taein Min</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=maintain0404" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/wallseat"><img src="https://avatars.githubusercontent.com/u/26143672?v=4?s=100" width="100px;" alt="Stanislav Lyu."/><br /><sub><b>Stanislav Lyu.</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Awallseat" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

