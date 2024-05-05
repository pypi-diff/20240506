# Comparing `tmp/phidata-2.3.90.tar.gz` & `tmp/phidata-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-2.3.90.tar", last modified: Fri May  3 15:30:14 2024, max compression
+gzip compressed data, was "phidata-2.4.0.tar", last modified: Sun May  5 23:07:22 2024, max compression
```

## Comparing `phidata-2.3.90.tar` & `phidata-2.4.0.tar`

### file list

```diff
@@ -1,650 +1,632 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.501718 phidata-2.3.90/
--rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-05-03 15:30:00.000000 phidata-2.3.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-05-03 15:30:14.501718 phidata-2.3.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-03 15:30:00.000000 phidata-2.3.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.417718 phidata-2.3.90/phi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.417718 phidata-2.3.90/phi/ai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/ai/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18047 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/ai/phi_ai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.417718 phidata-2.3.90/phi/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/ai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.421718 phidata-2.3.90/phi/api/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/schemas/ai.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/schemas/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/schemas/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/schemas/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/schemas/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.421718 phidata-2.3.90/phi/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/app/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/app/db_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/app/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.421718 phidata-2.3.90/phi/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39908 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    11160 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.421718 phidata-2.3.90/phi/assistant/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/openai/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/openai/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.425718 phidata-2.3.90/phi/assistant/openai/file/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/openai/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/openai/file/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/openai/file/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/openai/file/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/openai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/openai/row.py
--rw-r--r--   0 runner    (1001) docker     (127)    15218 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/openai/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/openai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.425718 phidata-2.3.90/phi/assistant/team/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/team/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/assistant/team/team.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.425718 phidata-2.3.90/phi/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.425718 phidata-2.3.90/phi/aws/app/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34343 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/app/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.425718 phidata-2.3.90/phi/aws/app/django/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/app/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/app/django/django.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.425718 phidata-2.3.90/phi/aws/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.425718 phidata-2.3.90/phi/aws/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/app/jupyter/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.425718 phidata-2.3.90/phi/aws/app/qdrant/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/app/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/app/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.425718 phidata-2.3.90/phi/aws/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.429718 phidata-2.3.90/phi/aws/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.429718 phidata-2.3.90/phi/aws/resource/acm/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/acm/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.429718 phidata-2.3.90/phi/aws/resource/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.429718 phidata-2.3.90/phi/aws/resource/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25483 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/ec2/security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/ec2/subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/ec2/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.429718 phidata-2.3.90/phi/aws/resource/ecs/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/ecs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/ecs/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    19749 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/ecs/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    23497 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/ecs/task_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/ecs/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.429718 phidata-2.3.90/phi/aws/resource/eks/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/eks/addon.py
--rw-r--r--   0 runner    (1001) docker     (127)    31036 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    13621 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    23482 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/eks/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.433718 phidata-2.3.90/phi/aws/resource/elasticache/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22631 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/elasticache/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.433718 phidata-2.3.90/phi/aws/resource/elb/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/elb/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/elb/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/elb/target_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.433718 phidata-2.3.90/phi/aws/resource/emr/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/emr/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.433718 phidata-2.3.90/phi/aws/resource/glue/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/glue/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.433718 phidata-2.3.90/phi/aws/resource/iam/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.433718 phidata-2.3.90/phi/aws/resource/rds/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42214 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/rds/db_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    36601 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/rds/db_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/rds/db_subnet_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.433718 phidata-2.3.90/phi/aws/resource/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/s3/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/s3/object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.433718 phidata-2.3.90/phi/aws/resource/secret/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/secret/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/secret/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    31475 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/aws/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.437718 phidata-2.3.90/phi/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/cli/auth_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/cli/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/cli/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    21503 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/cli/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.437718 phidata-2.3.90/phi/cli/k/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/cli/k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/cli/k/k_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/cli/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/cli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.437718 phidata-2.3.90/phi/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28536 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/cli/ws/ws_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.437718 phidata-2.3.90/phi/docker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.437718 phidata-2.3.90/phi/docker/app/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.437718 phidata-2.3.90/phi/docker/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17444 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/airflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/airflow/flower.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/airflow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/airflow/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/airflow/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.437718 phidata-2.3.90/phi/docker/app/django/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/django/django.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.441718 phidata-2.3.90/phi/docker/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.441718 phidata-2.3.90/phi/docker/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/jupyter/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.441718 phidata-2.3.90/phi/docker/app/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/mysql/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.441718 phidata-2.3.90/phi/docker/app/ollama/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/ollama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/ollama/ollama.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.441718 phidata-2.3.90/phi/docker/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/postgres/pgvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/postgres/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.441718 phidata-2.3.90/phi/docker/app/qdrant/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.441718 phidata-2.3.90/phi/docker/app/redis/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.441718 phidata-2.3.90/phi/docker/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.441718 phidata-2.3.90/phi/docker/app/superset/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/superset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/superset/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/superset/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/superset/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/superset/worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.441718 phidata-2.3.90/phi/docker/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/traefik/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.445718 phidata-2.3.90/phi/docker/app/whoami/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/whoami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/app/whoami/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.445718 phidata-2.3.90/phi/docker/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/resource/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    18301 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/resource/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/resource/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    31821 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/docker/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.445718 phidata-2.3.90/phi/document/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.445718 phidata-2.3.90/phi/document/reader/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/reader/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/reader/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/reader/docx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/reader/firecrawl_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/reader/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/reader/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.445718 phidata-2.3.90/phi/document/reader/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/reader/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/reader/s3/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/reader/s3/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/reader/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/document/reader/website.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.449718 phidata-2.3.90/phi/embedder/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/embedder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/embedder/anyscale.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/embedder/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/embedder/fireworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/embedder/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/embedder/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/embedder/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/embedder/together.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.449718 phidata-2.3.90/phi/file/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.449718 phidata-2.3.90/phi/file/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/file/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/file/local/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/file/local/txt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.449718 phidata-2.3.90/phi/infra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/infra/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/infra/type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.449718 phidata-2.3.90/phi/k8s/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.449718 phidata-2.3.90/phi/k8s/app/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.453718 phidata-2.3.90/phi/k8s/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/airflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/airflow/flower.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/airflow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/airflow/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/airflow/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    59192 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.453718 phidata-2.3.90/phi/k8s/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.453718 phidata-2.3.90/phi/k8s/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/jupyter/jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.453718 phidata-2.3.90/phi/k8s/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/postgres/pgvector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/postgres/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.453718 phidata-2.3.90/phi/k8s/app/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.453718 phidata-2.3.90/phi/k8s/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.453718 phidata-2.3.90/phi/k8s/app/superset/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/superset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/superset/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/superset/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/superset/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/superset/worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.453718 phidata-2.3.90/phi/k8s/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   115745 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/traefik/crds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/app/traefik/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.457718 phidata-2.3.90/phi/k8s/create/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.457718 phidata-2.3.90/phi/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.457718 phidata-2.3.90/phi/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.457718 phidata-2.3.90/phi/k8s/create/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.457718 phidata-2.3.90/phi/k8s/create/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.457718 phidata-2.3.90/phi/k8s/create/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/common/port.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.457718 phidata-2.3.90/phi/k8s/create/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.457718 phidata-2.3.90/phi/k8s/create/core/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.457718 phidata-2.3.90/phi/k8s/create/crb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/crb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/crb/eks_admin_crb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.461718 phidata-2.3.90/phi/k8s/create/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.461718 phidata-2.3.90/phi/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.461718 phidata-2.3.90/phi/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.461718 phidata-2.3.90/phi/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.461718 phidata-2.3.90/phi/k8s/create/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.461718 phidata-2.3.90/phi/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.461718 phidata-2.3.90/phi/k8s/enums/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/enums/api_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/enums/api_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/enums/image_pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/enums/kind.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/enums/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/enums/pv.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/enums/restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/enums/service_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/enums/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/enums/volume_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.461718 phidata-2.3.90/phi/k8s/helm/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/helm/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/helm/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.465718 phidata-2.3.90/phi/k8s/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.465718 phidata-2.3.90/phi/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.465718 phidata-2.3.90/phi/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.465718 phidata-2.3.90/phi/k8s/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.465718 phidata-2.3.90/phi/k8s/resource/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10016 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.465718 phidata-2.3.90/phi/k8s/resource/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.469718 phidata-2.3.90/phi/k8s/resource/core/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    18798 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    20764 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.469718 phidata-2.3.90/phi/k8s/resource/meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.469718 phidata-2.3.90/phi/k8s/resource/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.469718 phidata-2.3.90/phi/k8s/resource/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.469718 phidata-2.3.90/phi/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.469718 phidata-2.3.90/phi/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.469718 phidata-2.3.90/phi/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.473718 phidata-2.3.90/phi/k8s/resource/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.473718 phidata-2.3.90/phi/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resource/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)    46880 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/k8s/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.473718 phidata-2.3.90/phi/knowledge/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/docx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.473718 phidata-2.3.90/phi/knowledge/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/s3/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/s3/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/s3/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/website.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/knowledge/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.473718 phidata-2.3.90/phi/llm/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.477718 phidata-2.3.90/phi/llm/anthropic/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/anthropic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/anthropic/claude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.477718 phidata-2.3.90/phi/llm/anyscale/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/anyscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/anyscale/anyscale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.477718 phidata-2.3.90/phi/llm/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/aws/bedrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/aws/claude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.477718 phidata-2.3.90/phi/llm/azure/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/azure/openai_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.477718 phidata-2.3.90/phi/llm/cohere/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/cohere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/cohere/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.477718 phidata-2.3.90/phi/llm/fireworks/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/fireworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/fireworks/fireworks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.477718 phidata-2.3.90/phi/llm/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/gemini/gemini.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.477718 phidata-2.3.90/phi/llm/groq/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/groq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/groq/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.477718 phidata-2.3.90/phi/llm/mistral/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/mistral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/mistral/mistral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.477718 phidata-2.3.90/phi/llm/ollama/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/ollama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/ollama/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    22661 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/ollama/hermes.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/ollama/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    22739 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/ollama/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.481718 phidata-2.3.90/phi/llm/openai/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35298 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/openai/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/openai/like.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.481718 phidata-2.3.90/phi/llm/openrouter/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/openrouter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/openrouter/openrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.481718 phidata-2.3.90/phi/llm/together/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/together/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/llm/together/together.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.481718 phidata-2.3.90/phi/memory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/memory/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.481718 phidata-2.3.90/phi/memory/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/memory/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/memory/task/llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.481718 phidata-2.3.90/phi/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/prompt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/prompt/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/prompt/template.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.481718 phidata-2.3.90/phi/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/resource/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.481718 phidata-2.3.90/phi/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.481718 phidata-2.3.90/phi/storage/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/storage/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/storage/assistant/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/storage/assistant/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/storage/assistant/singlestore.py
--rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/storage/assistant/sqllite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.485718 phidata-2.3.90/phi/table/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.485718 phidata-2.3.90/phi/table/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/table/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/table/sql/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.485718 phidata-2.3.90/phi/task/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/task/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.485718 phidata-2.3.90/phi/task/llm/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/task/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39590 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/task/llm/llm_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.485718 phidata-2.3.90/phi/task/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/task/py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/task/py/python_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.489718 phidata-2.3.90/phi/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/apify.py
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/arxiv_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/csv_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14650 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/exa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.493718 phidata-2.3.90/phi/tools/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/fastapi/playground.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/newspaper4k.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/newspaper_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/openbb_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/phi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/pubmed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/resend_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/serpapi_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.493718 phidata-2.3.90/phi/tools/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/streamlit/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/tavily.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/tool_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/yfinance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/youtube_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/tools/zendesk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.493718 phidata-2.3.90/phi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/format_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/json_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/merge_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/py_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/response_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/utils/yaml_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.497718 phidata-2.3.90/phi/vectordb/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/distance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.497718 phidata-2.3.90/phi/vectordb/lancedb/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/lancedb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/lancedb/lancedb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.497718 phidata-2.3.90/phi/vectordb/pgvector/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/pgvector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/pgvector/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    13562 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/pgvector/pgvector.py
--rw-r--r--   0 runner    (1001) docker     (127)    15451 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/pgvector/pgvector2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.497718 phidata-2.3.90/phi/vectordb/pineconedb/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/pineconedb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/pineconedb/pineconedb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.497718 phidata-2.3.90/phi/vectordb/qdrant/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.497718 phidata-2.3.90/phi/vectordb/singlestore/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/singlestore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/singlestore/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/vectordb/singlestore/s2vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.501718 phidata-2.3.90/phi/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25334 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/workspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/workspace/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/workspace/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    31881 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/workspace/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-03 15:30:00.000000 phidata-2.3.90/phi/workspace/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.501718 phidata-2.3.90/phidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-05-03 15:30:14.000000 phidata-2.3.90/phidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15103 2024-05-03 15:30:14.000000 phidata-2.3.90/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:30:14.000000 phidata-2.3.90/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 15:30:14.000000 phidata-2.3.90/phidata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-03 15:30:14.000000 phidata-2.3.90/phidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-03 15:30:14.000000 phidata-2.3.90/phidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-03 15:30:00.000000 phidata-2.3.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:30:14.501718 phidata-2.3.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-03 15:30:00.000000 phidata-2.3.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:30:14.501718 phidata-2.3.90/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 15:30:00.000000 phidata-2.3.90/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.467978 phidata-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16754 2024-05-05 23:07:09.000000 phidata-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-05-05 23:07:22.467978 phidata-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-05 23:07:09.000000 phidata-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.387978 phidata-2.4.0/phi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.387978 phidata-2.4.0/phi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.387978 phidata-2.4.0/phi/api/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/schemas/ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/schemas/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/schemas/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/schemas/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/schemas/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.387978 phidata-2.4.0/phi/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/app/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/app/db_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/app/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.391978 phidata-2.4.0/phi/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67349 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.391978 phidata-2.4.0/phi/assistant/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/openai/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/openai/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.391978 phidata-2.4.0/phi/assistant/openai/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/openai/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/openai/file/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/openai/file/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/openai/file/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/openai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/openai/row.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15218 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/openai/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/openai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/assistant/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.391978 phidata-2.4.0/phi/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.391978 phidata-2.4.0/phi/aws/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34343 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/app/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.395978 phidata-2.4.0/phi/aws/app/django/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/app/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/app/django/django.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.395978 phidata-2.4.0/phi/aws/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.395978 phidata-2.4.0/phi/aws/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/app/jupyter/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.395978 phidata-2.4.0/phi/aws/app/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/app/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/app/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.395978 phidata-2.4.0/phi/aws/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.395978 phidata-2.4.0/phi/aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.395978 phidata-2.4.0/phi/aws/resource/acm/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/acm/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.395978 phidata-2.4.0/phi/aws/resource/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.395978 phidata-2.4.0/phi/aws/resource/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25483 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/ec2/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/ec2/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/ec2/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.399978 phidata-2.4.0/phi/aws/resource/ecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/ecs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/ecs/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19749 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/ecs/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23497 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/ecs/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.399978 phidata-2.4.0/phi/aws/resource/eks/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/eks/addon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31036 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13621 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23482 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/eks/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.399978 phidata-2.4.0/phi/aws/resource/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22631 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.399978 phidata-2.4.0/phi/aws/resource/elb/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/elb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/elb/target_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.399978 phidata-2.4.0/phi/aws/resource/emr/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/emr/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.399978 phidata-2.4.0/phi/aws/resource/glue/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12558 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/glue/crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.399978 phidata-2.4.0/phi/aws/resource/iam/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.403978 phidata-2.4.0/phi/aws/resource/rds/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42214 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36601 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/rds/db_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/rds/db_subnet_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.403978 phidata-2.4.0/phi/aws/resource/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/s3/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/s3/object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.403978 phidata-2.4.0/phi/aws/resource/secret/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11187 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/secret/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/secret/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31475 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/aws/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.403978 phidata-2.4.0/phi/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/cli/auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/cli/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19471 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/cli/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.403978 phidata-2.4.0/phi/cli/k/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/cli/k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/cli/k/k_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/cli/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/cli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.403978 phidata-2.4.0/phi/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28536 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/cli/ws/ws_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.403978 phidata-2.4.0/phi/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.407978 phidata-2.4.0/phi/docker/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.407978 phidata-2.4.0/phi/docker/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17444 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/airflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/airflow/flower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/airflow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/airflow/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/airflow/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.407978 phidata-2.4.0/phi/docker/app/django/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/django/django.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.407978 phidata-2.4.0/phi/docker/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.407978 phidata-2.4.0/phi/docker/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/jupyter/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.407978 phidata-2.4.0/phi/docker/app/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/mysql/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.407978 phidata-2.4.0/phi/docker/app/ollama/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/ollama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/ollama/ollama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.407978 phidata-2.4.0/phi/docker/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/postgres/pgvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/postgres/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.407978 phidata-2.4.0/phi/docker/app/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.407978 phidata-2.4.0/phi/docker/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/redis/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.411978 phidata-2.4.0/phi/docker/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.411978 phidata-2.4.0/phi/docker/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/superset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/superset/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/superset/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/superset/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/superset/worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.411978 phidata-2.4.0/phi/docker/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/traefik/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.411978 phidata-2.4.0/phi/docker/app/whoami/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/whoami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/app/whoami/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.411978 phidata-2.4.0/phi/docker/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/resource/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18301 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/resource/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/resource/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31821 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/docker/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.411978 phidata-2.4.0/phi/document/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.415978 phidata-2.4.0/phi/document/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/reader/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/reader/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/reader/docx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/reader/firecrawl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/reader/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/reader/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.415978 phidata-2.4.0/phi/document/reader/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/reader/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/reader/s3/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/reader/s3/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/reader/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/document/reader/website.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.415978 phidata-2.4.0/phi/embedder/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/embedder/anyscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/embedder/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/embedder/fireworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/embedder/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/embedder/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/embedder/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/embedder/together.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.415978 phidata-2.4.0/phi/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.415978 phidata-2.4.0/phi/file/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/file/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/file/local/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/file/local/txt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.415978 phidata-2.4.0/phi/infra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/infra/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/infra/type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.419978 phidata-2.4.0/phi/k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.419978 phidata-2.4.0/phi/k8s/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.419978 phidata-2.4.0/phi/k8s/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/airflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/airflow/flower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/airflow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/airflow/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/airflow/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59192 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.419978 phidata-2.4.0/phi/k8s/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.419978 phidata-2.4.0/phi/k8s/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/jupyter/jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.419978 phidata-2.4.0/phi/k8s/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/postgres/pgvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/postgres/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.419978 phidata-2.4.0/phi/k8s/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/redis/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.423978 phidata-2.4.0/phi/k8s/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.423978 phidata-2.4.0/phi/k8s/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/superset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/superset/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/superset/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/superset/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/superset/worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.423978 phidata-2.4.0/phi/k8s/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   115745 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/traefik/crds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/app/traefik/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.423978 phidata-2.4.0/phi/k8s/create/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.423978 phidata-2.4.0/phi/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.423978 phidata-2.4.0/phi/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.423978 phidata-2.4.0/phi/k8s/create/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.423978 phidata-2.4.0/phi/k8s/create/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.423978 phidata-2.4.0/phi/k8s/create/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/common/port.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.423978 phidata-2.4.0/phi/k8s/create/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.427978 phidata-2.4.0/phi/k8s/create/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.427978 phidata-2.4.0/phi/k8s/create/crb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/crb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/crb/eks_admin_crb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.427978 phidata-2.4.0/phi/k8s/create/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.427978 phidata-2.4.0/phi/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.427978 phidata-2.4.0/phi/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.427978 phidata-2.4.0/phi/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.427978 phidata-2.4.0/phi/k8s/create/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.427978 phidata-2.4.0/phi/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.431978 phidata-2.4.0/phi/k8s/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/enums/api_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/enums/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/enums/kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/enums/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/enums/pv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/enums/restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/enums/service_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/enums/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/enums/volume_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.431978 phidata-2.4.0/phi/k8s/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/helm/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/helm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.431978 phidata-2.4.0/phi/k8s/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.431978 phidata-2.4.0/phi/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.431978 phidata-2.4.0/phi/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.431978 phidata-2.4.0/phi/k8s/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.435978 phidata-2.4.0/phi/k8s/resource/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10016 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.435978 phidata-2.4.0/phi/k8s/resource/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.439978 phidata-2.4.0/phi/k8s/resource/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18798 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20764 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.439978 phidata-2.4.0/phi/k8s/resource/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.439978 phidata-2.4.0/phi/k8s/resource/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.439978 phidata-2.4.0/phi/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.439978 phidata-2.4.0/phi/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.439978 phidata-2.4.0/phi/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.439978 phidata-2.4.0/phi/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.439978 phidata-2.4.0/phi/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.439978 phidata-2.4.0/phi/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resource/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46880 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/k8s/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.443978 phidata-2.4.0/phi/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/docx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.443978 phidata-2.4.0/phi/knowledge/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/s3/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/s3/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/s3/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/knowledge/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.443978 phidata-2.4.0/phi/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.443978 phidata-2.4.0/phi/llm/anthropic/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/anthropic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/anthropic/claude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.443978 phidata-2.4.0/phi/llm/anyscale/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/anyscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/anyscale/anyscale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.443978 phidata-2.4.0/phi/llm/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/aws/bedrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/aws/claude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.447978 phidata-2.4.0/phi/llm/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/azure/openai_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.447978 phidata-2.4.0/phi/llm/cohere/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/cohere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/cohere/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.447978 phidata-2.4.0/phi/llm/fireworks/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/fireworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/fireworks/fireworks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.447978 phidata-2.4.0/phi/llm/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/gemini/gemini.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.447978 phidata-2.4.0/phi/llm/groq/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/groq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/groq/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.447978 phidata-2.4.0/phi/llm/mistral/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/mistral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/mistral/mistral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.447978 phidata-2.4.0/phi/llm/ollama/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/ollama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20162 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/ollama/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22661 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/ollama/hermes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/ollama/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22739 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/ollama/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.447978 phidata-2.4.0/phi/llm/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54253 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/openai/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/openai/like.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.447978 phidata-2.4.0/phi/llm/openrouter/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/openrouter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/openrouter/openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.451978 phidata-2.4.0/phi/llm/together/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/together/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/llm/together/together.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.451978 phidata-2.4.0/phi/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/memory/assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.451978 phidata-2.4.0/phi/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/prompt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/prompt/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/prompt/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.451978 phidata-2.4.0/phi/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/resource/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.451978 phidata-2.4.0/phi/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.451978 phidata-2.4.0/phi/storage/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/storage/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/storage/assistant/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/storage/assistant/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/storage/assistant/singlestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/storage/assistant/sqllite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.451978 phidata-2.4.0/phi/table/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.451978 phidata-2.4.0/phi/table/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/table/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/table/sql/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.451978 phidata-2.4.0/phi/task/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.459978 phidata-2.4.0/phi/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/apify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/arxiv_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/csv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14650 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/exa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.459978 phidata-2.4.0/phi/tools/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/fastapi/playground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/newspaper4k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/newspaper_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/openbb_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/phi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/pubmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/resend_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/serpapi_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.459978 phidata-2.4.0/phi/tools/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/streamlit/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/tavily.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/tool_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/yfinance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/youtube_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/tools/zendesk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.463978 phidata-2.4.0/phi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/format_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/merge_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/py_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/response_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/utils/yaml_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.463978 phidata-2.4.0/phi/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/distance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.463978 phidata-2.4.0/phi/vectordb/lancedb/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/lancedb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/lancedb/lancedb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.463978 phidata-2.4.0/phi/vectordb/pgvector/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/pgvector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/pgvector/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13562 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/pgvector/pgvector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15451 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/pgvector/pgvector2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.463978 phidata-2.4.0/phi/vectordb/pineconedb/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/pineconedb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/pineconedb/pineconedb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.463978 phidata-2.4.0/phi/vectordb/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.463978 phidata-2.4.0/phi/vectordb/singlestore/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/singlestore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/singlestore/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/vectordb/singlestore/s2vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.467978 phidata-2.4.0/phi/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.467978 phidata-2.4.0/phi/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25334 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/workspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/workspace/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/workspace/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31881 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/workspace/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-05 23:07:09.000000 phidata-2.4.0/phi/workspace/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.467978 phidata-2.4.0/phidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-05-05 23:07:22.000000 phidata-2.4.0/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-05-05 23:07:22.000000 phidata-2.4.0/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 23:07:22.000000 phidata-2.4.0/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-05 23:07:22.000000 phidata-2.4.0/phidata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-05 23:07:22.000000 phidata-2.4.0/phidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-05 23:07:22.000000 phidata-2.4.0/phidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-05 23:07:09.000000 phidata-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 23:07:22.467978 phidata-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-05 23:07:09.000000 phidata-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:07:22.467978 phidata-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-05 23:07:09.000000 phidata-2.4.0/tests/test_placeholder.py
```

### Comparing `phidata-2.3.90/LICENSE` & `phidata-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/PKG-INFO` & `phidata-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.3.90
-Summary: Add memory, knowledge and tools to LLMs.
+Version: 2.4.0
+Summary: Memory, knowledge and tools for LLMs.
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gitpython
 Requires-Dist: httpx
 Requires-Dist: pydantic
 Requires-Dist: pydantic-settings
 Requires-Dist: python-dotenv
```

### Comparing `phidata-2.3.90/README.md` & `phidata-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/api/api.py` & `phidata-2.4.0/phi/api/api.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/api/assistant.py` & `phidata-2.4.0/phi/api/assistant.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,41 +2,38 @@
 from typing import Union, Dict, List
 
 from httpx import Response
 
 from phi.api.api import api, invalid_response
 from phi.api.routes import ApiRoutes
 from phi.api.schemas.assistant import (
-    AssistantWorkspace,
     AssistantEventCreate,
     AssistantRunCreate,
 )
-from phi.constants import WORKSPACE_ID_ENV_VAR, WORKSPACE_HASH_ENV_VAR, WORKSPACE_KEY_ENV_VAR
+from phi.constants import PHI_API_KEY_ENV_VAR, PHI_WS_KEY_ENV_VAR
 from phi.cli.settings import phi_cli_settings
-from phi.utils.common import str_to_int
 from phi.utils.log import logger
 
 
 def create_assistant_run(run: AssistantRunCreate) -> bool:
     if not phi_cli_settings.api_enabled:
         return True
 
-    # logger.debug("--o-o-- Creating Assistant Run")
+    logger.debug("--o-o-- Creating Assistant Run")
     with api.AuthenticatedClient() as api_client:
         try:
-            assistant_workspace = AssistantWorkspace(
-                id_workspace=str_to_int(getenv(WORKSPACE_ID_ENV_VAR)),
-                ws_hash=getenv(WORKSPACE_HASH_ENV_VAR),
-                ws_key=getenv(WORKSPACE_KEY_ENV_VAR),
-            )
             r: Response = api_client.post(
                 ApiRoutes.ASSISTANT_RUN_CREATE,
+                headers={
+                    "Authorization": f"Bearer {getenv(PHI_API_KEY_ENV_VAR)}",
+                    "PHI-WORKSPACE": f"{getenv(PHI_WS_KEY_ENV_VAR)}",
+                },
                 json={
                     "run": run.model_dump(exclude_none=True),
-                    "workspace": assistant_workspace.model_dump(exclude_none=True),
+                    # "workspace": assistant_workspace.model_dump(exclude_none=True),
                 },
             )
             if invalid_response(r):
                 return False
 
             response_json: Union[Dict, List] = r.json()
             if response_json is None:
@@ -49,26 +46,26 @@
     return False
 
 
 def create_assistant_event(event: AssistantEventCreate) -> bool:
     if not phi_cli_settings.api_enabled:
         return True
 
+    logger.debug("--o-o-- Creating Assistant Event")
     with api.AuthenticatedClient() as api_client:
         try:
-            assistant_workspace = AssistantWorkspace(
-                id_workspace=str_to_int(getenv(WORKSPACE_ID_ENV_VAR)),
-                ws_hash=getenv(WORKSPACE_HASH_ENV_VAR),
-                ws_key=getenv(WORKSPACE_KEY_ENV_VAR),
-            )
             r: Response = api_client.post(
                 ApiRoutes.ASSISTANT_EVENT_CREATE,
+                headers={
+                    "Authorization": f"Bearer {getenv(PHI_API_KEY_ENV_VAR)}",
+                    "PHI-WORKSPACE": f"{getenv(PHI_WS_KEY_ENV_VAR)}",
+                },
                 json={
                     "event": event.model_dump(exclude_none=True),
-                    "workspace": assistant_workspace.model_dump(exclude_none=True),
+                    # "workspace": assistant_workspace.model_dump(exclude_none=True),
                 },
             )
             if invalid_response(r):
                 return False
 
             response_json: Union[Dict, List] = r.json()
             if response_json is None:
```

### Comparing `phidata-2.3.90/phi/api/prompt.py` & `phidata-2.4.0/phi/api/prompt.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/api/routes.py` & `phidata-2.4.0/phi/api/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,21 +19,14 @@
     WORKSPACE_UPDATE: str = "/v1/workspace/update"
     WORKSPACE_DELETE: str = "/v1/workspace/delete"
     WORKSPACE_EVENT_CREATE: str = "/v1/workspace/event/create"
     WORKSPACE_UPDATE_PRIMARY: str = "/v1/workspace/update/primary"
     WORKSPACE_READ_PRIMARY: str = "/v1/workspace/read/primary"
     WORKSPACE_READ_AVAILABLE: str = "/v1/workspace/read/available"
 
-    # monitor paths
-    MONITOR_EVENT_CREATE: str = "/v1/monitor/event/create"
-
-    # conversation paths
-    CONVERSATION_MONITOR_CREATE: str = "/v1/conversation/monitor/create"
-    CONVERSATION_EVENT_CREATE: str = "/v1/conversation/event/create"
-
     # assistant paths
     ASSISTANT_RUN_CREATE: str = "/v1/assistant/run/create"
     ASSISTANT_EVENT_CREATE: str = "/v1/assistant/event/create"
 
     # prompt paths
     PROMPT_REGISTRY_SYNC: str = "/v1/prompt/registry/sync"
     PROMPT_TEMPLATE_SYNC: str = "/v1/prompt/template/sync"
```

### Comparing `phidata-2.3.90/phi/api/schemas/prompt.py` & `phidata-2.4.0/phi/api/schemas/prompt.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/api/schemas/workspace.py` & `phidata-2.4.0/phi/api/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/api/user.py` & `phidata-2.4.0/phi/api/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
     from phi.cli.credentials import save_auth_token
 
     logger.debug("--o-o-- Creating anon user")
     with api.Client() as api_client:
         try:
             r: Response = api_client.post(
-                ApiRoutes.USER_CREATE, json={"email": "anon", "username": "anon", "is_bot": True}
+                ApiRoutes.USER_CREATE, json={"user": {"email": "anon", "username": "anon", "is_bot": True}}
             )
             if invalid_response(r):
                 return None
 
             phidata_auth_token = r.headers.get(phi_cli_settings.auth_token_header)
             if phidata_auth_token is None:
                 logger.error("Could not authenticate user")
```

### Comparing `phidata-2.3.90/phi/api/workspace.py` & `phidata-2.4.0/phi/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/app/base.py` & `phidata-2.4.0/phi/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/app/context.py` & `phidata-2.4.0/phi/app/context.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/app/db_app.py` & `phidata-2.4.0/phi/app/db_app.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/app/group.py` & `phidata-2.4.0/phi/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/assistant/duckdb.py` & `phidata-2.4.0/phi/assistant/duckdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Optional, List
 from pathlib import Path
 
 from pydantic import model_validator
 from textwrap import dedent
 
-from phi.assistant.custom import CustomAssistant
+from phi.assistant import Assistant
 from phi.tools.duckdb import DuckDbTools
 from phi.tools.file import FileTools
 from phi.utils.log import logger
 
 try:
     import duckdb
 except ImportError:
     raise ImportError("`duckdb` not installed. Please install using `pip install duckdb`.")
 
 
-class DuckDbAssistant(CustomAssistant):
+class DuckDbAssistant(Assistant):
     name: str = "DuckDbAssistant"
     semantic_model: Optional[str] = None
 
     add_chat_history_to_messages: bool = True
     num_history_messages: int = 6
 
     followups: bool = False
```

### Comparing `phidata-2.3.90/phi/assistant/openai/assistant.py` & `phidata-2.4.0/phi/assistant/openai/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/assistant/openai/file/file.py` & `phidata-2.4.0/phi/assistant/openai/file/file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/assistant/openai/file/local.py` & `phidata-2.4.0/phi/assistant/openai/file/local.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/assistant/openai/file/url.py` & `phidata-2.4.0/phi/assistant/openai/file/url.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/assistant/openai/message.py` & `phidata-2.4.0/phi/assistant/openai/message.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/assistant/openai/row.py` & `phidata-2.4.0/phi/assistant/openai/row.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/assistant/openai/run.py` & `phidata-2.4.0/phi/assistant/openai/run.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/assistant/openai/thread.py` & `phidata-2.4.0/phi/assistant/openai/thread.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/assistant/python.py` & `phidata-2.4.0/phi/assistant/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Optional, List, Dict, Any
 from pathlib import Path
 
 from pydantic import model_validator
 from textwrap import dedent
 
-from phi.assistant.custom import CustomAssistant
+from phi.assistant import Assistant
 from phi.file import File
 from phi.tools.python import PythonTools
 from phi.utils.log import logger
 
 
-class PythonAssistant(CustomAssistant):
+class PythonAssistant(Assistant):
     name: str = "PythonAssistant"
 
     files: Optional[List[File]] = None
     file_information: Optional[str] = None
 
     add_chat_history_to_messages: bool = True
     num_history_messages: int = 6
```

### Comparing `phidata-2.3.90/phi/assistant/run.py` & `phidata-2.4.0/phi/assistant/run.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/api_client.py` & `phidata-2.4.0/phi/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/app/base.py` & `phidata-2.4.0/phi/aws/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/app/django/django.py` & `phidata-2.4.0/phi/aws/app/django/django.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/app/fastapi/fastapi.py` & `phidata-2.4.0/phi/aws/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/app/jupyter/jupyter.py` & `phidata-2.4.0/phi/aws/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/app/qdrant/qdrant.py` & `phidata-2.4.0/phi/aws/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/app/streamlit/streamlit.py` & `phidata-2.4.0/phi/aws/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/acm/certificate.py` & `phidata-2.4.0/phi/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/base.py` & `phidata-2.4.0/phi/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/cloudformation/stack.py` & `phidata-2.4.0/phi/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/ec2/security_group.py` & `phidata-2.4.0/phi/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/ec2/subnet.py` & `phidata-2.4.0/phi/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/ec2/volume.py` & `phidata-2.4.0/phi/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/ecs/cluster.py` & `phidata-2.4.0/phi/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/ecs/container.py` & `phidata-2.4.0/phi/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/ecs/service.py` & `phidata-2.4.0/phi/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/ecs/task_definition.py` & `phidata-2.4.0/phi/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/ecs/volume.py` & `phidata-2.4.0/phi/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/eks/addon.py` & `phidata-2.4.0/phi/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/eks/cluster.py` & `phidata-2.4.0/phi/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/eks/fargate_profile.py` & `phidata-2.4.0/phi/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/eks/kubeconfig.py` & `phidata-2.4.0/phi/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/eks/node_group.py` & `phidata-2.4.0/phi/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/elasticache/cluster.py` & `phidata-2.4.0/phi/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/elasticache/subnet_group.py` & `phidata-2.4.0/phi/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/elb/listener.py` & `phidata-2.4.0/phi/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/elb/load_balancer.py` & `phidata-2.4.0/phi/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/elb/target_group.py` & `phidata-2.4.0/phi/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/emr/cluster.py` & `phidata-2.4.0/phi/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/glue/crawler.py` & `phidata-2.4.0/phi/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/iam/policy.py` & `phidata-2.4.0/phi/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/iam/role.py` & `phidata-2.4.0/phi/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/rds/db_cluster.py` & `phidata-2.4.0/phi/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/rds/db_instance.py` & `phidata-2.4.0/phi/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/rds/db_subnet_group.py` & `phidata-2.4.0/phi/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/s3/bucket.py` & `phidata-2.4.0/phi/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/s3/object.py` & `phidata-2.4.0/phi/aws/resource/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/secret/manager.py` & `phidata-2.4.0/phi/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/secret/reader.py` & `phidata-2.4.0/phi/aws/resource/secret/reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resource/types.py` & `phidata-2.4.0/phi/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/aws/resources.py` & `phidata-2.4.0/phi/aws/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/base.py` & `phidata-2.4.0/phi/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/cli/auth_server.py` & `phidata-2.4.0/phi/cli/auth_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 
 class CliAuthServer:
     """
     Source: https://stackoverflow.com/a/38196725/10953921
     """
 
-    def __init__(self, port=9191):
+    def __init__(self, port: int = 9191):
         import threading
 
         self._server = HTTPServer(("", port), CliAuthRequestHandler)
         self._thread = threading.Thread(target=self.run)
         self._thread.daemon = True
         self._server.running = False  # type: ignore
 
@@ -78,20 +78,33 @@
     def start(self):
         self._thread.start()
 
     def shut_down(self):
         self._thread.close()  # type: ignore
 
 
+def check_port(port: int):
+    import socket
+
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        try:
+            return s.connect_ex(("localhost", port)) == 0
+        except Exception as e:
+            print(f"Error occurred: {e}")
+            return False
+
+
 def get_port_for_auth_server():
-    # TODO: Check if port is available
-    return 9191
+    starting_port = 9191
+    for port in range(starting_port, starting_port + 100):
+        if not check_port(port):
+            return port
 
 
-def get_auth_token_from_web_flow(port) -> Optional[str]:
+def get_auth_token_from_web_flow(port: int) -> Optional[str]:
     """
     GET request: curl http://localhost:9191
     POST request: curl -d "foo=bar&bin=baz" http://localhost:9191
     """
     import json
 
     server = CliAuthServer(port)
```

### Comparing `phidata-2.3.90/phi/cli/config.py` & `phidata-2.4.0/phi/cli/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/cli/console.py` & `phidata-2.4.0/phi/cli/console.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/cli/credentials.py` & `phidata-2.4.0/phi/cli/credentials.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/cli/entrypoint.py` & `phidata-2.4.0/phi/cli/entrypoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,86 +204,14 @@
 
     if print_debug_log:
         set_log_level_to_debug()
 
     set_workspace_as_active(ws_dir_name=ws_name)
 
 
-@phi_cli.command(short_help="Chat with Phi AI", options_metavar="", hidden=True)
-def ai(
-    start_new_conversation: bool = typer.Option(
-        False,
-        "-n",
-        "--new",
-        help="Start a new conversation.",
-    ),
-    autonomous_conversation: bool = typer.Option(
-        True,
-        "-a",
-        "--autonomous",
-        help="Start an autonomous conversation that can call functions and take actions.",
-    ),
-    print_conversation_history: bool = typer.Option(
-        False,
-        "-h",
-        "--history",
-        help="Show all previous messages.",
-    ),
-    batch: bool = typer.Option(
-        False,
-        "-b",
-        "--batch",
-        help="Return the response as a batch i.e do not stream the response.",
-    ),
-    print_debug_log: bool = typer.Option(
-        False,
-        "-d",
-        "--debug",
-        help="Print debug logs.",
-    ),
-):
-    """
-    Chat with Phi AI
-
-    \b
-    Examples:
-    $ `phi ai`      -> Start a conversation with Phi AI
-    """
-
-    if print_debug_log:
-        set_log_level_to_debug()
-
-    from phi.cli.config import PhiCliConfig
-    from phi.cli.operator import initialize_phi
-    from phi.cli.console import log_config_not_available_msg
-    from phi.ai.operator import phi_ai_conversation
-
-    phi_config: Optional[PhiCliConfig] = PhiCliConfig.from_saved_config()
-    if not phi_config:
-        init_success = initialize_phi()
-        if not init_success:
-            from phi.cli.console import log_phi_init_failed_msg
-
-            log_phi_init_failed_msg()
-            return False
-        phi_config = PhiCliConfig.from_saved_config()
-        # If phi_config is still None, throw an error
-        if not phi_config:
-            log_config_not_available_msg()
-            return False
-
-    phi_ai_conversation(
-        phi_config=phi_config,
-        start_new_conversation=start_new_conversation,
-        autonomous_conversation=autonomous_conversation,
-        print_conversation_history=print_conversation_history,
-        stream=(not batch),
-    )
-
-
 @phi_cli.command(short_help="Start resources defined in a resources.py file")
 def start(
     resources_file: str = typer.Argument(
         "resources.py",
         help="Path to workspace file.",
         show_default=False,
     ),
```

### Comparing `phidata-2.3.90/phi/cli/k/k_cli.py` & `phidata-2.4.0/phi/cli/k/k_cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/cli/operator.py` & `phidata-2.4.0/phi/cli/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/cli/settings.py` & `phidata-2.4.0/phi/cli/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/cli/ws/ws_cli.py` & `phidata-2.4.0/phi/cli/ws/ws_cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/constants.py` & `phidata-2.4.0/phi/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 PYTHONPATH_ENV_VAR: str = "PYTHONPATH"
 PHI_RUNTIME_ENV_VAR: str = "PHI_RUNTIME"
+PHI_API_KEY_ENV_VAR: str = "PHI_API_KEY"
+PHI_WS_KEY_ENV_VAR: str = "PHI_WS_KEY"
 
 SCRIPTS_DIR_ENV_VAR: str = "PHI_SCRIPTS_DIR"
 STORAGE_DIR_ENV_VAR: str = "PHI_STORAGE_DIR"
 WORKFLOWS_DIR_ENV_VAR: str = "PHI_WORKFLOWS_DIR"
 WORKSPACE_NAME_ENV_VAR: str = "PHI_WORKSPACE_NAME"
 WORKSPACE_ROOT_ENV_VAR: str = "PHI_WORKSPACE_ROOT"
 WORKSPACES_MOUNT_ENV_VAR: str = "PHI_WORKSPACES_MOUNT"
```

### Comparing `phidata-2.3.90/phi/docker/api_client.py` & `phidata-2.4.0/phi/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/app/airflow/base.py` & `phidata-2.4.0/phi/docker/app/airflow/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/app/airflow/worker.py` & `phidata-2.4.0/phi/docker/app/airflow/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/app/base.py` & `phidata-2.4.0/phi/docker/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/app/django/django.py` & `phidata-2.4.0/phi/docker/app/django/django.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/app/fastapi/fastapi.py` & `phidata-2.4.0/phi/docker/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/app/jupyter/jupyter.py` & `phidata-2.4.0/phi/docker/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/app/mysql/mysql.py` & `phidata-2.4.0/phi/docker/app/mysql/mysql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/app/postgres/postgres.py` & `phidata-2.4.0/phi/docker/app/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/app/qdrant/qdrant.py` & `phidata-2.4.0/phi/docker/app/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/app/redis/redis.py` & `phidata-2.4.0/phi/docker/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/app/streamlit/streamlit.py` & `phidata-2.4.0/phi/docker/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/app/superset/base.py` & `phidata-2.4.0/phi/docker/app/superset/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/app/traefik/router.py` & `phidata-2.4.0/phi/docker/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/resource/base.py` & `phidata-2.4.0/phi/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/resource/container.py` & `phidata-2.4.0/phi/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/resource/image.py` & `phidata-2.4.0/phi/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/resource/network.py` & `phidata-2.4.0/phi/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/resource/types.py` & `phidata-2.4.0/phi/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/resource/volume.py` & `phidata-2.4.0/phi/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/docker/resources.py` & `phidata-2.4.0/phi/docker/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/document/base.py` & `phidata-2.4.0/phi/document/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/document/reader/arxiv.py` & `phidata-2.4.0/phi/document/reader/arxiv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/document/reader/base.py` & `phidata-2.4.0/phi/document/reader/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/document/reader/docx.py` & `phidata-2.4.0/phi/document/reader/docx.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/document/reader/firecrawl_reader.py` & `phidata-2.4.0/phi/document/reader/firecrawl_reader.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/document/reader/json.py` & `phidata-2.4.0/phi/document/reader/json.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/document/reader/pdf.py` & `phidata-2.4.0/phi/document/reader/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/document/reader/s3/pdf.py` & `phidata-2.4.0/phi/document/reader/s3/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/document/reader/s3/text.py` & `phidata-2.4.0/phi/document/reader/s3/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/document/reader/text.py` & `phidata-2.4.0/phi/document/reader/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/document/reader/website.py` & `phidata-2.4.0/phi/document/reader/website.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/embedder/mistral.py` & `phidata-2.4.0/phi/embedder/mistral.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/embedder/ollama.py` & `phidata-2.4.0/phi/embedder/ollama.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/embedder/openai.py` & `phidata-2.4.0/phi/embedder/openai.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/file/local/csv.py` & `phidata-2.4.0/phi/file/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/infra/resources.py` & `phidata-2.4.0/phi/infra/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/api_client.py` & `phidata-2.4.0/phi/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/app/airflow/base.py` & `phidata-2.4.0/phi/k8s/app/airflow/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/app/airflow/worker.py` & `phidata-2.4.0/phi/k8s/app/airflow/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/app/base.py` & `phidata-2.4.0/phi/k8s/app/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/app/fastapi/fastapi.py` & `phidata-2.4.0/phi/k8s/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/app/jupyter/jupyter.py` & `phidata-2.4.0/phi/k8s/app/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/app/postgres/postgres.py` & `phidata-2.4.0/phi/k8s/app/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/app/redis/redis.py` & `phidata-2.4.0/phi/k8s/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/app/streamlit/streamlit.py` & `phidata-2.4.0/phi/k8s/app/streamlit/streamlit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/app/superset/base.py` & `phidata-2.4.0/phi/k8s/app/superset/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/app/traefik/crds.py` & `phidata-2.4.0/phi/k8s/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/app/traefik/router.py` & `phidata-2.4.0/phi/k8s/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.4.0/phi/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.4.0/phi/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/apps/v1/deployment.py` & `phidata-2.4.0/phi/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/base.py` & `phidata-2.4.0/phi/k8s/create/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/common/port.py` & `phidata-2.4.0/phi/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/core/v1/config_map.py` & `phidata-2.4.0/phi/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/core/v1/container.py` & `phidata-2.4.0/phi/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/core/v1/namespace.py` & `phidata-2.4.0/phi/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/core/v1/persistent_volume.py` & `phidata-2.4.0/phi/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-2.4.0/phi/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/core/v1/secret.py` & `phidata-2.4.0/phi/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/core/v1/service.py` & `phidata-2.4.0/phi/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/core/v1/service_account.py` & `phidata-2.4.0/phi/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/core/v1/volume.py` & `phidata-2.4.0/phi/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/crb/eks_admin_crb.py` & `phidata-2.4.0/phi/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-2.4.0/phi/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.4.0/phi/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.4.0/phi/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-2.4.0/phi/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/enums/api_version.py` & `phidata-2.4.0/phi/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/enums/kind.py` & `phidata-2.4.0/phi/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/enums/pv.py` & `phidata-2.4.0/phi/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/helm/chart.py` & `phidata-2.4.0/phi/k8s/helm/chart.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/helm/cli.py` & `phidata-2.4.0/phi/k8s/helm/cli.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/operator.py` & `phidata-2.4.0/phi/k8s/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-2.4.0/phi/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-2.4.0/phi/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/apps/v1/deployment.py` & `phidata-2.4.0/phi/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-2.4.0/phi/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/base.py` & `phidata-2.4.0/phi/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/config_map.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/container.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/local_object_reference.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/namespace.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/node_selector.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/object_reference.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/persistent_volume.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/pod.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/pod_spec.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/pod_template_spec.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/resource_requirements.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/secret.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/service.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/service_account.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/toleration.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/volume.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/core/v1/volume_source.py` & `phidata-2.4.0/phi/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/kubeconfig.py` & `phidata-2.4.0/phi/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/meta/v1/label_selector.py` & `phidata-2.4.0/phi/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/meta/v1/object_meta.py` & `phidata-2.4.0/phi/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-2.4.0/phi/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-2.4.0/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-2.4.0/phi/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-2.4.0/phi/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/types.py` & `phidata-2.4.0/phi/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resource/yaml.py` & `phidata-2.4.0/phi/k8s/resource/yaml.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/k8s/resources.py` & `phidata-2.4.0/phi/k8s/resources.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/arxiv.py` & `phidata-2.4.0/phi/knowledge/arxiv.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/base.py` & `phidata-2.4.0/phi/knowledge/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/combined.py` & `phidata-2.4.0/phi/knowledge/combined.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/document.py` & `phidata-2.4.0/phi/knowledge/document.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/docx.py` & `phidata-2.4.0/phi/knowledge/docx.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/json.py` & `phidata-2.4.0/phi/knowledge/json.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/langchain.py` & `phidata-2.4.0/phi/knowledge/langchain.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/pdf.py` & `phidata-2.4.0/phi/knowledge/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/s3/base.py` & `phidata-2.4.0/phi/knowledge/s3/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/s3/pdf.py` & `phidata-2.4.0/phi/knowledge/s3/pdf.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/s3/text.py` & `phidata-2.4.0/phi/knowledge/s3/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/text.py` & `phidata-2.4.0/phi/knowledge/text.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/website.py` & `phidata-2.4.0/phi/knowledge/website.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/knowledge/wikipedia.py` & `phidata-2.4.0/phi/knowledge/wikipedia.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/llm/anthropic/claude.py` & `phidata-2.4.0/phi/llm/anthropic/claude.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/llm/aws/bedrock.py` & `phidata-2.4.0/phi/llm/aws/bedrock.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/llm/aws/claude.py` & `phidata-2.4.0/phi/llm/aws/claude.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/llm/azure/openai_chat.py` & `phidata-2.4.0/phi/llm/azure/openai_chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,32 +19,34 @@
     azure_deployment: Optional[str] = getenv("AZURE_DEPLOYMENT")
     base_url: Optional[str] = None
     azure_ad_token: Optional[str] = None
     azure_ad_token_provider: Optional[Any] = None
     openai_client: Optional[AzureOpenAIClient] = None
 
     @property
-    def client(self) -> AzureOpenAIClient:
+    def get_client(self) -> AzureOpenAIClient:  # type: ignore
         if self.openai_client:
             return self.openai_client
 
-        _openai_params: Dict[str, Any] = {}
+        _client_params: Dict[str, Any] = {}
         if self.api_key:
-            _openai_params["api_key"] = self.api_key
+            _client_params["api_key"] = self.api_key
         if self.api_version:
-            _openai_params["api_version"] = self.api_version
+            _client_params["api_version"] = self.api_version
         if self.organization:
-            _openai_params["organization"] = self.organization
+            _client_params["organization"] = self.organization
         if self.azure_endpoint:
-            _openai_params["azure_endpoint"] = self.azure_endpoint
+            _client_params["azure_endpoint"] = self.azure_endpoint
         if self.azure_deployment:
-            _openai_params["azure_deployment"] = self.azure_deployment
+            _client_params["azure_deployment"] = self.azure_deployment
         if self.base_url:
-            _openai_params["base_url"] = self.base_url
+            _client_params["base_url"] = self.base_url
         if self.azure_ad_token:
-            _openai_params["azure_ad_token"] = self.azure_ad_token
+            _client_params["azure_ad_token"] = self.azure_ad_token
         if self.azure_ad_token_provider:
-            _openai_params["azure_ad_token_provider"] = self.azure_ad_token_provider
+            _client_params["azure_ad_token_provider"] = self.azure_ad_token_provider
+        if self.http_client:
+            _client_params["http_client"] = self.http_client
         if self.client_params:
-            _openai_params.update(self.client_params)
+            _client_params.update(self.client_params)
 
-        return AzureOpenAIClient(**_openai_params)
+        return AzureOpenAIClient(**_client_params)
```

### Comparing `phidata-2.3.90/phi/llm/base.py` & `phidata-2.4.0/phi/llm/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,23 +54,35 @@
     @property
     def api_kwargs(self) -> Dict[str, Any]:
         raise NotImplementedError
 
     def invoke(self, *args, **kwargs) -> Any:
         raise NotImplementedError
 
+    async def ainvoke(self, *args, **kwargs) -> Any:
+        raise NotImplementedError
+
     def invoke_stream(self, *args, **kwargs) -> Iterator[Any]:
         raise NotImplementedError
 
+    async def ainvoke_stream(self, *args, **kwargs) -> Any:
+        raise NotImplementedError
+
     def response(self, messages: List[Message]) -> str:
         raise NotImplementedError
 
+    async def aresponse(self, messages: List[Message]) -> str:
+        raise NotImplementedError
+
     def response_stream(self, messages: List[Message]) -> Iterator[str]:
         raise NotImplementedError
 
+    async def aresponse_stream(self, messages: List[Message]) -> Any:
+        raise NotImplementedError
+
     def generate(self, messages: List[Message]) -> Dict:
         raise NotImplementedError
 
     def generate_stream(self, messages: List[Message]) -> Iterator[Dict]:
         raise NotImplementedError
 
     def to_dict(self) -> Dict[str, Any]:
```

### Comparing `phidata-2.3.90/phi/llm/cohere/chat.py` & `phidata-2.4.0/phi/llm/cohere/chat.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/llm/gemini/gemini.py` & `phidata-2.4.0/phi/llm/gemini/gemini.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/llm/groq/groq.py` & `phidata-2.4.0/phi/llm/groq/groq.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/llm/message.py` & `phidata-2.4.0/phi/llm/message.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,7 +73,12 @@
             _logger(self.content)
         if self.tool_calls:
             _logger(f"Tool Calls: {json.dumps(self.tool_calls, indent=2)}")
         if self.function_call:
             _logger(f"Function Call: {json.dumps(self.function_call, indent=2)}")
         # if self.model_extra and "images" in self.model_extra:
         #     _logger("images: {}".format(self.model_extra["images"]))
+
+    def content_is_valid(self) -> bool:
+        """Check if the message content is valid."""
+
+        return self.content is not None and len(self.content) > 0
```

### Comparing `phidata-2.3.90/phi/llm/mistral/mistral.py` & `phidata-2.4.0/phi/llm/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/llm/ollama/chat.py` & `phidata-2.4.0/phi/llm/ollama/chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -219,18 +219,22 @@
             m.log()
 
         assistant_message_content = ""
         response_is_tool_call = False
         tool_call_bracket_count = 0
         is_last_tool_call_bracket = False
         completion_tokens = 0
+        time_to_first_token = None
         response_timer = Timer()
         response_timer.start()
         for response in self.invoke_stream(messages=messages):
             completion_tokens += 1
+            if completion_tokens == 1:
+                time_to_first_token = response_timer.elapsed
+                logger.debug(f"Time to first token: {time_to_first_token:.4f}s")
 
             # -*- Parse response
             # logger.info(f"Ollama partial response: {response}")
             # logger.info(f"Ollama partial response type: {type(response)}")
             response_message: Optional[dict] = response.get("message")
             response_content = response_message.get("content") if response_message else None
             # logger.info(f"Ollama partial response content: {response_content}")
@@ -264,14 +268,17 @@
                 if is_last_tool_call_bracket and response_content.strip().endswith("}"):
                     is_last_tool_call_bracket = False
                     continue
 
                 yield response_content
 
         response_timer.stop()
+        logger.debug(f"Tokens generated: {completion_tokens}")
+        logger.debug(f"Time per output token: {response_timer.elapsed / completion_tokens:.4f}s")
+        logger.debug(f"Throughput: {completion_tokens / response_timer.elapsed:.4f} tokens/s")
         logger.debug(f"Time to generate response: {response_timer.elapsed:.4f}s")
 
         # -*- Create assistant message
         assistant_message = Message(
             role="assistant",
             content=assistant_message_content,
         )
@@ -302,18 +309,26 @@
                             assistant_message.tool_calls = tool_calls
         except Exception:
             logger.warning(f"Could not parse tool calls from response: {assistant_message_content}")
             pass
 
         # -*- Update usage metrics
         # Add response time to metrics
-        assistant_message.metrics["time"] = response_timer.elapsed
+        assistant_message.metrics["time"] = f"{response_timer.elapsed:.4f}"
+        assistant_message.metrics["time_to_first_token"] = f"{time_to_first_token:.4f}s"
+        assistant_message.metrics["time_per_output_token"] = f"{response_timer.elapsed / completion_tokens:.4f}s"
         if "response_times" not in self.metrics:
             self.metrics["response_times"] = []
         self.metrics["response_times"].append(response_timer.elapsed)
+        if "time_to_first_token" not in self.metrics:
+            self.metrics["time_to_first_token"] = []
+        self.metrics["time_to_first_token"].append(f"{time_to_first_token:.4f}s")
+        if "tokens_per_second" not in self.metrics:
+            self.metrics["tokens_per_second"] = []
+        self.metrics["tokens_per_second"].append(f"{completion_tokens / response_timer.elapsed:.4f}")
 
         # -*- Add assistant message to messages
         messages.append(assistant_message)
         assistant_message.log()
 
         # -*- Parse and run function call
         if assistant_message.tool_calls is not None and self.run_tools:
```

### Comparing `phidata-2.3.90/phi/llm/ollama/hermes.py` & `phidata-2.4.0/phi/llm/ollama/hermes.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/llm/ollama/tools.py` & `phidata-2.4.0/phi/llm/ollama/tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/llm/openai/chat.py` & `phidata-2.4.0/phi/llm/openai/chat.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from phi.tools.function import FunctionCall
 from phi.utils.log import logger
 from phi.utils.timer import Timer
 from phi.utils.functions import get_function_call
 from phi.utils.tools import get_function_call_for_tool_call
 
 try:
-    from openai import OpenAI as OpenAIClient
+    from openai import OpenAI as OpenAIClient, AsyncOpenAI as AsyncOpenAIClient
     from openai.types.completion_usage import CompletionUsage
     from openai.types.chat.chat_completion import ChatCompletion
     from openai.types.chat.chat_completion_chunk import (
         ChatCompletionChunk,
         ChoiceDelta,
         ChoiceDeltaFunctionCall,
         ChoiceDeltaToolCall,
@@ -52,20 +52,26 @@
     api_key: Optional[str] = None
     organization: Optional[str] = None
     base_url: Optional[Union[str, httpx.URL]] = None
     timeout: Optional[float] = None
     max_retries: Optional[int] = None
     default_headers: Optional[Any] = None
     default_query: Optional[Any] = None
+    http_client: Optional[httpx.Client] = None
     client_params: Optional[Dict[str, Any]] = None
     # -*- Provide the OpenAI client manually
+    client: Optional[OpenAIClient] = None
+    async_client: Optional[AsyncOpenAIClient] = None
+    # Deprecated: will be removed in v3
     openai_client: Optional[OpenAIClient] = None
 
-    @property
-    def client(self) -> OpenAIClient:
+    def get_client(self) -> OpenAIClient:
+        if self.client:
+            return self.client
+
         if self.openai_client:
             return self.openai_client
 
         _client_params: Dict[str, Any] = {}
         if self.api_key:
             _client_params["api_key"] = self.api_key
         if self.organization:
@@ -76,18 +82,49 @@
             _client_params["timeout"] = self.timeout
         if self.max_retries:
             _client_params["max_retries"] = self.max_retries
         if self.default_headers:
             _client_params["default_headers"] = self.default_headers
         if self.default_query:
             _client_params["default_query"] = self.default_query
+        if self.http_client:
+            _client_params["http_client"] = self.http_client
         if self.client_params:
             _client_params.update(self.client_params)
         return OpenAIClient(**_client_params)
 
+    def get_async_client(self) -> AsyncOpenAIClient:
+        if self.async_client:
+            return self.async_client
+
+        _client_params: Dict[str, Any] = {}
+        if self.api_key:
+            _client_params["api_key"] = self.api_key
+        if self.organization:
+            _client_params["organization"] = self.organization
+        if self.base_url:
+            _client_params["base_url"] = self.base_url
+        if self.timeout:
+            _client_params["timeout"] = self.timeout
+        if self.max_retries:
+            _client_params["max_retries"] = self.max_retries
+        if self.default_headers:
+            _client_params["default_headers"] = self.default_headers
+        if self.default_query:
+            _client_params["default_query"] = self.default_query
+        if self.http_client:
+            _client_params["http_client"] = self.http_client
+        else:
+            _client_params["http_client"] = httpx.AsyncClient(
+                limits=httpx.Limits(max_connections=1000, max_keepalive_connections=100)
+            )
+        if self.client_params:
+            _client_params.update(self.client_params)
+        return AsyncOpenAIClient(**_client_params)
+
     @property
     def api_kwargs(self) -> Dict[str, Any]:
         _request_params: Dict[str, Any] = {}
         if self.frequency_penalty:
             _request_params["frequency_penalty"] = self.frequency_penalty
         if self.logit_bias:
             _request_params["logit_bias"] = self.logit_bias
@@ -160,28 +197,45 @@
             if self.tool_choice is None:
                 _dict["tool_choice"] = "auto"
             else:
                 _dict["tool_choice"] = self.tool_choice
         return _dict
 
     def invoke(self, messages: List[Message]) -> ChatCompletion:
-        return self.client.chat.completions.create(
+        return self.get_client().chat.completions.create(
+            model=self.model,
+            messages=[m.to_dict() for m in messages],  # type: ignore
+            **self.api_kwargs,
+        )
+
+    async def ainvoke(self, messages: List[Message]) -> Any:
+        return await self.get_async_client().chat.completions.create(
             model=self.model,
             messages=[m.to_dict() for m in messages],  # type: ignore
             **self.api_kwargs,
         )
 
     def invoke_stream(self, messages: List[Message]) -> Iterator[ChatCompletionChunk]:
-        yield from self.client.chat.completions.create(
+        yield from self.get_client().chat.completions.create(
             model=self.model,
             messages=[m.to_dict() for m in messages],  # type: ignore
             stream=True,
             **self.api_kwargs,
         )  # type: ignore
 
+    async def ainvoke_stream(self, messages: List[Message]) -> Any:
+        async_stream = await self.get_async_client().chat.completions.create(
+            model=self.model,
+            messages=[m.to_dict() for m in messages],  # type: ignore
+            stream=True,
+            **self.api_kwargs,
+        )
+        async for chunk in async_stream:  # type: ignore
+            yield chunk
+
     def run_function(self, function_call: Dict[str, Any]) -> Tuple[Message, Optional[FunctionCall]]:
         _function_name = function_call.get("name")
         _function_arguments_str = function_call.get("arguments")
         if _function_name is not None:
             # Get function call
             _function_call = get_function_call(
                 name=_function_name,
@@ -345,14 +399,139 @@
                 return final_response
         logger.debug("---------- OpenAI Response End ----------")
         # -*- Return content if no function calls are present
         if assistant_message.content is not None:
             return assistant_message.get_content_string()
         return "Something went wrong, please try again."
 
+    async def aresponse(self, messages: List[Message]) -> str:
+        logger.debug("---------- OpenAI Async Response Start ----------")
+        # -*- Log messages for debugging
+        for m in messages:
+            m.log()
+
+        response_timer = Timer()
+        response_timer.start()
+        response: ChatCompletion = await self.ainvoke(messages=messages)
+        response_timer.stop()
+        logger.debug(f"Time to generate response: {response_timer.elapsed:.4f}s")
+        # logger.debug(f"OpenAI response type: {type(response)}")
+        # logger.debug(f"OpenAI response: {response}")
+
+        # -*- Parse response
+        response_message: ChatCompletionMessage = response.choices[0].message
+        response_role = response_message.role
+        response_content: Optional[str] = response_message.content
+        response_function_call: Optional[ChatCompletionFunctionCall] = response_message.function_call
+        response_tool_calls: Optional[List[ChatCompletionMessageToolCall]] = response_message.tool_calls
+
+        # -*- Create assistant message
+        assistant_message = Message(
+            role=response_role or "assistant",
+            content=response_content,
+        )
+        if response_function_call is not None:
+            assistant_message.function_call = response_function_call.model_dump()
+        if response_tool_calls is not None:
+            assistant_message.tool_calls = [t.model_dump() for t in response_tool_calls]
+
+        # -*- Update usage metrics
+        # Add response time to metrics
+        assistant_message.metrics["time"] = response_timer.elapsed
+        if "response_times" not in self.metrics:
+            self.metrics["response_times"] = []
+        self.metrics["response_times"].append(response_timer.elapsed)
+
+        # Add token usage to metrics
+        response_usage: Optional[CompletionUsage] = response.usage
+        prompt_tokens = response_usage.prompt_tokens if response_usage is not None else None
+        if prompt_tokens is not None:
+            assistant_message.metrics["prompt_tokens"] = prompt_tokens
+            if "prompt_tokens" not in self.metrics:
+                self.metrics["prompt_tokens"] = prompt_tokens
+            else:
+                self.metrics["prompt_tokens"] += prompt_tokens
+        completion_tokens = response_usage.completion_tokens if response_usage is not None else None
+        if completion_tokens is not None:
+            assistant_message.metrics["completion_tokens"] = completion_tokens
+            if "completion_tokens" not in self.metrics:
+                self.metrics["completion_tokens"] = completion_tokens
+            else:
+                self.metrics["completion_tokens"] += completion_tokens
+        total_tokens = response_usage.total_tokens if response_usage is not None else None
+        if total_tokens is not None:
+            assistant_message.metrics["total_tokens"] = total_tokens
+            if "total_tokens" not in self.metrics:
+                self.metrics["total_tokens"] = total_tokens
+            else:
+                self.metrics["total_tokens"] += total_tokens
+
+        # -*- Add assistant message to messages
+        messages.append(assistant_message)
+        assistant_message.log()
+
+        # -*- Parse and run function call
+        need_to_run_functions = assistant_message.function_call is not None or assistant_message.tool_calls is not None
+        if need_to_run_functions and self.run_tools:
+            if assistant_message.function_call is not None:
+                function_call_message, function_call = self.run_function(function_call=assistant_message.function_call)
+                messages.append(function_call_message)
+                # -*- Get new response using result of function call
+                final_response = ""
+                if self.show_tool_calls and function_call is not None:
+                    final_response += f"\n - Running: {function_call.get_call_str()}\n\n"
+                final_response += self.response(messages=messages)
+                return final_response
+            elif assistant_message.tool_calls is not None:
+                final_response = ""
+                function_calls_to_run: List[FunctionCall] = []
+                for tool_call in assistant_message.tool_calls:
+                    _tool_call_id = tool_call.get("id")
+                    _function_call = get_function_call_for_tool_call(tool_call, self.functions)
+                    if _function_call is None:
+                        messages.append(
+                            Message(
+                                role="tool",
+                                tool_call_id=_tool_call_id,
+                                content="Could not find function to call.",
+                            )
+                        )
+                        continue
+                    if _function_call.error is not None:
+                        messages.append(
+                            Message(
+                                role="tool",
+                                tool_call_id=_tool_call_id,
+                                content=_function_call.error,
+                            )
+                        )
+                        continue
+                    function_calls_to_run.append(_function_call)
+
+                if self.show_tool_calls:
+                    if len(function_calls_to_run) == 1:
+                        final_response += f"\n - Running: {function_calls_to_run[0].get_call_str()}\n\n"
+                    elif len(function_calls_to_run) > 1:
+                        final_response += "\nRunning:"
+                        for _f in function_calls_to_run:
+                            final_response += f"\n - {_f.get_call_str()}"
+                        final_response += "\n\n"
+
+                function_call_results = self.run_function_calls(function_calls_to_run)
+                if len(function_call_results) > 0:
+                    messages.extend(function_call_results)
+                # -*- Get new response using result of tool call
+                final_response += await self.aresponse(messages=messages)
+                return final_response
+        logger.debug("---------- OpenAI Async Response End ----------")
+        # -*- Return content if no function calls are present
+        if assistant_message.content is not None:
+            return assistant_message.get_content_string()
+        return "Something went wrong, please try again."
+
     def generate(self, messages: List[Message]) -> Dict:
         logger.debug("---------- OpenAI Response Start ----------")
         # -*- Log messages for debugging
         for m in messages:
             m.log()
 
         response_timer = Timer()
@@ -608,14 +787,213 @@
                     #     yield "\n"
                     #     yield f.get_content_string()
                     #     yield "\n"
                 # -*- Yield new response using results of tool calls
                 yield from self.response_stream(messages=messages)
         logger.debug("---------- OpenAI Response End ----------")
 
+    async def aresponse_stream(self, messages: List[Message]) -> Any:
+        logger.debug("---------- OpenAI Async Response Start ----------")
+        # -*- Log messages for debugging
+        for m in messages:
+            m.log()
+
+        assistant_message_content = ""
+        assistant_message_function_name = ""
+        assistant_message_function_arguments_str = ""
+        assistant_message_tool_calls: Optional[List[ChoiceDeltaToolCall]] = None
+        completion_tokens = 0
+        response_timer = Timer()
+        response_timer.start()
+        async_stream = self.ainvoke_stream(messages=messages)
+        async for response in async_stream:
+            # logger.debug(f"OpenAI response type: {type(response)}")
+            # logger.debug(f"OpenAI response: {response}")
+            response_content: Optional[str] = None
+            response_function_call: Optional[ChoiceDeltaFunctionCall] = None
+            response_tool_calls: Optional[List[ChoiceDeltaToolCall]] = None
+            if len(response.choices) > 0:
+                # -*- Parse response
+                response_delta: ChoiceDelta = response.choices[0].delta
+                response_content = response_delta.content
+                response_function_call = response_delta.function_call
+                response_tool_calls = response_delta.tool_calls
+
+            # -*- Return content if present, otherwise get function call
+            if response_content is not None:
+                assistant_message_content += response_content
+                completion_tokens += 1
+                yield response_content
+
+            # -*- Parse function call
+            if response_function_call is not None:
+                _function_name_stream = response_function_call.name
+                if _function_name_stream is not None:
+                    assistant_message_function_name += _function_name_stream
+                _function_args_stream = response_function_call.arguments
+                if _function_args_stream is not None:
+                    assistant_message_function_arguments_str += _function_args_stream
+
+            # -*- Parse tool calls
+            if response_tool_calls is not None:
+                if assistant_message_tool_calls is None:
+                    assistant_message_tool_calls = []
+                assistant_message_tool_calls.extend(response_tool_calls)
+
+        response_timer.stop()
+        logger.debug(f"Time to generate response: {response_timer.elapsed:.4f}s")
+
+        # -*- Create assistant message
+        assistant_message = Message(role="assistant")
+        # -*- Add content to assistant message
+        if assistant_message_content != "":
+            assistant_message.content = assistant_message_content
+        # -*- Add function call to assistant message
+        if assistant_message_function_name != "":
+            assistant_message.function_call = {
+                "name": assistant_message_function_name,
+                "arguments": assistant_message_function_arguments_str,
+            }
+        # -*- Add tool calls to assistant message
+        if assistant_message_tool_calls is not None:
+            # Build tool calls
+            tool_calls: List[Dict[str, Any]] = []
+            for _tool_call in assistant_message_tool_calls:
+                _index = _tool_call.index
+                _tool_call_id = _tool_call.id
+                _tool_call_type = _tool_call.type
+                _tool_call_function_name = _tool_call.function.name if _tool_call.function is not None else None
+                _tool_call_function_arguments_str = (
+                    _tool_call.function.arguments if _tool_call.function is not None else None
+                )
+
+                tool_call_at_index = tool_calls[_index] if len(tool_calls) > _index else None
+                if tool_call_at_index is None:
+                    tool_call_at_index_function_dict = {}
+                    if _tool_call_function_name is not None:
+                        tool_call_at_index_function_dict["name"] = _tool_call_function_name
+                    if _tool_call_function_arguments_str is not None:
+                        tool_call_at_index_function_dict["arguments"] = _tool_call_function_arguments_str
+                    tool_call_at_index_dict = {
+                        "id": _tool_call.id,
+                        "type": _tool_call_type,
+                        "function": tool_call_at_index_function_dict,
+                    }
+                    tool_calls.insert(_index, tool_call_at_index_dict)
+                else:
+                    if _tool_call_function_name is not None:
+                        if "name" not in tool_call_at_index["function"]:
+                            tool_call_at_index["function"]["name"] = _tool_call_function_name
+                        else:
+                            tool_call_at_index["function"]["name"] += _tool_call_function_name
+                    if _tool_call_function_arguments_str is not None:
+                        if "arguments" not in tool_call_at_index["function"]:
+                            tool_call_at_index["function"]["arguments"] = _tool_call_function_arguments_str
+                        else:
+                            tool_call_at_index["function"]["arguments"] += _tool_call_function_arguments_str
+                    if _tool_call_id is not None:
+                        tool_call_at_index["id"] = _tool_call_id
+                    if _tool_call_type is not None:
+                        tool_call_at_index["type"] = _tool_call_type
+            assistant_message.tool_calls = tool_calls
+
+        # -*- Update usage metrics
+        # Add response time to metrics
+        assistant_message.metrics["time"] = response_timer.elapsed
+        if "response_times" not in self.metrics:
+            self.metrics["response_times"] = []
+        self.metrics["response_times"].append(response_timer.elapsed)
+
+        # Add token usage to metrics
+        # TODO: compute prompt tokens
+        prompt_tokens = 0
+        assistant_message.metrics["prompt_tokens"] = prompt_tokens
+        if "prompt_tokens" not in self.metrics:
+            self.metrics["prompt_tokens"] = prompt_tokens
+        else:
+            self.metrics["prompt_tokens"] += prompt_tokens
+        logger.debug(f"Estimated completion tokens: {completion_tokens}")
+        assistant_message.metrics["completion_tokens"] = completion_tokens
+        if "completion_tokens" not in self.metrics:
+            self.metrics["completion_tokens"] = completion_tokens
+        else:
+            self.metrics["completion_tokens"] += completion_tokens
+        total_tokens = prompt_tokens + completion_tokens
+        assistant_message.metrics["total_tokens"] = total_tokens
+        if "total_tokens" not in self.metrics:
+            self.metrics["total_tokens"] = total_tokens
+        else:
+            self.metrics["total_tokens"] += total_tokens
+
+        # -*- Add assistant message to messages
+        messages.append(assistant_message)
+        assistant_message.log()
+
+        # -*- Parse and run function call
+        need_to_run_functions = assistant_message.function_call is not None or assistant_message.tool_calls is not None
+        if need_to_run_functions and self.run_tools:
+            if assistant_message.function_call is not None:
+                function_call_message, function_call = self.run_function(function_call=assistant_message.function_call)
+                messages.append(function_call_message)
+                if self.show_tool_calls and function_call is not None:
+                    yield f"\n - Running: {function_call.get_call_str()}\n\n"
+                # -*- Yield new response using result of function call
+                fc_stream = self.aresponse_stream(messages=messages)
+                async for fc in fc_stream:
+                    yield fc
+                # yield from self.response_stream(messages=messages)
+            elif assistant_message.tool_calls is not None:
+                function_calls_to_run: List[FunctionCall] = []
+                for tool_call in assistant_message.tool_calls:
+                    _tool_call_id = tool_call.get("id")
+                    _function_call = get_function_call_for_tool_call(tool_call, self.functions)
+                    if _function_call is None:
+                        messages.append(
+                            Message(
+                                role="tool",
+                                tool_call_id=_tool_call_id,
+                                content="Could not find function to call.",
+                            )
+                        )
+                        continue
+                    if _function_call.error is not None:
+                        messages.append(
+                            Message(
+                                role="tool",
+                                tool_call_id=_tool_call_id,
+                                content=_function_call.error,
+                            )
+                        )
+                        continue
+                    function_calls_to_run.append(_function_call)
+
+                if self.show_tool_calls:
+                    if len(function_calls_to_run) == 1:
+                        yield f"\n - Running: {function_calls_to_run[0].get_call_str()}\n\n"
+                    elif len(function_calls_to_run) > 1:
+                        yield "\nRunning:"
+                        for _f in function_calls_to_run:
+                            yield f"\n - {_f.get_call_str()}"
+                        yield "\n\n"
+
+                function_call_results = self.run_function_calls(function_calls_to_run)
+                if len(function_call_results) > 0:
+                    messages.extend(function_call_results)
+                    # Code to show function call results
+                    # for f in function_call_results:
+                    #     yield "\n"
+                    #     yield f.get_content_string()
+                    #     yield "\n"
+                # -*- Yield new response using results of tool calls
+                fc_stream = self.aresponse_stream(messages=messages)
+                async for fc in fc_stream:
+                    yield fc
+                # yield from self.response_stream(messages=messages)
+        logger.debug("---------- OpenAI Async Response End ----------")
+
     def generate_stream(self, messages: List[Message]) -> Iterator[Dict]:
         logger.debug("---------- OpenAI Response Start ----------")
         # -*- Log messages for debugging
         for m in messages:
             m.log()
 
         assistant_message_content = ""
```

### Comparing `phidata-2.3.90/phi/llm/together/together.py` & `phidata-2.4.0/phi/llm/together/together.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/memory/assistant.py` & `phidata-2.4.0/phi/memory/assistant.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,16 @@
 from pydantic import BaseModel
 
 from phi.llm.message import Message
 from phi.llm.references import References
 
 
 class AssistantMemory(BaseModel):
-    """
-    This class provides memory for an Assistant.
-    """
-
-    # Messages between the user and the LLM.
-    # Note: the actual prompts are stored in the llm_messages
+    # Messages between the user and the Assistant.
+    # Note: the llm prompts are stored in the llm_messages
     chat_history: List[Message] = []
     # Prompts sent to the LLM and the LLM responses.
     llm_messages: List[Message] = []
     # References from the vector database.
     references: List[References] = []
 
     def to_dict(self) -> Dict[str, Any]:
```

### Comparing `phidata-2.3.90/phi/prompt/registry.py` & `phidata-2.4.0/phi/prompt/registry.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/prompt/template.py` & `phidata-2.4.0/phi/prompt/template.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/resource/base.py` & `phidata-2.4.0/phi/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/resource/group.py` & `phidata-2.4.0/phi/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/storage/assistant/base.py` & `phidata-2.4.0/phi/storage/assistant/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/storage/assistant/postgres.py` & `phidata-2.4.0/phi/storage/assistant/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/storage/assistant/singlestore.py` & `phidata-2.4.0/phi/storage/assistant/singlestore.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/storage/assistant/sqllite.py` & `phidata-2.4.0/phi/storage/assistant/sqllite.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/airflow.py` & `phidata-2.4.0/phi/tools/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/apify.py` & `phidata-2.4.0/phi/tools/apify.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/arxiv_toolkit.py` & `phidata-2.4.0/phi/tools/arxiv_toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/csv_tools.py` & `phidata-2.4.0/phi/tools/csv_tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/duckdb.py` & `phidata-2.4.0/phi/tools/duckdb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/duckduckgo.py` & `phidata-2.4.0/phi/tools/duckduckgo.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/email.py` & `phidata-2.4.0/phi/tools/email.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/exa.py` & `phidata-2.4.0/phi/tools/exa.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/file.py` & `phidata-2.4.0/phi/tools/file.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/function.py` & `phidata-2.4.0/phi/tools/function.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/google.py` & `phidata-2.4.0/phi/tools/google.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/newspaper4k.py` & `phidata-2.4.0/phi/tools/newspaper4k.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 
 
 class Newspaper4k(Toolkit):
     def __init__(
         self,
         read_article: bool = True,
         include_summary: bool = False,
+        article_length: Optional[int] = None,
     ):
         super().__init__(name="newspaper_tools")
 
         self.include_summary: bool = include_summary
+        self.article_length: Optional[int] = article_length
         if read_article:
             self.register(self.read_article)
 
     def get_article_data(self, url: str) -> Optional[Dict[str, Any]]:
         """Read and get article data from a URL.
 
         Args:
@@ -66,10 +68,13 @@
         """
 
         try:
             article_data = self.get_article_data(url)
             if not article_data:
                 return f"Error reading article from {url}: No data found."
 
+            if self.article_length and "text" in article_data:
+                article_data["text"] = article_data["text"][: self.article_length]
+
             return json.dumps(article_data, indent=2)
         except Exception as e:
             return f"Error reading article from {url}: {e}"
```

### Comparing `phidata-2.3.90/phi/tools/newspaper_toolkit.py` & `phidata-2.4.0/phi/tools/newspaper_toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/openbb_tools.py` & `phidata-2.4.0/phi/tools/openbb_tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/pandas.py` & `phidata-2.4.0/phi/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/phi.py` & `phidata-2.4.0/phi/tools/phi.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/pubmed.py` & `phidata-2.4.0/phi/tools/pubmed.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/python.py` & `phidata-2.4.0/phi/tools/python.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/resend_toolkit.py` & `phidata-2.4.0/phi/tools/resend_toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/serpapi_toolkit.py` & `phidata-2.4.0/phi/tools/serpapi_toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/shell.py` & `phidata-2.4.0/phi/tools/shell.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/sql.py` & `phidata-2.4.0/phi/tools/sql.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/streamlit/components.py` & `phidata-2.4.0/phi/tools/streamlit/components.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/tavily.py` & `phidata-2.4.0/phi/tools/tavily.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/toolkit.py` & `phidata-2.4.0/phi/tools/toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/website.py` & `phidata-2.4.0/phi/tools/website.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/wikipedia.py` & `phidata-2.4.0/phi/tools/wikipedia.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/yfinance.py` & `phidata-2.4.0/phi/tools/yfinance.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/youtube_toolkit.py` & `phidata-2.4.0/phi/tools/youtube_toolkit.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/tools/zendesk.py` & `phidata-2.4.0/phi/tools/zendesk.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/common.py` & `phidata-2.4.0/phi/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/defaults.py` & `phidata-2.4.0/phi/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/enum.py` & `phidata-2.4.0/phi/utils/enum.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/filesystem.py` & `phidata-2.4.0/phi/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/functions.py` & `phidata-2.4.0/phi/utils/functions.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/git.py` & `phidata-2.4.0/phi/utils/git.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/json_io.py` & `phidata-2.4.0/phi/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/json_schema.py` & `phidata-2.4.0/phi/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/load_env.py` & `phidata-2.4.0/phi/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/log.py` & `phidata-2.4.0/phi/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/merge_dict.py` & `phidata-2.4.0/phi/utils/merge_dict.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/message.py` & `phidata-2.4.0/phi/utils/message.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/pickle.py` & `phidata-2.4.0/phi/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/py_io.py` & `phidata-2.4.0/phi/utils/py_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/pyproject.py` & `phidata-2.4.0/phi/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/resource_filter.py` & `phidata-2.4.0/phi/utils/resource_filter.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/shell.py` & `phidata-2.4.0/phi/utils/shell.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/timer.py` & `phidata-2.4.0/phi/utils/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/tools.py` & `phidata-2.4.0/phi/utils/tools.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/utils/yaml_io.py` & `phidata-2.4.0/phi/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/vectordb/base.py` & `phidata-2.4.0/phi/vectordb/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/vectordb/lancedb/lancedb.py` & `phidata-2.4.0/phi/vectordb/lancedb/lancedb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/vectordb/pgvector/pgvector.py` & `phidata-2.4.0/phi/vectordb/pgvector/pgvector.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/vectordb/pgvector/pgvector2.py` & `phidata-2.4.0/phi/vectordb/pgvector/pgvector2.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/vectordb/pineconedb/pineconedb.py` & `phidata-2.4.0/phi/vectordb/pineconedb/pineconedb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/vectordb/qdrant/qdrant.py` & `phidata-2.4.0/phi/vectordb/qdrant/qdrant.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/vectordb/singlestore/index.py` & `phidata-2.4.0/phi/vectordb/singlestore/index.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/vectordb/singlestore/s2vectordb.py` & `phidata-2.4.0/phi/vectordb/singlestore/s2vectordb.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/workspace/config.py` & `phidata-2.4.0/phi/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/workspace/helpers.py` & `phidata-2.4.0/phi/workspace/helpers.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/workspace/operator.py` & `phidata-2.4.0/phi/workspace/operator.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phi/workspace/settings.py` & `phidata-2.4.0/phi/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-2.3.90/phidata.egg-info/PKG-INFO` & `phidata-2.4.0/phidata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.3.90
-Summary: Add memory, knowledge and tools to LLMs.
+Version: 2.4.0
+Summary: Memory, knowledge and tools for LLMs.
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gitpython
 Requires-Dist: httpx
 Requires-Dist: pydantic
 Requires-Dist: pydantic-settings
 Requires-Dist: python-dotenv
```

### Comparing `phidata-2.3.90/phidata.egg-info/SOURCES.txt` & `phidata-2.4.0/phidata.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,17 @@
 README.md
 pyproject.toml
 setup.py
 phi/__init__.py
 phi/base.py
 phi/constants.py
 phi/py.typed
-phi/ai/__init__.py
-phi/ai/operator.py
-phi/ai/phi_ai.py
 phi/api/__init__.py
-phi/api/ai.py
 phi/api/api.py
 phi/api/assistant.py
-phi/api/llm.py
-phi/api/monitor.py
 phi/api/prompt.py
 phi/api/routes.py
 phi/api/user.py
 phi/api/workspace.py
 phi/api/schemas/__init__.py
 phi/api/schemas/ai.py
 phi/api/schemas/assistant.py
@@ -30,15 +24,14 @@
 phi/app/__init__.py
 phi/app/base.py
 phi/app/context.py
 phi/app/db_app.py
 phi/app/group.py
 phi/assistant/__init__.py
 phi/assistant/assistant.py
-phi/assistant/custom.py
 phi/assistant/duckdb.py
 phi/assistant/python.py
 phi/assistant/run.py
 phi/assistant/openai/__init__.py
 phi/assistant/openai/assistant.py
 phi/assistant/openai/exceptions.py
 phi/assistant/openai/message.py
@@ -46,16 +39,14 @@
 phi/assistant/openai/run.py
 phi/assistant/openai/thread.py
 phi/assistant/openai/tool.py
 phi/assistant/openai/file/__init__.py
 phi/assistant/openai/file/file.py
 phi/assistant/openai/file/local.py
 phi/assistant/openai/file/url.py
-phi/assistant/team/__init__.py
-phi/assistant/team/team.py
 phi/aws/__init__.py
 phi/aws/api_client.py
 phi/aws/resources.py
 phi/aws/app/__init__.py
 phi/aws/app/base.py
 phi/aws/app/context.py
 phi/aws/app/django/__init__.py
@@ -388,16 +379,14 @@
 phi/llm/openai/like.py
 phi/llm/openrouter/__init__.py
 phi/llm/openrouter/openrouter.py
 phi/llm/together/__init__.py
 phi/llm/together/together.py
 phi/memory/__init__.py
 phi/memory/assistant.py
-phi/memory/task/__init__.py
-phi/memory/task/llm.py
 phi/prompt/__init__.py
 phi/prompt/exceptions.py
 phi/prompt/registry.py
 phi/prompt/template.py
 phi/resource/__init__.py
 phi/resource/base.py
 phi/resource/group.py
@@ -407,20 +396,15 @@
 phi/storage/assistant/postgres.py
 phi/storage/assistant/singlestore.py
 phi/storage/assistant/sqllite.py
 phi/table/__init__.py
 phi/table/sql/__init__.py
 phi/table/sql/base.py
 phi/task/__init__.py
-phi/task/decorator.py
 phi/task/task.py
-phi/task/llm/__init__.py
-phi/task/llm/llm_task.py
-phi/task/py/__init__.py
-phi/task/py/python_task.py
 phi/tools/__init__.py
 phi/tools/airflow.py
 phi/tools/apify.py
 phi/tools/arxiv_toolkit.py
 phi/tools/csv_tools.py
 phi/tools/duckdb.py
 phi/tools/duckduckgo.py
@@ -490,14 +474,16 @@
 phi/vectordb/pineconedb/__init__.py
 phi/vectordb/pineconedb/pineconedb.py
 phi/vectordb/qdrant/__init__.py
 phi/vectordb/qdrant/qdrant.py
 phi/vectordb/singlestore/__init__.py
 phi/vectordb/singlestore/index.py
 phi/vectordb/singlestore/s2vectordb.py
+phi/workflow/__init__.py
+phi/workflow/workflow.py
 phi/workspace/__init__.py
 phi/workspace/config.py
 phi/workspace/enums.py
 phi/workspace/helpers.py
 phi/workspace/operator.py
 phi/workspace/settings.py
 phidata.egg-info/PKG-INFO
```

### Comparing `phidata-2.3.90/pyproject.toml` & `phidata-2.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "phidata"
-version = "2.3.90"
-description = "Add memory, knowledge and tools to LLMs."
-requires-python = ">=3.8"
+version = "2.4.0"
+description = "Memory, knowledge and tools for LLMs."
+requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
   "gitpython",
```

