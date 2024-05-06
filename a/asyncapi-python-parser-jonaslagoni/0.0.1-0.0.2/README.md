# Comparing `tmp/asyncapi_python_parser_jonaslagoni-0.0.1.tar.gz` & `tmp/asyncapi_python_parser_jonaslagoni-0.0.2.tar.gz`

## Comparing `asyncapi_python_parser_jonaslagoni-0.0.1.tar` & `asyncapi_python_parser_jonaslagoni-0.0.2.tar`

### file list

```diff
@@ -1,896 +1,898 @@
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/Makefile
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/requirements.txt
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/.vscode/launch.json
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0   125627 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/package-lock.json
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/package.json
--rw-r--r--   0        0        0    35938 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/1.0.0-without-$id.json
--rw-r--r--   0        0        0    38632 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/1.1.0-without-$id.json
--rw-r--r--   0        0        0    44302 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/1.2.0-without-$id.json
--rw-r--r--   0        0        0    53832 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.0.0-rc1-without-$id.json
--rw-r--r--   0        0        0    53814 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.0.0-rc2-without-$id.json
--rw-r--r--   0        0        0    83618 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.0.0-without-$id.json
--rw-r--r--   0        0        0    88760 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.1.0-without-$id.json
--rw-r--r--   0        0        0    88343 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.2.0-without-$id.json
--rw-r--r--   0        0        0    89226 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.3.0-without-$id.json
--rw-r--r--   0        0        0    90282 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.4.0-without-$id.json
--rw-r--r--   0        0        0    90909 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.5.0-without-$id.json
--rw-r--r--   0        0        0   125233 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.6.0-without-$id.json
--rw-r--r--   0        0        0   347699 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/3.0.0-without-$id.json
--rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/scripts/fetch-schemas.sh
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/generator/src/generate-models.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/__init__.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/parser.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/traits.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/validator.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKey.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKeyHttpSecurityScheme.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKeyHttpSecuritySchemeIn.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKeyHttpSecuritySchemeType.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKeyIn.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKeyType.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/AsymmetricEncryption.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/AsymmetricEncryptionType.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/AsyncApi1Dot0SchemaDot.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Asyncapi.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/BearerHttpSecurityScheme.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/BearerHttpSecuritySchemeScheme.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/BearerHttpSecuritySchemeType.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Components.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Contact.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ExternalDocs.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Info.py
--rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/JsonMinusSchemaMinusDraftMinus07MinusSchema.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/License.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Message.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Reference.py
--rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Schema.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Server.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ServerScheme.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ServerVariable.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/SymmetricEncryption.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/SymmetricEncryptionType.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Tag.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/TopicItem.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Topics.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/UserPassword.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/UserPasswordType.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/X509.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/X509Type.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Xml.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKey.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKeyHttpSecurityScheme.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKeyHttpSecuritySchemeIn.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKeyHttpSecuritySchemeType.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKeyIn.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKeyType.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/AsymmetricEncryption.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/AsymmetricEncryptionType.py
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/AsyncApi1Dot1Dot0SchemaDot.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Asyncapi.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/BearerHttpSecurityScheme.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/BearerHttpSecuritySchemeScheme.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/BearerHttpSecuritySchemeType.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Components.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Contact.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ExternalDocs.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Info.py
--rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/JsonMinusSchemaMinusDraftMinus07MinusSchema.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/License.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Message.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Operation.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/OperationOneOf1.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Parameter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Reference.py
--rw-r--r--   0        0        0    15733 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Schema.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Server.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ServerScheme.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ServerVariable.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/SymmetricEncryption.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/SymmetricEncryptionType.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Tag.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/TopicItem.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Topics.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/UserPassword.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/UserPasswordType.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/X509.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/X509Type.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Xml.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AnonymSchema1.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AnonymSchema2.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AnonymSchema3.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKey.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKeyHttpSecurityScheme.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKeyHttpSecuritySchemeIn.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKeyHttpSecuritySchemeType.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKeyIn.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKeyType.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AsymmetricEncryption.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AsymmetricEncryptionType.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Asyncapi.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/BearerHttpSecurityScheme.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/BearerHttpSecuritySchemeScheme.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/BearerHttpSecuritySchemeType.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Components.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Contact.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ExternalDocs.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Info.py
--rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/JsonMinusSchemaMinusDraftMinus07MinusSchema.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/License.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Message.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OneOf0.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OneOf1.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OneOf2.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Operation.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OperationOneOf1.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Parameter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Reference.py
--rw-r--r--   0        0        0    15733 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Schema.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Server.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ServerScheme.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ServerVariable.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFraming.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFraming1.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingDelimiter.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingDelimiter1.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf0.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf0Delimiter.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf0Type.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf1.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf1Delimiter.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf1Type.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingType.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingType1.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamObject.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/SymmetricEncryption.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/SymmetricEncryptionType.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Tag.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/TopicItem.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Topics.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/UserPassword.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/UserPasswordType.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/X509.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/X509Type.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Xml.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKey.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKeyHttpSecurityScheme.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKeyHttpSecuritySchemeIn.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKeyHttpSecuritySchemeType.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKeyIn.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKeyType.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/AsymmetricEncryption.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/AsymmetricEncryptionType.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/AsyncApi2Dot0Dot0SchemaDot.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Asyncapi.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/BearerHttpSecurityScheme.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/BearerHttpSecuritySchemeScheme.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/BearerHttpSecuritySchemeType.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/BindingsObject.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ChannelItem.py
--rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Components.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Contact.py
--rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/CoreSchemaMetaMinusSchemaObject.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/CorrelationId.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ExternalDocs.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Info.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/License.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Message.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Message1.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageExamplesItem.py
--rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageHeadersObject.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf0.py
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1ExamplesItem.py
--rw-r--r--   0        0        0    17851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1HeadersObject.py
--rw-r--r--   0        0        0    16910 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1PayloadObject.py
--rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessagePayloadObject.py
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageTrait.py
--rw-r--r--   0        0        0    17837 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageTraitHeadersObject.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2Flows.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlows.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsAuthorizationCode.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsClientCredentials.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsImplicit.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsPassword.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsType.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OpenIdConnect.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OpenIdConnectType.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OpenapiSchema30Xml.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Operation.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OperationTrait.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Parameter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Reference.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SchemaAllOf1DiscriminatorObject.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SchemaDiscriminatorObject.py
--rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SchemaObject.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Server.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ServerVariable.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SymmetricEncryption.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SymmetricEncryptionType.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Tag.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/UserPassword.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/UserPasswordType.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/X509.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/X509Type.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKey.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKeyHttpSecurityScheme.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKeyHttpSecuritySchemeIn.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKeyHttpSecuritySchemeType.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKeyIn.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKeyType.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/AsymmetricEncryption.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/AsymmetricEncryptionType.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/AsyncApi2Dot0Dot0MinusRc1SchemaDot.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Asyncapi.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/BearerHttpSecurityScheme.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/BearerHttpSecuritySchemeScheme.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/BearerHttpSecuritySchemeType.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ChannelItem.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Components.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Contact.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/CorrelationId.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ExternalDocs.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Info.py
--rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/JsonMinusSchemaMinusDraftMinus07MinusSchema.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/License.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Message.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/MessageTrait.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2Flows.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlows.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsAuthorizationCode.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsClientCredentials.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsImplicit.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsPassword.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsType.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OpenIdConnect.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OpenIdConnectType.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Operation.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OperationMessage.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OperationMessageOneOf1.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OperationTrait.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Parameter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Reference.py
--rw-r--r--   0        0        0    16230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Schema.py
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Server.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ServerVariable.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/SymmetricEncryption.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/SymmetricEncryptionType.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Tag.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/UserPassword.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/UserPasswordType.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/X509.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/X509Type.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Xml.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKey.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKeyHttpSecurityScheme.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKeyHttpSecuritySchemeIn.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKeyHttpSecuritySchemeType.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKeyIn.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKeyType.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/AsymmetricEncryption.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/AsymmetricEncryptionType.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/AsyncApi2Dot0Dot0MinusRc2SchemaDot.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Asyncapi.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/BearerHttpSecurityScheme.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/BearerHttpSecuritySchemeScheme.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/BearerHttpSecuritySchemeType.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/BindingsObject.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ChannelItem.py
--rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Components.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Contact.py
--rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/CoreSchemaMetaMinusSchemaObject.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/CorrelationId.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ExternalDocs.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Info.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/License.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Message.py
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Message1.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/MessageOneOf1OneOf0.py
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/MessageOneOf1OneOf1.py
--rw-r--r--   0        0        0     4562 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/MessageTrait.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2Flows.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlows.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsAuthorizationCode.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsClientCredentials.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsImplicit.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsPassword.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsType.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/OpenIdConnect.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/OpenIdConnectType.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Operation.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/OperationTrait.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Parameter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Reference.py
--rw-r--r--   0        0        0    16626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/SchemaObject.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Server.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ServerVariable.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/SymmetricEncryption.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/SymmetricEncryptionType.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Tag.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/UserPassword.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/UserPasswordType.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/X509.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/X509Type.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKey.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKeyHttpSecurityScheme.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKeyHttpSecuritySchemeIn.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKeyHttpSecuritySchemeType.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKeyIn.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKeyType.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/AsymmetricEncryption.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/AsymmetricEncryptionType.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/AsyncApi2Dot1Dot0SchemaDot.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Asyncapi.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/BearerHttpSecurityScheme.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/BearerHttpSecuritySchemeScheme.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/BearerHttpSecuritySchemeType.py
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/BindingsObject.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ChannelItem.py
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Components.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Contact.py
--rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/CoreSchemaMetaMinusSchemaObject.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/CorrelationId.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ExternalDocs.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Info.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/License.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Message.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Message1.py
--rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageHeadersObject.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf0.py
--rw-r--r--   0        0        0     5492 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf1.py
--rw-r--r--   0        0        0    17851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf1HeadersObject.py
--rw-r--r--   0        0        0    16910 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf1PayloadObject.py
--rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessagePayloadObject.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageTrait.py
--rw-r--r--   0        0        0    17837 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageTraitHeadersObject.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2Flows.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlows.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsAuthorizationCode.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsClientCredentials.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsImplicit.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsPassword.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsType.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OpenIdConnect.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OpenIdConnectType.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OpenapiSchema30Xml.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Operation.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OperationTrait.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Parameter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Reference.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslGssapiSecurityScheme.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslGssapiSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslPlainSecurityScheme.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslPlainSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslScramSecurityScheme.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslScramSecuritySchemeType.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SchemaAllOf1DiscriminatorObject.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SchemaDiscriminatorObject.py
--rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SchemaObject.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Server.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ServerVariable.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SymmetricEncryption.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SymmetricEncryptionType.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Tag.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/UserPassword.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/UserPasswordType.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/X509.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/X509Type.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKey.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKeyHttpSecurityScheme.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKeyHttpSecuritySchemeIn.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKeyHttpSecuritySchemeType.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKeyIn.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKeyType.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/AsymmetricEncryption.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/AsymmetricEncryptionType.py
--rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/AsyncApi2Dot2Dot0SchemaDot.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Asyncapi.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/BearerHttpSecurityScheme.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/BearerHttpSecuritySchemeScheme.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/BearerHttpSecuritySchemeType.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/BindingsObject.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ChannelItem.py
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Components.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Contact.py
--rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/CoreSchemaMetaMinusSchemaObject.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/CorrelationId.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ExternalDocs.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Info.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/License.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Message.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Message1.py
--rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageHeadersObject.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf0.py
--rw-r--r--   0        0        0     5492 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf1.py
--rw-r--r--   0        0        0    17851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf1HeadersObject.py
--rw-r--r--   0        0        0    16910 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf1PayloadObject.py
--rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessagePayloadObject.py
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageTrait.py
--rw-r--r--   0        0        0    17837 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageTraitHeadersObject.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2Flows.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlows.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsAuthorizationCode.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsClientCredentials.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsImplicit.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsPassword.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsType.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OpenIdConnect.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OpenIdConnectType.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OpenapiSchema30Xml.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Operation.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OperationTrait.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Parameter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Reference.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslGssapiSecurityScheme.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslGssapiSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslPlainSecurityScheme.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslPlainSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslScramSecurityScheme.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslScramSecuritySchemeType.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SchemaAllOf1DiscriminatorObject.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SchemaDiscriminatorObject.py
--rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SchemaObject.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Server.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ServerVariable.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SymmetricEncryption.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SymmetricEncryptionType.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Tag.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/UserPassword.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/UserPasswordType.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/X509.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/X509Type.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKey.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKeyHttpSecurityScheme.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKeyHttpSecuritySchemeIn.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKeyHttpSecuritySchemeType.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKeyIn.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKeyType.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/AsymmetricEncryption.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/AsymmetricEncryptionType.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/AsyncApi2Dot3Dot0SchemaDot.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Asyncapi.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/BearerHttpSecurityScheme.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/BearerHttpSecuritySchemeScheme.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/BearerHttpSecuritySchemeType.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/BindingsObject.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ChannelItem.py
--rw-r--r--   0        0        0     8158 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Components.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Contact.py
--rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/CoreSchemaMetaMinusSchemaObject.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/CorrelationId.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ExternalDocs.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Info.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/License.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Message.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Message1.py
--rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageHeadersObject.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf0.py
--rw-r--r--   0        0        0     5492 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf1.py
--rw-r--r--   0        0        0    17851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf1HeadersObject.py
--rw-r--r--   0        0        0    16910 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf1PayloadObject.py
--rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessagePayloadObject.py
--rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageTrait.py
--rw-r--r--   0        0        0    17837 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageTraitHeadersObject.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2Flows.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlows.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsAuthorizationCode.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsClientCredentials.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsImplicit.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsPassword.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsType.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OpenIdConnect.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OpenIdConnectType.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OpenapiSchema30Xml.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Operation.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OperationTrait.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Parameter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Reference.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslGssapiSecurityScheme.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslGssapiSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslPlainSecurityScheme.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslPlainSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslScramSecurityScheme.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslScramSecuritySchemeType.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SchemaAllOf1DiscriminatorObject.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SchemaDiscriminatorObject.py
--rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SchemaObject.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Server.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ServerVariable.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SymmetricEncryption.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SymmetricEncryptionType.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Tag.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/UserPassword.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/UserPasswordType.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/X509.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/X509Type.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKey.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKeyHttpSecurityScheme.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKeyHttpSecuritySchemeIn.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKeyHttpSecuritySchemeType.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKeyIn.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKeyType.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/AsymmetricEncryption.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/AsymmetricEncryptionType.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/AsyncApi2Dot4Dot0SchemaDot.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Asyncapi.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/BearerHttpSecurityScheme.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/BearerHttpSecuritySchemeScheme.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/BearerHttpSecuritySchemeType.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/BindingsObject.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ChannelItem.py
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Components.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Contact.py
--rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/CoreSchemaMetaMinusSchemaObject.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/CorrelationId.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ExternalDocs.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Info.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/License.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Message.py
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Message1.py
--rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageHeadersObject.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf0.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf1.py
--rw-r--r--   0        0        0    17851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf1HeadersObject.py
--rw-r--r--   0        0        0    16910 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf1PayloadObject.py
--rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessagePayloadObject.py
--rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageTrait.py
--rw-r--r--   0        0        0    17837 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageTraitHeadersObject.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2Flows.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlows.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsAuthorizationCode.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsClientCredentials.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsImplicit.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsPassword.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsType.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OpenIdConnect.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OpenIdConnectType.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OpenapiSchema30Xml.py
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Operation.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OperationTrait.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Parameter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Reference.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslGssapiSecurityScheme.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslGssapiSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslPlainSecurityScheme.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslPlainSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslScramSecurityScheme.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslScramSecuritySchemeType.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SchemaAllOf1DiscriminatorObject.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SchemaDiscriminatorObject.py
--rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SchemaObject.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Server.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ServerVariable.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SymmetricEncryption.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SymmetricEncryptionType.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Tag.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/UserPassword.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/UserPasswordType.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/X509.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/X509Type.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKey.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKeyHttpSecurityScheme.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKeyHttpSecuritySchemeIn.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKeyHttpSecuritySchemeType.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKeyIn.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKeyType.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/AsymmetricEncryption.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/AsymmetricEncryptionType.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/AsyncApi2Dot5Dot0SchemaDot.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Asyncapi.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/BearerHttpSecurityScheme.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/BearerHttpSecuritySchemeScheme.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/BearerHttpSecuritySchemeType.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/BindingsObject.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ChannelItem.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Components.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Contact.py
--rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/CoreSchemaMetaMinusSchemaObject.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/CorrelationId.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ExternalDocs.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Info.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/License.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Message.py
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Message1.py
--rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageHeadersObject.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf0.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf1.py
--rw-r--r--   0        0        0    17851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf1HeadersObject.py
--rw-r--r--   0        0        0    16910 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf1PayloadObject.py
--rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessagePayloadObject.py
--rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageTrait.py
--rw-r--r--   0        0        0    17837 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageTraitHeadersObject.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2Flows.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlows.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsAuthorizationCode.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsClientCredentials.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsImplicit.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsPassword.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsType.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OpenIdConnect.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OpenIdConnectType.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OpenapiSchema30Xml.py
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Operation.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OperationTrait.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Parameter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Reference.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslGssapiSecurityScheme.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslGssapiSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslPlainSecurityScheme.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslPlainSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslScramSecurityScheme.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslScramSecuritySchemeType.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SchemaAllOf1DiscriminatorObject.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SchemaDiscriminatorObject.py
--rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SchemaObject.py
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Server.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ServerVariable.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SymmetricEncryption.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SymmetricEncryptionType.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Tag.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/UserPassword.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/UserPasswordType.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/X509.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/X509Type.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKey.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKeyHttpSecurityScheme.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKeyHttpSecuritySchemeIn.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKeyHttpSecuritySchemeType.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKeyIn.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKeyType.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/AsymmetricEncryption.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/AsymmetricEncryptionType.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/AsyncApi2Dot6Dot0SchemaDot.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Asyncapi.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/BearerHttpSecurityScheme.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/BearerHttpSecuritySchemeScheme.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/BearerHttpSecuritySchemeType.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/BindingsObject.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ChannelItem.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Components.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Contact.py
--rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/CoreSchemaMetaMinusSchemaObject.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/CorrelationId.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ExternalDocs.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Info.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/License.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Message.py
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Message1.py
--rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageHeadersObject.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf0.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf1.py
--rw-r--r--   0        0        0    17851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf1HeadersObject.py
--rw-r--r--   0        0        0    16910 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf1PayloadObject.py
--rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessagePayloadObject.py
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageTrait.py
--rw-r--r--   0        0        0    17837 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageTraitHeadersObject.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2Flows.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlows.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsAuthorizationCode.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsClientCredentials.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsImplicit.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsPassword.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsType.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OpenIdConnect.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OpenIdConnectType.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OpenapiSchema30Xml.py
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Operation.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OperationTrait.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Parameter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Reference.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslGssapiSecurityScheme.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslGssapiSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslPlainSecurityScheme.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslPlainSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslScramSecurityScheme.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslScramSecuritySchemeType.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SchemaAllOf1DiscriminatorObject.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SchemaDiscriminatorObject.py
--rw-r--r--   0        0        0    17811 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SchemaObject.py
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Server.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ServerVariable.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SymmetricEncryption.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SymmetricEncryptionType.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Tag.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/UserPassword.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/UserPasswordType.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/X509.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/X509Type.py
--rw-r--r--   0        0        0    17781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AnySchemaObject.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKey.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKeyHttpSecurityScheme.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKeyHttpSecuritySchemeIn.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKeyHttpSecuritySchemeType.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKeyIn.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKeyType.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Array.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AsymmetricEncryption.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AsymmetricEncryptionType.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AsyncApi3Dot0Dot0SchemaDot.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AvroSchemaV1AvroFieldOrder.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BearerHttpSecurityScheme.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BearerHttpSecuritySchemeScheme.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BearerHttpSecuritySchemeType.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusAmqpMinus0Dot3Dot0MinusOperationDeliveryMode.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusAnypointmqMinus0Dot0Dot1MinusChannelDestinationType.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusGooglepubsubMinus0Dot2Dot0MinusChannelMessageStoragePolicy.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusGooglepubsubMinus0Dot2Dot0MinusChannelSchemaSettings.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusGooglepubsubMinus0Dot2Dot0MinusMessageSchema.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusHttpMinus0Dot2Dot0MinusOperationMethod.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusJmsMinus0Dot0Dot1MinusChannelDestinationType.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusJmsMinus0Dot0Dot1MinusServerBindingVersion.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusKafkaMinus0Dot4Dot0MinusChannelTopicConfiguration.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusKafkaMinus0Dot4Dot0MinusChannelTopicConfigurationCleanupDotPolicyItem.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusKafkaMinus0Dot4Dot0MinusMessageSchemaIdLocation.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusMqttMinus0Dot2Dot0MinusMessagePayloadFormatIndicator.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusMqttMinus0Dot2Dot0MinusOperationQos.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusMqttMinus0Dot2Dot0MinusServerLastWill.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusMqttMinus0Dot2Dot0MinusServerLastWillQos.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusPulsarMinus0Dot1Dot0MinusChannelPersistence.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusPulsarMinus0Dot1Dot0MinusChannelRetention.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItem.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItem1.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemDeliveryMode.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf0.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf0Queue.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf0QueueAccessType.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf1.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemQueue.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemQueueAccessType.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSqsMinus0Dot2Dot0MinusChannelBindingVersion.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSqsMinus0Dot2Dot0MinusOperationBindingVersion.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusWebsocketsMinus0Dot1Dot0MinusChannelMethod.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Channel.py
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObject.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectAmqp.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectAmqpBindingVersion.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectAnypointmq.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectAnypointmqBindingVersion.py
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectGooglepubsub.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectGooglepubsubBindingVersion.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectIbmmq.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectIbmmqBindingVersion.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectJms.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectJmsBindingVersion.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectKafka.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectKafkaBindingVersion.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectPulsar.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectPulsarBindingVersion.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectSns.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectSqs.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectWs.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectWsBindingVersion.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelSchema.py
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Components.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Contact.py
--rw-r--r--   0        0        0    16309 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/CoreSchemaMetaMinusSchemaObject.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/CorrelationId.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Enum.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ExternalDocs.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Field.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Fixed.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Info.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
--rw-r--r--   0        0        0    16751 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/JsonSchemaObject.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/License.py
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Map.py
--rw-r--r--   0        0        0     5965 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObject.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectAmqp.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectAmqpBindingVersion.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectAnypointmq.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectAnypointmqBindingVersion.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectGooglepubsub.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectGooglepubsubBindingVersion.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectHttp.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectHttpBindingVersion.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectIbmmq.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectIbmmqBindingVersion.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectJms.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectJmsBindingVersion.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectKafka.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectKafkaBindingVersion.py
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectMqtt.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectMqttBindingVersion.py
--rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageObject.py
--rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageTrait.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MultiFormatSchemaElseSchemaFormat1.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MultiFormatSchemaElseSchemaFormatAnyOf1.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MultiFormatSchemaElseSchemaFormatAnyOf2.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2Flows.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlows.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsAuthorizationCode.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsClientCredentials.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsImplicit.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsPassword.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsType.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OpenIdConnect.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OpenIdConnectType.py
--rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Operation.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationAction.py
--rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObject.py
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectAmqp.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectAmqpBindingVersion.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectHttp.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectHttpBindingVersion.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectKafka.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectKafkaBindingVersion.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectMqtt.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectMqttBindingVersion.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectNats.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectNatsBindingVersion.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSns.py
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSolace.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSolaceBindingVersion.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSqs.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationReply.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationReplyAddress.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationSchema.py
--rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationTrait.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Parameter.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/PrimitiveType.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/PrimitiveTypeWithMetadata.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Record.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Reference.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslGssapiSecurityScheme.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslGssapiSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslPlainSecurityScheme.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslPlainSecuritySchemeType.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslScramSecurityScheme.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslScramSecuritySchemeType.py
--rw-r--r--   0        0        0    16689 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SchemaObject.py
--rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Server.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObject.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectIbmmq.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectIbmmqBindingVersion.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectJms.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectKafka.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectKafkaBindingVersion.py
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectMqtt.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectMqttBindingVersion.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectPulsar.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectPulsarBindingVersion.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectSolace.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectSolaceBindingVersion.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerSchema.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerVariable.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SymmetricEncryption.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SymmetricEncryptionType.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Tag.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/UserPassword.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/UserPasswordType.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/X509.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/X509Type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/tests/test_docs.py
--rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/tests/test_parser.py
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/tests/test_traits.py
--rw-r--r--   0        0        0    36019 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/tests/docs/3.0.0/streetlights-all.json
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/tests/docs/3.0.0/streetlights-asyncapi.json
--rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/tests/docs/3.0.0/streetlights-avro.json
--rw-r--r--   0        0        0     8347 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/tests/docs/3.0.0/streetlights-json.json
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/tests/docs/3.0.0/streetlights-openapi.json
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/tests/docs/3.0.0/streetlights-unknown.json
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/.gitignore
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/README.md
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/Makefile
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/.github/workflows/semantic-release.yml
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/.vscode/launch.json
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0   125627 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/package-lock.json
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/package.json
+-rw-r--r--   0        0        0    35938 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/1.0.0-without-$id.json
+-rw-r--r--   0        0        0    38632 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/1.1.0-without-$id.json
+-rw-r--r--   0        0        0    44302 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/1.2.0-without-$id.json
+-rw-r--r--   0        0        0    53832 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.0.0-rc1-without-$id.json
+-rw-r--r--   0        0        0    53814 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.0.0-rc2-without-$id.json
+-rw-r--r--   0        0        0    83618 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.0.0-without-$id.json
+-rw-r--r--   0        0        0    88760 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.1.0-without-$id.json
+-rw-r--r--   0        0        0    88343 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.2.0-without-$id.json
+-rw-r--r--   0        0        0    89226 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.3.0-without-$id.json
+-rw-r--r--   0        0        0    90282 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.4.0-without-$id.json
+-rw-r--r--   0        0        0    90909 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.5.0-without-$id.json
+-rw-r--r--   0        0        0   125233 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.6.0-without-$id.json
+-rw-r--r--   0        0        0   347699 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/3.0.0-without-$id.json
+-rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/scripts/fetch-schemas.sh
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/generator/src/generate-models.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/__init__.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/parser.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/traits.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/validator.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKey.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKeyHttpSecurityScheme.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKeyHttpSecuritySchemeIn.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKeyHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKeyIn.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKeyType.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/AsymmetricEncryption.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/AsymmetricEncryptionType.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/AsyncApi1Dot0SchemaDot.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Asyncapi.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/BearerHttpSecurityScheme.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/BearerHttpSecuritySchemeScheme.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/BearerHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Components.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Contact.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ExternalDocs.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Info.py
+-rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/JsonMinusSchemaMinusDraftMinus07MinusSchema.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/License.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Message.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Reference.py
+-rw-r--r--   0        0        0    14978 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Schema.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Server.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ServerScheme.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ServerVariable.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/SymmetricEncryption.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/SymmetricEncryptionType.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Tag.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/TopicItem.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Topics.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/UserPassword.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/UserPasswordType.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/X509.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/X509Type.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Xml.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKey.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKeyHttpSecurityScheme.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKeyHttpSecuritySchemeIn.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKeyHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKeyIn.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKeyType.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/AsymmetricEncryption.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/AsymmetricEncryptionType.py
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/AsyncApi1Dot1Dot0SchemaDot.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Asyncapi.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/BearerHttpSecurityScheme.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/BearerHttpSecuritySchemeScheme.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/BearerHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Components.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Contact.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ExternalDocs.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Info.py
+-rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/JsonMinusSchemaMinusDraftMinus07MinusSchema.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/License.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Message.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Operation.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/OperationOneOf1.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Parameter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Reference.py
+-rw-r--r--   0        0        0    15733 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Schema.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Server.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ServerScheme.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ServerVariable.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/SymmetricEncryption.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/SymmetricEncryptionType.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Tag.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/TopicItem.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Topics.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/UserPassword.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/UserPasswordType.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/X509.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/X509Type.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Xml.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AnonymSchema1.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AnonymSchema2.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AnonymSchema3.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKey.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKeyHttpSecurityScheme.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKeyHttpSecuritySchemeIn.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKeyHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKeyIn.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKeyType.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AsymmetricEncryption.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AsymmetricEncryptionType.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Asyncapi.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/BearerHttpSecurityScheme.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/BearerHttpSecuritySchemeScheme.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/BearerHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Components.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Contact.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ExternalDocs.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Info.py
+-rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/JsonMinusSchemaMinusDraftMinus07MinusSchema.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/License.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Message.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OneOf0.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OneOf1.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OneOf2.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Operation.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OperationOneOf1.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Parameter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Reference.py
+-rw-r--r--   0        0        0    15733 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Schema.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Server.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ServerScheme.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ServerVariable.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFraming.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFraming1.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingDelimiter.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingDelimiter1.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf0.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf0Delimiter.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf0Type.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf1.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf1Delimiter.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf1Type.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingType.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingType1.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamObject.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/SymmetricEncryption.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/SymmetricEncryptionType.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Tag.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/TopicItem.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Topics.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/UserPassword.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/UserPasswordType.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/X509.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/X509Type.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Xml.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKey.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKeyHttpSecurityScheme.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKeyHttpSecuritySchemeIn.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKeyHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKeyIn.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKeyType.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/AsymmetricEncryption.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/AsymmetricEncryptionType.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/AsyncApi2Dot0Dot0SchemaDot.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Asyncapi.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/BearerHttpSecurityScheme.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/BearerHttpSecuritySchemeScheme.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/BearerHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/BindingsObject.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ChannelItem.py
+-rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Components.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Contact.py
+-rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/CoreSchemaMetaMinusSchemaObject.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/CorrelationId.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ExternalDocs.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Info.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/License.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Message.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Message1.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageExamplesItem.py
+-rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageHeadersObject.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf0.py
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1ExamplesItem.py
+-rw-r--r--   0        0        0    17869 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1HeadersObject.py
+-rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1PayloadObject.py
+-rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessagePayloadObject.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageTrait.py
+-rw-r--r--   0        0        0    17855 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageTraitHeadersObject.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2Flows.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlows.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsAuthorizationCode.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsClientCredentials.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsImplicit.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsPassword.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsType.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OpenIdConnect.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OpenIdConnectType.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OpenapiSchema30Xml.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Operation.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OperationTrait.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Parameter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Reference.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SchemaAllOf1DiscriminatorObject.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SchemaDiscriminatorObject.py
+-rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SchemaObject.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Server.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ServerVariable.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SymmetricEncryption.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SymmetricEncryptionType.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Tag.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/UserPassword.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/UserPasswordType.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/X509.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/X509Type.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKey.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKeyHttpSecurityScheme.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKeyHttpSecuritySchemeIn.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKeyHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKeyIn.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKeyType.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/AsymmetricEncryption.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/AsymmetricEncryptionType.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/AsyncApi2Dot0Dot0MinusRc1SchemaDot.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Asyncapi.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/BearerHttpSecurityScheme.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/BearerHttpSecuritySchemeScheme.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/BearerHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ChannelItem.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Components.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Contact.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/CorrelationId.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ExternalDocs.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Info.py
+-rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/JsonMinusSchemaMinusDraftMinus07MinusSchema.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/License.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Message.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/MessageTrait.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2Flows.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlows.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsAuthorizationCode.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsClientCredentials.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsImplicit.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsPassword.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsType.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OpenIdConnect.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OpenIdConnectType.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Operation.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OperationMessage.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OperationMessageOneOf1.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OperationTrait.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Parameter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Reference.py
+-rw-r--r--   0        0        0    16230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Schema.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Server.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ServerVariable.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/SymmetricEncryption.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/SymmetricEncryptionType.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Tag.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/UserPassword.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/UserPasswordType.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/X509.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/X509Type.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Xml.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKey.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKeyHttpSecurityScheme.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKeyHttpSecuritySchemeIn.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKeyHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKeyIn.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKeyType.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/AsymmetricEncryption.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/AsymmetricEncryptionType.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/AsyncApi2Dot0Dot0MinusRc2SchemaDot.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Asyncapi.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/BearerHttpSecurityScheme.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/BearerHttpSecuritySchemeScheme.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/BearerHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/BindingsObject.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ChannelItem.py
+-rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Components.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Contact.py
+-rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/CoreSchemaMetaMinusSchemaObject.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/CorrelationId.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ExternalDocs.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Info.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/License.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Message.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Message1.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/MessageOneOf1OneOf0.py
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/MessageOneOf1OneOf1.py
+-rw-r--r--   0        0        0     4562 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/MessageTrait.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2Flows.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlows.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsAuthorizationCode.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsClientCredentials.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsImplicit.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsPassword.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsType.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/OpenIdConnect.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/OpenIdConnectType.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Operation.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/OperationTrait.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Parameter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Reference.py
+-rw-r--r--   0        0        0    16680 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/SchemaObject.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Server.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ServerVariable.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/SymmetricEncryption.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/SymmetricEncryptionType.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Tag.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/UserPassword.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/UserPasswordType.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/X509.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/X509Type.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKey.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKeyHttpSecurityScheme.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKeyHttpSecuritySchemeIn.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKeyHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKeyIn.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKeyType.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/AsymmetricEncryption.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/AsymmetricEncryptionType.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/AsyncApi2Dot1Dot0SchemaDot.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Asyncapi.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/BearerHttpSecurityScheme.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/BearerHttpSecuritySchemeScheme.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/BearerHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/BindingsObject.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ChannelItem.py
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Components.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Contact.py
+-rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/CoreSchemaMetaMinusSchemaObject.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/CorrelationId.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ExternalDocs.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Info.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/License.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Message.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Message1.py
+-rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageHeadersObject.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf0.py
+-rw-r--r--   0        0        0     5492 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf1.py
+-rw-r--r--   0        0        0    17869 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf1HeadersObject.py
+-rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf1PayloadObject.py
+-rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessagePayloadObject.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageTrait.py
+-rw-r--r--   0        0        0    17855 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageTraitHeadersObject.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2Flows.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlows.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsAuthorizationCode.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsClientCredentials.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsImplicit.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsPassword.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsType.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OpenIdConnect.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OpenIdConnectType.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OpenapiSchema30Xml.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Operation.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OperationTrait.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Parameter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Reference.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslGssapiSecurityScheme.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslGssapiSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslPlainSecurityScheme.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslPlainSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslScramSecurityScheme.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslScramSecuritySchemeType.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SchemaAllOf1DiscriminatorObject.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SchemaDiscriminatorObject.py
+-rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SchemaObject.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Server.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ServerVariable.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SymmetricEncryption.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SymmetricEncryptionType.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Tag.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/UserPassword.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/UserPasswordType.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/X509.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/X509Type.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKey.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKeyHttpSecurityScheme.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKeyHttpSecuritySchemeIn.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKeyHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKeyIn.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKeyType.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/AsymmetricEncryption.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/AsymmetricEncryptionType.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/AsyncApi2Dot2Dot0SchemaDot.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Asyncapi.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/BearerHttpSecurityScheme.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/BearerHttpSecuritySchemeScheme.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/BearerHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/BindingsObject.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ChannelItem.py
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Components.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Contact.py
+-rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/CoreSchemaMetaMinusSchemaObject.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/CorrelationId.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ExternalDocs.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Info.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/License.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Message.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Message1.py
+-rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageHeadersObject.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf0.py
+-rw-r--r--   0        0        0     5492 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf1.py
+-rw-r--r--   0        0        0    17869 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf1HeadersObject.py
+-rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf1PayloadObject.py
+-rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessagePayloadObject.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageTrait.py
+-rw-r--r--   0        0        0    17855 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageTraitHeadersObject.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2Flows.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlows.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsAuthorizationCode.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsClientCredentials.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsImplicit.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsPassword.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsType.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OpenIdConnect.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OpenIdConnectType.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OpenapiSchema30Xml.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Operation.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OperationTrait.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Parameter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Reference.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslGssapiSecurityScheme.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslGssapiSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslPlainSecurityScheme.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslPlainSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslScramSecurityScheme.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslScramSecuritySchemeType.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SchemaAllOf1DiscriminatorObject.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SchemaDiscriminatorObject.py
+-rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SchemaObject.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Server.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ServerVariable.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SymmetricEncryption.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SymmetricEncryptionType.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Tag.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/UserPassword.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/UserPasswordType.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/X509.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/X509Type.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKey.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKeyHttpSecurityScheme.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKeyHttpSecuritySchemeIn.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKeyHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKeyIn.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKeyType.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/AsymmetricEncryption.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/AsymmetricEncryptionType.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/AsyncApi2Dot3Dot0SchemaDot.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Asyncapi.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/BearerHttpSecurityScheme.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/BearerHttpSecuritySchemeScheme.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/BearerHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/BindingsObject.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ChannelItem.py
+-rw-r--r--   0        0        0     8158 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Components.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Contact.py
+-rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/CoreSchemaMetaMinusSchemaObject.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/CorrelationId.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ExternalDocs.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Info.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/License.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Message.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Message1.py
+-rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageHeadersObject.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf0.py
+-rw-r--r--   0        0        0     5492 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf1.py
+-rw-r--r--   0        0        0    17869 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf1HeadersObject.py
+-rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf1PayloadObject.py
+-rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessagePayloadObject.py
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageTrait.py
+-rw-r--r--   0        0        0    17855 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageTraitHeadersObject.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2Flows.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlows.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsAuthorizationCode.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsClientCredentials.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsImplicit.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsPassword.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsType.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OpenIdConnect.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OpenIdConnectType.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OpenapiSchema30Xml.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Operation.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OperationTrait.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Parameter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Reference.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslGssapiSecurityScheme.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslGssapiSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslPlainSecurityScheme.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslPlainSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslScramSecurityScheme.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslScramSecuritySchemeType.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SchemaAllOf1DiscriminatorObject.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SchemaDiscriminatorObject.py
+-rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SchemaObject.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Server.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ServerVariable.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SymmetricEncryption.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SymmetricEncryptionType.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Tag.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/UserPassword.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/UserPasswordType.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/X509.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/X509Type.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKey.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKeyHttpSecurityScheme.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKeyHttpSecuritySchemeIn.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKeyHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKeyIn.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKeyType.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/AsymmetricEncryption.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/AsymmetricEncryptionType.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/AsyncApi2Dot4Dot0SchemaDot.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Asyncapi.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/BearerHttpSecurityScheme.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/BearerHttpSecuritySchemeScheme.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/BearerHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/BindingsObject.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ChannelItem.py
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Components.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Contact.py
+-rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/CoreSchemaMetaMinusSchemaObject.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/CorrelationId.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ExternalDocs.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Info.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/License.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Message.py
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Message1.py
+-rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageHeadersObject.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf0.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf1.py
+-rw-r--r--   0        0        0    17869 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf1HeadersObject.py
+-rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf1PayloadObject.py
+-rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessagePayloadObject.py
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageTrait.py
+-rw-r--r--   0        0        0    17855 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageTraitHeadersObject.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2Flows.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlows.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsAuthorizationCode.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsClientCredentials.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsImplicit.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsPassword.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsType.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OpenIdConnect.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OpenIdConnectType.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OpenapiSchema30Xml.py
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Operation.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OperationTrait.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Parameter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Reference.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslGssapiSecurityScheme.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslGssapiSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslPlainSecurityScheme.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslPlainSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslScramSecurityScheme.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslScramSecuritySchemeType.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SchemaAllOf1DiscriminatorObject.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SchemaDiscriminatorObject.py
+-rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SchemaObject.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Server.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ServerVariable.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SymmetricEncryption.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SymmetricEncryptionType.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Tag.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/UserPassword.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/UserPasswordType.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/X509.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/X509Type.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKey.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKeyHttpSecurityScheme.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKeyHttpSecuritySchemeIn.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKeyHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKeyIn.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKeyType.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/AsymmetricEncryption.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/AsymmetricEncryptionType.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/AsyncApi2Dot5Dot0SchemaDot.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Asyncapi.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/BearerHttpSecurityScheme.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/BearerHttpSecuritySchemeScheme.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/BearerHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/BindingsObject.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ChannelItem.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Components.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Contact.py
+-rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/CoreSchemaMetaMinusSchemaObject.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/CorrelationId.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ExternalDocs.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Info.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/License.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Message.py
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Message1.py
+-rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageHeadersObject.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf0.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf1.py
+-rw-r--r--   0        0        0    17869 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf1HeadersObject.py
+-rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf1PayloadObject.py
+-rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessagePayloadObject.py
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageTrait.py
+-rw-r--r--   0        0        0    17855 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageTraitHeadersObject.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2Flows.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlows.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsAuthorizationCode.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsClientCredentials.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsImplicit.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsPassword.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsType.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OpenIdConnect.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OpenIdConnectType.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OpenapiSchema30Xml.py
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Operation.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OperationTrait.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Parameter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Reference.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslGssapiSecurityScheme.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslGssapiSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslPlainSecurityScheme.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslPlainSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslScramSecurityScheme.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslScramSecuritySchemeType.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SchemaAllOf1DiscriminatorObject.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SchemaDiscriminatorObject.py
+-rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SchemaObject.py
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Server.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ServerVariable.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SymmetricEncryption.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SymmetricEncryptionType.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Tag.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/UserPassword.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/UserPasswordType.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/X509.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/X509Type.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKey.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKeyHttpSecurityScheme.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKeyHttpSecuritySchemeIn.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKeyHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKeyIn.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKeyType.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/AsymmetricEncryption.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/AsymmetricEncryptionType.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/AsyncApi2Dot6Dot0SchemaDot.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Asyncapi.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/BearerHttpSecurityScheme.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/BearerHttpSecuritySchemeScheme.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/BearerHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/BindingsObject.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ChannelItem.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Components.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Contact.py
+-rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/CoreSchemaMetaMinusSchemaObject.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/CorrelationId.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ExternalDocs.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Info.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaType.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/License.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Message.py
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Message1.py
+-rw-r--r--   0        0        0    15725 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageHeadersObject.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf0.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf1.py
+-rw-r--r--   0        0        0    17869 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf1HeadersObject.py
+-rw-r--r--   0        0        0    16919 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf1PayloadObject.py
+-rw-r--r--   0        0        0    15918 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessagePayloadObject.py
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageTrait.py
+-rw-r--r--   0        0        0    17855 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageTraitHeadersObject.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2Flows.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlows.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsAuthorizationCode.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsClientCredentials.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsImplicit.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsPassword.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsType.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OpenIdConnect.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OpenIdConnectType.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OpenapiSchema30Xml.py
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Operation.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OperationTrait.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Parameter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Reference.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslGssapiSecurityScheme.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslGssapiSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslPlainSecurityScheme.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslPlainSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslScramSecurityScheme.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslScramSecuritySchemeType.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SchemaAllOf1DiscriminatorObject.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SchemaDiscriminatorObject.py
+-rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SchemaObject.py
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Server.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ServerVariable.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SymmetricEncryption.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SymmetricEncryptionType.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Tag.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/UserPassword.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/UserPasswordType.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/X509.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/X509Type.py
+-rw-r--r--   0        0        0    17835 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AnySchemaObject.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKey.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKeyHttpSecurityScheme.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKeyHttpSecuritySchemeIn.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKeyHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKeyIn.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKeyType.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Array.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AsymmetricEncryption.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AsymmetricEncryptionType.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AsyncApi3Dot0Dot0SchemaDot.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AvroSchemaV1AvroFieldOrder.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BearerHttpSecurityScheme.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BearerHttpSecuritySchemeScheme.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BearerHttpSecuritySchemeType.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusAmqpMinus0Dot3Dot0MinusOperationDeliveryMode.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusAnypointmqMinus0Dot0Dot1MinusChannelDestinationType.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusGooglepubsubMinus0Dot2Dot0MinusChannelMessageStoragePolicy.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusGooglepubsubMinus0Dot2Dot0MinusChannelSchemaSettings.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusGooglepubsubMinus0Dot2Dot0MinusMessageSchema.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusHttpMinus0Dot2Dot0MinusOperationMethod.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusJmsMinus0Dot0Dot1MinusChannelDestinationType.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusJmsMinus0Dot0Dot1MinusServerBindingVersion.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusKafkaMinus0Dot4Dot0MinusChannelTopicConfiguration.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusKafkaMinus0Dot4Dot0MinusChannelTopicConfigurationCleanupDotPolicyItem.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusKafkaMinus0Dot4Dot0MinusMessageSchemaIdLocation.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusMqttMinus0Dot2Dot0MinusMessagePayloadFormatIndicator.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusMqttMinus0Dot2Dot0MinusOperationQos.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusMqttMinus0Dot2Dot0MinusServerLastWill.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusMqttMinus0Dot2Dot0MinusServerLastWillQos.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusPulsarMinus0Dot1Dot0MinusChannelPersistence.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusPulsarMinus0Dot1Dot0MinusChannelRetention.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItem.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItem1.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemDeliveryMode.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf0.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf0Queue.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf0QueueAccessType.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf1.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemQueue.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemQueueAccessType.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSqsMinus0Dot2Dot0MinusChannelBindingVersion.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSqsMinus0Dot2Dot0MinusOperationBindingVersion.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusWebsocketsMinus0Dot1Dot0MinusChannelMethod.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Channel.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObject.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectAmqp.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectAmqpBindingVersion.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectAnypointmq.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectAnypointmqBindingVersion.py
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectGooglepubsub.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectGooglepubsubBindingVersion.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectIbmmq.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectIbmmqBindingVersion.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectJms.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectJmsBindingVersion.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectKafka.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectKafkaBindingVersion.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectPulsar.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectPulsarBindingVersion.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectSns.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectSqs.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectWs.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectWsBindingVersion.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelSchema.py
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Components.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Contact.py
+-rw-r--r--   0        0        0    16309 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/CoreSchemaMetaMinusSchemaObject.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/CorrelationId.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Enum.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ExternalDocs.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Field.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Fixed.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Info.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.py
+-rw-r--r--   0        0        0    16751 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/JsonSchemaObject.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/License.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Map.py
+-rw-r--r--   0        0        0     5965 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObject.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectAmqp.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectAmqpBindingVersion.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectAnypointmq.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectAnypointmqBindingVersion.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectGooglepubsub.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectGooglepubsubBindingVersion.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectHttp.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectHttpBindingVersion.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectIbmmq.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectIbmmqBindingVersion.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectJms.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectJmsBindingVersion.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectKafka.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectKafkaBindingVersion.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectMqtt.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectMqttBindingVersion.py
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageObject.py
+-rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageTrait.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MultiFormatSchemaElseSchemaFormat1.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MultiFormatSchemaElseSchemaFormatAnyOf1.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MultiFormatSchemaElseSchemaFormatAnyOf2.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2Flows.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlows.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsAuthorizationCode.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsClientCredentials.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsImplicit.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsPassword.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsType.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OpenIdConnect.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OpenIdConnectType.py
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Operation.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationAction.py
+-rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObject.py
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectAmqp.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectAmqpBindingVersion.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectHttp.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectHttpBindingVersion.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectKafka.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectKafkaBindingVersion.py
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectMqtt.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectMqttBindingVersion.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectNats.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectNatsBindingVersion.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSns.py
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSolace.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSolaceBindingVersion.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSqs.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationReply.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationReplyAddress.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationSchema.py
+-rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationTrait.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Parameter.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/PrimitiveType.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/PrimitiveTypeWithMetadata.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Record.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Reference.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslGssapiSecurityScheme.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslGssapiSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslPlainSecurityScheme.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslPlainSecuritySchemeType.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslScramSecurityScheme.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslScramSecuritySchemeType.py
+-rw-r--r--   0        0        0    16743 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SchemaObject.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Server.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObject.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectIbmmq.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectIbmmqBindingVersion.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectJms.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectKafka.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectKafkaBindingVersion.py
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectMqtt.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectMqttBindingVersion.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectPulsar.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectPulsarBindingVersion.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectSolace.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectSolaceBindingVersion.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerSchema.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerVariable.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SymmetricEncryption.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SymmetricEncryptionType.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Tag.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/UserPassword.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/UserPasswordType.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/X509.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/X509Type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/tests/asyncapi_python_parser_jonaslagoni/__init__.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/tests/asyncapi_python_parser_jonaslagoni/test_docs.py
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/tests/asyncapi_python_parser_jonaslagoni/test_parser.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/tests/asyncapi_python_parser_jonaslagoni/test_traits.py
+-rw-r--r--   0        0        0    36019 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/tests/docs/3.0.0/streetlights-all.json
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/tests/docs/3.0.0/streetlights-asyncapi.json
+-rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/tests/docs/3.0.0/streetlights-avro.json
+-rw-r--r--   0        0        0     8347 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/tests/docs/3.0.0/streetlights-json.json
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/tests/docs/3.0.0/streetlights-openapi.json
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/tests/docs/3.0.0/streetlights-unknown.json
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/.gitignore
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/README.md
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 asyncapi_python_parser_jonaslagoni-0.0.2/PKG-INFO
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/.github/workflows/publish-to-pypi.yml` & `asyncapi_python_parser_jonaslagoni-0.0.2/.github/workflows/publish-to-pypi.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 name: Publish Python 🐍 distribution 📦 to PyPI and TestPyPI
-
-on: push
+on:
+  release:
+    types: [published]
 jobs:
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
@@ -24,15 +25,14 @@
       uses: actions/upload-artifact@v3
       with:
         name: python-package-distributions
         path: dist/
   publish-to-pypi:
     name: >-
       Publish Python 🐍 distribution 📦 to PyPI
-    if: startsWith(github.ref, 'refs/tags/')  # only publish to PyPI on tag pushes
     needs:
     - build
     runs-on: ubuntu-latest
     environment:
       name: pypi
       url: https://pypi.org/p/asyncapi_python_parser_jonaslagoni
     permissions:
@@ -67,46 +67,23 @@
       uses: sigstore/gh-action-sigstore-python@v1.2.3
       with:
         inputs: >-
           ./dist/*.tar.gz
           ./dist/*.whl
     - name: Create GitHub Release
       env:
-        GITHUB_TOKEN: ${{ github.token }}
+        GITHUB_TOKEN: ${{ secrets.GH_TOKEN }}
       run: >-
         gh release create
         '${{ github.ref_name }}'
         --repo '${{ github.repository }}'
         --notes ""
     - name: Upload artifact signatures to GitHub Release
       env:
-        GITHUB_TOKEN: ${{ github.token }}
+        GITHUB_TOKEN: ${{ secrets.GH_TOKEN }}
       # Upload to GitHub Release using the `gh` CLI.
       # `dist/` contains the built packages, and the
       # sigstore-produced signatures and certificates.
       run: >-
         gh release upload
         '${{ github.ref_name }}' dist/**
         --repo '${{ github.repository }}'
-  publish-to-testpypi:
-    name: Publish Python 🐍 distribution 📦 to TestPyPI
-    needs:
-    - build
-    runs-on: ubuntu-latest
-
-    environment:
-      name: testpypi
-      url: https://test.pypi.org/p/asyncapi_python_parser_jonaslagoni
-
-    permissions:
-      id-token: write  # IMPORTANT: mandatory for trusted publishing
-
-    steps:
-    - name: Download all the dists
-      uses: actions/download-artifact@v3
-      with:
-        name: python-package-distributions
-        path: dist/
-    - name: Publish distribution 📦 to TestPyPI
-      uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        repository-url: https://test.pypi.org/legacy/
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/.vscode/launch.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/package-lock.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/package-lock.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/1.0.0-without-$id.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/1.0.0-without-$id.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/1.1.0-without-$id.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/1.1.0-without-$id.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/1.2.0-without-$id.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/1.2.0-without-$id.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.0.0-rc1-without-$id.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.0.0-rc1-without-$id.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.0.0-rc2-without-$id.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.0.0-rc2-without-$id.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.0.0-without-$id.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.0.0-without-$id.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.1.0-without-$id.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.1.0-without-$id.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.2.0-without-$id.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.2.0-without-$id.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.3.0-without-$id.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.3.0-without-$id.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.4.0-without-$id.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.4.0-without-$id.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.5.0-without-$id.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.5.0-without-$id.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/2.6.0-without-$id.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/2.6.0-without-$id.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/definitions/3.0.0-without-$id.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/definitions/3.0.0-without-$id.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/generator/src/generate-models.ts` & `asyncapi_python_parser_jonaslagoni-0.0.2/generator/src/generate-models.ts`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/parser.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import yaml
 from jsonschema import RefResolver
-from src.validator import validate_input, ValidationError
-from src.traits import apply_traits
-from src.models.asyncapi_3_0_0.AsyncApi3Dot0Dot0SchemaDot import AsyncApi3Dot0Dot0SchemaDot 
-from src.models.asyncapi_2_6_0.AsyncApi2Dot6Dot0SchemaDot import AsyncApi2Dot6Dot0SchemaDot 
-from src.models.asyncapi_2_5_0.AsyncApi2Dot5Dot0SchemaDot import AsyncApi2Dot5Dot0SchemaDot 
-from src.models.asyncapi_2_4_0.AsyncApi2Dot4Dot0SchemaDot import AsyncApi2Dot4Dot0SchemaDot 
-from src.models.asyncapi_2_3_0.AsyncApi2Dot3Dot0SchemaDot import AsyncApi2Dot3Dot0SchemaDot 
-from src.models.asyncapi_2_2_0.AsyncApi2Dot2Dot0SchemaDot import AsyncApi2Dot2Dot0SchemaDot 
-from src.models.asyncapi_2_1_0.AsyncApi2Dot1Dot0SchemaDot import AsyncApi2Dot1Dot0SchemaDot 
-from src.models.asyncapi_2_0_0.AsyncApi2Dot0Dot0SchemaDot import AsyncApi2Dot0Dot0SchemaDot 
+from .validator import validate_input, ValidationError
+from .traits import apply_traits
+from .models.asyncapi_3_0_0.AsyncApi3Dot0Dot0SchemaDot import AsyncApi3Dot0Dot0SchemaDot 
+from .models.asyncapi_2_6_0.AsyncApi2Dot6Dot0SchemaDot import AsyncApi2Dot6Dot0SchemaDot 
+from .models.asyncapi_2_5_0.AsyncApi2Dot5Dot0SchemaDot import AsyncApi2Dot5Dot0SchemaDot 
+from .models.asyncapi_2_4_0.AsyncApi2Dot4Dot0SchemaDot import AsyncApi2Dot4Dot0SchemaDot 
+from .models.asyncapi_2_3_0.AsyncApi2Dot3Dot0SchemaDot import AsyncApi2Dot3Dot0SchemaDot 
+from .models.asyncapi_2_2_0.AsyncApi2Dot2Dot0SchemaDot import AsyncApi2Dot2Dot0SchemaDot 
+from .models.asyncapi_2_1_0.AsyncApi2Dot1Dot0SchemaDot import AsyncApi2Dot1Dot0SchemaDot 
+from .models.asyncapi_2_0_0.AsyncApi2Dot0Dot0SchemaDot import AsyncApi2Dot0Dot0SchemaDot 
 
 class ParserOptions: 
     def __init__(self, input: dict):
         if 'validate_input' in input:
             self._validate_input: bool = input["validate_input"]
         else:
             self._validate_input: bool = True
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/traits.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/traits.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/validator.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/validator.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKey.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKey.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKeyHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ApiKeyHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/AsymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/AsymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/AsyncApi1Dot0SchemaDot.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/AsyncApi1Dot0SchemaDot.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/BearerHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/BearerHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Components.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Components.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Contact.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Contact.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ExternalDocs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ExternalDocs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Info.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Info.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/JsonMinusSchemaMinusDraftMinus07MinusSchema.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/JsonMinusSchemaMinusDraftMinus07MinusSchema.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/License.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/License.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Message.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Message.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Reference.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Reference.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Schema.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Schema.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Server.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Server.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ServerVariable.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/ServerVariable.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/SymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/SymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Tag.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Tag.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/TopicItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/TopicItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Topics.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Topics.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/UserPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/UserPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/X509.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/X509.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Xml.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_0_0/Xml.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKey.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKey.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKeyHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ApiKeyHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/AsymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/AsymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/AsyncApi1Dot1Dot0SchemaDot.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/AsyncApi1Dot1Dot0SchemaDot.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/BearerHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/BearerHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Components.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Components.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Contact.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Contact.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ExternalDocs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ExternalDocs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Info.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Info.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/JsonMinusSchemaMinusDraftMinus07MinusSchema.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/JsonMinusSchemaMinusDraftMinus07MinusSchema.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/License.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/License.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Message.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Message.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Operation.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Operation.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/OperationOneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/OperationOneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Parameter.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Parameter.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Reference.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Reference.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Schema.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Schema.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Server.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Server.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ServerVariable.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/ServerVariable.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/SymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/SymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Tag.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Tag.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/TopicItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/TopicItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Topics.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Topics.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/UserPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/UserPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/X509.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/X509.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Xml.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_1_0/Xml.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AnonymSchema1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AnonymSchema1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AnonymSchema2.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AnonymSchema2.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AnonymSchema3.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AnonymSchema3.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKey.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKey.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKeyHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ApiKeyHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AsymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/AsymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/BearerHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/BearerHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Components.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Components.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Contact.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Contact.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ExternalDocs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ExternalDocs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Info.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Info.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/JsonMinusSchemaMinusDraftMinus07MinusSchema.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/JsonMinusSchemaMinusDraftMinus07MinusSchema.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/License.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/License.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Message.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Message.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OneOf0.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OneOf0.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OneOf2.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OneOf2.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Operation.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Operation.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OperationOneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/OperationOneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Parameter.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Parameter.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Reference.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Reference.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Schema.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Schema.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Server.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Server.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ServerVariable.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/ServerVariable.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFraming.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFraming.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFraming1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFraming1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf0.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf0.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamFramingOneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/StreamObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/SymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/SymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Tag.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Tag.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/TopicItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/TopicItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Topics.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Topics.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/UserPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/UserPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/X509.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/X509.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Xml.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_1_2_0/Xml.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKey.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKey.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKeyHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ApiKeyHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/AsymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/AsymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/AsyncApi2Dot0Dot0SchemaDot.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/AsyncApi2Dot0Dot0SchemaDot.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/BearerHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/BearerHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/BindingsObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/BindingsObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ChannelItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ChannelItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Components.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Components.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Contact.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Contact.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/CoreSchemaMetaMinusSchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/CoreSchemaMetaMinusSchemaObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/CorrelationId.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/CorrelationId.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ExternalDocs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ExternalDocs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Info.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Info.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/License.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/License.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Message.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Message.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Message1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Message1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageExamplesItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageExamplesItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageHeadersObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf0.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf0.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1ExamplesItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1ExamplesItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1HeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageTraitHeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any, List, Dict
 from . import CoreSchemaMetaMinusSchemaObject
 from . import MessageOneOf1OneOf1PayloadObject
 from . import JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes
 from . import SchemaAllOf1DiscriminatorObject
 from . import ExternalDocs
-class MessageOneOf1OneOf1HeadersObject: 
+class MessageTraitHeadersObject: 
   def __init__(self, input: Dict):
     if 'dollar_id' in input:
       self._dollar_id: str = input['dollar_id']
     if 'dollar_schema' in input:
       self._dollar_schema: str = input['dollar_schema']
     if 'dollar_ref' in input:
       self._dollar_ref: str = input['dollar_ref']
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -459,8 +459,8 @@
     self._reserved_additional_properties = reserved_additional_properties
 
   def serialize_to_json(self):
     return json.dumps(self.__dict__, default=lambda o: o.__dict__, indent=2)
 
   @staticmethod
   def deserialize_from_json(json_string):
-    return MessageOneOf1OneOf1HeadersObject(**json.loads(json_string))
+    return MessageTraitHeadersObject(**json.loads(json_string))
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1PayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1PayloadObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: MessageOneOf1OneOf1PayloadObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType = JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType.OBJECT
@@ -328,18 +328,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> MessageOneOf1OneOf1PayloadObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: MessageOneOf1OneOf1PayloadObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessagePayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessagePayloadObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageTraitHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SchemaObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any, List, Dict
 from . import CoreSchemaMetaMinusSchemaObject
 from . import MessageOneOf1OneOf1PayloadObject
 from . import JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes
 from . import SchemaAllOf1DiscriminatorObject
 from . import ExternalDocs
-class MessageTraitHeadersObject: 
+class SchemaObject: 
   def __init__(self, input: Dict):
     if 'dollar_id' in input:
       self._dollar_id: str = input['dollar_id']
     if 'dollar_schema' in input:
       self._dollar_schema: str = input['dollar_schema']
     if 'dollar_ref' in input:
       self._dollar_ref: str = input['dollar_ref']
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -459,8 +459,8 @@
     self._reserved_additional_properties = reserved_additional_properties
 
   def serialize_to_json(self):
     return json.dumps(self.__dict__, default=lambda o: o.__dict__, indent=2)
 
   @staticmethod
   def deserialize_from_json(json_string):
-    return MessageTraitHeadersObject(**json.loads(json_string))
+    return SchemaObject(**json.loads(json_string))
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2Flows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2Flows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsAuthorizationCode.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsAuthorizationCode.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsClientCredentials.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsClientCredentials.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsImplicit.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsImplicit.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Oauth2FlowsFlowsPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OpenIdConnect.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OpenIdConnect.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OpenapiSchema30Xml.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OpenapiSchema30Xml.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Operation.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Operation.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OperationTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/OperationTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Parameter.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Parameter.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Reference.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Reference.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SchemaAllOf1DiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SchemaAllOf1DiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SchemaDiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SchemaDiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SchemaObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Server.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Server.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ServerVariable.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/ServerVariable.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/SymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Tag.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/Tag.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/UserPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/UserPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/X509.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/X509.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKey.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKey.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKeyHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ApiKeyHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/AsymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/AsymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/AsyncApi2Dot0Dot0MinusRc1SchemaDot.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/AsyncApi2Dot0Dot0MinusRc1SchemaDot.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/BearerHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/BearerHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ChannelItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ChannelItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Components.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Components.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Contact.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Contact.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/CorrelationId.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/CorrelationId.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ExternalDocs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ExternalDocs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Info.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Info.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/JsonMinusSchemaMinusDraftMinus07MinusSchema.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/JsonMinusSchemaMinusDraftMinus07MinusSchema.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/License.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/License.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Message.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Message.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/MessageTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/MessageTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2Flows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2Flows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsAuthorizationCode.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsAuthorizationCode.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsClientCredentials.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsClientCredentials.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsImplicit.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsImplicit.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Oauth2FlowsFlowsPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OpenIdConnect.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OpenIdConnect.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Operation.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Operation.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OperationMessage.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OperationMessage.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OperationMessageOneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OperationMessageOneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OperationTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/OperationTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Parameter.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Parameter.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Reference.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Reference.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Schema.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Schema.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Server.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Server.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ServerVariable.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/ServerVariable.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/SymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/SymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Tag.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Tag.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/UserPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/UserPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/X509.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/X509.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Xml.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc1/Xml.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKey.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKey.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKeyHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ApiKeyHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/AsymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/AsymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/AsyncApi2Dot0Dot0MinusRc2SchemaDot.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/AsyncApi2Dot0Dot0MinusRc2SchemaDot.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/BearerHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/BearerHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/BindingsObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/BindingsObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ChannelItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ChannelItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Components.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Components.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Contact.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Contact.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/CoreSchemaMetaMinusSchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/CoreSchemaMetaMinusSchemaObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/CorrelationId.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/CorrelationId.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ExternalDocs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ExternalDocs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Info.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Info.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/License.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/License.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Message.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Message.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Message1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Message1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/MessageOneOf1OneOf0.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/MessageOneOf1OneOf0.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/MessageOneOf1OneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/MessageOneOf1OneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/MessageTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/MessageTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2Flows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2Flows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsAuthorizationCode.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsAuthorizationCode.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsClientCredentials.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsClientCredentials.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsImplicit.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsImplicit.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Oauth2FlowsFlowsPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/OpenIdConnect.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/OpenIdConnect.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Operation.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Operation.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/OperationTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/OperationTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Parameter.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Parameter.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Reference.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Reference.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/SchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/SchemaObject.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[] = input['items']
+      self._items: Any | List[Any] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -65,15 +65,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     if 'type' in input:
@@ -87,19 +87,19 @@
     if 'reserved_if' in input:
       self._reserved_if: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['reserved_if']
     if 'then' in input:
       self._then: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['then']
     if 'reserved_else' in input:
       self._reserved_else: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['reserved_else']
     if 'all_of' in input:
-      self._all_of: List[] = input['all_of']
+      self._all_of: List[Any] = input['all_of']
     if 'any_of' in input:
-      self._any_of: List[] = input['any_of']
+      self._any_of: List[Any] = input['any_of']
     if 'one_of' in input:
-      self._one_of: List[] = input['one_of']
+      self._one_of: List[Any] = input['one_of']
     if 'reserved_not' in input:
       self._reserved_not: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['reserved_not']
     if 'discriminator' in input:
       self._discriminator: str = input['discriminator']
     if 'external_docs' in input:
       self._external_docs: ExternalDocs.ExternalDocs = ExternalDocs.ExternalDocs(input['external_docs'])
     if 'deprecated' in input:
@@ -237,18 +237,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[]:
+  def items(self) -> Any | List[Any]:
     return self._items
   @items.setter
-  def items(self, items:  | List[]):
+  def items(self, items: Any | List[Any]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -321,18 +321,18 @@
   def pattern_properties(self) -> dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -398,32 +398,32 @@
   def reserved_else(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._reserved_else
   @reserved_else.setter
   def reserved_else(self, reserved_else: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._reserved_else = reserved_else
 
   @property
-  def all_of(self) -> List[]:
+  def all_of(self) -> List[Any]:
     return self._all_of
   @all_of.setter
-  def all_of(self, all_of: List[]):
+  def all_of(self, all_of: List[Any]):
     self._all_of = all_of
 
   @property
-  def any_of(self) -> List[]:
+  def any_of(self) -> List[Any]:
     return self._any_of
   @any_of.setter
-  def any_of(self, any_of: List[]):
+  def any_of(self, any_of: List[Any]):
     self._any_of = any_of
 
   @property
-  def one_of(self) -> List[]:
+  def one_of(self) -> List[Any]:
     return self._one_of
   @one_of.setter
-  def one_of(self, one_of: List[]):
+  def one_of(self, one_of: List[Any]):
     self._one_of = one_of
 
   @property
   def reserved_not(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._reserved_not
   @reserved_not.setter
   def reserved_not(self, reserved_not: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Server.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Server.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ServerVariable.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/ServerVariable.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/SymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/SymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Tag.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/Tag.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/UserPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/UserPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/X509.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0-rc2/X509.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKey.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKey.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKeyHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ApiKeyHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/AsymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/AsymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/AsyncApi2Dot1Dot0SchemaDot.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/AsyncApi2Dot1Dot0SchemaDot.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/BearerHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/BearerHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/BindingsObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/BindingsObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ChannelItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ChannelItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Components.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Components.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Contact.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Contact.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/CoreSchemaMetaMinusSchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/CoreSchemaMetaMinusSchemaObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/CorrelationId.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/CorrelationId.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ExternalDocs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ExternalDocs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Info.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Info.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/License.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/License.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Message.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Message.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Message1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Message1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageHeadersObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf0.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf0.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf1HeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageTraitHeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any, List, Dict
 from . import CoreSchemaMetaMinusSchemaObject
 from . import MessageOneOf1OneOf1PayloadObject
 from . import JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes
 from . import SchemaAllOf1DiscriminatorObject
 from . import ExternalDocs
-class MessageOneOf1OneOf1HeadersObject: 
+class MessageTraitHeadersObject: 
   def __init__(self, input: Dict):
     if 'dollar_id' in input:
       self._dollar_id: str = input['dollar_id']
     if 'dollar_schema' in input:
       self._dollar_schema: str = input['dollar_schema']
     if 'dollar_ref' in input:
       self._dollar_ref: str = input['dollar_ref']
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -459,8 +459,8 @@
     self._reserved_additional_properties = reserved_additional_properties
 
   def serialize_to_json(self):
     return json.dumps(self.__dict__, default=lambda o: o.__dict__, indent=2)
 
   @staticmethod
   def deserialize_from_json(json_string):
-    return MessageOneOf1OneOf1HeadersObject(**json.loads(json_string))
+    return MessageTraitHeadersObject(**json.loads(json_string))
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf1PayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf1PayloadObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: MessageOneOf1OneOf1PayloadObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType = JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType.OBJECT
@@ -328,18 +328,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> MessageOneOf1OneOf1PayloadObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: MessageOneOf1OneOf1PayloadObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessagePayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessagePayloadObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageTraitHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageTraitHeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2Flows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2Flows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsAuthorizationCode.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsAuthorizationCode.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsClientCredentials.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsClientCredentials.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsImplicit.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsImplicit.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Oauth2FlowsFlowsPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OpenIdConnect.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OpenIdConnect.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OpenapiSchema30Xml.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OpenapiSchema30Xml.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Operation.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Operation.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OperationTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/OperationTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Parameter.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Parameter.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Reference.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Reference.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslGssapiSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslGssapiSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslPlainSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslPlainSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslScramSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SaslScramSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SchemaAllOf1DiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SchemaAllOf1DiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SchemaDiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SchemaDiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SchemaObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Server.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Server.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ServerVariable.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/ServerVariable.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/SymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Tag.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/Tag.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/UserPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/UserPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/X509.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/X509.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKey.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKey.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKeyHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ApiKeyHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/AsymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/AsymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/AsyncApi2Dot2Dot0SchemaDot.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/AsyncApi2Dot2Dot0SchemaDot.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/BearerHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/BearerHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/BindingsObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/BindingsObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ChannelItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ChannelItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Components.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Components.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Contact.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Contact.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/CoreSchemaMetaMinusSchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/CoreSchemaMetaMinusSchemaObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/CorrelationId.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/CorrelationId.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ExternalDocs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ExternalDocs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Info.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Info.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/License.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/License.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Message.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Message.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Message1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Message1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageHeadersObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf0.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf0.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf1HeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageTraitHeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any, List, Dict
 from . import CoreSchemaMetaMinusSchemaObject
 from . import MessageOneOf1OneOf1PayloadObject
 from . import JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes
 from . import SchemaAllOf1DiscriminatorObject
 from . import ExternalDocs
-class MessageOneOf1OneOf1HeadersObject: 
+class MessageTraitHeadersObject: 
   def __init__(self, input: Dict):
     if 'dollar_id' in input:
       self._dollar_id: str = input['dollar_id']
     if 'dollar_schema' in input:
       self._dollar_schema: str = input['dollar_schema']
     if 'dollar_ref' in input:
       self._dollar_ref: str = input['dollar_ref']
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -459,8 +459,8 @@
     self._reserved_additional_properties = reserved_additional_properties
 
   def serialize_to_json(self):
     return json.dumps(self.__dict__, default=lambda o: o.__dict__, indent=2)
 
   @staticmethod
   def deserialize_from_json(json_string):
-    return MessageOneOf1OneOf1HeadersObject(**json.loads(json_string))
+    return MessageTraitHeadersObject(**json.loads(json_string))
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf1PayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf1PayloadObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: MessageOneOf1OneOf1PayloadObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType = JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType.OBJECT
@@ -328,18 +328,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> MessageOneOf1OneOf1PayloadObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: MessageOneOf1OneOf1PayloadObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessagePayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessagePayloadObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageTraitHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SchemaObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any, List, Dict
 from . import CoreSchemaMetaMinusSchemaObject
 from . import MessageOneOf1OneOf1PayloadObject
 from . import JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes
 from . import SchemaAllOf1DiscriminatorObject
 from . import ExternalDocs
-class MessageTraitHeadersObject: 
+class SchemaObject: 
   def __init__(self, input: Dict):
     if 'dollar_id' in input:
       self._dollar_id: str = input['dollar_id']
     if 'dollar_schema' in input:
       self._dollar_schema: str = input['dollar_schema']
     if 'dollar_ref' in input:
       self._dollar_ref: str = input['dollar_ref']
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -459,8 +459,8 @@
     self._reserved_additional_properties = reserved_additional_properties
 
   def serialize_to_json(self):
     return json.dumps(self.__dict__, default=lambda o: o.__dict__, indent=2)
 
   @staticmethod
   def deserialize_from_json(json_string):
-    return MessageTraitHeadersObject(**json.loads(json_string))
+    return SchemaObject(**json.loads(json_string))
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2Flows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2Flows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsAuthorizationCode.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsAuthorizationCode.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsClientCredentials.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsClientCredentials.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsImplicit.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsImplicit.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Oauth2FlowsFlowsPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OpenIdConnect.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OpenIdConnect.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OpenapiSchema30Xml.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OpenapiSchema30Xml.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Operation.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Operation.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OperationTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/OperationTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Parameter.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Parameter.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Reference.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Reference.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslGssapiSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslGssapiSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslPlainSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslPlainSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslScramSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SaslScramSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SchemaAllOf1DiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SchemaAllOf1DiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SchemaDiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SchemaDiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SchemaObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Server.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Server.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ServerVariable.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/ServerVariable.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/SymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Tag.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/Tag.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/UserPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/UserPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/X509.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/X509.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKey.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKey.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKeyHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ApiKeyHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/AsymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/AsymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/AsyncApi2Dot3Dot0SchemaDot.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/AsyncApi2Dot3Dot0SchemaDot.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/BearerHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/BearerHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/BindingsObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/BindingsObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ChannelItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ChannelItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Components.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Components.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Contact.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Contact.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/CoreSchemaMetaMinusSchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/CoreSchemaMetaMinusSchemaObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/CorrelationId.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/CorrelationId.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ExternalDocs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ExternalDocs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Info.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Info.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/License.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/License.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Message.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Message.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Message1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Message1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageHeadersObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf0.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf0.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf1HeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageTraitHeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any, List, Dict
 from . import CoreSchemaMetaMinusSchemaObject
 from . import MessageOneOf1OneOf1PayloadObject
 from . import JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes
 from . import SchemaAllOf1DiscriminatorObject
 from . import ExternalDocs
-class MessageOneOf1OneOf1HeadersObject: 
+class MessageTraitHeadersObject: 
   def __init__(self, input: Dict):
     if 'dollar_id' in input:
       self._dollar_id: str = input['dollar_id']
     if 'dollar_schema' in input:
       self._dollar_schema: str = input['dollar_schema']
     if 'dollar_ref' in input:
       self._dollar_ref: str = input['dollar_ref']
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -459,8 +459,8 @@
     self._reserved_additional_properties = reserved_additional_properties
 
   def serialize_to_json(self):
     return json.dumps(self.__dict__, default=lambda o: o.__dict__, indent=2)
 
   @staticmethod
   def deserialize_from_json(json_string):
-    return MessageOneOf1OneOf1HeadersObject(**json.loads(json_string))
+    return MessageTraitHeadersObject(**json.loads(json_string))
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf1PayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf1PayloadObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: MessageOneOf1OneOf1PayloadObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType = JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType.OBJECT
@@ -328,18 +328,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> MessageOneOf1OneOf1PayloadObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: MessageOneOf1OneOf1PayloadObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessagePayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessagePayloadObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageTraitHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageTraitHeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2Flows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2Flows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsAuthorizationCode.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsAuthorizationCode.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsClientCredentials.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsClientCredentials.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsImplicit.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsImplicit.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Oauth2FlowsFlowsPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OpenIdConnect.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OpenIdConnect.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OpenapiSchema30Xml.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OpenapiSchema30Xml.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Operation.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Operation.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OperationTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/OperationTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Parameter.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Parameter.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Reference.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Reference.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslGssapiSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslGssapiSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslPlainSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslPlainSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslScramSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SaslScramSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SchemaAllOf1DiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SchemaAllOf1DiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SchemaDiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SchemaDiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SchemaObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Server.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Server.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ServerVariable.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/ServerVariable.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/SymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Tag.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/Tag.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/UserPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/UserPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/X509.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/X509.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKey.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKey.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKeyHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ApiKeyHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/AsymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/AsymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/AsyncApi2Dot4Dot0SchemaDot.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/AsyncApi2Dot4Dot0SchemaDot.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/BearerHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/BearerHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/BindingsObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/BindingsObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ChannelItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ChannelItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Components.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Components.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Contact.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Contact.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/CoreSchemaMetaMinusSchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/CoreSchemaMetaMinusSchemaObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/CorrelationId.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/CorrelationId.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ExternalDocs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ExternalDocs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Info.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Info.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/License.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/License.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Message.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Message.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Message1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Message1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageHeadersObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf0.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf0.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf1HeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageTraitHeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any, List, Dict
 from . import CoreSchemaMetaMinusSchemaObject
 from . import MessageOneOf1OneOf1PayloadObject
 from . import JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes
 from . import SchemaAllOf1DiscriminatorObject
 from . import ExternalDocs
-class MessageOneOf1OneOf1HeadersObject: 
+class MessageTraitHeadersObject: 
   def __init__(self, input: Dict):
     if 'dollar_id' in input:
       self._dollar_id: str = input['dollar_id']
     if 'dollar_schema' in input:
       self._dollar_schema: str = input['dollar_schema']
     if 'dollar_ref' in input:
       self._dollar_ref: str = input['dollar_ref']
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -459,8 +459,8 @@
     self._reserved_additional_properties = reserved_additional_properties
 
   def serialize_to_json(self):
     return json.dumps(self.__dict__, default=lambda o: o.__dict__, indent=2)
 
   @staticmethod
   def deserialize_from_json(json_string):
-    return MessageOneOf1OneOf1HeadersObject(**json.loads(json_string))
+    return MessageTraitHeadersObject(**json.loads(json_string))
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf1PayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf1PayloadObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: MessageOneOf1OneOf1PayloadObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType = JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType.OBJECT
@@ -328,18 +328,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> MessageOneOf1OneOf1PayloadObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: MessageOneOf1OneOf1PayloadObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessagePayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessagePayloadObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageTraitHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SchemaObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any, List, Dict
 from . import CoreSchemaMetaMinusSchemaObject
 from . import MessageOneOf1OneOf1PayloadObject
 from . import JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes
 from . import SchemaAllOf1DiscriminatorObject
 from . import ExternalDocs
-class MessageTraitHeadersObject: 
+class SchemaObject: 
   def __init__(self, input: Dict):
     if 'dollar_id' in input:
       self._dollar_id: str = input['dollar_id']
     if 'dollar_schema' in input:
       self._dollar_schema: str = input['dollar_schema']
     if 'dollar_ref' in input:
       self._dollar_ref: str = input['dollar_ref']
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -459,8 +459,8 @@
     self._reserved_additional_properties = reserved_additional_properties
 
   def serialize_to_json(self):
     return json.dumps(self.__dict__, default=lambda o: o.__dict__, indent=2)
 
   @staticmethod
   def deserialize_from_json(json_string):
-    return MessageTraitHeadersObject(**json.loads(json_string))
+    return SchemaObject(**json.loads(json_string))
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2Flows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2Flows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsAuthorizationCode.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsAuthorizationCode.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsClientCredentials.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsClientCredentials.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsImplicit.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsImplicit.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Oauth2FlowsFlowsPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OpenIdConnect.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OpenIdConnect.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OpenapiSchema30Xml.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OpenapiSchema30Xml.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Operation.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Operation.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OperationTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/OperationTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Parameter.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Parameter.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Reference.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Reference.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslGssapiSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslGssapiSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslPlainSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslPlainSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslScramSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SaslScramSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SchemaAllOf1DiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SchemaAllOf1DiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SchemaDiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SchemaDiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_0_0/MessageOneOf1OneOf1HeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any, List, Dict
 from . import CoreSchemaMetaMinusSchemaObject
 from . import MessageOneOf1OneOf1PayloadObject
 from . import JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes
 from . import SchemaAllOf1DiscriminatorObject
 from . import ExternalDocs
-class SchemaObject: 
+class MessageOneOf1OneOf1HeadersObject: 
   def __init__(self, input: Dict):
     if 'dollar_id' in input:
       self._dollar_id: str = input['dollar_id']
     if 'dollar_schema' in input:
       self._dollar_schema: str = input['dollar_schema']
     if 'dollar_ref' in input:
       self._dollar_ref: str = input['dollar_ref']
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -459,8 +459,8 @@
     self._reserved_additional_properties = reserved_additional_properties
 
   def serialize_to_json(self):
     return json.dumps(self.__dict__, default=lambda o: o.__dict__, indent=2)
 
   @staticmethod
   def deserialize_from_json(json_string):
-    return SchemaObject(**json.loads(json_string))
+    return MessageOneOf1OneOf1HeadersObject(**json.loads(json_string))
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Server.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Server.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ServerVariable.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/ServerVariable.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/SymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Tag.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/Tag.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/UserPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/UserPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/X509.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/X509.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKey.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKey.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKeyHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ApiKeyHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/AsymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/AsymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/AsyncApi2Dot5Dot0SchemaDot.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/AsyncApi2Dot5Dot0SchemaDot.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/BearerHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/BearerHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/BindingsObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/BindingsObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ChannelItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ChannelItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Components.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Components.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Contact.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Contact.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/CoreSchemaMetaMinusSchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/CoreSchemaMetaMinusSchemaObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/CorrelationId.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/CorrelationId.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ExternalDocs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ExternalDocs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Info.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Info.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/License.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/License.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Message.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Message.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Message1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Message1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageHeadersObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf0.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf0.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf1HeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_1_0/MessageOneOf1OneOf1HeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf1PayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf1PayloadObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: MessageOneOf1OneOf1PayloadObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType = JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType.OBJECT
@@ -328,18 +328,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> MessageOneOf1OneOf1PayloadObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: MessageOneOf1OneOf1PayloadObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessagePayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessagePayloadObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageTraitHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_2_0/MessageOneOf1OneOf1HeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any, List, Dict
 from . import CoreSchemaMetaMinusSchemaObject
 from . import MessageOneOf1OneOf1PayloadObject
 from . import JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes
 from . import SchemaAllOf1DiscriminatorObject
 from . import ExternalDocs
-class MessageTraitHeadersObject: 
+class MessageOneOf1OneOf1HeadersObject: 
   def __init__(self, input: Dict):
     if 'dollar_id' in input:
       self._dollar_id: str = input['dollar_id']
     if 'dollar_schema' in input:
       self._dollar_schema: str = input['dollar_schema']
     if 'dollar_ref' in input:
       self._dollar_ref: str = input['dollar_ref']
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -459,8 +459,8 @@
     self._reserved_additional_properties = reserved_additional_properties
 
   def serialize_to_json(self):
     return json.dumps(self.__dict__, default=lambda o: o.__dict__, indent=2)
 
   @staticmethod
   def deserialize_from_json(json_string):
-    return MessageTraitHeadersObject(**json.loads(json_string))
+    return MessageOneOf1OneOf1HeadersObject(**json.loads(json_string))
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2Flows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2Flows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsAuthorizationCode.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsAuthorizationCode.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsClientCredentials.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsClientCredentials.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsImplicit.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsImplicit.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Oauth2FlowsFlowsPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OpenIdConnect.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OpenIdConnect.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OpenapiSchema30Xml.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OpenapiSchema30Xml.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Operation.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Operation.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OperationTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/OperationTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Parameter.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Parameter.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Reference.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Reference.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslGssapiSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslGssapiSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslPlainSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslPlainSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslScramSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SaslScramSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SchemaAllOf1DiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SchemaAllOf1DiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SchemaDiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SchemaDiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_3_0/MessageOneOf1OneOf1HeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any, List, Dict
 from . import CoreSchemaMetaMinusSchemaObject
 from . import MessageOneOf1OneOf1PayloadObject
 from . import JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes
 from . import SchemaAllOf1DiscriminatorObject
 from . import ExternalDocs
-class SchemaObject: 
+class MessageOneOf1OneOf1HeadersObject: 
   def __init__(self, input: Dict):
     if 'dollar_id' in input:
       self._dollar_id: str = input['dollar_id']
     if 'dollar_schema' in input:
       self._dollar_schema: str = input['dollar_schema']
     if 'dollar_ref' in input:
       self._dollar_ref: str = input['dollar_ref']
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -459,8 +459,8 @@
     self._reserved_additional_properties = reserved_additional_properties
 
   def serialize_to_json(self):
     return json.dumps(self.__dict__, default=lambda o: o.__dict__, indent=2)
 
   @staticmethod
   def deserialize_from_json(json_string):
-    return SchemaObject(**json.loads(json_string))
+    return MessageOneOf1OneOf1HeadersObject(**json.loads(json_string))
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Server.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Server.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ServerVariable.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/ServerVariable.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/SymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Tag.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/Tag.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/UserPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/UserPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/X509.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/X509.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKey.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKey.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKeyHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ApiKeyHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/AsymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/AsymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/AsyncApi2Dot6Dot0SchemaDot.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/AsyncApi2Dot6Dot0SchemaDot.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/BearerHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/BearerHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/BindingsObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/BindingsObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ChannelItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ChannelItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Components.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Components.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Contact.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Contact.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/CoreSchemaMetaMinusSchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/CoreSchemaMetaMinusSchemaObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/CorrelationId.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/CorrelationId.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ExternalDocs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ExternalDocs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Info.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Info.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/License.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/License.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Message.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Message.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Message1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Message1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageHeadersObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf0.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf0.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf1HeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_4_0/MessageOneOf1OneOf1HeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf1PayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf1PayloadObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: MessageOneOf1OneOf1PayloadObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType = JsonMinusSchemaMinusDraftMinus07MinusSchemaType.JsonMinusSchemaMinusDraftMinus07MinusSchemaType.OBJECT
@@ -328,18 +328,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> MessageOneOf1OneOf1PayloadObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: MessageOneOf1OneOf1PayloadObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessagePayloadObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessagePayloadObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageTraitHeadersObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_5_0/MessageOneOf1OneOf1HeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any, List, Dict
 from . import CoreSchemaMetaMinusSchemaObject
 from . import MessageOneOf1OneOf1PayloadObject
 from . import JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes
 from . import SchemaAllOf1DiscriminatorObject
 from . import ExternalDocs
-class MessageTraitHeadersObject: 
+class MessageOneOf1OneOf1HeadersObject: 
   def __init__(self, input: Dict):
     if 'dollar_id' in input:
       self._dollar_id: str = input['dollar_id']
     if 'dollar_schema' in input:
       self._dollar_schema: str = input['dollar_schema']
     if 'dollar_ref' in input:
       self._dollar_ref: str = input['dollar_ref']
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -459,8 +459,8 @@
     self._reserved_additional_properties = reserved_additional_properties
 
   def serialize_to_json(self):
     return json.dumps(self.__dict__, default=lambda o: o.__dict__, indent=2)
 
   @staticmethod
   def deserialize_from_json(json_string):
-    return MessageTraitHeadersObject(**json.loads(json_string))
+    return MessageOneOf1OneOf1HeadersObject(**json.loads(json_string))
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2Flows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2Flows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsAuthorizationCode.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsAuthorizationCode.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsClientCredentials.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsClientCredentials.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsImplicit.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsImplicit.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Oauth2FlowsFlowsPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OpenIdConnect.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OpenIdConnect.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OpenapiSchema30Xml.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OpenapiSchema30Xml.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Operation.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Operation.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OperationTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/OperationTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Parameter.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Parameter.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Reference.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Reference.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslGssapiSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslGssapiSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslPlainSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslPlainSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslScramSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SaslScramSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SchemaAllOf1DiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SchemaAllOf1DiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SchemaDiscriminatorObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SchemaDiscriminatorObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/MessageOneOf1OneOf1HeadersObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any, List, Dict
 from . import CoreSchemaMetaMinusSchemaObject
 from . import MessageOneOf1OneOf1PayloadObject
 from . import JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes
 from . import SchemaAllOf1DiscriminatorObject
 from . import ExternalDocs
-class SchemaObject: 
+class MessageOneOf1OneOf1HeadersObject: 
   def __init__(self, input: Dict):
     if 'dollar_id' in input:
       self._dollar_id: str = input['dollar_id']
     if 'dollar_schema' in input:
       self._dollar_schema: str = input['dollar_schema']
     if 'dollar_ref' in input:
       self._dollar_ref: str = input['dollar_ref']
@@ -43,15 +43,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
+      self._items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -67,15 +67,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     self._type: JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes | List[JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes.JsonMinusSchemaMinusDraftMinus07MinusSchemaSimpleTypes] = undefined
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
+  def items(self) -> Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._items
   @items.setter
-  def items(self, items:  | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
+  def items(self, items: Any | List[MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, MessageOneOf1OneOf1PayloadObject.MessageOneOf1OneOf1PayloadObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -459,8 +459,8 @@
     self._reserved_additional_properties = reserved_additional_properties
 
   def serialize_to_json(self):
     return json.dumps(self.__dict__, default=lambda o: o.__dict__, indent=2)
 
   @staticmethod
   def deserialize_from_json(json_string):
-    return SchemaObject(**json.loads(json_string))
+    return MessageOneOf1OneOf1HeadersObject(**json.loads(json_string))
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Server.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Server.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ServerVariable.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/ServerVariable.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/SymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Tag.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/Tag.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/UserPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/UserPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/X509.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_2_6_0/X509.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AnySchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AnySchemaObject.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[] = input['items']
+      self._items: Any | List[Any] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -68,15 +68,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     if 'type' in input:
@@ -90,19 +90,19 @@
     if 'reserved_if' in input:
       self._reserved_if: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['reserved_if']
     if 'then' in input:
       self._then: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['then']
     if 'reserved_else' in input:
       self._reserved_else: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['reserved_else']
     if 'all_of' in input:
-      self._all_of: List[] = input['all_of']
+      self._all_of: List[Any] = input['all_of']
     if 'any_of' in input:
-      self._any_of: List[] = input['any_of']
+      self._any_of: List[Any] = input['any_of']
     if 'one_of' in input:
-      self._one_of: List[] = input['one_of']
+      self._one_of: List[Any] = input['one_of']
     if 'reserved_not' in input:
       self._reserved_not: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['reserved_not']
     if 'discriminator' in input:
       self._discriminator: str = input['discriminator']
     if 'external_docs' in input:
       self._external_docs: Reference.Reference | ExternalDocs.ExternalDocs = input['external_docs']
     if 'deprecated' in input:
@@ -244,18 +244,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[]:
+  def items(self) -> Any | List[Any]:
     return self._items
   @items.setter
-  def items(self, items:  | List[]):
+  def items(self, items: Any | List[Any]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -328,18 +328,18 @@
   def pattern_properties(self) -> dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -405,32 +405,32 @@
   def reserved_else(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._reserved_else
   @reserved_else.setter
   def reserved_else(self, reserved_else: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._reserved_else = reserved_else
 
   @property
-  def all_of(self) -> List[]:
+  def all_of(self) -> List[Any]:
     return self._all_of
   @all_of.setter
-  def all_of(self, all_of: List[]):
+  def all_of(self, all_of: List[Any]):
     self._all_of = all_of
 
   @property
-  def any_of(self) -> List[]:
+  def any_of(self) -> List[Any]:
     return self._any_of
   @any_of.setter
-  def any_of(self, any_of: List[]):
+  def any_of(self, any_of: List[Any]):
     self._any_of = any_of
 
   @property
-  def one_of(self) -> List[]:
+  def one_of(self) -> List[Any]:
     return self._one_of
   @one_of.setter
-  def one_of(self, one_of: List[]):
+  def one_of(self, one_of: List[Any]):
     self._one_of = one_of
 
   @property
   def reserved_not(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._reserved_not
   @reserved_not.setter
   def reserved_not(self, reserved_not: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKey.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKey.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKeyHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ApiKeyHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Array.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Array.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       self._name: str = input['name']
     if 'namespace' in input:
       self._namespace: str = input['namespace']
     if 'doc' in input:
       self._doc: str = input['doc']
     if 'aliases' in input:
       self._aliases: List[str] = input['aliases']
-    self._items: PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array | Map.Map | Fixed.Fixed | List[] = input['items']
+    self._items: PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array | Map.Map | Fixed.Fixed | List[Any] = input['items']
     if 'additional_properties' in input:
       self._additional_properties: dict[str, Any] = input['additional_properties']
 
   @property
   def type(self) -> str:
     return self._type
 
@@ -51,18 +51,18 @@
   def aliases(self) -> List[str]:
     return self._aliases
   @aliases.setter
   def aliases(self, aliases: List[str]):
     self._aliases = aliases
 
   @property
-  def items(self) -> PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array | Map.Map | Fixed.Fixed | List[]:
+  def items(self) -> PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array | Map.Map | Fixed.Fixed | List[Any]:
     return self._items
   @items.setter
-  def items(self, items: PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array | Map.Map | Fixed.Fixed | List[]):
+  def items(self, items: PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array | Map.Map | Fixed.Fixed | List[Any]):
     self._items = items
 
   @property
   def additional_properties(self) -> dict[str, Any]:
     return self._additional_properties
   @additional_properties.setter
   def additional_properties(self, additional_properties: dict[str, Any]):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AsymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AsymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AsyncApi3Dot0Dot0SchemaDot.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/AsyncApi3Dot0Dot0SchemaDot.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BearerHttpSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BearerHttpSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusGooglepubsubMinus0Dot2Dot0MinusChannelMessageStoragePolicy.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusGooglepubsubMinus0Dot2Dot0MinusChannelMessageStoragePolicy.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusGooglepubsubMinus0Dot2Dot0MinusChannelSchemaSettings.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusGooglepubsubMinus0Dot2Dot0MinusChannelSchemaSettings.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusGooglepubsubMinus0Dot2Dot0MinusMessageSchema.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusGooglepubsubMinus0Dot2Dot0MinusMessageSchema.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusKafkaMinus0Dot4Dot0MinusChannelTopicConfiguration.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusKafkaMinus0Dot4Dot0MinusChannelTopicConfiguration.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusMqttMinus0Dot2Dot0MinusServerLastWill.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusMqttMinus0Dot2Dot0MinusServerLastWill.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusPulsarMinus0Dot1Dot0MinusChannelRetention.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusPulsarMinus0Dot1Dot0MinusChannelRetention.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItem.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItem.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItem1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItem1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf0.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf0.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf0Queue.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf0Queue.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemOneOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemQueue.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/BindingsMinusSolaceMinus0Dot3Dot0MinusOperationDestinationsItemQueue.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Channel.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Channel.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectAmqp.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectAmqp.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectAnypointmq.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectAnypointmq.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectGooglepubsub.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectGooglepubsub.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectIbmmq.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectIbmmq.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectJms.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectJms.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectKafka.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectKafka.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectPulsar.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectPulsar.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectSns.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectSns.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectSqs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectSqs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectWs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelBindingsObjectWs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelSchema.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ChannelSchema.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Components.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Components.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Contact.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Contact.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/CoreSchemaMetaMinusSchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/CoreSchemaMetaMinusSchemaObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/CorrelationId.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/CorrelationId.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Enum.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Enum.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ExternalDocs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ExternalDocs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Field.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Field.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from . import Array
 from . import Map
 from . import Fixed
 from . import AvroSchemaV1AvroFieldOrder
 class Field: 
   def __init__(self, input: Dict):
     self._name: str = input['name']
-    self._type: PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map.Map | Fixed.Fixed | List[] = input['type']
+    self._type: PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map.Map | Fixed.Fixed | List[Any] = input['type']
     if 'doc' in input:
       self._doc: str = input['doc']
     if 'default' in input:
       self._default: Any = input['default']
     if 'order' in input:
       self._order: AvroSchemaV1AvroFieldOrder.AvroSchemaV1AvroFieldOrder = AvroSchemaV1AvroFieldOrder.AvroSchemaV1AvroFieldOrder(input['order'])
     if 'aliases' in input:
@@ -28,18 +28,18 @@
   def name(self) -> str:
     return self._name
   @name.setter
   def name(self, name: str):
     self._name = name
 
   @property
-  def type(self) -> PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map.Map | Fixed.Fixed | List[]:
+  def type(self) -> PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map.Map | Fixed.Fixed | List[Any]:
     return self._type
   @type.setter
-  def type(self, type: PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map.Map | Fixed.Fixed | List[]):
+  def type(self, type: PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map.Map | Fixed.Fixed | List[Any]):
     self._type = type
 
   @property
   def doc(self) -> str:
     return self._doc
   @doc.setter
   def doc(self, doc: str):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Fixed.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Fixed.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Info.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Info.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/JsonSchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/JsonSchemaObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/License.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/License.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Map.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Map.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       self._name: str = input['name']
     if 'namespace' in input:
       self._namespace: str = input['namespace']
     if 'doc' in input:
       self._doc: str = input['doc']
     if 'aliases' in input:
       self._aliases: List[str] = input['aliases']
-    self._values: PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map | Fixed.Fixed | List[] = input['values']
+    self._values: PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map | Fixed.Fixed | List[Any] = input['values']
     if 'additional_properties' in input:
       self._additional_properties: dict[str, Any] = input['additional_properties']
 
   @property
   def type(self) -> str:
     return self._type
 
@@ -51,18 +51,18 @@
   def aliases(self) -> List[str]:
     return self._aliases
   @aliases.setter
   def aliases(self, aliases: List[str]):
     self._aliases = aliases
 
   @property
-  def values(self) -> PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map | Fixed.Fixed | List[]:
+  def values(self) -> PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map | Fixed.Fixed | List[Any]:
     return self._values
   @values.setter
-  def values(self, values: PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map | Fixed.Fixed | List[]):
+  def values(self, values: PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map | Fixed.Fixed | List[Any]):
     self._values = values
 
   @property
   def additional_properties(self) -> dict[str, Any]:
     return self._additional_properties
   @additional_properties.setter
   def additional_properties(self, additional_properties: dict[str, Any]):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectAmqp.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectAmqp.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectAnypointmq.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectAnypointmq.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectGooglepubsub.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectGooglepubsub.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectHttp.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectHttp.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectIbmmq.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectIbmmq.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectJms.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectJms.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectKafka.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectKafka.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from . import Fixed
 from . import BindingsMinusKafkaMinus0Dot4Dot0MinusMessageSchemaIdLocation
 class MessageBindingsObjectKafka: 
   def __init__(self, input: Dict):
     if 'binding_version' in input:
       self._binding_version: MessageBindingsObjectKafkaBindingVersion.MessageBindingsObjectKafkaBindingVersion = MessageBindingsObjectKafkaBindingVersion.MessageBindingsObjectKafkaBindingVersion(input['binding_version'])
     if 'key' in input:
-      self._key: Reference.Reference | SchemaObject.SchemaObject | bool | PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map.Map | Fixed.Fixed | List[] = input['key']
+      self._key: Reference.Reference | SchemaObject.SchemaObject | bool | PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map.Map | Fixed.Fixed | List[Any] = input['key']
     if 'schema_id_location' in input:
       self._schema_id_location: BindingsMinusKafkaMinus0Dot4Dot0MinusMessageSchemaIdLocation.BindingsMinusKafkaMinus0Dot4Dot0MinusMessageSchemaIdLocation = BindingsMinusKafkaMinus0Dot4Dot0MinusMessageSchemaIdLocation.BindingsMinusKafkaMinus0Dot4Dot0MinusMessageSchemaIdLocation(input['schema_id_location'])
     if 'schema_id_payload_encoding' in input:
       self._schema_id_payload_encoding: str = input['schema_id_payload_encoding']
     if 'schema_lookup_strategy' in input:
       self._schema_lookup_strategy: str = input['schema_lookup_strategy']
     if 'additional_properties' in input:
@@ -31,18 +31,18 @@
   def binding_version(self) -> MessageBindingsObjectKafkaBindingVersion.MessageBindingsObjectKafkaBindingVersion:
     return self._binding_version
   @binding_version.setter
   def binding_version(self, binding_version: MessageBindingsObjectKafkaBindingVersion.MessageBindingsObjectKafkaBindingVersion):
     self._binding_version = binding_version
 
   @property
-  def key(self) -> Reference.Reference | SchemaObject.SchemaObject | bool | PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map.Map | Fixed.Fixed | List[]:
+  def key(self) -> Reference.Reference | SchemaObject.SchemaObject | bool | PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map.Map | Fixed.Fixed | List[Any]:
     return self._key
   @key.setter
-  def key(self, key: Reference.Reference | SchemaObject.SchemaObject | bool | PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map.Map | Fixed.Fixed | List[]):
+  def key(self, key: Reference.Reference | SchemaObject.SchemaObject | bool | PrimitiveType.PrimitiveType | PrimitiveTypeWithMetadata.PrimitiveTypeWithMetadata | Any | Record.Record | Enum.Enum | Array.Array | Map.Map | Fixed.Fixed | List[Any]):
     self._key = key
 
   @property
   def schema_id_location(self) -> BindingsMinusKafkaMinus0Dot4Dot0MinusMessageSchemaIdLocation.BindingsMinusKafkaMinus0Dot4Dot0MinusMessageSchemaIdLocation:
     return self._schema_id_location
   @schema_id_location.setter
   def schema_id_location(self, schema_id_location: BindingsMinusKafkaMinus0Dot4Dot0MinusMessageSchemaIdLocation.BindingsMinusKafkaMinus0Dot4Dot0MinusMessageSchemaIdLocation):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectMqtt.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageBindingsObjectMqtt.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MessageTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MultiFormatSchemaElseSchemaFormat1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MultiFormatSchemaElseSchemaFormat1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MultiFormatSchemaElseSchemaFormatAnyOf1.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MultiFormatSchemaElseSchemaFormatAnyOf1.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MultiFormatSchemaElseSchemaFormatAnyOf2.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/MultiFormatSchemaElseSchemaFormatAnyOf2.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2Flows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2Flows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlows.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlows.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsAuthorizationCode.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsAuthorizationCode.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsClientCredentials.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsClientCredentials.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsImplicit.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsImplicit.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Oauth2FlowsFlowsPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OpenIdConnect.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OpenIdConnect.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Operation.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Operation.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectAmqp.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectAmqp.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectHttp.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectHttp.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectKafka.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectKafka.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectMqtt.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectMqtt.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectNats.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectNats.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSns.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSns.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSolace.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSolace.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSqs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationBindingsObjectSqs.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationReply.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationReply.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationReplyAddress.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationReplyAddress.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationSchema.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationSchema.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationTrait.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/OperationTrait.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Parameter.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Parameter.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/PrimitiveTypeWithMetadata.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/PrimitiveTypeWithMetadata.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Record.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Record.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Reference.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Reference.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslGssapiSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslGssapiSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslPlainSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslPlainSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslScramSecurityScheme.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SaslScramSecurityScheme.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SchemaObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SchemaObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     if 'min_length' in input:
       self._min_length: int = input['min_length']
     if 'pattern' in input:
       self._pattern: str = input['pattern']
     if 'additional_items' in input:
       self._additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['additional_items']
     if 'items' in input:
-      self._items:  | List[] = input['items']
+      self._items: Any | List[Any] = input['items']
     if 'max_items' in input:
       self._max_items: int = input['max_items']
     if 'min_items' in input:
       self._min_items: int = input['min_items']
     if 'unique_items' in input:
       self._unique_items: bool = input['unique_items']
     if 'contains' in input:
@@ -66,15 +66,15 @@
     if 'definitions' in input:
       self._definitions: dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool] = input['definitions']
     if 'properties' in input:
       self._properties: dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool] = input['properties']
     if 'pattern_properties' in input:
       self._pattern_properties: dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool] = input['pattern_properties']
     if 'dependencies' in input:
-      self._dependencies: dict[str,  | List[str]] = input['dependencies']
+      self._dependencies: dict[str, Any | List[str]] = input['dependencies']
     if 'property_names' in input:
       self._property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['property_names']
     if 'const' in input:
       self._const: Any = input['const']
     if 'enum' in input:
       self._enum: List[Any] = input['enum']
     if 'type' in input:
@@ -88,19 +88,19 @@
     if 'reserved_if' in input:
       self._reserved_if: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['reserved_if']
     if 'then' in input:
       self._then: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['then']
     if 'reserved_else' in input:
       self._reserved_else: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['reserved_else']
     if 'all_of' in input:
-      self._all_of: List[] = input['all_of']
+      self._all_of: List[Any] = input['all_of']
     if 'any_of' in input:
-      self._any_of: List[] = input['any_of']
+      self._any_of: List[Any] = input['any_of']
     if 'one_of' in input:
-      self._one_of: List[] = input['one_of']
+      self._one_of: List[Any] = input['one_of']
     if 'reserved_not' in input:
       self._reserved_not: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool = input['reserved_not']
     if 'discriminator' in input:
       self._discriminator: str = input['discriminator']
     if 'external_docs' in input:
       self._external_docs: Reference.Reference | ExternalDocs.ExternalDocs = input['external_docs']
     if 'deprecated' in input:
@@ -238,18 +238,18 @@
   def additional_items(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._additional_items
   @additional_items.setter
   def additional_items(self, additional_items: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._additional_items = additional_items
 
   @property
-  def items(self) ->  | List[]:
+  def items(self) -> Any | List[Any]:
     return self._items
   @items.setter
-  def items(self, items:  | List[]):
+  def items(self, items: Any | List[Any]):
     self._items = items
 
   @property
   def max_items(self) -> int:
     return self._max_items
   @max_items.setter
   def max_items(self, max_items: int):
@@ -322,18 +322,18 @@
   def pattern_properties(self) -> dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool]:
     return self._pattern_properties
   @pattern_properties.setter
   def pattern_properties(self, pattern_properties: dict[str, CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool]):
     self._pattern_properties = pattern_properties
 
   @property
-  def dependencies(self) -> dict[str,  | List[str]]:
+  def dependencies(self) -> dict[str, Any | List[str]]:
     return self._dependencies
   @dependencies.setter
-  def dependencies(self, dependencies: dict[str,  | List[str]]):
+  def dependencies(self, dependencies: dict[str, Any | List[str]]):
     self._dependencies = dependencies
 
   @property
   def property_names(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._property_names
   @property_names.setter
   def property_names(self, property_names: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
@@ -399,32 +399,32 @@
   def reserved_else(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._reserved_else
   @reserved_else.setter
   def reserved_else(self, reserved_else: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
     self._reserved_else = reserved_else
 
   @property
-  def all_of(self) -> List[]:
+  def all_of(self) -> List[Any]:
     return self._all_of
   @all_of.setter
-  def all_of(self, all_of: List[]):
+  def all_of(self, all_of: List[Any]):
     self._all_of = all_of
 
   @property
-  def any_of(self) -> List[]:
+  def any_of(self) -> List[Any]:
     return self._any_of
   @any_of.setter
-  def any_of(self, any_of: List[]):
+  def any_of(self, any_of: List[Any]):
     self._any_of = any_of
 
   @property
-  def one_of(self) -> List[]:
+  def one_of(self) -> List[Any]:
     return self._one_of
   @one_of.setter
-  def one_of(self, one_of: List[]):
+  def one_of(self, one_of: List[Any]):
     self._one_of = one_of
 
   @property
   def reserved_not(self) -> CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool:
     return self._reserved_not
   @reserved_not.setter
   def reserved_not(self, reserved_not: CoreSchemaMetaMinusSchemaObject.CoreSchemaMetaMinusSchemaObject | bool):
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Server.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Server.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObject.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObject.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectIbmmq.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectIbmmq.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectJms.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectJms.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectKafka.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectKafka.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectMqtt.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectMqtt.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectPulsar.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectPulsar.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectSolace.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerBindingsObjectSolace.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerSchema.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerSchema.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerVariable.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/ServerVariable.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SymmetricEncryption.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/SymmetricEncryption.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Tag.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/Tag.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/UserPassword.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/UserPassword.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/X509.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/src/asyncapi_python_parser_jonaslagoni/models/asyncapi_3_0_0/X509.py`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/tests/test_docs.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/tests/asyncapi_python_parser_jonaslagoni/test_docs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from src.parser import parse, ParserOptions, ValidationError
+from src.asyncapi_python_parser_jonaslagoni.parser import parse, ParserOptions, ValidationError
 from os import listdir
 from os.path import isfile, join
 import json
 
 class TestDocuments(unittest.TestCase):
     def test_all_3_0_0_example_docs(self):
         """
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/tests/test_parser.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/tests/asyncapi_python_parser_jonaslagoni/test_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import unittest
-from src.parser import parse, ParserOptions
-from src.validator import ValidationError
-from src.models.asyncapi_3_0_0.AsyncApi3Dot0Dot0SchemaDot import AsyncApi3Dot0Dot0SchemaDot 
-from src.models.asyncapi_2_6_0.AsyncApi2Dot6Dot0SchemaDot import AsyncApi2Dot6Dot0SchemaDot 
-from src.models.asyncapi_2_5_0.AsyncApi2Dot5Dot0SchemaDot import AsyncApi2Dot5Dot0SchemaDot 
-from src.models.asyncapi_2_4_0.AsyncApi2Dot4Dot0SchemaDot import AsyncApi2Dot4Dot0SchemaDot 
-from src.models.asyncapi_2_3_0.AsyncApi2Dot3Dot0SchemaDot import AsyncApi2Dot3Dot0SchemaDot 
-from src.models.asyncapi_2_2_0.AsyncApi2Dot2Dot0SchemaDot import AsyncApi2Dot2Dot0SchemaDot 
-from src.models.asyncapi_2_1_0.AsyncApi2Dot1Dot0SchemaDot import AsyncApi2Dot1Dot0SchemaDot 
-from src.models.asyncapi_2_0_0.AsyncApi2Dot0Dot0SchemaDot import AsyncApi2Dot0Dot0SchemaDot 
+from src.asyncapi_python_parser_jonaslagoni.parser import parse, ParserOptions
+from src.asyncapi_python_parser_jonaslagoni.validator import ValidationError
+from src.asyncapi_python_parser_jonaslagoni.models.asyncapi_3_0_0.AsyncApi3Dot0Dot0SchemaDot import AsyncApi3Dot0Dot0SchemaDot 
+from src.asyncapi_python_parser_jonaslagoni.models.asyncapi_2_6_0.AsyncApi2Dot6Dot0SchemaDot import AsyncApi2Dot6Dot0SchemaDot 
+from src.asyncapi_python_parser_jonaslagoni.models.asyncapi_2_5_0.AsyncApi2Dot5Dot0SchemaDot import AsyncApi2Dot5Dot0SchemaDot 
+from src.asyncapi_python_parser_jonaslagoni.models.asyncapi_2_4_0.AsyncApi2Dot4Dot0SchemaDot import AsyncApi2Dot4Dot0SchemaDot 
+from src.asyncapi_python_parser_jonaslagoni.models.asyncapi_2_3_0.AsyncApi2Dot3Dot0SchemaDot import AsyncApi2Dot3Dot0SchemaDot 
+from src.asyncapi_python_parser_jonaslagoni.models.asyncapi_2_2_0.AsyncApi2Dot2Dot0SchemaDot import AsyncApi2Dot2Dot0SchemaDot 
+from src.asyncapi_python_parser_jonaslagoni.models.asyncapi_2_1_0.AsyncApi2Dot1Dot0SchemaDot import AsyncApi2Dot1Dot0SchemaDot 
+from src.asyncapi_python_parser_jonaslagoni.models.asyncapi_2_0_0.AsyncApi2Dot0Dot0SchemaDot import AsyncApi2Dot0Dot0SchemaDot 
 
 class TestParser(unittest.TestCase):
     def test_parser_with_no_validation(self):
         """
         Test that we can parse with no validation
         """
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/tests/test_traits.py` & `asyncapi_python_parser_jonaslagoni-0.0.2/tests/asyncapi_python_parser_jonaslagoni/test_traits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from src.traits import apply_traits
+from src.asyncapi_python_parser_jonaslagoni.traits import apply_traits
 
 class TestTraits(unittest.TestCase):
   def test_traits_are_applied_correctly_for_v3(self):
     """
     Test that we can apply traits for v3 in all locations
     """
     message = {
```

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/tests/docs/3.0.0/streetlights-all.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/tests/docs/3.0.0/streetlights-all.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/tests/docs/3.0.0/streetlights-asyncapi.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/tests/docs/3.0.0/streetlights-asyncapi.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/tests/docs/3.0.0/streetlights-avro.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/tests/docs/3.0.0/streetlights-avro.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/tests/docs/3.0.0/streetlights-json.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/tests/docs/3.0.0/streetlights-json.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/tests/docs/3.0.0/streetlights-openapi.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/tests/docs/3.0.0/streetlights-openapi.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/tests/docs/3.0.0/streetlights-unknown.json` & `asyncapi_python_parser_jonaslagoni-0.0.2/tests/docs/3.0.0/streetlights-unknown.json`

 * *Files identical despite different names*

### Comparing `asyncapi_python_parser_jonaslagoni-0.0.1/pyproject.toml` & `asyncapi_python_parser_jonaslagoni-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "asyncapi_python_parser_jonaslagoni"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="jonaslagoni", email="jonas-lt@live.dk" },
 ]
 description = "An AsyncAPI python parser, that supports all versions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent",
-    "Development Status :: 2 - Pre-Alpha",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: Apache Software License",
+  "Operating System :: OS Independent",
+  "Development Status :: 2 - Pre-Alpha",
 ]
 
 [project.urls]
 Homepage = "https://github.com/jonaslagoni/asyncapi-python-parser"
 Issues = "https://github.com/jonaslagoni/asyncapi-python-parser/issues"
 
 [tool.semantic_release]
 assets = []
-commit_message = "{version}\n\nAutomatically generated by python-semantic-release"
+commit_message = "chore(release): v{version}\n\nAutomatically generated by python-semantic-release"
 commit_parser = "angular"
 logging_use_named_masks = false
 major_on_zero = true
 allow_zero_version = true
 tag_format = "v{version}"
+version_variable = [
+  "pyproject.toml:version",
+]
 
 [tool.semantic_release.branches.main]
-match = "(next|master)"
-prerelease_token = "rc"
+match = "main"
 prerelease = false
 
+[tool.semantic_release.branches.next]
+match = "next"
+prerelease_token = "next"
+prerelease = true
+
 [tool.semantic_release.changelog]
 template_dir = "templates"
 changelog_file = "CHANGELOG.md"
 exclude_commit_patterns = []
 
 [tool.semantic_release.changelog.environment]
 block_start_string = "{%"
```

