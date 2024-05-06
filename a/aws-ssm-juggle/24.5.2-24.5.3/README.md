# Comparing `tmp/aws_ssm_juggle-24.5.2.tar.gz` & `tmp/aws_ssm_juggle-24.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_ssm_juggle-24.5.2.tar", max compression
+gzip compressed data, was "aws_ssm_juggle-24.5.3.tar", max compression
```

## Comparing `aws_ssm_juggle-24.5.2.tar` & `aws_ssm_juggle-24.5.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1065 2024-04-26 13:12:27.770715 aws_ssm_juggle-24.5.2/LICENSE
--rw-r--r--   0        0        0     2003 2024-04-26 13:24:15.999968 aws_ssm_juggle-24.5.2/README.md
--rw-r--r--   0        0        0     2307 2024-05-03 12:36:18.759626 aws_ssm_juggle-24.5.2/aws_ssm_juggle/__init__.py
--rw-r--r--   0        0        0     6936 2024-05-03 12:37:57.704544 aws_ssm_juggle-24.5.2/aws_ssm_juggle/ec2.py
--rw-r--r--   0        0        0    10970 2024-05-03 12:38:14.119563 aws_ssm_juggle-24.5.2/aws_ssm_juggle/ecs.py
--rw-r--r--   0        0        0      744 2024-05-03 12:38:49.585761 aws_ssm_juggle-24.5.2/pyproject.toml
--rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.5.2/setup.py
--rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-06 19:39:07.643146 aws_ssm_juggle-24.5.3/LICENSE
+-rw-r--r--   0        0        0     2003 2024-05-06 19:39:07.643146 aws_ssm_juggle-24.5.3/README.md
+-rw-r--r--   0        0        0     2301 2024-05-06 19:39:07.643146 aws_ssm_juggle-24.5.3/aws_ssm_juggle/__init__.py
+-rw-r--r--   0        0        0     7349 2024-05-06 19:39:07.644146 aws_ssm_juggle-24.5.3/aws_ssm_juggle/ec2.py
+-rw-r--r--   0        0        0    10748 2024-05-06 19:39:07.644146 aws_ssm_juggle-24.5.3/aws_ssm_juggle/ecs.py
+-rw-r--r--   0        0        0      744 2024-05-06 19:39:07.644146 aws_ssm_juggle-24.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3150 1970-01-01 00:00:00.000000 aws_ssm_juggle-24.5.3/PKG-INFO
```

### Comparing `aws_ssm_juggle-24.5.2/LICENSE` & `aws_ssm_juggle-24.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.5.2/README.md` & `aws_ssm_juggle-24.5.3/README.md`

 * *Files identical despite different names*

### Comparing `aws_ssm_juggle-24.5.2/aws_ssm_juggle/__init__.py` & `aws_ssm_juggle-24.5.3/aws_ssm_juggle/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,15 @@
     if index is None:
         exit(0)
     if items[index] == "Back":
         return None, index
     return source[index], index
 
 
-def port_forward(
-    boto3_session: session.Session, remote_port: int, local_port: int, target: str
-) -> None:
+def port_forward(boto3_session: session.Session, remote_port: int, local_port: int, target: str) -> None:
     """
     forward port
     """
     parameters = {
         "portNumber": [str(remote_port)],
         "localPortNumber": [str(local_port)],
     }
```

### Comparing `aws_ssm_juggle-24.5.2/aws_ssm_juggle/ec2.py` & `aws_ssm_juggle-24.5.3/aws_ssm_juggle/ec2.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,14 +125,18 @@
         help="AWS region name",
         default="eu-central-1",
     )
     parser.add_argument(
         "--instance-id",
         help="EC2 instance id",
     )
+    parser.add_argument(
+        "--instance-name",
+        help="Show only EC2 instances where name matches (e.g. 'web' matches 'my-app-web-server')",
+    )
     subparsers = parser.add_subparsers(
         dest="action",
         help="action",
     )
     subparsers.required = True
     subparsers.add_parser("start", help="Start interactive ssm session")
     ssh = subparsers.add_parser("ssh", help="Start ssh session")
@@ -165,33 +169,39 @@
     paginator = ec2.get_paginator(paginator)
     iterator = paginator.paginate(**kwargs)
     for page in iterator:
         res.extend(page.get(leaf))
     return res
 
 
-def get_instance_id(boto3_session: session.Session, instance_id: str):
+def get_instance_id(boto3_session: session.Session, instance_id: str, instance_name: str = ""):
     """
     get instance_id
     """
     if instance_id:
         return instance_id, None
     print("fetching available instances...")
+    filters = [
+        {
+            "Name": "instance-state-name",
+            "Values": ["running"],
+        },
+    ]
+    if instance_name:
+        filters.append(
+            {
+                "Name": "tag:Name",
+                "Values": [f"*{instance_name}*"]
+            }
+        )
     reservations = ec2_paginator(
         boto3_session=boto3_session,
         paginator="describe_instances",
         leaf="Reservations",
-        Filters=[
-            {
-                "Name": "instance-state-name",
-                "Values": [
-                    "running",
-                ],
-            },
-        ],
+        Filters=filters,
     )
     instances = []
     for reservation in reservations:
         for instance in reservation.get("Instances"):
             tags = {tag["Key"]: tag["Value"] for tag in instance.get("Tags", [])}
             instances.append(f'{instance.get("InstanceId")} - {tags.get("Name")}')
     return show_menu(
@@ -206,25 +216,28 @@
     parser = get_parser()
     arguments = parser.parse_args()
     boto3_session_args = {
         "region_name": arguments.region,
         "profile_name": arguments.profile,
     }
     boto3_session = session.Session(**boto3_session_args)
+    instance_name = arguments.instance_name
     instance_id = arguments.instance_id
     ssh_args, remote_port, local_port = None, None, None
     if "ssh_args" in arguments:
         ssh_args = arguments.ssh_args
     if "remote_port" in arguments:
         remote_port = arguments.remote_port
     if "local_port" in arguments:
         local_port = arguments.local_port
     while not instance_id:
         instance_id, _ = get_instance_id(
-            boto3_session=boto3_session, instance_id=instance_id
+            boto3_session=boto3_session,
+            instance_id=instance_id,
+            instance_name=instance_name,
         )
         instance_id = instance_id.split(" - ")[0]
     ec2_session = EC2Session(
         boto3_session=boto3_session,
         instance_id=instance_id,
         local_port=local_port,
         remote_port=remote_port,
```

### Comparing `aws_ssm_juggle-24.5.2/aws_ssm_juggle/ecs.py` & `aws_ssm_juggle-24.5.3/aws_ssm_juggle/ecs.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,26 +41,18 @@
         self.container_index = container_index
         self.ecs = self.boto3_session.client("ecs")
         self.local_port = local_port
         self.remote_port = remote_port
         self.ssm = self.boto3_session.client("ssm")
         self.task = task
         self.task_details = task_details
-        self.runtime_id = (
-            task_details.get("tasks")[0]
-            .get("containers")[container_index]
-            .get("runtimeId")
-        )
+        self.runtime_id = task_details.get("tasks")[0].get("containers")[container_index].get("runtimeId")
         if not self.runtime_id:
-            raise RuntimeError(
-                "unable to get runtimeId from container, looks like it's not running."
-            )
-        self.target = (
-            f"ecs:{self.cluster}_{self.runtime_id.split('-')[0]}_{self.runtime_id}"
-        )
+            raise RuntimeError("unable to get runtimeId from container, looks like it's not running.")
+        self.target = f"ecs:{self.cluster}_{self.runtime_id.split('-')[0]}_{self.runtime_id}"
 
     def port_forward(self):
         port_forward(
             boto3_session=self.boto3_session,
             remote_port=self.remote_port,
             local_port=self.local_port,
             target=self.target,
@@ -246,17 +238,15 @@
         clear_screen=True,
     )
     if ret[0] is None:
         return (cluster, None, *ret)
     return (cluster, service, *ret)
 
 
-def get_container(
-    cluster: str, service: str, task: str, containers: list, container: str
-):
+def get_container(cluster: str, service: str, task: str, containers: list, container: str):
     """
     get container
     """
     if container:
         return task, container, containers.index(container)
     ret = show_menu(
         items=containers,
@@ -288,17 +278,15 @@
         clear_screen=True,
     )
     if ret[0] is None:
         return (None, *ret)
     return (container, *ret)
 
 
-def menu_loop_condition(
-    cluster: str, service: str, task: str, container: str, remote_port: int, action: str
-):
+def menu_loop_condition(cluster: str, service: str, task: str, container: str, remote_port: int, action: str):
     menu_loop_condition = cluster and service and task and container
     if action == "forward":
         menu_loop_condition = menu_loop_condition and remote_port
     return menu_loop_condition
 
 
 def run():
@@ -332,41 +320,34 @@
         task=task,
         container=container,
         remote_port=remote_port,
         action=arguments.action,
     ):
         cluster, _ = get_cluster(ecs=ecs, cluster=cluster)
         cluster, service, _ = get_service(ecs=ecs, cluster=cluster, service=service)
-        cluster, service, task, _ = get_task(
-            ecs=ecs, cluster=cluster, service=service, task=task
-        )
+        cluster, service, task, _ = get_task(ecs=ecs, cluster=cluster, service=service, task=task)
         if cluster and task:
             task_details = ecs.describe_tasks(cluster=cluster, tasks=[task])
-            containers = [
-                container.get("name")
-                for container in task_details.get("tasks")[0].get("containers")
-            ]
+            containers = [container.get("name") for container in task_details.get("tasks")[0].get("containers")]
             ret = get_container(
                 cluster=cluster,
                 service=service,
                 task=task,
                 containers=containers,
                 container=container,
             )
             task, container, container_index = ret
         if (arguments.action == "forward" and container) and not remote_port:
             task_definition_arn = task_details.get("tasks")[0].get("taskDefinitionArn")
-            task_definition = task_definition or ecs.describe_task_definition(
-                taskDefinition=task_definition_arn
-            ).get("taskDefinition")
+            task_definition = task_definition or ecs.describe_task_definition(taskDefinition=task_definition_arn).get(
+                "taskDefinition"
+            )
             ports = [
                 str(container.get("containerPort"))
-                for container in task_definition.get("containerDefinitions")[
-                    container_index
-                ].get("portMappings")
+                for container in task_definition.get("containerDefinitions")[container_index].get("portMappings")
             ]
             container, remote_port, _ = get_port(
                 cluster=cluster,
                 service=service,
                 task=task,
                 container=container,
                 containers=containers,
```

### Comparing `aws_ssm_juggle-24.5.2/pyproject.toml` & `aws_ssm_juggle-24.5.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-ssm-juggle"
-version = "24.5.2"
+version = "24.5.3"
 description = "AWS SSM tool for ECS/EC2 (Shell, Port Forwarding, ...)"
 authors = ["Stefan Heitmüller <stefan.heitmueller@gmx.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/morph027/aws-ssm-juggle"
 
 [tool.poetry.dependencies]
```

### Comparing `aws_ssm_juggle-24.5.2/PKG-INFO` & `aws_ssm_juggle-24.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-juggle
-Version: 24.5.2
+Version: 24.5.3
 Summary: AWS SSM tool for ECS/EC2 (Shell, Port Forwarding, ...)
 Home-page: https://github.com/morph027/aws-ssm-juggle
 License: MIT
 Author: Stefan Heitmüller
 Author-email: stefan.heitmueller@gmx.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3
 Requires-Dist: configargparse
 Requires-Dist: diskcache
 Requires-Dist: shtab
 Requires-Dist: simple_term_menu
 Project-URL: Repository, https://github.com/morph027/aws-ssm-juggle
 Description-Content-Type: text/markdown
```

