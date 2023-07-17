# Comparing `tmp/dbt_copilot_tools-0.1.5.tar.gz` & `tmp/dbt_copilot_tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_copilot_tools-0.1.5.tar", max compression
+gzip compressed data, was "dbt_copilot_tools-0.1.6.tar", max compression
```

## Comparing `dbt_copilot_tools-0.1.5.tar` & `dbt_copilot_tools-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.5/LICENSE
--rw-r--r--   0        0        0    13596 2023-06-27 16:14:10.422589 dbt_copilot_tools-0.1.5/commands/COMMANDS.md
--rw-r--r--   0        0        0     1737 2023-06-27 16:14:10.422751 dbt_copilot_tools-0.1.5/commands/README.md
--rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.5/commands/__init__.py
--rwxr-xr-x   0        0        0    10214 2023-06-27 16:01:04.635244 dbt_copilot_tools-0.1.5/commands/bootstrap_cli.py
--rwxr-xr-x   0        0        0     2560 2023-06-20 14:07:55.205282 dbt_copilot_tools-0.1.5/commands/check_cloudformation.py
--rwxr-xr-x   0        0        0    13488 2023-06-20 09:47:08.337250 dbt_copilot_tools-0.1.5/commands/codebuild_cli.py
--rwxr-xr-x   0        0        0     8582 2023-06-15 16:41:34.056908 dbt_copilot_tools-0.1.5/commands/copilot_cli.py
--rwxr-xr-x   0        0        0    20842 2023-06-27 16:01:14.828248 dbt_copilot_tools-0.1.5/commands/dns_cli.py
--rw-r--r--   0        0        0     5994 2023-06-27 16:14:10.423077 dbt_copilot_tools-0.1.5/commands/utils.py
--rw-r--r--   0        0        0     5695 2023-06-27 16:01:14.828564 dbt_copilot_tools-0.1.5/commands/waf_cli.py
--rwxr-xr-x   0        0        0      970 2023-06-27 16:14:10.423415 dbt_copilot_tools-0.1.5/copilot_helper.py
--rw-r--r--   0        0        0     1188 2023-06-27 16:14:10.423762 dbt_copilot_tools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2750 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.6/LICENSE
+-rw-r--r--   0        0        0    12476 2023-07-17 16:56:50.134294 dbt_copilot_tools-0.1.6/commands/COMMANDS.md
+-rw-r--r--   0        0        0     1737 2023-06-27 16:14:10.422751 dbt_copilot_tools-0.1.6/commands/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.6/commands/__init__.py
+-rwxr-xr-x   0        0        0     9834 2023-06-30 15:36:41.153299 dbt_copilot_tools-0.1.6/commands/bootstrap_cli.py
+-rwxr-xr-x   0        0        0     2563 2023-07-14 15:07:33.244634 dbt_copilot_tools-0.1.6/commands/check_cloudformation.py
+-rwxr-xr-x   0        0        0    13573 2023-06-30 14:36:32.763424 dbt_copilot_tools-0.1.6/commands/codebuild_cli.py
+-rwxr-xr-x   0        0        0     6991 2023-06-28 16:19:20.994539 dbt_copilot_tools-0.1.6/commands/copilot_cli.py
+-rwxr-xr-x   0        0        0    20986 2023-07-14 15:07:33.244923 dbt_copilot_tools-0.1.6/commands/dns_cli.py
+-rw-r--r--   0        0        0     5927 2023-06-28 11:36:58.070298 dbt_copilot_tools-0.1.6/commands/utils.py
+-rw-r--r--   0        0        0     6007 2023-07-14 15:07:33.245135 dbt_copilot_tools-0.1.6/commands/waf_cli.py
+-rwxr-xr-x   0        0        0      970 2023-06-28 12:16:25.470546 dbt_copilot_tools-0.1.6/copilot_helper.py
+-rw-r--r--   0        0        0     1095 2023-07-17 16:57:12.377505 dbt_copilot_tools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2793 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.6/PKG-INFO
```

### Comparing `dbt_copilot_tools-0.1.5/LICENSE` & `dbt_copilot_tools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.5/commands/COMMANDS.md` & `dbt_copilot_tools-0.1.6/commands/COMMANDS.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 - [copilot-helper bootstrap make-config](#copilot-helper-bootstrap-make-config)
 - [copilot-helper bootstrap migrate-secrets](#copilot-helper-bootstrap-migrate-secrets)
 - [copilot-helper bootstrap instructions](#copilot-helper-bootstrap-instructions)
 - [copilot-helper check-cloudformation](#copilot-helper-check-cloudformation)
 - [copilot-helper check-cloudformation lint](#copilot-helper-check-cloudformation-lint)
 - [copilot-helper copilot](#copilot-helper-copilot)
 - [copilot-helper copilot make-storage](#copilot-helper-copilot-make-storage)
-- [copilot-helper copilot apply-waf](#copilot-helper-copilot-apply-waf)
 - [copilot-helper copilot get-env-secrets](#copilot-helper-copilot-get-env-secrets)
 - [copilot-helper codebuild](#copilot-helper-codebuild)
 - [copilot-helper codebuild link-github](#copilot-helper-codebuild-link-github)
 - [copilot-helper codebuild create-codedeploy-role](#copilot-helper-codebuild-create-codedeploy-role)
 - [copilot-helper codebuild codedeploy](#copilot-helper-codebuild-codedeploy)
 - [copilot-helper codebuild buildproject](#copilot-helper-codebuild-buildproject)
 - [copilot-helper codebuild delete-project](#copilot-helper-codebuild-delete-project)
@@ -52,16 +51,15 @@
 # copilot-helper bootstrap
 
 [↩ Parent](#copilot-helper)
 
 ## Usage
 
 ```
-Usage: copilot-helper bootstrap 
-           [OPTIONS] COMMAND [ARGS]...
+Usage: copilot-helper bootstrap [OPTIONS] COMMAND [ARGS]...
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
@@ -71,31 +69,22 @@
 - [`make-config` ↪](#copilot-helper-bootstrap-make-config)
 - [`migrate-secrets` ↪](#copilot-helper-bootstrap-migrate-secrets)
 
 # copilot-helper bootstrap make-config
 
 [↩ Parent](#copilot-helper-bootstrap)
 
-    Generate copilot boilerplate code.
-
-    CONFIG-FILE is the path to the input yaml config file OUTPUT is the location
-    of the repo root dir. Defaults to the current directory.
+    Generate Copilot boilerplate code.
 
 ## Usage
 
 ```
-Usage: copilot-helper bootstrap make-config 
-           [OPTIONS] CONFIG_FILE [OUTPUT]
+Usage: copilot-helper bootstrap make-config [OPTIONS]
 ```
 
-## Arguments
-
-- `config-file <path>`
-- `output <path>`
-
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
 # copilot-helper bootstrap migrate-secrets
 
@@ -108,22 +97,17 @@
     If you're using AWS profiles, use the AWS_PROFILE env var to indicate the which profile to use, e.g.:
 
     AWS_PROFILE=myaccount copilot-bootstrap.py ...
 
 ## Usage
 
 ```
-Usage: copilot-helper bootstrap migrate-secrets 
-           [OPTIONS] CONFIG_FILE
+Usage: copilot-helper bootstrap migrate-secrets [OPTIONS]
 ```
 
-## Arguments
-
-- `config-file <path>`
-
 ## Options
 
 - `--project-profile <text>`
   - aws account profile name
 - `--env <text>`
   - Migrate secrets from a specific environment
 - `--svc <text>`
@@ -140,22 +124,17 @@
 [↩ Parent](#copilot-helper-bootstrap)
 
     Show migration instructions.
 
 ## Usage
 
 ```
-Usage: copilot-helper bootstrap instructions 
-           [OPTIONS] CONFIG_FILE
+Usage: copilot-helper bootstrap instructions [OPTIONS]
 ```
 
-## Arguments
-
-- `config-file <path>`
-
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
 # copilot-helper check-cloudformation
 
@@ -164,17 +143,16 @@
     Runs the checks passed in the command arguments.
 
     If no argument is passed, it will run all the checks.
 
 ## Usage
 
 ```
-Usage: copilot-helper check-cloudformation 
-           [OPTIONS] COMMAND1 [ARGS]... [COMMAND2
-           [ARGS]...]...
+Usage: copilot-helper check-cloudformation [OPTIONS] COMMAND1 [ARGS]...
+                                           [COMMAND2 [ARGS]...]...
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
@@ -187,78 +165,52 @@
 [↩ Parent](#copilot-helper-check-cloudformation)
 
     Runs cfn-lint against the generated CloudFormation templates.
 
 ## Usage
 
 ```
-Usage: copilot-helper check-cloudformation lint 
-           [OPTIONS]
+Usage: copilot-helper check-cloudformation lint [OPTIONS]
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
 # copilot-helper copilot
 
 [↩ Parent](#copilot-helper)
 
 ## Usage
 
 ```
-Usage: copilot-helper copilot [OPTIONS] COMMAND
-                              [ARGS]...
+Usage: copilot-helper copilot [OPTIONS] COMMAND [ARGS]...
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
 ## Commands
 
-- [`apply-waf` ↪](#copilot-helper-copilot-apply-waf)
 - [`get-env-secrets` ↪](#copilot-helper-copilot-get-env-secrets)
 - [`make-storage` ↪](#copilot-helper-copilot-make-storage)
 
 # copilot-helper copilot make-storage
 
 [↩ Parent](#copilot-helper-copilot)
 
-    Generate storage cloudformation for each environment.
-
-## Usage
-
-```
-Usage: copilot-helper copilot make-storage 
-           [OPTIONS] STORAGE_CONFIG_FILE
-```
-
-## Arguments
-
-- `storage-config-file <path>`
-
-## Options
-
-- `--help <boolean>` _Defaults to False._
-  - Show this message and exit.
-
-# copilot-helper copilot apply-waf
-
-[↩ Parent](#copilot-helper-copilot)
-
-    Apply the WAF environment addon.
+    Generate storage CloudFormation for each environment.
 
 ## Usage
 
 ```
-Usage: copilot-helper copilot apply-waf 
-           [OPTIONS]
+Usage: copilot-helper copilot make-storage [OPTIONS]
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
@@ -267,16 +219,15 @@
 [↩ Parent](#copilot-helper-copilot)
 
     List secret names and values for an environment.
 
 ## Usage
 
 ```
-Usage: copilot-helper copilot get-env-secrets 
-           [OPTIONS] APP ENV
+Usage: copilot-helper copilot get-env-secrets [OPTIONS] APP ENV
 ```
 
 ## Arguments
 
 - `app <text>`
 - `env <text>`
 
@@ -288,16 +239,15 @@
 # copilot-helper codebuild
 
 [↩ Parent](#copilot-helper)
 
 ## Usage
 
 ```
-Usage: copilot-helper codebuild 
-           [OPTIONS] COMMAND [ARGS]...
+Usage: copilot-helper codebuild [OPTIONS] COMMAND [ARGS]...
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
@@ -315,16 +265,15 @@
 [↩ Parent](#copilot-helper-codebuild)
 
     Links CodeDeploy to Github via users PAT.
 
 ## Usage
 
 ```
-Usage: copilot-helper codebuild link-github 
-           [OPTIONS]
+Usage: copilot-helper codebuild link-github [OPTIONS]
 ```
 
 ## Options
 
 - `--pat <text>`
   - PAT Token
 - `--project-profile <text>`
@@ -337,16 +286,15 @@
 [↩ Parent](#copilot-helper-codebuild)
 
     Add AWS Role needed for codedeploy.
 
 ## Usage
 
 ```
-Usage: copilot-helper codebuild create-codedeploy-role 
-           [OPTIONS]
+Usage: copilot-helper codebuild create-codedeploy-role [OPTIONS]
 ```
 
 ## Options
 
 - `--project-profile <text>`
   - aws account profile name
 - `--type <choice>` _Defaults to ci._
@@ -359,16 +307,15 @@
 [↩ Parent](#copilot-helper-codebuild)
 
     Builds Code build boilerplate.
 
 ## Usage
 
 ```
-Usage: copilot-helper codebuild codedeploy 
-           [OPTIONS]
+Usage: copilot-helper codebuild codedeploy [OPTIONS]
 ```
 
 ## Options
 
 - `--update <boolean>` _Defaults to False._
   - Update config
 - `--name <text>`
@@ -395,16 +342,15 @@
 [↩ Parent](#copilot-helper-codebuild)
 
     Builds Code build for ad hoc projects.
 
 ## Usage
 
 ```
-Usage: copilot-helper codebuild buildproject 
-           [OPTIONS]
+Usage: copilot-helper codebuild buildproject [OPTIONS]
 ```
 
 ## Options
 
 - `--update <boolean>` _Defaults to False._
   - Update config
 - `--name <text>`
@@ -429,16 +375,15 @@
 [↩ Parent](#copilot-helper-codebuild)
 
     Delete CodeBuild projects.
 
 ## Usage
 
 ```
-Usage: copilot-helper codebuild delete-project 
-           [OPTIONS]
+Usage: copilot-helper codebuild delete-project [OPTIONS]
 ```
 
 ## Options
 
 - `--name <text>`
   - Name of project
 - `--project-profile <text>`
@@ -451,16 +396,15 @@
 [↩ Parent](#copilot-helper-codebuild)
 
     Add Slack credentials into AWS Parameter Store.
 
 ## Usage
 
 ```
-Usage: copilot-helper codebuild slackcreds 
-           [OPTIONS]
+Usage: copilot-helper codebuild slackcreds [OPTIONS]
 ```
 
 ## Options
 
 - `--workspace <text>`
   - Slack Workspace id
 - `--channel <text>`
@@ -475,16 +419,15 @@
 # copilot-helper domain
 
 [↩ Parent](#copilot-helper)
 
 ## Usage
 
 ```
-Usage: copilot-helper domain [OPTIONS] COMMAND
-                             [ARGS]...
+Usage: copilot-helper domain [OPTIONS] COMMAND [ARGS]...
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
@@ -498,22 +441,19 @@
 [↩ Parent](#copilot-helper-domain)
 
     Scans to see if Domain exists.
 
 ## Usage
 
 ```
-Usage: copilot-helper domain check-domain 
-           [OPTIONS]
+Usage: copilot-helper domain check-domain [OPTIONS]
 ```
 
 ## Options
 
-- `--path <text>`
-  - path of copilot folder
 - `--domain-profile <text>`
   - aws account profile name for R53 domains account
 - `--project-profile <text>`
   - aws account profile name for certificates account
 - `--base-domain <text>`
   - root domain
 - `--help <boolean>` _Defaults to False._
@@ -524,16 +464,15 @@
 [↩ Parent](#copilot-helper-domain)
 
     Check R53 domain is pointing to the correct ECS Load Blanacer.
 
 ## Usage
 
 ```
-Usage: copilot-helper domain assign-domain 
-           [OPTIONS]
+Usage: copilot-helper domain assign-domain [OPTIONS]
 ```
 
 ## Options
 
 - `--app <text>`
   - Application Name
 - `--domain-profile <text>`
@@ -550,16 +489,15 @@
 # copilot-helper waf
 
 [↩ Parent](#copilot-helper)
 
 ## Usage
 
 ```
-Usage: copilot-helper waf [OPTIONS] COMMAND
-                          [ARGS]...
+Usage: copilot-helper waf [OPTIONS] COMMAND [ARGS]...
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
@@ -568,21 +506,20 @@
 - [`attach-waf` ↪](#copilot-helper-waf-attach-waf)
 - [`custom-waf` ↪](#copilot-helper-waf-custom-waf)
 
 # copilot-helper waf attach-waf
 
 [↩ Parent](#copilot-helper-waf)
 
-    Attach default WAF rule to ECS Load Blanacer.
+    Attach default WAF rule to ECS Load Balancer.
 
 ## Usage
 
 ```
-Usage: copilot-helper waf attach-waf 
-           [OPTIONS]
+Usage: copilot-helper waf attach-waf [OPTIONS]
 ```
 
 ## Options
 
 - `--app <text>`
   - Application Name
 - `--project-profile <text>`
@@ -594,21 +531,20 @@
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
 # copilot-helper waf custom-waf
 
 [↩ Parent](#copilot-helper-waf)
 
-    Attach custom WAF to ECS Load Blanacer.
+    Attach custom WAF to ECS Load Balancer.
 
 ## Usage
 
 ```
-Usage: copilot-helper waf custom-waf 
-           [OPTIONS]
+Usage: copilot-helper waf custom-waf [OPTIONS]
 ```
 
 ## Options
 
 - `--app <text>`
   - Application Name
 - `--project-profile <text>`
```

### Comparing `dbt_copilot_tools-0.1.5/commands/README.md` & `dbt_copilot_tools-0.1.6/commands/README.md`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.5/commands/bootstrap_cli.py` & `dbt_copilot_tools-0.1.6/commands/bootstrap_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -106,26 +106,19 @@
 
 @click.group()
 def bootstrap():
     pass
 
 
 @bootstrap.command()
-@click.argument("config-file", type=click.Path(exists=True))
-@click.argument("output", type=click.Path(exists=True), default=".")
-def make_config(config_file, output):
-    """
-    Generate copilot boilerplate code.
-
-    CONFIG-FILE is the path to the input yaml config file OUTPUT is the location
-    of the repo root dir. Defaults to the current directory.
-    """
+def make_config():
+    """Generate Copilot boilerplate code."""
 
-    base_path = Path(output)
-    config = load_and_validate_config(config_file)
+    base_path = Path(".")
+    config = load_and_validate_config("bootstrap.yml")
 
     templates = setup_templates()
 
     click.echo(">>> Generating Copilot configuration files\n")
 
     # create copilot directory
     mkdir(base_path, "copilot")
@@ -148,15 +141,15 @@
     # create each service directory and manifest.yml
     for service in config["services"]:
         service["ipfilter"] = any(env.get("ipfilter", False) for _, env in service["environments"].items())
         name = service["name"]
         mkdir(base_path, f"copilot/{name}/addons/")
 
         if "secrets_from" in service:
-            # Copy secrets from the app referredd to in the "secrets_from" key
+            # Copy secrets from the app referred to in the "secrets_from" key
             related_service = [s for s in config["services"] if s["name"] == service["secrets_from"]][0]
 
             service["secrets"].update(related_service["secrets"])
 
         contents = templates["svc"][service["type"] + "-manifest"].render(service)
 
         click.echo(mkfile(base_path, f"copilot/{name}/manifest.yml", contents))
@@ -171,35 +164,35 @@
     click.echo(
         "\nGitHub documentation: "
         "https://github.com/uktrade/platform-documentation/blob/main/gov-pass-to-copiltot-migration",
     )
 
 
 @bootstrap.command()
-@click.argument("config-file", type=click.Path(exists=True))
 @click.option("--project-profile", required=True, help="aws account profile name")
 @click.option("--env", help="Migrate secrets from a specific environment")
 @click.option("--svc", help="Migrate secrets from a specific service")
 @click.option("--overwrite", is_flag=True, show_default=True, default=False, help="Overwrite existing secrets?")
 @click.option("--dry-run", is_flag=True, show_default=True, default=False, help="dry run")
-def migrate_secrets(config_file, project_profile, env, svc, overwrite, dry_run):
+def migrate_secrets(project_profile, env, svc, overwrite, dry_run):
     """
     Migrate secrets from your gov paas application to AWS/copilot.
 
     You need to be authenticated via cf cli and the AWS cli to use this commmand.
 
     If you're using AWS profiles, use the AWS_PROFILE env var to indicate the which profile to use, e.g.:
 
     AWS_PROFILE=myaccount copilot-bootstrap.py ...
     """
 
     check_aws_conn(project_profile)
     # TODO: optional SSM or secret manager
 
     cf_client = CloudFoundryClient.build_from_cf_config()
+    config_file = "bootstrap.yml"
     config = load_and_validate_config(config_file)
 
     if env and env not in config["environments"].keys():
         raise click.ClickException(f"{env} is not an environment in {config_file}")
 
     if svc and svc not in [service["name"] for service in config["services"]]:
         raise click.ClickException(f"{svc} is not a service in {config_file}")
@@ -263,19 +256,19 @@
                     text = "Created" if not param_exists else "Overwritten" if overwrite else "NOT overwritten"
                     click.echo(f"{text} {ssm_path}")
                 else:
                     click.echo(f"{ssm_path} not created because `--dry-run` flag was included.")
 
 
 @bootstrap.command()
-@click.argument("config-file", type=click.Path(exists=True))
-def instructions(config_file):
+def instructions():
     """Show migration instructions."""
     templates = setup_templates()
 
+    config_file = "bootstrap.yml"
     config = load_and_validate_config(config_file)
     config["config_file"] = config_file
 
     instructions = templates["instructions"].render(config)
 
     click.echo(instructions)
```

### Comparing `dbt_copilot_tools-0.1.5/commands/check_cloudformation.py` & `dbt_copilot_tools-0.1.6/commands/check_cloudformation.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,27 +27,31 @@
 
     if ctx.invoked_subcommand is None:
         click.secho(f"\n>>> Running all checks", fg="yellow")
         for name, command in ctx.command.commands.items():
             ctx.invoke(command)
 
 
+def get_lint_result(path: str):
+    command = ["cfn-lint", path]
+
+    click.secho(f"\n>>> Running lint check", fg="yellow")
+    click.secho(f"""    {" ".join(command)}\n""", fg="yellow")
+
+    return run(command, capture_output=True)
+
+
 @check_cloudformation.command()
 @click.pass_context
 def lint(ctx: click.Context) -> None:
     """Runs cfn-lint against the generated CloudFormation templates."""
 
     BASE_DIR = Path(__file__).parent.parent
 
-    command = ["cfn-lint", f"{BASE_DIR}/tests/test-application/copilot/**/addons/*.yml"]
-
-    click.secho(f"\n>>> Running lint check", fg="yellow")
-    click.secho(f"""    {" ".join(command)}\n""", fg="yellow")
-
-    result = run(command, capture_output=True)
+    result = get_lint_result(f"{BASE_DIR}/tests/test-application/copilot/**/addons/*.yml")
 
     click.secho(result.stdout.decode())
     if result.returncode == 0:
         ctx.obj["passing_checks"].append("lint")
     else:
         click.secho(result.stderr.decode())
         ctx.obj["failing_checks"].append("lint")
@@ -70,9 +74,9 @@
 
 def prepare_cloudformation_templates(ctx: click.Context) -> None:
     click.secho(f"\n>>> Preparing CloudFormation templates\n", fg="yellow")
     os.chdir(f"{BASE_DIR}/tests/test-application")
     copilot_directory = Path("./copilot")
     if copilot_directory.exists():
         rmtree(copilot_directory)
-    ctx.invoke(make_config, config_file="bootstrap.yml")
-    ctx.invoke(make_storage, storage_config_file="storage.yml")
+    ctx.invoke(make_config)
+    ctx.invoke(make_storage)
```

### Comparing `dbt_copilot_tools-0.1.5/commands/codebuild_cli.py` & `dbt_copilot_tools-0.1.6/commands/codebuild_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 import json
 import os
 
 import click
 from boto3.session import Session
 from mypy_boto3_codebuild.client import CodeBuildClient
+
 from .utils import check_aws_conn
 from .utils import check_response
 
 AWS_REGION = "eu-west-2"
 DEFAULT_CI_BUILDER = "public.ecr.aws/uktrade/ci-image-builder"
 
 
@@ -24,16 +25,17 @@
 
 
 def check_github_conn(client: CodeBuildClient):
     response = client.list_source_credentials()
 
     # If there are no source code creds defined then AWS is not linked to Github
     if not response["sourceCredentialsInfos"]:
-        if not click.confirm(click.style(
-                "GitHub is not linked in this AWS account\nDo you want to link with a PAT?", fg="yellow")):
+        if not click.confirm(
+            click.style("GitHub is not linked in this AWS account\nDo you want to link with a PAT?", fg="yellow")
+        ):
             exit()
 
         pat = input(
             """
             Create a bots PAT with the following scope:
                 repo:   status: Grants read/write access to public and private repository commit statuses.
                 admin:  repo_hook: Grants full control of repository hooks.
@@ -50,18 +52,19 @@
 
     try:
         response = client.get_role(RoleName=role_name)
         role_arn = response["Role"]["Arn"]
 
     except client.exceptions.NoSuchEntityException:
         click.echo(
-            click.style("Service Role", fg="yellow") +
-            click.style(f" {role_name} ", fg="white", bold=True) +
-            click.style("does not exist; run: ", fg="yellow") +
-            click.style("copilot-helper.py codebuild create-codedeploy-role --type <ci/custom>", fg="cyan"))
+            click.style("Service Role", fg="yellow")
+            + click.style(f" {role_name} ", fg="white", bold=True)
+            + click.style("does not exist; run: ", fg="yellow")
+            + click.style("copilot-helper.py codebuild create-codedeploy-role --type <ci/custom>", fg="cyan")
+        )
         role_arn = ""
         exit()
 
     return role_arn
 
 
 def update_parameter(project_session: Session, name: str, description: str, value: str):
@@ -85,23 +88,26 @@
 
     if git_part[0] == "https":
         git_url = git
     elif git_part[0] == "git@github.com":
         git_url = "https://github.com/" + git_part[1]
     else:
         click.echo(
-            click.style("Unable to recognise Git URL format, make sure it is either:\n", fg="red") +
-            click.style("https://github.com/<org>/<repository-name>\n" +
-            "git@github.com:<org>/<repository-name>", fg="white", bold=True))
+            click.style("Unable to recognise Git URL format, make sure it is either:\n", fg="red")
+            + click.style(
+                "https://github.com/<org>/<repository-name>\n" + "git@github.com:<org>/<repository-name>",
+                fg="white",
+                bold=True,
+            )
+        )
         exit()
     return git_url
 
 
 def modify_project(project_session, update, name, desc, git, branch, buildspec, builderimage, release, role_type):
-
     git_url = check_git_url(git)
     role_arn = check_service_role("ci-CodeBuild-role", project_session)
     client = project_session.client("codebuild", region_name=AWS_REGION)
     check_github_conn(client)
 
     environment = {
         "type": "LINUX_CONTAINER",
@@ -192,17 +198,19 @@
 
         except client.exceptions.ResourceAlreadyExistsException:
             click.secho("Project already exists, use the --update flag", fg="red")
             exit()
 
     check_response(response)
     check_response(response_webhook)
-    click.echo(click.style("Codebuild project ", fg="yellow") +
-                click.style(f"{name} ",fg="white", bold=True) +
-                click.style("updated", fg="yellow"))
+    click.echo(
+        click.style("Codebuild project ", fg="yellow")
+        + click.style(f"{name} ", fg="white", bold=True)
+        + click.style("updated", fg="yellow")
+    )
 
 
 @click.group()
 def codebuild():
     pass
 
 
@@ -254,16 +262,17 @@
                 SetAsDefault=True,
             )
             check_response(response)
             click.secho("Policy updated", fg="green")
 
         except client.exceptions.LimitExceededException:
             click.secho(
-                "You have hit the limit of max managed policies, "
-                "please delete an existing version and try again", fg="red")
+                "You have hit the limit of max managed policies, " "please delete an existing version and try again",
+                fg="red",
+            )
             exit()
 
     with open(f"{current_filepath}/../templates/create-codebuild-role.json") as f:
         role_doc = json.load(f)
 
     # Now create a role if not present and attach policy
     try:
@@ -319,16 +328,18 @@
 @click.option("--project-profile", required=True, help="aws account profile name")
 def delete_project(name, project_profile):
     """Delete CodeBuild projects."""
 
     project_session = check_aws_conn(project_profile)
     client = project_session.client("codebuild", region_name=AWS_REGION)
 
-    if not click.confirm(click.style("Are you sure you want to delete the project ", fg="yellow") +
-                         click.style(f"{name}", fg="white", bold=True)):
+    if not click.confirm(
+        click.style("Are you sure you want to delete the project ", fg="yellow")
+        + click.style(f"{name}", fg="white", bold=True)
+    ):
         exit()
 
     response = client.delete_project(name=name)
     check_response(response)
     click.secho("Project deleted", fg="green")
 
 
@@ -347,16 +358,17 @@
             "description": "Slack Workspace ID",
             "value": workspace,
         },
         "channel": {"name": "/codebuild/slack_channel_id", "description": "Slack Channel ID", "value": channel},
         "token": {"name": "/codebuild/slack_api_token", "description": "Slack API Token", "value": token},
     }
 
-    if not click.confirm(click.style(
-            "Updating Parameter Store with Slack credentials.\nDo you want to update it?", fg="yellow")):
+    if not click.confirm(
+        click.style("Updating Parameter Store with Slack credentials.\nDo you want to update it?", fg="yellow")
+    ):
         exit()
 
     for item, value in SLACK.items():
         update_parameter(project_session, value["name"], value["description"], value["value"])
     click.secho("Paramater Store updated", fg="green")
```

### Comparing `dbt_copilot_tools-0.1.5/commands/copilot_cli.py` & `dbt_copilot_tools-0.1.6/commands/copilot_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -120,28 +120,27 @@
 
         normalised_config[storage_name]["environments"] = normalised_environments
 
     return normalised_config
 
 
 @copilot.command()
-@click.argument("storage-config-file", type=click.Path(exists=True))
-def make_storage(storage_config_file):
-    """Generate storage cloudformation for each environment."""
+def make_storage():
+    """Generate storage CloudFormation for each environment."""
 
     overwrite = True
     output_dir = Path(".").absolute()
 
     ensure_cwd_is_repo_root()
 
     templates = setup_templates()
 
     config = _validate_and_normalise_config(BASE_DIR / "default-storage.yml")
 
-    project_config = _validate_and_normalise_config(storage_config_file)
+    project_config = _validate_and_normalise_config("storage.yml")
 
     config.update(project_config)
 
     click.echo("\n>>> Generating storage cloudformation\n")
 
     path = Path(f"copilot/environments/addons/")
     mkdir(output_dir, path)
@@ -188,61 +187,14 @@
                 mkdir(output_dir, service_path)
                 click.echo(mkfile(output_dir, service_path / f"{storage_name}.yml", contents, overwrite=overwrite))
 
     click.echo(templates["storage-instructions"].render(services=services))
 
 
 @copilot.command()
-def apply_waf():
-    """Apply the WAF environment addon."""
-
-    templates = setup_templates()
-    overwrite = True
-
-    ensure_cwd_is_repo_root()
-
-    env_names = list_copilot_local_environments()
-
-    if not env_names:
-        click.secho(f"Cannot add WAF CFN templates: No environments found in ./copilot/environments/", fg="red")
-        exit(1)
-
-    def _validate_arn(arn):
-        return arn and arn.startswith("arn:aws:wafv2:")
-
-    arns = {}
-
-    for name in env_names:
-        with open(f"./copilot/environments/{name}/manifest.yml", "r") as fd:
-            config = yaml.safe_load(fd)
-
-        arns[name] = config.get(WAF_ACL_ARN_KEY) if config else None
-
-    if not all(_validate_arn(arn) for arn in arns.values()):
-        click.secho(
-            f"Cannot add WAF CFN templates: Set a valid `{WAF_ACL_ARN_KEY}` in each ./copilot/environments/*/manifest.yml file",
-            fg="red",
-        )
-        exit(1)
-
-    # create the addons dir if it doesn't already exist
-    path = Path("./copilot/environments/addons")
-    mkdir(".", path)
-
-    # create the ./copilot/environments/addons/addons.parameters.yml file
-    contents = templates["env"]["parameters"].render({})
-    click.echo(mkfile(".", path / "addons.parameters.yml", contents, overwrite=overwrite))
-
-    # create the ./copilot/environments/addons/waf.yml file
-    contents = templates["env"]["waf"].render({"arns": arns})
-
-    click.echo(mkfile(".", path / "waf.yml", contents, overwrite=overwrite))
-
-
-@copilot.command()
 @click.argument("app", type=str)
 @click.argument("env", type=str)
 def get_env_secrets(app, env):
     """List secret names and values for an environment."""
 
     client = boto3.client("ssm")
```

### Comparing `dbt_copilot_tools-0.1.5/commands/dns_cli.py` & `dbt_copilot_tools-0.1.6/commands/dns_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python
 
 import os
 import time
+from typing import Tuple
 
 import click
 import yaml
+from boto3 import Session
 
 from .utils import check_aws_conn
 from .utils import check_response
 from .utils import ensure_cwd_is_repo_root
 
 # To do
 # -----
@@ -315,15 +317,15 @@
 
     # add records to hosted zone to validate certificate
     cert_arn = create_cert(acm_client, domain_client, domain, base_len)
 
     return cert_arn
 
 
-def lb_domain(project_session, app, svc, env):
+def lb_domain(project_session: Session, app: str, svc: str, env: str) -> Tuple[str, dict]:
     proj_client = project_session.client("ecs")
 
     response = proj_client.list_clusters()
     check_response(response)
     no_items = True
     for cluster_arn in response["clusterArns"]:
         cluster_name = cluster_arn.split("/")[1]
@@ -333,15 +335,15 @@
         if cluster_app == app and cluster_env == env:
             no_items = False
             break
 
     if no_items:
         click.echo(
             click.style("There are no clusters matching ", fg="red")
-            + click.style(f"{app}", fg="white", bold=True)
+            + click.style(f"{app} ", fg="white", bold=True)
             + click.style("in this aws account", fg="red"),
         )
         exit()
 
     response = proj_client.list_services(cluster=cluster_name)
     check_response(response)
     no_items = True
@@ -387,30 +389,33 @@
     with open(f"./copilot/{svc}/manifest.yml", "r") as fd:
         conf = yaml.safe_load(fd)
         if "environments" in conf:
             for domain in conf["environments"].items():
                 if domain[0] == env:
                     domain_name = domain[1]["http"]["alias"]
 
+        # What happens if domain_name isn't set? Should we raise an error? Return default ? Or None?
+
     return domain_name, response
 
 
 @click.group()
 def domain():
     pass
 
 
 @domain.command()
-@click.option("--path", help="path of copilot folder", required=True)
 @click.option("--domain-profile", help="aws account profile name for R53 domains account", required=True)
 @click.option("--project-profile", help="aws account profile name for certificates account", required=True)
 @click.option("--base-domain", help="root domain", required=True)
-def check_domain(path, domain_profile, project_profile, base_domain):
+def check_domain(domain_profile, project_profile, base_domain):
     """Scans to see if Domain exists."""
 
+    path = "copilot"
+
     domain_session = check_aws_conn(domain_profile)
     project_session = check_aws_conn(project_profile)
 
     if not os.path.exists(path):
         click.secho("Please check path, manifest file not found", fg="red")
         exit()
```

### Comparing `dbt_copilot_tools-0.1.5/commands/utils.py` & `dbt_copilot_tools-0.1.6/commands/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,14 @@
         "env": {
             "manifest": templateEnv.get_template("env/manifest.yml"),
             "opensearch": templateEnv.get_template("addons/env/opensearch.yml"),
             "rds-postgres": templateEnv.get_template("addons/env/rds-postgres.yml"),
             "aurora-postgres": templateEnv.get_template("addons/env/aurora-postgres.yml"),
             "redis": templateEnv.get_template("addons/env/redis-cluster.yml"),
             "s3": templateEnv.get_template("addons/env/s3.yml"),
-            "waf": templateEnv.get_template("addons/env/waf.yml"),
             "parameters": templateEnv.get_template("addons/env/addons.parameters.yml"),
         },
         "docs": templateEnv.get_template("COMMANDS.md.jinja"),
     }
 
     return templates
```

### Comparing `dbt_copilot_tools-0.1.5/commands/waf_cli.py` & `dbt_copilot_tools-0.1.6/commands/waf_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 #!/usr/bin/env python
 import time
 import uuid
 from pathlib import Path
 
+import boto3
+import botocore  # noqa
 import cfn_flip.yaml_dumper
 import click
 import yaml
 from cfn_tools import load_yaml
 
+from commands.check_cloudformation import get_lint_result
 from commands.dns_cli import lb_domain
 
 from .utils import check_aws_conn
 from .utils import check_response
 from .utils import ensure_cwd_is_repo_root
 
 # This may need to change, once we determine what the default WAF name will be.
 WAF_DEFAULT_NAME = "default"
 
 
-def check_waf(project_session):
+def check_waf(project_session: boto3.Session) -> str:
     click.secho("Checking WAF exists", fg="cyan")
     client = project_session.client("wafv2")
 
     response = client.list_web_acls(Scope="REGIONAL")
     arn = ""
     for waf in response["WebACLs"]:
         if waf["Name"] == WAF_DEFAULT_NAME:
@@ -37,15 +40,15 @@
 
 @waf.command()
 @click.option("--app", help="Application Name", required=True)
 @click.option("--project-profile", help="aws account profile name for application account", required=True)
 @click.option("--svc", help="Service Name", required=True)
 @click.option("--env", help="Environment", required=True)
 def attach_waf(app, project_profile, svc, env):
-    """Attach default WAF rule to ECS Load Blanacer."""
+    """Attach default WAF rule to ECS Load Balancer."""
 
     project_session = check_aws_conn(project_profile)
     waf_arn = check_waf(project_session)
     if not waf_arn:
         click.secho(
             "Default WAF rule does not exists in this AWS account, " "please have this created by the SRE team",
             fg="red",
@@ -64,53 +67,62 @@
         click.style("Default WAF is now associated with ", fg="green")
         + click.style(f"{elb_name} ", fg="white", bold=True)
         + click.style("for domain ", fg="green")
         + click.style(f"{domain_name}", fg="white", bold=True),
     )
 
 
+def create_stack(cf_client, app, svc, env, raw):
+    return cf_client.create_stack(
+        StackName=f"{app}-{svc}-{env}-CustomWAFStack",
+        TemplateBody=raw,
+        TimeoutInMinutes=5,
+        OnFailure="DELETE",
+        Tags=[
+            {"Key": "Name", "Value": "copilot tools custom waf"},
+        ],
+        ClientRequestToken=uuid.uuid4().hex,
+        EnableTerminationProtection=False,
+    )
+
+
 @waf.command()
 @click.option("--app", help="Application Name", required=True)
 @click.option("--project-profile", help="aws account profile name for application account", required=True)
 @click.option("--svc", help="Service Name", required=True)
 @click.option("--env", help="Environment", required=True)
 @click.option("--waf-path", help="path to waf.yml file", required=True)
 def custom_waf(app, project_profile, svc, env, waf_path):
-    """Attach custom WAF to ECS Load Blanacer."""
+    """Attach custom WAF to ECS Load Balancer."""
 
     project_session = check_aws_conn(project_profile)
     ensure_cwd_is_repo_root()
     path = Path().resolve() / waf_path
 
     try:
         with open(path, "r") as fd:
             data_dict = load_yaml(fd)
     except FileNotFoundError:
         click.secho(f"File not found...\n{path}", fg="red")
         exit()
+
     # The YAML data_dict needs verification, need to create a function to lint/check YAML formatting.
+    result = get_lint_result(str(path))
+    if result.returncode != 0:
+        click.secho(f"File failed lint check.\n{str(path)}", fg="red")
+        exit()
 
     # dumper is used to resolve the shorthand in YAML file, eg !GetAtt
     dumper = cfn_flip.yaml_dumper.get_dumper(clean_up=True, long_form=False)
     raw = yaml.dump(data_dict, Dumper=dumper, default_flow_style=False, allow_unicode=True)
 
     cf_client = project_session.client("cloudformation")
 
     try:
-        cs_response = cf_client.create_stack(
-            StackName=f"{app}-{svc}-{env}-CustomWAFStack",
-            TemplateBody=raw,
-            TimeoutInMinutes=5,
-            OnFailure="DELETE",
-            Tags=[
-                {"Key": "Name", "Value": "copilot tools custom waf"},
-            ],
-            ClientRequestToken=uuid.uuid4().hex,
-            EnableTerminationProtection=False,
-        )
+        cs_response = create_stack()
     except cf_client.exceptions.AlreadyExistsException:
         click.echo(
             click.style("CloudFormation Stack already exists, please delete the stack first.\n", fg="red")
             + click.style(f"{app}-{svc}-{env}-CustomWAFStack", fg="red"),
         )
         exit()
```

### Comparing `dbt_copilot_tools-0.1.5/copilot_helper.py` & `dbt_copilot_tools-0.1.6/copilot_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.5/PKG-INFO` & `dbt_copilot_tools-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-copilot-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Requires-Dist: boto3 (==1.26.31)
 Requires-Dist: boto3-stubs (==1.26.148)
 Requires-Dist: botocore (==1.29.31)
 Requires-Dist: cfn-flip (==1.3.0)
 Requires-Dist: click (==8.1.3)
 Requires-Dist: cloudfoundry-client (==1.35.0)
 Requires-Dist: jsonschema (==4.17.3)
+Requires-Dist: moto[all] (>=4.1.12,<5.0.0)
 Requires-Dist: mypy-boto3-codebuild (==1.26.0.post1)
 Requires-Dist: schema (==0.7.5)
 Description-Content-Type: text/markdown
 
 # DBT Copilot Tools
 
 This package contains a set of tools in the form of a Command Line Interface (CLI) primarily for transferring applications/services from [GOV.UK PaaS](https://www.cloud.service.gov.uk) to Department for Business and Trade (DBT) PaaS which augments [AWS Copilot](https://aws.github.io/copilot-cli/). These tools can also be used to provision AWS resources and/or make sure the CloudFormation templates conform to best practices.
```

