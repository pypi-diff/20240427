# Comparing `tmp/fastapi_jsonapi-2.7.0.tar.gz` & `tmp/fastapi_jsonapi-2.8.0.tar.gz`

## Comparing `fastapi_jsonapi-2.7.0.tar` & `fastapi_jsonapi-2.8.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/__init__.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_limited_methods.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_minimal.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/custom_filter_example.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/asgi.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/config.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/main.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/api/__init__.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/api/views_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/extensions/__init__.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/helpers/__init__.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/child.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/computer.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/enums.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/parent.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/parent_child_association.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/post.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/post_comment.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/user.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/user_bio.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/child.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/computer.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/parent.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/parent_child_association.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/post.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/post_comment.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/user.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/user_bio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/__init__.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/asgi.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/main.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/urls.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/api/__init__.py
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/api/user.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/__init__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/faker.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/meta_base.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/__init__.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/enums.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/pydantic/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/pydantic/user.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/tortoise/__init__.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/tortoise/user.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/VERSION
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/__init__.py
--rw-r--r--   0        0        0    25785 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/api.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_typing.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/jsonapi_typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/py.typed
--rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/querystring.py
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/schema.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/schema_base.py
--rw-r--r--   0        0        0    22054 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/schema_builder.py
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/signature.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/splitter.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/validation_utils.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/__init__.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/atomic.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/atomic_handler.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/prepared_atomic_operation.py
--rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/__init__.py
--rw-r--r--   0        0        0    18596 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/base.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/orm.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/shared.py
--rw-r--r--   0        0        0    37874 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sqla_orm.py
--rw-r--r--   0        0        0    17077 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/tortoise_orm.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/fields/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/fields/enum.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/fields/mixins.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/__init__.py
--rw-r--r--   0        0        0    17542 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py
--rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sorting/__init__.py
--rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/__init__.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/base.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/handlers.py
--rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/json_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/misc/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/misc/sqla/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/misc/sqla/generics/__init__.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/misc/sqla/generics/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/utils/__init__.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/utils/dependency_helper.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/utils/exceptions.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/utils/sqla.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/__init__.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/detail_view.py
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/list_view.py
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/utils.py
--rw-r--r--   0        0        0    17950 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/view_base.py
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/LICENSE
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/README.md
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     7869 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/__init__.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_limited_methods.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_minimal.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/custom_filter_example.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/asgi.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/config.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/main.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/api/__init__.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/api/views_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/extensions/__init__.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/helpers/__init__.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/child.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/computer.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/enums.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/parent.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/parent_child_association.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/post.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/post_comment.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/user.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/user_bio.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/child.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/computer.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/parent.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/parent_child_association.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/post.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/post_comment.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/user.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/user_bio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/__init__.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/asgi.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/main.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/urls.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/api/__init__.py
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/api/user.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/factories/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/factories/faker.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/factories/meta_base.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/factories/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/updaters/__init__.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/models/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/models/enums.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/models/pydantic/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/models/pydantic/user.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/models/tortoise/__init__.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/models/tortoise/user.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/VERSION
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/__init__.py
+-rw-r--r--   0        0        0    25849 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/api.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_typing.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/jsonapi_typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/py.typed
+-rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/querystring.py
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/schema.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/schema_base.py
+-rw-r--r--   0        0        0    23464 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/schema_builder.py
+-rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/signature.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/splitter.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/validation_utils.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/atomic/__init__.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/atomic/atomic.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/atomic/atomic_handler.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/atomic/prepared_atomic_operation.py
+-rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/atomic/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/__init__.py
+-rw-r--r--   0        0        0    18596 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/base.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/orm.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/shared.py
+-rw-r--r--   0        0        0    37874 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/sqla_orm.py
+-rw-r--r--   0        0        0    17077 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/tortoise_orm.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/fields/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/fields/enum.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/fields/mixins.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/filtering/__init__.py
+-rw-r--r--   0        0        0    17542 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py
+-rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/sorting/__init__.py
+-rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/exceptions/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/exceptions/base.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/exceptions/handlers.py
+-rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/exceptions/json_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/misc/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/misc/sqla/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/misc/sqla/generics/__init__.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/misc/sqla/generics/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/utils/__init__.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/utils/dependency_helper.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/utils/exceptions.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/utils/sqla.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/views/__init__.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/views/detail_view.py
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/views/list_view.py
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/views/utils.py
+-rw-r--r--   0        0        0    17950 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/fastapi_jsonapi/views/view_base.py
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/LICENSE
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/README.md
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7869 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.8.0/PKG-INFO
```

### Comparing `fastapi_jsonapi-2.7.0/examples/api_limited_methods.py` & `fastapi_jsonapi-2.8.0/examples/api_limited_methods.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_minimal.py` & `fastapi_jsonapi-2.8.0/examples/api_minimal.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/custom_filter_example.py` & `fastapi_jsonapi-2.8.0/examples/custom_filter_example.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/main.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/urls.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/urls.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/api/views_base.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/api/views_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/__init__.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/child.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/child.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/computer.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/computer.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/parent.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/parent.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/parent_child_association.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/parent_child_association.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/post.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/post.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/post_comment.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/post_comment.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/user.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/user_bio.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/user_bio.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/__init__.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/child.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/child.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/computer.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/computer.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/parent.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/parent.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/parent_child_association.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/parent_child_association.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/post.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/post.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/post_comment.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/post_comment.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/user.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/user_bio.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/models/schemas/user_bio.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py` & `fastapi_jsonapi-2.8.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/main.py` & `fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/urls.py` & `fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/urls.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/api/user.py` & `fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/api/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py` & `fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/meta_base.py` & `fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/factories/meta_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/user.py` & `fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/factories/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py` & `fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py` & `fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py` & `fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/pydantic/user.py` & `fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/models/pydantic/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/tortoise/user.py` & `fastapi_jsonapi-2.8.0/examples/api_for_tortoise_orm/models/tortoise/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/__init__.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/api.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         schema_in_post: Optional[Type[BaseModel]] = None,
         schema_in_patch: Optional[Type[BaseModel]] = None,
         pagination_default_size: Optional[int] = 25,
         pagination_default_number: Optional[int] = 1,
         pagination_default_offset: Optional[int] = None,
         pagination_default_limit: Optional[int] = None,
         methods: Iterable[str] = (),
+        max_cache_size: int = 0,
     ) -> None:
         """
         Initialize router items.
 
         :param router: APIRouter from FastAPI
         :param path: path prefix, for example `/users`
         :param tags: swagger tags
@@ -123,15 +124,15 @@
             raise ValueError(msg)
         self.all_jsonapi_routers[self.type_] = self
 
         self.pagination_default_size: Optional[int] = pagination_default_size
         self.pagination_default_number: Optional[int] = pagination_default_number
         self.pagination_default_offset: Optional[int] = pagination_default_offset
         self.pagination_default_limit: Optional[int] = pagination_default_limit
-        self.schema_builder = SchemaBuilder(resource_type=resource_type)
+        self.schema_builder = SchemaBuilder(resource_type=resource_type, max_cache_size=max_cache_size)
 
         dto = self.schema_builder.create_schemas(
             schema=schema,
             schema_in_post=schema_in_post,
             schema_in_patch=schema_in_patch,
         )
         # we need to save post_data and patch_data
```

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/querystring.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/querystring.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/schema.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/schema_base.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/schema_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/schema_builder.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/schema_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """JSON API schemas builder class."""
 from dataclasses import dataclass
+from functools import lru_cache
 from typing import (
     Any,
     Callable,
     ClassVar,
     Dict,
     Iterable,
     List,
@@ -118,16 +119,24 @@
     object_schemas_cache: ClassVar = {}
     relationship_schema_cache: ClassVar = {}
     base_jsonapi_object_schemas_cache: ClassVar = {}
 
     def __init__(
         self,
         resource_type: str,
+        max_cache_size: int = 0,
     ):
         self._resource_type = resource_type
+        self._init_cache(max_cache_size)
+
+    def _init_cache(self, max_cache_size: int):
+        # TODO: remove crutch
+        self._get_info_from_schema_for_building_cached = lru_cache(maxsize=max_cache_size)(
+            self._get_info_from_schema_for_building_cached,
+        )
 
     def _create_schemas_objects_list(self, schema: Type[BaseModel]) -> Type[JSONAPIResultListSchema]:
         object_jsonapi_list_schema, list_jsonapi_schema = self.build_list_schemas(schema)
         # TODO: do we need this `object_jsonapi_list_schema` field? it's not used anywhere 🤔
         # self.object_jsonapi_list_schema: Type[JSONAPIObjectSchema] = object_jsonapi_list_schema
         return list_jsonapi_schema
 
@@ -183,15 +192,15 @@
         schema_in: Type[BaseModel],
         schema_name_suffix: str = "",
         non_optional_relationships: bool = False,
         id_field_required: bool = False,
     ) -> Tuple[Type[BaseJSONAPIDataInSchema], Type[BaseJSONAPIItemInSchema]]:
         base_schema_name = schema_in.__name__.removesuffix("Schema") + schema_name_suffix
 
-        dto = self._get_info_from_schema_for_building(
+        dto = self._get_info_from_schema_for_building_wrapper(
             base_name=base_schema_name,
             schema=schema_in,
             non_optional_relationships=non_optional_relationships,
         )
 
         object_jsonapi_schema = self._build_jsonapi_object(
             base_name=base_schema_name,
@@ -254,14 +263,48 @@
         return self._build_schema(
             base_name=f"{schema.__name__}List",
             schema=schema,
             builder=self.build_schema_for_list_result,
             includes=includes,
         )
 
+    def _get_info_from_schema_for_building_cached(
+        self,
+        base_name: str,
+        schema: Type[BaseModel],
+        includes: Iterable[str],
+        non_optional_relationships: bool,
+    ):
+        return self._get_info_from_schema_for_building(
+            base_name=base_name,
+            schema=schema,
+            includes=includes,
+            non_optional_relationships=non_optional_relationships,
+        )
+
+    def _get_info_from_schema_for_building_wrapper(
+        self,
+        base_name: str,
+        schema: Type[BaseModel],
+        includes: Iterable[str] = not_passed,
+        non_optional_relationships: bool = False,
+    ):
+        """
+        Wrapper function for return cached schema result
+        """
+        if includes is not not_passed:
+            includes = tuple(includes)
+
+        return self._get_info_from_schema_for_building_cached(
+            base_name=base_name,
+            schema=schema,
+            includes=includes,
+            non_optional_relationships=non_optional_relationships,
+        )
+
     def _get_info_from_schema_for_building(
         self,
         base_name: str,
         schema: Type[BaseModel],
         includes: Iterable[str] = not_passed,
         non_optional_relationships: bool = False,
     ) -> SchemasInfoDTO:
@@ -490,15 +533,15 @@
 
         schema.update_forward_refs(**registry.schemas)
         base_name = base_name or schema.__name__
 
         if includes is not not_passed:
             includes = set(includes)
 
-        dto = self._get_info_from_schema_for_building(
+        dto = self._get_info_from_schema_for_building_wrapper(
             base_name=base_name,
             schema=schema,
             includes=includes,
         )
 
         object_jsonapi_schema = self._build_jsonapi_object(
             base_name=base_name,
```

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/signature.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/signature.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/validation_utils.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/validation_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/atomic.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/atomic/atomic.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/atomic_handler.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/atomic/atomic_handler.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/prepared_atomic_operation.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/atomic/prepared_atomic_operation.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/schemas.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/atomic/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/base.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/shared.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/shared.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sqla_orm.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/sqla_orm.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/tortoise_orm.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/tortoise_orm.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/fields/mixins.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/fields/mixins.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/__init__.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/base.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/json_api.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/exceptions/json_api.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/utils/dependency_helper.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/utils/dependency_helper.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/utils/sqla.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/utils/sqla.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/detail_view.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/views/detail_view.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/list_view.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/views/list_view.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/utils.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/views/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/view_base.py` & `fastapi_jsonapi-2.8.0/fastapi_jsonapi/views/view_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/.gitignore` & `fastapi_jsonapi-2.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/LICENSE` & `fastapi_jsonapi-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/README.md` & `fastapi_jsonapi-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/pyproject.toml` & `fastapi_jsonapi-2.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.7.0/PKG-INFO` & `fastapi_jsonapi-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: FastAPI-JSONAPI
-Version: 2.7.0
+Version: 2.8.0
 Summary: FastAPI extension to create REST web api according to JSON:API 1.0 specification with FastAPI, Pydantic and data provider of your choice (SQLAlchemy, Tortoise ORM)
 Project-URL: Documentation, https://fastapi-jsonapi.readthedocs.io/
 Project-URL: Source, https://github.com/mts-ai/FastAPI-JSONAPI
 Author-email: Aleksey Nekrasov <a.nekrasov@mts.ai>, Suren Khorenyan <s.khorenyan@mts.ai>, German Bernadskiy <german11235813@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: fastapi,json:api,jsonapi
```

