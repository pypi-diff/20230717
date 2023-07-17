# Comparing `tmp/iparapheur-provisioning-1.7.1.tar.gz` & `tmp/iparapheur-provisioning-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iparapheur-provisioning-1.7.1.tar", last modified: Wed Jul 12 16:47:15 2023, max compression
+gzip compressed data, was "iparapheur-provisioning-1.7.2.tar", last modified: Mon Jul 17 16:19:24 2023, max compression
```

## Comparing `iparapheur-provisioning-1.7.1.tar` & `iparapheur-provisioning-1.7.2.tar`

### file list

```diff
@@ -1,314 +1,316 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/
--rw-r--r--   0 root         (0) root         (0)     1111 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      421 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20775 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.009614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/
--rw-r--r--   0 root         (0) root         (0)      907 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58620 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.009614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/
--rw-r--r--   0 root         (0) root         (0)      214 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7584 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.013614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/
--rw-r--r--   0 root         (0) root         (0)      250 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      261 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
--rw-r--r--   0 root         (0) root         (0)      315 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id.py
--rw-r--r--   0 root         (0) root         (0)      338 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py
--rw-r--r--   0 root         (0) root         (0)      329 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)      210 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition.py
--rw-r--r--   0 root         (0) root         (0)      264 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.013614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/
--rw-r--r--   0 root         (0) root         (0)      622 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_all_users_api.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_tenant_api.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_typology_api.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py
--rw-r--r--   0 root         (0) root         (0)    15677 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/
--rw-r--r--   0 root         (0) root         (0)      357 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-07-12 16:45:38.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    24041 2023-07-12 16:45:40.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/desk_dto.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-07-12 16:45:41.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     4553 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/error_response.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)     2680 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3284 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     7908 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     1356 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     9141 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     9205 2023-07-12 16:45:45.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)     9132 2023-07-12 16:45:45.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     9123 2023-07-12 16:45:45.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-07-12 16:45:46.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-07-12 16:45:46.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)     9232 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_workflow_definition_representation.py
--rw-r--r--   0 root         (0) root         (0)     5251 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/pageable_object.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)     6982 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/seal_certificate_dto.py
--rw-r--r--   0 root         (0) root         (0)     4500 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/signature_format.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/sort_object.py
--rw-r--r--   0 root         (0) root         (0)    29448 2023-07-12 16:45:49.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     3274 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     9365 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/type_dto.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/type_representation.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    29666 2023-07-12 16:45:52.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_dto.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-07-12 16:45:53.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-07-12 16:45:53.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_representation.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     4499 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/workflow_definition_representation.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/models/
--rw-r--r--   0 root         (0) root         (0)     4365 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/
--rw-r--r--   0 root         (0) root         (0)     2558 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)      369 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13070 2023-07-12 16:46:08.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py
--rw-r--r--   0 root         (0) root         (0)    13629 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)      389 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11083 2023-07-12 16:46:08.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11332 2023-07-12 16:46:08.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15808 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)      399 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15034 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
--rw-r--r--   0 root         (0) root         (0)    16302 2023-07-12 16:45:58.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.021614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-07-12 16:45:58.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11677 2023-07-12 16:45:59.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16545 2023-07-12 16:45:59.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/
--rw-r--r--   0 root         (0) root         (0)      407 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15486 2023-07-12 16:46:02.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py
--rw-r--r--   0 root         (0) root         (0)    16907 2023-07-12 16:46:01.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
--rw-r--r--   0 root         (0) root         (0)      431 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11413 2023-07-12 16:46:01.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-07-12 16:46:02.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16979 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
--rw-r--r--   0 root         (0) root         (0)      423 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14894 2023-07-12 16:46:05.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py
--rw-r--r--   0 root         (0) root         (0)    19934 2023-07-12 16:46:04.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
--rw-r--r--   0 root         (0) root         (0)      463 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12091 2023-07-12 16:46:04.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    12371 2023-07-12 16:46:05.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py
--rw-r--r--   0 root         (0) root         (0)    20252 2023-07-12 16:46:06.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)      417 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14728 2023-07-12 16:46:15.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
--rw-r--r--   0 root         (0) root         (0)    15777 2023-07-12 16:46:12.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)      433 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-07-12 16:46:13.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11590 2023-07-12 16:46:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15521 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.025614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)      449 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15050 2023-07-12 16:46:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
--rw-r--r--   0 root         (0) root         (0)    16640 2023-07-12 16:46:12.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)      471 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11672 2023-07-12 16:46:13.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11934 2023-07-12 16:46:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16645 2023-07-12 16:46:15.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)      399 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15944 2023-07-12 16:46:10.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
--rw-r--r--   0 root         (0) root         (0)    15781 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11580 2023-07-12 16:46:10.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16046 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
--rw-r--r--   0 root         (0) root         (0)      429 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15256 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
--rw-r--r--   0 root         (0) root         (0)      477 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11623 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)      365 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13222 2023-07-12 16:45:56.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.029614 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11207 2023-07-12 16:45:55.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11978 2023-07-12 16:45:56.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15946 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
--rw-r--r--   0 root         (0) root         (0)    10635 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/rest.py
--rw-r--r--   0 root         (0) root         (0)    97752 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.009614 iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      421 2023-07-12 16:47:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    19038 2023-07-12 16:47:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 16:47:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-12 16:47:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 16:47:14.000000 iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1322 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.005614 iparapheur-provisioning-1.7.1/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.037614 iparapheur-provisioning-1.7.1/test/test_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:18.000000 iparapheur-provisioning-1.7.1/test/test_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-07-12 16:45:39.000000 iparapheur-provisioning-1.7.1/test/test_models/test_delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-07-12 16:45:41.000000 iparapheur-provisioning-1.7.1/test/test_models/test_desk_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-07-12 16:45:41.000000 iparapheur-provisioning-1.7.1/test/test_models/test_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/test/test_models/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)      767 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/test/test_models/test_external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/test/test_models/test_external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/test/test_models/test_external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/test/test_models/test_folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-07-12 16:45:42.000000 iparapheur-provisioning-1.7.1/test/test_models/test_internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/test/test_models/test_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/test/test_models/test_layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      661 2023-07-12 16:45:43.000000 iparapheur-provisioning-1.7.1/test/test_models/test_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/test/test_models/test_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/test/test_models/test_metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/test/test_models/test_metadata_type.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      722 2023-07-12 16:45:44.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      751 2023-07-12 16:45:45.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-07-12 16:45:45.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      714 2023-07-12 16:45:46.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-07-12 16:45:46.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-07-12 16:45:46.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      763 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/test/test_models/test_page_workflow_definition_representation.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/test/test_models/test_pageable_object.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-07-12 16:45:47.000000 iparapheur-provisioning-1.7.1/test/test_models/test_pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/test/test_models/test_seal_certificate_dto.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/test/test_models/test_seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/test/test_models/test_seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/test/test_models/test_signature_format.py
--rw-r--r--   0 root         (0) root         (0)      685 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/test/test_models/test_signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-07-12 16:45:48.000000 iparapheur-provisioning-1.7.1/test/test_models/test_sort_object.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/test/test_models/test_subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/test/test_models/test_subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/test/test_models/test_subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/test/test_models/test_subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-07-12 16:45:50.000000 iparapheur-provisioning-1.7.1/test/test_models/test_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      653 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/test/test_models/test_tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/test/test_models/test_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/test/test_models/test_tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/test/test_models/test_type_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/test/test_models/test_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-07-12 16:45:51.000000 iparapheur-provisioning-1.7.1/test/test_models/test_typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-07-12 16:45:53.000000 iparapheur-provisioning-1.7.1/test/test_models/test_user_dto.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-07-12 16:45:53.000000 iparapheur-provisioning-1.7.1/test/test_models/test_user_privilege.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/test/test_models/test_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/test/test_models/test_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/test/test_models/test_workflow_definition_representation.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-07-12 16:45:54.000000 iparapheur-provisioning-1.7.1/test/test_models/test_workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.037614 iparapheur-provisioning-1.7.1/test/test_paths/
--rw-r--r--   0 root         (0) root         (0)     1995 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.037614 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)      887 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-07-12 16:46:09.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      924 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-07-12 16:46:00.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)      970 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1005 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      989 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-07-12 16:46:03.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      970 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py
--rw-r--r--   0 root         (0) root         (0)      976 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1064 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1051 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1025 2023-07-12 16:46:07.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.041615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-12 16:46:16.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-07-12 16:46:11.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)      982 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1081 2023-07-12 16:46:17.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 16:47:15.045615 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-07-12 16:45:57.000000 iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.410673 iparapheur-provisioning-1.7.2/
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      421 2023-07-17 16:19:24.410673 iparapheur-provisioning-1.7.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20844 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.366673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/
+-rw-r--r--   0 root         (0) root         (0)      907 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58620 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.370673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7584 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/path_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.370673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/
+-rw-r--r--   0 root         (0) root         (0)      250 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      261 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-07-17 16:18:42.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-17 16:18:42.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
+-rw-r--r--   0 root         (0) root         (0)      315 2023-07-17 16:18:45.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-07-17 16:18:45.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id.py
+-rw-r--r--   0 root         (0) root         (0)      338 2023-07-17 16:18:48.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-07-17 16:18:48.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-07-17 16:18:52.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-17 16:18:52.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)      210 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition.py
+-rw-r--r--   0 root         (0) root         (0)      264 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-17 16:18:39.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-07-17 16:18:39.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tag_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.374673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/
+-rw-r--r--   0 root         (0) root         (0)      622 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-07-17 16:18:39.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_all_users_api.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-07-17 16:18:43.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-07-17 16:18:45.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-07-17 16:18:48.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_tenant_api.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-07-17 16:18:52.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py
+-rw-r--r--   0 root         (0) root         (0)    15677 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.382673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6643 2023-07-17 16:18:24.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/certificate_informations.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-07-17 16:18:24.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    24041 2023-07-17 16:18:25.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-07-17 16:18:26.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-07-17 16:18:26.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2023-07-17 16:18:26.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3284 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     7908 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-07-17 16:18:28.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-07-17 16:18:28.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-07-17 16:18:28.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9141 2023-07-17 16:18:28.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9205 2023-07-17 16:18:28.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9132 2023-07-17 16:18:29.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9123 2023-07-17 16:18:29.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-07-17 16:18:29.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-07-17 16:18:30.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9232 2023-07-17 16:18:30.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-07-17 16:18:30.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-07-17 16:18:31.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     8300 2023-07-17 16:18:31.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/seal_certificate_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4500 2023-07-17 16:18:31.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-07-17 16:18:31.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-07-17 16:18:31.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-07-17 16:18:31.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-07-17 16:18:31.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/sort_object.py
+-rw-r--r--   0 root         (0) root         (0)    29448 2023-07-17 16:18:32.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-07-17 16:18:33.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-07-17 16:18:33.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-07-17 16:18:33.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-07-17 16:18:33.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-07-17 16:18:33.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-07-17 16:18:34.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-17 16:18:34.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     9365 2023-07-17 16:18:34.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/type_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-07-17 16:18:34.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-07-17 16:18:34.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    29666 2023-07-17 16:18:35.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-07-17 16:18:36.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-07-17 16:18:36.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-07-17 16:18:36.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     4499 2023-07-17 16:18:36.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-07-17 16:18:36.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.382673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/models/
+-rw-r--r--   0 root         (0) root         (0)     4456 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.382673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.382673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13070 2023-07-17 16:18:49.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py
+-rw-r--r--   0 root         (0) root         (0)    13629 2023-07-17 16:18:48.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.386673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)      389 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11083 2023-07-17 16:18:49.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11332 2023-07-17 16:18:49.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15808 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.386673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-07-17 16:18:42.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15034 2023-07-17 16:18:42.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
+-rw-r--r--   0 root         (0) root         (0)    16302 2023-07-17 16:18:40.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.386673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-17 16:18:42.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-07-17 16:18:41.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11677 2023-07-17 16:18:41.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16545 2023-07-17 16:18:41.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.386673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-07-17 16:18:45.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15486 2023-07-17 16:18:44.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py
+-rw-r--r--   0 root         (0) root         (0)    16907 2023-07-17 16:18:43.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.386673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
+-rw-r--r--   0 root         (0) root         (0)      431 2023-07-17 16:18:45.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11413 2023-07-17 16:18:44.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-07-17 16:18:44.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16979 2023-07-17 16:18:45.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.386673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-07-17 16:18:48.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14894 2023-07-17 16:18:47.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py
+-rw-r--r--   0 root         (0) root         (0)    19934 2023-07-17 16:18:46.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.386673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
+-rw-r--r--   0 root         (0) root         (0)      463 2023-07-17 16:18:48.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12091 2023-07-17 16:18:46.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    12371 2023-07-17 16:18:46.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    20252 2023-07-17 16:18:47.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.390673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)      417 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14728 2023-07-17 16:18:56.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
+-rw-r--r--   0 root         (0) root         (0)    15777 2023-07-17 16:18:53.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.390673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-07-17 16:18:54.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2023-07-17 16:18:55.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15521 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.390673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)      449 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15050 2023-07-17 16:18:56.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-07-17 16:18:53.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.390673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11672 2023-07-17 16:18:54.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11934 2023-07-17 16:18:55.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16645 2023-07-17 16:18:56.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.390673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-07-17 16:18:52.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15944 2023-07-17 16:18:51.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
+-rw-r--r--   0 root         (0) root         (0)    16306 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.390673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-17 16:18:52.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11932 2023-07-17 16:18:51.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11580 2023-07-17 16:18:51.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16046 2023-07-17 16:18:52.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.394673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
+-rw-r--r--   0 root         (0) root         (0)      429 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15256 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.394673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
+-rw-r--r--   0 root         (0) root         (0)      477 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11623 2023-07-17 16:18:58.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.394673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-07-17 16:18:39.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-07-17 16:18:38.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.394673 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-17 16:18:39.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11207 2023-07-17 16:18:38.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11978 2023-07-17 16:18:38.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-07-17 16:18:39.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
+-rw-r--r--   0 root         (0) root         (0)    10635 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/rest.py
+-rw-r--r--   0 root         (0) root         (0)    97752 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.366673 iparapheur-provisioning-1.7.2/iparapheur_provisioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-07-17 16:19:24.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    19146 2023-07-17 16:19:24.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 16:19:24.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-17 16:19:24.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-17 16:19:24.000000 iparapheur-provisioning-1.7.2/iparapheur_provisioning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-17 16:19:24.410673 iparapheur-provisioning-1.7.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.362672 iparapheur-provisioning-1.7.2/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.402673 iparapheur-provisioning-1.7.2/test/test_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/test/test_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-17 16:18:24.000000 iparapheur-provisioning-1.7.2/test/test_models/test_certificate_informations.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-07-17 16:18:24.000000 iparapheur-provisioning-1.7.2/test/test_models/test_delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-07-17 16:18:25.000000 iparapheur-provisioning-1.7.2/test/test_models/test_desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-17 16:18:26.000000 iparapheur-provisioning-1.7.2/test/test_models/test_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-17 16:18:26.000000 iparapheur-provisioning-1.7.2/test/test_models/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/test/test_models/test_external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/test/test_models/test_external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/test/test_models/test_external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/test/test_models/test_folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/test/test_models/test_internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/test/test_models/test_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/test/test_models/test_layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      661 2023-07-17 16:18:27.000000 iparapheur-provisioning-1.7.2/test/test_models/test_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-07-17 16:18:28.000000 iparapheur-provisioning-1.7.2/test/test_models/test_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-07-17 16:18:28.000000 iparapheur-provisioning-1.7.2/test/test_models/test_metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-07-17 16:18:28.000000 iparapheur-provisioning-1.7.2/test/test_models/test_metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-07-17 16:18:28.000000 iparapheur-provisioning-1.7.2/test/test_models/test_page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-07-17 16:18:28.000000 iparapheur-provisioning-1.7.2/test/test_models/test_page_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      751 2023-07-17 16:18:29.000000 iparapheur-provisioning-1.7.2/test/test_models/test_page_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-07-17 16:18:29.000000 iparapheur-provisioning-1.7.2/test/test_models/test_page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-07-17 16:18:29.000000 iparapheur-provisioning-1.7.2/test/test_models/test_page_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-07-17 16:18:29.000000 iparapheur-provisioning-1.7.2/test/test_models/test_page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-07-17 16:18:30.000000 iparapheur-provisioning-1.7.2/test/test_models/test_page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      763 2023-07-17 16:18:30.000000 iparapheur-provisioning-1.7.2/test/test_models/test_page_workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-07-17 16:18:30.000000 iparapheur-provisioning-1.7.2/test/test_models/test_pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-07-17 16:18:31.000000 iparapheur-provisioning-1.7.2/test/test_models/test_pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-17 16:18:31.000000 iparapheur-provisioning-1.7.2/test/test_models/test_seal_certificate_dto.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-17 16:18:31.000000 iparapheur-provisioning-1.7.2/test/test_models/test_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-07-17 16:18:31.000000 iparapheur-provisioning-1.7.2/test/test_models/test_seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-07-17 16:18:31.000000 iparapheur-provisioning-1.7.2/test/test_models/test_signature_format.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-07-17 16:18:31.000000 iparapheur-provisioning-1.7.2/test/test_models/test_signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-17 16:18:32.000000 iparapheur-provisioning-1.7.2/test/test_models/test_sort_object.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-17 16:18:32.000000 iparapheur-provisioning-1.7.2/test/test_models/test_subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-07-17 16:18:33.000000 iparapheur-provisioning-1.7.2/test/test_models/test_subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-17 16:18:33.000000 iparapheur-provisioning-1.7.2/test/test_models/test_subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-17 16:18:33.000000 iparapheur-provisioning-1.7.2/test/test_models/test_subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-07-17 16:18:33.000000 iparapheur-provisioning-1.7.2/test/test_models/test_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      653 2023-07-17 16:18:34.000000 iparapheur-provisioning-1.7.2/test/test_models/test_tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)      697 2023-07-17 16:18:34.000000 iparapheur-provisioning-1.7.2/test/test_models/test_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-07-17 16:18:34.000000 iparapheur-provisioning-1.7.2/test/test_models/test_tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-07-17 16:18:34.000000 iparapheur-provisioning-1.7.2/test/test_models/test_type_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-17 16:18:34.000000 iparapheur-provisioning-1.7.2/test/test_models/test_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-07-17 16:18:34.000000 iparapheur-provisioning-1.7.2/test/test_models/test_typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-07-17 16:18:35.000000 iparapheur-provisioning-1.7.2/test/test_models/test_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-17 16:18:36.000000 iparapheur-provisioning-1.7.2/test/test_models/test_user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-17 16:18:36.000000 iparapheur-provisioning-1.7.2/test/test_models/test_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-07-17 16:18:36.000000 iparapheur-provisioning-1.7.2/test/test_models/test_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-17 16:18:36.000000 iparapheur-provisioning-1.7.2/test/test_models/test_workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-07-17 16:18:36.000000 iparapheur-provisioning-1.7.2/test/test_models/test_workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.402673 iparapheur-provisioning-1.7.2/test/test_paths/
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/test/test_paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.402673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.402673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-07-17 16:18:50.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.402673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:42.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      924 2023-07-17 16:18:42.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-07-17 16:18:42.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.402673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:42.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-07-17 16:18:42.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-17 16:18:42.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-07-17 16:18:42.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.402673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:45.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-07-17 16:18:45.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-07-17 16:18:45.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.402673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:45.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-07-17 16:18:45.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-07-17 16:18:45.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-07-17 16:18:45.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.402673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:48.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-07-17 16:18:48.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-07-17 16:18:48.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.406673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:48.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-07-17 16:18:48.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-07-17 16:18:48.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-07-17 16:18:48.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.406673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.406673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.406673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.406673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-17 16:18:57.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.406673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:52.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-07-17 16:18:52.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-07-17 16:18:52.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.406673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:52.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-07-17 16:18:52.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-17 16:18:52.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-07-17 16:18:52.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.406673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      982 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.406673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-07-17 16:18:59.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.406673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:39.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-07-17 16:18:39.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 16:19:24.410673 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 16:18:39.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-07-17 16:18:39.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-07-17 16:18:39.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-07-17 16:18:39.000000 iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
```

### Comparing `iparapheur-provisioning-1.7.1/LICENSE.md` & `iparapheur-provisioning-1.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/README.md` & `iparapheur-provisioning-1.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 The main link between every sub-services, integrating business code logic.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: DEVELOP
-- Package version: 1.7.1
+- Package version: 1.7.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://libriciel.fr](https://libriciel.fr)
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
 
@@ -224,14 +224,15 @@
 *AdminTypologyApi* | [**update_subtype**](docs/apis/tags/AdminTypologyApi.md#update_subtype) | **put** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId} | Edit a subtype
 *AdminTypologyApi* | [**update_type**](docs/apis/tags/AdminTypologyApi.md#update_type) | **put** /api/provisioning/v1/admin/tenant/{tenantId}/typology/type/{typeId} | Edit a type
 *AdminWorkflowDefinitionApi* | [**delete_workflow_definition**](docs/apis/tags/AdminWorkflowDefinitionApi.md#delete_workflow_definition) | **delete** /api/provisioning/v1/admin/tenant/{tenantId}/workflowDefinition/{workflowDefinitionKey} | Delete a workflow definition
 *AdminWorkflowDefinitionApi* | [**list_workflow_definitions**](docs/apis/tags/AdminWorkflowDefinitionApi.md#list_workflow_definitions) | **get** /api/provisioning/v1/admin/tenant/{tenantId}/workflowDefinition | List workflow definitions
 
 ## Documentation For Models
 
+ - [CertificateInformations](docs/models/CertificateInformations.md)
  - [DelegationSortBy](docs/models/DelegationSortBy.md)
  - [DeskDto](docs/models/DeskDto.md)
  - [DeskRepresentation](docs/models/DeskRepresentation.md)
  - [ErrorResponse](docs/models/ErrorResponse.md)
  - [ExternalSignatureConfigRepresentation](docs/models/ExternalSignatureConfigRepresentation.md)
  - [ExternalSignatureConfigSortBy](docs/models/ExternalSignatureConfigSortBy.md)
  - [ExternalSignatureProvider](docs/models/ExternalSignatureProvider.md)
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/__init__.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
     The version of the OpenAPI document: DEVELOP
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.7.1"
+__version__ = "1.7.2"
 
 # import ApiClient
 from iparapheur_provisioning.api_client import ApiClient
 
 # import Configuration
 from iparapheur_provisioning.configuration import Configuration
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/api_client.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.7.1/python'
+        self.user_agent = 'OpenAPI-Generator/1.7.2/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/path_to_api.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tag_to_api.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/__init__.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_all_users_api.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_all_users_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_desk_api.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_desk_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_metadata_api.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_metadata_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_tenant_api.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_tenant_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_typology_api.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_typology_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/configuration.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: DEVELOP\n"\
-               "SDK Package Version: 1.7.1".\
+               "SDK Package Version: 1.7.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/exceptions.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/exceptions.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/delegation_sort_by.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/desk_dto.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/desk_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/error_response.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/external_signature_config_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/external_signature_config_sort_by.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/external_signature_provider.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/folder_sort_by.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/internal_metadata.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/layer_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/layer_sort_by.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_dto.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_sort_by.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/metadata_type.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_desk_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_metadata_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_seal_certificate_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_subtype_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_tenant_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_type_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_user_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/page_workflow_definition_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/page_workflow_definition_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/pageable_object.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/pageable_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,97 +38,97 @@
         
         class properties:
             offset = schemas.Int64Schema
         
             @staticmethod
             def sort() -> typing.Type['SortObject']:
                 return SortObject
+            unpaged = schemas.BoolSchema
             pageSize = schemas.Int32Schema
             paged = schemas.BoolSchema
             pageNumber = schemas.Int32Schema
-            unpaged = schemas.BoolSchema
             __annotations__ = {
                 "offset": offset,
                 "sort": sort,
+                "unpaged": unpaged,
                 "pageSize": pageSize,
                 "paged": paged,
                 "pageNumber": pageNumber,
-                "unpaged": unpaged,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["offset"]) -> MetaOapg.properties.offset: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sort"]) -> 'SortObject': ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["unpaged"]) -> MetaOapg.properties.unpaged: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["pageSize"]) -> MetaOapg.properties.pageSize: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["paged"]) -> MetaOapg.properties.paged: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["pageNumber"]) -> MetaOapg.properties.pageNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["unpaged"]) -> MetaOapg.properties.unpaged: ...
-    
-    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["offset", "sort", "pageSize", "paged", "pageNumber", "unpaged", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["offset", "sort", "unpaged", "pageSize", "paged", "pageNumber", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["offset"]) -> typing.Union[MetaOapg.properties.offset, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sort"]) -> typing.Union['SortObject', schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["unpaged"]) -> typing.Union[MetaOapg.properties.unpaged, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["pageSize"]) -> typing.Union[MetaOapg.properties.pageSize, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["paged"]) -> typing.Union[MetaOapg.properties.paged, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["pageNumber"]) -> typing.Union[MetaOapg.properties.pageNumber, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["unpaged"]) -> typing.Union[MetaOapg.properties.unpaged, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["offset", "sort", "pageSize", "paged", "pageNumber", "unpaged", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["offset", "sort", "unpaged", "pageSize", "paged", "pageNumber", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         offset: typing.Union[MetaOapg.properties.offset, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         sort: typing.Union['SortObject', schemas.Unset] = schemas.unset,
+        unpaged: typing.Union[MetaOapg.properties.unpaged, bool, schemas.Unset] = schemas.unset,
         pageSize: typing.Union[MetaOapg.properties.pageSize, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         paged: typing.Union[MetaOapg.properties.paged, bool, schemas.Unset] = schemas.unset,
         pageNumber: typing.Union[MetaOapg.properties.pageNumber, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        unpaged: typing.Union[MetaOapg.properties.unpaged, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'PageableObject':
         return super().__new__(
             cls,
             *_args,
             offset=offset,
             sort=sort,
+            unpaged=unpaged,
             pageSize=pageSize,
             paged=paged,
             pageNumber=pageNumber,
-            unpaged=unpaged,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.sort_object import SortObject
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/pdf_signature_position.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/seal_certificate_dto.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/seal_certificate_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -94,21 +94,31 @@
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'password':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
+        
+            @staticmethod
+            def issuer() -> typing.Type['CertificateInformations']:
+                return CertificateInformations
+        
+            @staticmethod
+            def subject() -> typing.Type['CertificateInformations']:
+                return CertificateInformations
             __annotations__ = {
                 "name": name,
                 "id": id,
                 "expirationDate": expirationDate,
                 "usageCount": usageCount,
                 "signatureImageContentId": signatureImageContentId,
                 "password": password,
+                "issuer": issuer,
+                "subject": subject,
             }
     
     name: MetaOapg.properties.name
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
@@ -124,17 +134,23 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["signatureImageContentId"]) -> MetaOapg.properties.signatureImageContentId: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["password"]) -> MetaOapg.properties.password: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["issuer"]) -> 'CertificateInformations': ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["subject"]) -> 'CertificateInformations': ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "expirationDate", "usageCount", "signatureImageContentId", "password", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "expirationDate", "usageCount", "signatureImageContentId", "password", "issuer", "subject", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
@@ -150,37 +166,49 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["signatureImageContentId"]) -> typing.Union[MetaOapg.properties.signatureImageContentId, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["password"]) -> typing.Union[MetaOapg.properties.password, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["issuer"]) -> typing.Union['CertificateInformations', schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["subject"]) -> typing.Union['CertificateInformations', schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "expirationDate", "usageCount", "signatureImageContentId", "password", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "expirationDate", "usageCount", "signatureImageContentId", "password", "issuer", "subject", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
         expirationDate: typing.Union[MetaOapg.properties.expirationDate, str, datetime, schemas.Unset] = schemas.unset,
         usageCount: typing.Union[MetaOapg.properties.usageCount, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         signatureImageContentId: typing.Union[MetaOapg.properties.signatureImageContentId, None, str, schemas.Unset] = schemas.unset,
         password: typing.Union[MetaOapg.properties.password, None, str, schemas.Unset] = schemas.unset,
+        issuer: typing.Union['CertificateInformations', schemas.Unset] = schemas.unset,
+        subject: typing.Union['CertificateInformations', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'SealCertificateDto':
         return super().__new__(
             cls,
             *_args,
             name=name,
             id=id,
             expirationDate=expirationDate,
             usageCount=usageCount,
             signatureImageContentId=signatureImageContentId,
             password=password,
+            issuer=issuer,
+            subject=subject,
             _configuration=_configuration,
             **kwargs,
         )
+
+from iparapheur_provisioning.model.certificate_informations import CertificateInformations
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/seal_certificate_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/seal_certificate_sort_by.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/signature_format.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/signature_protocol.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/sort_object.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/sort_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,66 +34,66 @@
     """
 
 
     class MetaOapg:
         
         class properties:
             empty = schemas.BoolSchema
-            unsorted = schemas.BoolSchema
             sorted = schemas.BoolSchema
+            unsorted = schemas.BoolSchema
             __annotations__ = {
                 "empty": empty,
-                "unsorted": unsorted,
                 "sorted": sorted,
+                "unsorted": unsorted,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["empty"]) -> MetaOapg.properties.empty: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["unsorted"]) -> MetaOapg.properties.unsorted: ...
+    def __getitem__(self, name: typing_extensions.Literal["sorted"]) -> MetaOapg.properties.sorted: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["sorted"]) -> MetaOapg.properties.sorted: ...
+    def __getitem__(self, name: typing_extensions.Literal["unsorted"]) -> MetaOapg.properties.unsorted: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["empty", "unsorted", "sorted", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["empty", "sorted", "unsorted", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["empty"]) -> typing.Union[MetaOapg.properties.empty, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["unsorted"]) -> typing.Union[MetaOapg.properties.unsorted, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["sorted"]) -> typing.Union[MetaOapg.properties.sorted, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["sorted"]) -> typing.Union[MetaOapg.properties.sorted, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["unsorted"]) -> typing.Union[MetaOapg.properties.unsorted, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["empty", "unsorted", "sorted", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["empty", "sorted", "unsorted", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
-        unsorted: typing.Union[MetaOapg.properties.unsorted, bool, schemas.Unset] = schemas.unset,
         sorted: typing.Union[MetaOapg.properties.sorted, bool, schemas.Unset] = schemas.unset,
+        unsorted: typing.Union[MetaOapg.properties.unsorted, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'SortObject':
         return super().__new__(
             cls,
             *_args,
             empty=empty,
-            unsorted=unsorted,
             sorted=sorted,
+            unsorted=unsorted,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_dto.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_layer_association.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_layer_dto.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_metadata_dto.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/subtype_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/tenant_dto.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/tenant_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/tenant_sort_by.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/type_dto.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/type_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/typology_sort_by.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_dto.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_privilege.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/user_sort_by.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/workflow_definition_representation.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/workflow_definition_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/model/workflow_definition_sort_by.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/model/workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/models/__init__.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from iparapheur_provisioning.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
+from iparapheur_provisioning.model.certificate_informations import CertificateInformations
 from iparapheur_provisioning.model.delegation_sort_by import DelegationSortBy
 from iparapheur_provisioning.model.desk_dto import DeskDto
 from iparapheur_provisioning.model.desk_representation import DeskRepresentation
 from iparapheur_provisioning.model.error_response import ErrorResponse
 from iparapheur_provisioning.model.external_signature_config_representation import ExternalSignatureConfigRepresentation
 from iparapheur_provisioning.model.external_signature_config_sort_by import ExternalSignatureConfigSortBy
 from iparapheur_provisioning.model.external_signature_provider import ExternalSignatureProvider
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/__init__.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -136,31 +136,31 @@
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -174,38 +174,38 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
-    '403': _response_for_403,
-    '400': _response_for_400,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -78,31 +78,31 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -116,39 +116,39 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '507': _response_for_507,
     '201': _response_for_201,
-    '403': _response_for_403,
-    '400': _response_for_400,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -85,57 +85,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -93,57 +93,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -104,31 +104,31 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -142,39 +142,39 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
-    '400': _response_for_400,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -162,31 +162,31 @@
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -200,38 +200,38 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
-    '403': _response_for_403,
-    '400': _response_for_400,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,33 +66,14 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
-
-
-@dataclass
-class ApiResponseFor507(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
-    ]
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
-    },
-)
 SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -104,31 +85,31 @@
 _response_for_409 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -142,31 +123,31 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -180,21 +161,40 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor403(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor403ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '507': _response_for_507,
     '409': _response_for_409,
-    '404': _response_for_404,
+    '507': _response_for_507,
     '201': _response_for_201,
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -93,57 +93,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -101,57 +101,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,69 +74,69 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
@@ -150,59 +150,59 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
     '409': _response_for_409,
     '200': _response_for_200,
+    '507': _response_for_507,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -189,57 +189,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,107 +66,107 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = MetadataDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = MetadataDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -180,41 +180,41 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
     '409': _response_for_409,
-    '404': _response_for_404,
+    '507': _response_for_507,
     '201': _response_for_201,
-    '403': _response_for_403,
-    '400': _response_for_400,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -93,57 +93,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -101,57 +101,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,26 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
+
+
+@dataclass
+class ApiResponseFor200(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: schemas.Unset = schemas.unset
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
+)
 SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -93,81 +105,69 @@
 _response_for_507 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
-)
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
-
-
-@dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -181,41 +181,41 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '406': _response_for_406,
     '200': _response_for_200,
+    '507': _response_for_507,
     '404': _response_for_404,
-    '403': _response_for_403,
-    '400': _response_for_400,
+    '406': _response_for_406,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -173,57 +173,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -182,31 +182,31 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -220,39 +220,39 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '507': _response_for_507,
     '201': _response_for_201,
-    '403': _response_for_403,
-    '400': _response_for_400,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,96 +74,96 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '406': _response_for_406,
     '404': _response_for_404,
-    '403': _response_for_403,
+    '406': _response_for_406,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -101,31 +101,31 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -139,39 +139,39 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
-    '400': _response_for_400,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -188,31 +188,31 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -226,39 +226,39 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
-    '400': _response_for_400,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -173,57 +173,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,50 +66,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -123,58 +123,58 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
     '409': _response_for_409,
+    '507': _response_for_507,
     '201': _response_for_201,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -93,57 +93,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -101,57 +101,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -112,57 +112,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -181,57 +181,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,33 +74,14 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
-
-
-@dataclass
-class ApiResponseFor507(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
-    ]
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
-    },
-)
 SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -112,31 +93,31 @@
 _response_for_409 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -150,31 +131,31 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -188,21 +169,40 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor403(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor403ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '507': _response_for_507,
     '409': _response_for_409,
-    '404': _response_for_404,
+    '507': _response_for_507,
     '201': _response_for_201,
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -101,57 +101,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -109,57 +109,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -120,50 +120,50 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor200ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -180,16 +180,16 @@
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
     '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -189,31 +189,31 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -227,39 +227,39 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
-    '400': _response_for_400,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,50 +66,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -123,31 +123,31 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -161,20 +161,40 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor403(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor403ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '507': _response_for_507,
     '409': _response_for_409,
+    '507': _response_for_507,
     '201': _response_for_201,
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,50 +74,50 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -131,19 +131,39 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor403(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor403ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
     '204': _response_for_204,
+    '404': _response_for_404,
     '406': _response_for_406,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -101,57 +101,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,33 +74,14 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
-
-
-@dataclass
-class ApiResponseFor406(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
-    ]
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
-    },
-)
 SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -131,31 +112,31 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -169,20 +150,39 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor403(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor403ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '406': _response_for_406,
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
+    '406': _response_for_406,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -181,57 +181,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
     '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -93,57 +93,57 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
     '404': _response_for_404,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -136,31 +136,31 @@
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -174,38 +174,38 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
-    '403': _response_for_403,
-    '400': _response_for_400,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,31 +66,31 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -104,38 +104,38 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
-    '400': _response_for_400,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -93,31 +93,31 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -131,39 +131,39 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
-    '400': _response_for_400,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -104,31 +104,31 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -142,39 +142,39 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '404': _response_for_404,
-    '403': _response_for_403,
-    '400': _response_for_400,
     '401': _response_for_401,
+    '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/rest.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/rest.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning/schemas.py` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning/schemas.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/iparapheur_provisioning.egg-info/SOURCES.txt` & `iparapheur-provisioning-1.7.2/iparapheur_provisioning.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 iparapheur_provisioning/apis/tags/admin_metadata_api.py
 iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py
 iparapheur_provisioning/apis/tags/admin_tenant_api.py
 iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
 iparapheur_provisioning/apis/tags/admin_typology_api.py
 iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py
 iparapheur_provisioning/model/__init__.py
+iparapheur_provisioning/model/certificate_informations.py
 iparapheur_provisioning/model/delegation_sort_by.py
 iparapheur_provisioning/model/desk_dto.py
 iparapheur_provisioning/model/desk_representation.py
 iparapheur_provisioning/model/error_response.py
 iparapheur_provisioning/model/external_signature_config_representation.py
 iparapheur_provisioning/model/external_signature_config_sort_by.py
 iparapheur_provisioning/model/external_signature_provider.py
@@ -151,14 +152,15 @@
 iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
 iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
 test/test_models/__init__.py
+test/test_models/test_certificate_informations.py
 test/test_models/test_delegation_sort_by.py
 test/test_models/test_desk_dto.py
 test/test_models/test_desk_representation.py
 test/test_models/test_error_response.py
 test/test_models/test_external_signature_config_representation.py
 test/test_models/test_external_signature_config_sort_by.py
 test/test_models/test_external_signature_provider.py
```

### Comparing `iparapheur-provisioning-1.7.1/setup.py` & `iparapheur-provisioning-1.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "iparapheur-provisioning"
-VERSION = "1.7.1"
+VERSION = "1.7.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_delegation_sort_by.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_desk_dto.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_desk_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_error_response.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_external_signature_config_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_external_signature_config_sort_by.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_external_signature_provider.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_folder_sort_by.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_internal_metadata.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_layer_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_layer_sort_by.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_metadata_dto.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_metadata_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_metadata_sort_by.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_metadata_type.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_page_desk_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_page_metadata_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_page_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_page_seal_certificate_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_page_seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_page_subtype_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_page_tenant_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_page_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_page_type_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_page_user_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_page_workflow_definition_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_page_workflow_definition_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_pageable_object.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_pdf_signature_position.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_seal_certificate_dto.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_seal_certificate_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_seal_certificate_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_seal_certificate_sort_by.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_signature_format.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_signature_protocol.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_sort_object.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_subtype_dto.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_subtype_layer_association.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_subtype_layer_dto.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_subtype_metadata_dto.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_subtype_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_tenant_dto.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_tenant_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_tenant_sort_by.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_type_dto.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_type_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_typology_sort_by.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_user_dto.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_user_privilege.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_user_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_user_sort_by.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_workflow_definition_representation.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_workflow_definition_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_models/test_workflow_definition_sort_by.py` & `iparapheur-provisioning-1.7.2/test/test_models/test_workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/__init__.py` & `iparapheur-provisioning-1.7.2/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 409
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Edit a desk  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Get a full user description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
-
-
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdMetadata(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdMetadata unit test stubs
-        Create a metadata  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
+        Edit a desk  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 409
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdMetadataMetadataId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId unit test stubs
-        Edit a metadata  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Get a full user representation  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
-
-
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
-        Create a type  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
+        Create a new user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 409
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype unit test stubs
-        Create a subtype  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
+        Create a type  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 409
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
-        Create a new user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Edit a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 200
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Get a full user description  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Delete a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    response_status = 204
+    response_body = ''
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_workflow_definition import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdWorkflowDefinition(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Edit a user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdWorkflowDefinition unit test stubs
+        List workflow definitions  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 406
-
-
+    response_status = 200
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_workflow_definition import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdWorkflowDefinition(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdWorkflowDefinition unit test stubs
-        List workflow definitions  # noqa: E501
+    ApiProvisioningV1AdminUser unit test stubs
+        List all users on the instance  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUser unit test stubs
-        List all users on the instance  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Edit a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
     response_status = 200
 
 
 
 
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,33 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdMetadata(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUserUserId unit test stubs
-        Delete a user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdMetadata unit test stubs
+        Create a metadata  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 409
+
+
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,34 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdMetadataMetadataId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUserUserId unit test stubs
-        Get a full user representation  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId unit test stubs
+        Edit a metadata  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
     response_status = 200
+    response_body = ''
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.1/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py` & `iparapheur-provisioning-1.7.2/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUserUserId unit test stubs
-        Edit a user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype unit test stubs
+        Create a subtype  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 409
 
 
 
 
 
 
 if __name__ == '__main__':
```

