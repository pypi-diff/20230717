# Comparing `tmp/OBP_reliability_pillar-0.1.1.tar.gz` & `tmp/OBP_reliability_pillar-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_reliability_pillar-0.1.1.tar", last modified: Tue Jun  6 07:22:41 2023, max compression
+gzip compressed data, was "OBP_reliability_pillar-0.1.2.tar", last modified: Mon Jul 17 19:04:42 2023, max compression
```

## Comparing `OBP_reliability_pillar-0.1.1.tar` & `OBP_reliability_pillar-0.1.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:41.352767 OBP_reliability_pillar-0.1.1/
--rw-rw-rw-   0        0        0        0 2022-11-24 06:08:48.000000 OBP_reliability_pillar-0.1.1/LICENCE
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:40.809289 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/
--rw-rw-rw-   0        0        0     4908 2023-06-06 07:11:41.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:40.863288 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/auto_scaling/
--rw-rw-rw-   0        0        0      197 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/auto_scaling/__init__.py
--rw-rw-rw-   0        0        0     2101 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py
--rw-rw-rw-   0        0        0      607 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/auto_scaling/compliance.py
--rw-rw-rw-   0        0        0     2223 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:40.893284 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/cloudwatch/
--rw-rw-rw-   0        0        0      193 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/cloudwatch/__init__.py
--rw-rw-rw-   0        0        0     3134 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/cloudwatch/alarm_action_check.py
--rw-rw-rw-   0        0        0      485 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/cloudwatch/compliance.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:40.939304 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/dynamodb/
--rw-rw-rw-   0        0        0      187 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      667 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/dynamodb/compliance.py
--rw-rw-rw-   0        0        0     2222 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py
--rw-rw-rw-   0        0        0     2106 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py
--rw-rw-rw-   0        0        0      557 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/dynamodb/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:40.980287 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/ec2/
--rw-rw-rw-   0        0        0      177 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/ec2/__init__.py
--rw-rw-rw-   0        0        0      709 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/ec2/compliance.py
--rw-rw-rw-   0        0        0     2233 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py
--rw-rw-rw-   0        0        0     2257 2023-05-31 08:17:16.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/ec2/instance_in_vpc.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:41.010306 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_beanstalk/
--rw-rw-rw-   0        0        0      205 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_beanstalk/__init__.py
--rw-rw-rw-   0        0        0      508 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_beanstalk/compliance.py
--rw-rw-rw-   0        0        0     2339 2023-05-31 08:23:26.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:41.060657 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_load_balancer/
--rw-rw-rw-   0        0        0      177 2023-01-27 09:44:59.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_load_balancer/__init__.py
--rw-rw-rw-   0        0        0      737 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_load_balancer/compliance.py
--rw-rw-rw-   0        0        0     1829 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py
--rw-rw-rw-   0        0        0     1994 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py
--rw-rw-rw-   0        0        0     1700 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_load_balancer/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:41.080280 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_search/
--rw-rw-rw-   0        0        0      197 2023-01-27 11:52:50.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_search/__init__.py
--rw-rw-rw-   0        0        0      432 2023-05-31 11:40:25.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_search/compliance.py
--rw-rw-rw-   0        0        0     1940 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:41.116737 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/guard_duty/
--rw-rw-rw-   0        0        0      207 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/guard_duty/__init__.py
--rw-rw-rw-   0        0        0      430 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/guard_duty/compliance.py
--rw-rw-rw-   0        0        0     1965 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:41.171822 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/lambdafn/
--rw-rw-rw-   0        0        0      181 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/lambdafn/__init__.py
--rw-rw-rw-   0        0        0      648 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/lambdafn/compliance.py
--rw-rw-rw-   0        0        0     1932 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py
--rw-rw-rw-   0        0        0     1737 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py
--rw-rw-rw-   0        0        0      844 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/lambdafn/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:41.247119 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/
--rw-rw-rw-   0        0        0      360 2023-06-06 07:06:27.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/__init__.py
--rw-rw-rw-   0        0        0     2126 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/compliance.py
--rw-rw-rw-   0        0        0     1558 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
--rw-rw-rw-   0        0        0     2319 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/rds_backup_enabled.py
--rw-rw-rw-   0        0        0     2126 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py
--rw-rw-rw-   0        0        0     1479 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py
--rw-rw-rw-   0        0        0     1375 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:41.288529 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/redshift/
--rw-rw-rw-   0        0        0      213 2023-05-31 08:47:40.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/redshift/__init__.py
--rw-rw-rw-   0        0        0     1738 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/redshift/compliance.py
--rw-rw-rw-   0        0        0     1383 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/redshift/redshift_backup_enabled.py
--rw-rw-rw-   0        0        0     1710 2023-05-31 08:41:05.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:41.340769 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/s3/
--rw-rw-rw-   0        0        0      297 2023-06-06 07:10:52.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/s3/__init__.py
--rw-rw-rw-   0        0        0     1112 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/s3/compliance.py
--rw-rw-rw-   0        0        0     1825 2023-05-31 08:23:26.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py
--rw-rw-rw-   0        0        0     1796 2023-05-31 09:39:39.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py
--rw-rw-rw-   0        0        0     1716 2023-05-31 08:23:25.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:41.349768 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/security_hub/
--rw-rw-rw-   0        0        0     1586 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/security_hub/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:22:40.817302 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar.egg-info/
--rw-rw-rw-   0        0        0     1114 2023-06-06 07:22:40.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3079 2023-06-06 07:22:40.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 07:22:40.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-06 07:22:40.000000 OBP_reliability_pillar-0.1.1/OBP_reliability_pillar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1114 2023-06-06 07:22:41.351845 OBP_reliability_pillar-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      755 2022-12-19 13:35:30.000000 OBP_reliability_pillar-0.1.1/README.md
--rw-rw-rw-   0        0        0      498 2023-06-06 07:11:41.000000 OBP_reliability_pillar-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 07:22:41.353770 OBP_reliability_pillar-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:42.550038 OBP_reliability_pillar-0.1.2/
+-rw-rw-rw-   0        0        0        0 2022-11-24 06:08:48.000000 OBP_reliability_pillar-0.1.2/LICENCE
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.059296 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/
+-rw-rw-rw-   0        0        0     4908 2023-07-17 19:04:06.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.177554 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/
+-rw-rw-rw-   0        0        0      197 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/__init__.py
+-rw-rw-rw-   0        0        0     2101 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py
+-rw-rw-rw-   0        0        0      607 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/compliance.py
+-rw-rw-rw-   0        0        0     2223 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.285200 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/cloudwatch/
+-rw-rw-rw-   0        0        0      193 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/cloudwatch/__init__.py
+-rw-rw-rw-   0        0        0     3134 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/cloudwatch/alarm_action_check.py
+-rw-rw-rw-   0        0        0      485 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/cloudwatch/compliance.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.369037 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/
+-rw-rw-rw-   0        0        0      187 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      667 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/compliance.py
+-rw-rw-rw-   0        0        0     2565 2023-07-17 18:59:49.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py
+-rw-rw-rw-   0        0        0     2106 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py
+-rw-rw-rw-   0        0        0      557 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.480043 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/
+-rw-rw-rw-   0        0        0      177 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/__init__.py
+-rw-rw-rw-   0        0        0      709 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/compliance.py
+-rw-rw-rw-   0        0        0     2233 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     2257 2023-05-31 08:17:16.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/instance_in_vpc.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.565664 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_beanstalk/
+-rw-rw-rw-   0        0        0      205 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_beanstalk/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_beanstalk/compliance.py
+-rw-rw-rw-   0        0        0     2339 2023-05-31 08:23:26.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.702452 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/
+-rw-rw-rw-   0        0        0      177 2023-01-27 09:44:59.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/__init__.py
+-rw-rw-rw-   0        0        0      737 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/compliance.py
+-rw-rw-rw-   0        0        0     1829 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py
+-rw-rw-rw-   0        0        0     1994 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py
+-rw-rw-rw-   0        0        0     1700 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.790888 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_search/
+-rw-rw-rw-   0        0        0      197 2023-01-27 11:52:50.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_search/__init__.py
+-rw-rw-rw-   0        0        0      432 2023-05-31 11:40:25.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_search/compliance.py
+-rw-rw-rw-   0        0        0     1940 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.880795 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/guard_duty/
+-rw-rw-rw-   0        0        0      207 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/guard_duty/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/guard_duty/compliance.py
+-rw-rw-rw-   0        0        0     1965 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:42.052487 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/
+-rw-rw-rw-   0        0        0      181 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/compliance.py
+-rw-rw-rw-   0        0        0     1932 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py
+-rw-rw-rw-   0        0        0     1737 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py
+-rw-rw-rw-   0        0        0      844 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:42.239343 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/
+-rw-rw-rw-   0        0        0      360 2023-06-06 07:06:27.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/__init__.py
+-rw-rw-rw-   0        0        0     2126 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/compliance.py
+-rw-rw-rw-   0        0        0     1558 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
+-rw-rw-rw-   0        0        0     2319 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_backup_enabled.py
+-rw-rw-rw-   0        0        0     2126 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     1479 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py
+-rw-rw-rw-   0        0        0     1375 2023-05-31 07:38:13.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:42.355567 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/
+-rw-rw-rw-   0        0        0      213 2023-05-31 08:47:40.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/__init__.py
+-rw-rw-rw-   0        0        0     1738 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/compliance.py
+-rw-rw-rw-   0        0        0     1383 2023-05-31 08:41:04.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/redshift_backup_enabled.py
+-rw-rw-rw-   0        0        0     1710 2023-05-31 08:41:05.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:42.506858 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/
+-rw-rw-rw-   0        0        0      297 2023-06-06 07:10:52.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/__init__.py
+-rw-rw-rw-   0        0        0     1112 2023-05-31 11:40:24.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/compliance.py
+-rw-rw-rw-   0        0        0     1825 2023-05-31 08:23:26.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py
+-rw-rw-rw-   0        0        0     1796 2023-05-31 09:39:39.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py
+-rw-rw-rw-   0        0        0     1716 2023-05-31 08:23:25.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:42.539690 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/security_hub/
+-rw-rw-rw-   0        0        0     1586 2023-01-27 05:16:17.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/security_hub/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:04:41.077247 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/
+-rw-rw-rw-   0        0        0     1114 2023-07-17 19:04:40.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3079 2023-07-17 19:04:41.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 19:04:40.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-17 19:04:40.000000 OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1114 2023-07-17 19:04:42.545674 OBP_reliability_pillar-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2022-12-19 13:35:30.000000 OBP_reliability_pillar-0.1.2/README.md
+-rw-rw-rw-   0        0        0      498 2023-07-17 19:04:06.000000 OBP_reliability_pillar-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 19:04:42.552073 OBP_reliability_pillar-0.1.2/setup.cfg
```

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/__init__.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from OBP_reliability_pillar.s3 import s3
 # from OBP_reliability_pillar.security_hub import security_hub
 from OBP_reliability_pillar.auto_scaling import auto_scaling
 from OBP_reliability_pillar.lambdafn import lambdafn
 from OBP_reliability_pillar.guard_duty import guard_duty
 from OBP_reliability_pillar.elastic_search import elastic_search
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 __author__ = 'Dheeraj Banodha'
 
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
```

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/asg_elb_healthcheck_required.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/auto_scaling/compliance.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/auto_scaling/launch_config_public_ip_disabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/cloudwatch/alarm_action_check.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/cloudwatch/alarm_action_check.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/dynamodb/compliance.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/dynamodb_autoscaling_enabled.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,23 +32,30 @@
             client = self.session.client('dynamodb', region_name=region)
 
             dynamodb_tables = list_dynamodb_tables(client)
             for table in dynamodb_tables:
                 response = client.describe_table(
                     TableName=table
                 )
-                global_secondary_index = [index_name['IndexName'] for index_name in response['table']['GlobalSecondaryIndexes']]
-                response_scalable_targets = client.describe_scalable_targets(
-                    ServiceNamespace='dynamodb',
-                    ResourceIds= [table].extend(global_secondary_index)
-                )
-                if len(response_scalable_targets['ScalableTargets']) == 0:
+                try:
+                    global_secondary_index = [index_name['IndexName'] for index_name in
+                                          response['Table']['GlobalSecondaryIndexes']]
+                    response_scalable_targets = client.describe_scalable_targets(
+                        ServiceNamespace='dynamodb',
+                        ResourceIds=[table].extend(global_secondary_index)
+                    )
+                    if len(response_scalable_targets['ScalableTargets']) == 0:
+                        result = False
+                        failReason = 'AWS DynamoDB Auto Scaling is not enabled for the table and/or its global secondary index.'
+                        offenders.append(table)
+                except KeyError:
                     result = False
                     failReason = 'AWS DynamoDB Auto Scaling is not enabled for the table and/or its global secondary index.'
                     offenders.append(table)
+
         except botocore.exceptions.ClientError as e:
             logger.error("Something went wrong with region {}: {}".format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
```

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/dynamodb_pitr_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/dynamodb/utils.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/ec2/compliance.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/ec2_instance_detailed_monitoring_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/ec2/instance_in_vpc.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/ec2/instance_in_vpc.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_beanstalk/enhanced_health_reporting_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_load_balancer/compliance.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/cross_zone_load_balancing_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/elb_deletion_protection.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_load_balancer/utils.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_load_balancer/utils.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/elastic_search/elastic_search_in_vpc_only.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/guard_duty/guard_duty_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/lambdafn/compliance.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/lambda_dlq_check.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/lambda_inside_vpc.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/lambdafn/utils.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/lambdafn/utils.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/compliance.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/rds_backup_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_backup_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_enhanced_monitoring_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_instance_deletion_protection_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/rds/rds_multi_az_support_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/redshift/compliance.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/redshift/redshift_backup_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/redshift_backup_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/redshift/redshift_cluster_maintenancesettings_check.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/s3/compliance.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/s3_bucket_default_lock_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/s3_bucket_replication_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/s3/s3_bucket_versioning_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar/security_hub/__init__.py` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar/security_hub/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar.egg-info/PKG-INFO` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OBP-reliability-pillar
-Version: 0.1.1
+Version: 0.1.2
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `OBP_reliability_pillar-0.1.1/OBP_reliability_pillar.egg-info/SOURCES.txt` & `OBP_reliability_pillar-0.1.2/OBP_reliability_pillar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OBP_reliability_pillar-0.1.1/PKG-INFO` & `OBP_reliability_pillar-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OBP_reliability_pillar
-Version: 0.1.1
+Version: 0.1.2
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `OBP_reliability_pillar-0.1.1/README.md` & `OBP_reliability_pillar-0.1.2/README.md`

 * *Files identical despite different names*

