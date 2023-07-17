# Comparing `tmp/django_restit-4.1.7.tar.gz` & `tmp/django_restit-4.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_restit-4.1.7.tar", max compression
+gzip compressed data, was "django_restit-4.1.8.tar", max compression
```

## Comparing `django_restit-4.1.7.tar` & `django_restit-4.1.8.tar`

### file list

```diff
@@ -1,458 +1,458 @@
--rw-r--r--   0        0        0     1068 2023-06-27 05:37:44.430230 django_restit-4.1.7/LICENSE.md
--rw-r--r--   0        0        0     6240 2023-06-30 17:03:51.486194 django_restit-4.1.7/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.430501 django_restit-4.1.7/account/__init__.py
--rw-r--r--   0        0        0     1839 2023-06-27 05:37:44.430617 django_restit-4.1.7/account/admin.py
--rw-r--r--   0        0        0      980 2023-06-27 05:37:44.430754 django_restit-4.1.7/account/fcm/__init__.py
--rw-r--r--   0        0        0    15894 2023-06-27 05:37:44.430954 django_restit-4.1.7/account/migrations/0001_initial.py
--rw-r--r--   0        0        0      738 2023-06-27 05:37:44.431054 django_restit-4.1.7/account/migrations/0003_member_phone_number.py
--rw-r--r--   0        0        0      551 2023-06-27 05:37:44.431131 django_restit-4.1.7/account/migrations/0004_group_modified_alter_group_created.py
--rw-r--r--   0        0        0      437 2023-06-27 05:37:44.431211 django_restit-4.1.7/account/migrations/0005_member_auth_code_expires.py
--rw-r--r--   0        0        0      450 2023-06-27 05:37:44.431293 django_restit-4.1.7/account/migrations/0006_member_security_token.py
--rw-r--r--   0        0        0     1654 2023-06-27 05:37:44.431375 django_restit-4.1.7/account/migrations/0007_authtoken_signature_authsession.py
--rw-r--r--   0        0        0     2379 2023-06-27 05:37:44.431464 django_restit-4.1.7/account/migrations/0008_memberdevice_memberdevicemetadata.py
--rw-r--r--   0        0        0      468 2023-06-27 05:37:44.431538 django_restit-4.1.7/account/migrations/0009_alter_member_phone_number.py
--rw-r--r--   0        0        0      305 2023-06-27 05:37:44.431613 django_restit-4.1.7/account/migrations/0010_delete_authtoken.py
--rw-r--r--   0        0        0     1062 2023-06-27 05:37:44.431685 django_restit-4.1.7/account/migrations/0011_authtoken.py
--rw-r--r--   0        0        0     2043 2023-06-27 05:37:44.431755 django_restit-4.1.7/account/migrations/0012_settings_settingsmetadata.py
--rw-r--r--   0        0        0      418 2023-07-13 15:44:27.208937 django_restit-4.1.7/account/migrations/0013_memberdevice_ip.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.431784 django_restit-4.1.7/account/migrations/__init__.py
--rw-r--r--   0        0        0      341 2023-06-27 05:37:44.431899 django_restit-4.1.7/account/models/__init__.py
--rw-r--r--   0        0        0     3680 2023-07-13 15:49:05.899210 django_restit-4.1.7/account/models/device.py
--rw-r--r--   0        0        0     1437 2023-06-27 05:37:44.432051 django_restit-4.1.7/account/models/feeds.py
--rw-r--r--   0        0        0    18212 2023-07-15 18:26:26.310351 django_restit-4.1.7/account/models/group.py
--rw-r--r--   0        0        0     2720 2023-06-27 05:37:44.432315 django_restit-4.1.7/account/models/legacy.py
--rw-r--r--   0        0        0    46768 2023-07-13 15:47:39.240494 django_restit-4.1.7/account/models/member.py
--rw-r--r--   0        0        0     6842 2023-06-27 05:37:44.432689 django_restit-4.1.7/account/models/membership.py
--rw-r--r--   0        0        0    10739 2023-06-27 05:37:44.432797 django_restit-4.1.7/account/models/notify.py
--rw-r--r--   0        0        0     3345 2023-06-27 05:37:44.432886 django_restit-4.1.7/account/models/session.py
--rw-r--r--   0        0        0     2137 2023-06-27 05:37:44.432966 django_restit-4.1.7/account/models/settings.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.433042 django_restit-4.1.7/account/oauth/__init__.py
--rw-r--r--   0        0        0     2078 2023-06-27 05:37:44.433131 django_restit-4.1.7/account/oauth/google.py
--rw-r--r--   0        0        0      578 2023-06-27 05:37:44.433195 django_restit-4.1.7/account/periodic.py
--rw-r--r--   0        0        0      152 2023-06-27 05:37:44.433297 django_restit-4.1.7/account/rpc/__init__.py
--rw-r--r--   0        0        0    12428 2023-06-27 05:37:44.433416 django_restit-4.1.7/account/rpc/auth.py
--rw-r--r--   0        0        0     2852 2023-07-13 15:33:42.583999 django_restit-4.1.7/account/rpc/device.py
--rw-r--r--   0        0        0     3078 2023-06-27 05:37:44.433585 django_restit-4.1.7/account/rpc/group.py
--rw-r--r--   0        0        0     1150 2023-06-27 05:37:44.433650 django_restit-4.1.7/account/rpc/member.py
--rw-r--r--   0        0        0     3344 2023-06-27 05:37:44.433726 django_restit-4.1.7/account/rpc/notify.py
--rw-r--r--   0        0        0     2610 2023-06-27 05:37:44.433805 django_restit-4.1.7/account/rpc/oauth.py
--rw-r--r--   0        0        0      271 2023-06-27 05:37:44.433874 django_restit-4.1.7/account/rpc/settings.py
--rw-r--r--   0        0        0       53 2023-06-27 05:37:44.433934 django_restit-4.1.7/account/settings.py
--rw-r--r--   0        0        0     9709 2023-06-27 05:37:44.434095 django_restit-4.1.7/account/templates/email/base.html
--rw-r--r--   0        0        0    10567 2023-06-27 05:37:44.434205 django_restit-4.1.7/account/templates/email/invite.html
--rw-r--r--   0        0        0    15185 2023-06-27 05:37:44.434344 django_restit-4.1.7/account/templates/email/plain/invite.html
--rw-r--r--   0        0        0    13954 2023-06-27 05:37:44.434450 django_restit-4.1.7/account/templates/email/plain/reset_code.html
--rw-r--r--   0        0        0    10261 2023-06-27 05:37:44.434528 django_restit-4.1.7/account/templates/email/reset_code.html
--rw-r--r--   0        0        0    15163 2023-06-27 05:37:44.434627 django_restit-4.1.7/account/templates/email/simple/invite.html
--rw-r--r--   0        0        0    13944 2023-06-27 05:37:44.434713 django_restit-4.1.7/account/templates/email/simple/reset_code.html
--rw-r--r--   0        0        0      520 2023-06-27 05:37:44.434828 django_restit-4.1.7/auditlog/README
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.434859 django_restit-4.1.7/auditlog/__init__.py
--rw-r--r--   0        0        0     1006 2023-06-27 05:37:44.434933 django_restit-4.1.7/auditlog/admin.py
--rw-r--r--   0        0        0     6553 2023-06-27 05:37:44.435019 django_restit-4.1.7/auditlog/decorators.py
--rw-r--r--   0        0        0     1329 2023-06-27 05:37:44.435081 django_restit-4.1.7/auditlog/middleware.py
--rw-r--r--   0        0        0     3309 2023-06-27 05:37:44.435191 django_restit-4.1.7/auditlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435224 django_restit-4.1.7/auditlog/migrations/__init__.py
--rw-r--r--   0        0        0    16051 2023-06-27 16:49:06.686531 django_restit-4.1.7/auditlog/models.py
--rw-r--r--   0        0        0      264 2023-06-27 05:37:44.435414 django_restit-4.1.7/auditlog/periodic.py
--rw-r--r--   0        0        0     3591 2023-06-27 05:37:44.435492 django_restit-4.1.7/auditlog/rpc.py
--rw-r--r--   0        0        0     2019 2023-06-27 05:37:44.435560 django_restit-4.1.7/auditlog/tq.py
--rw-r--r--   0        0        0      163 2023-06-27 05:37:44.435623 django_restit-4.1.7/auditlog/urls.py
--rw-r--r--   0        0        0     2169 2023-06-27 05:37:44.435745 django_restit-4.1.7/inbox/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435775 django_restit-4.1.7/inbox/__init__.py
--rw-r--r--   0        0        0      243 2023-06-27 05:37:44.435850 django_restit-4.1.7/inbox/admin.py
--rw-r--r--   0        0        0     5621 2023-06-27 05:37:44.435936 django_restit-4.1.7/inbox/handlers.py
--rw-r--r--   0        0        0     6429 2023-06-27 05:37:44.436034 django_restit-4.1.7/inbox/migrations/0001_initial.py
--rw-r--r--   0        0        0      380 2023-06-27 05:37:44.436102 django_restit-4.1.7/inbox/migrations/0002_alter_message_cc.py
--rw-r--r--   0        0        0      416 2023-06-27 05:37:44.436177 django_restit-4.1.7/inbox/migrations/0003_attachment_content_type.py
--rw-r--r--   0        0        0     1140 2023-06-27 05:37:44.436249 django_restit-4.1.7/inbox/migrations/0004_mailtemplate.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.436274 django_restit-4.1.7/inbox/migrations/__init__.py
--rw-r--r--   0        0        0      174 2023-06-27 05:37:44.436383 django_restit-4.1.7/inbox/models/__init__.py
--rw-r--r--   0        0        0     2832 2023-06-27 05:37:44.436463 django_restit-4.1.7/inbox/models/bounce.py
--rw-r--r--   0        0        0     2468 2023-06-27 05:37:44.436568 django_restit-4.1.7/inbox/models/complaint.py
--rw-r--r--   0        0        0     2879 2023-06-27 05:37:44.436797 django_restit-4.1.7/inbox/models/message.py
--rw-r--r--   0        0        0     1013 2023-06-27 05:37:44.436870 django_restit-4.1.7/inbox/models/template.py
--rw-r--r--   0        0        0     1534 2023-06-27 05:37:44.436956 django_restit-4.1.7/inbox/rpc.py
--rw-r--r--   0        0        0       89 2023-06-27 05:37:44.437057 django_restit-4.1.7/inbox/utils/__init__.py
--rw-r--r--   0        0        0     4366 2023-06-27 05:37:44.437161 django_restit-4.1.7/inbox/utils/parsing.py
--rw-r--r--   0        0        0     4098 2023-06-27 05:37:44.437260 django_restit-4.1.7/inbox/utils/render.py
--rw-r--r--   0        0        0     2109 2023-06-27 05:37:44.437361 django_restit-4.1.7/inbox/utils/sending.py
--rw-r--r--   0        0        0     1114 2023-06-27 05:37:44.437469 django_restit-4.1.7/incident/README.md
--rw-r--r--   0        0        0     1468 2023-06-27 22:00:18.628468 django_restit-4.1.7/incident/__init__.py
--rw-r--r--   0        0        0     9720 2023-06-27 05:37:44.437670 django_restit-4.1.7/incident/migrations/0001_initial.py
--rw-r--r--   0        0        0      595 2023-06-27 05:37:44.437757 django_restit-4.1.7/incident/migrations/0002_event_component_event_component_id.py
--rw-r--r--   0        0        0      425 2023-06-27 05:37:44.437826 django_restit-4.1.7/incident/migrations/0003_rule_action.py
--rw-r--r--   0        0        0      662 2023-06-27 05:37:44.437890 django_restit-4.1.7/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py
--rw-r--r--   0        0        0      698 2023-06-27 05:37:44.437964 django_restit-4.1.7/incident/migrations/0005_incident_component_alter_incident_state.py
--rw-r--r--   0        0        0      324 2023-06-27 05:37:44.438034 django_restit-4.1.7/incident/migrations/0006_delete_eventmetadata.py
--rw-r--r--   0        0        0      414 2023-06-27 05:37:44.438100 django_restit-4.1.7/incident/migrations/0007_event_metadata.py
--rw-r--r--   0        0        0      903 2023-06-27 05:37:44.438184 django_restit-4.1.7/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438214 django_restit-4.1.7/incident/migrations/__init__.py
--rw-r--r--   0        0        0      167 2023-06-27 05:37:44.438331 django_restit-4.1.7/incident/models/__init__.py
--rw-r--r--   0        0        0     5068 2023-06-27 22:00:18.628641 django_restit-4.1.7/incident/models/event.py
--rw-r--r--   0        0        0    10022 2023-06-27 05:37:44.438560 django_restit-4.1.7/incident/models/incident.py
--rw-r--r--   0        0        0     2187 2023-06-27 05:37:44.438718 django_restit-4.1.7/incident/models/ossec.py
--rw-r--r--   0        0        0     5300 2023-06-27 05:37:44.438826 django_restit-4.1.7/incident/models/rules.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438911 django_restit-4.1.7/incident/parsers/__init__.py
--rw-r--r--   0        0        0     5289 2023-06-27 05:37:44.439057 django_restit-4.1.7/incident/parsers/ossec.py
--rw-r--r--   0        0        0      723 2023-06-27 05:37:44.439158 django_restit-4.1.7/incident/periodic.py
--rw-r--r--   0        0        0     2831 2023-06-27 05:37:44.439252 django_restit-4.1.7/incident/rpc.py
--rw-r--r--   0        0        0    12732 2023-06-27 05:37:44.439416 django_restit-4.1.7/incident/templates/email/incident_change.html
--rw-r--r--   0        0        0    15173 2023-06-27 05:37:44.439515 django_restit-4.1.7/incident/templates/email/incident_new.html
--rw-r--r--   0        0        0    13208 2023-06-27 05:37:44.439626 django_restit-4.1.7/incident/templates/email/incident_plain.html
--rw-r--r--   0        0        0      796 2023-06-27 05:37:44.439700 django_restit-4.1.7/incident/tq.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.439791 django_restit-4.1.7/location/__init__.py
--rw-r--r--   0        0        0      297 2023-06-27 05:37:44.439885 django_restit-4.1.7/location/admin.py
--rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.440042 django_restit-4.1.7/location/geolocate.py
--rw-r--r--   0        0        0     7000 2023-06-27 05:37:44.440236 django_restit-4.1.7/location/migrations/0001_initial.py
--rw-r--r--   0        0        0      576 2023-06-27 05:37:44.440313 django_restit-4.1.7/location/migrations/0002_geoip_subnet_alter_geoip_ip.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440339 django_restit-4.1.7/location/migrations/__init__.py
--rw-r--r--   0        0        0      230 2023-06-27 05:37:44.440480 django_restit-4.1.7/location/models/__init__.py
--rw-r--r--   0        0        0     2028 2023-06-27 05:37:44.440559 django_restit-4.1.7/location/models/address.py
--rw-r--r--   0        0        0     3500 2023-06-27 05:37:44.440656 django_restit-4.1.7/location/models/ip.py
--rw-r--r--   0        0        0     1994 2023-06-27 05:37:44.440722 django_restit-4.1.7/location/models/legacy.py
--rw-r--r--   0        0        0     2316 2023-06-27 05:37:44.440785 django_restit-4.1.7/location/models/location.py
--rw-r--r--   0        0        0     1474 2023-06-27 05:37:44.440843 django_restit-4.1.7/location/models/track.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440920 django_restit-4.1.7/location/providers/__init__.py
--rw-r--r--   0        0        0      730 2023-06-27 05:37:44.441046 django_restit-4.1.7/location/providers/iplookup/__init__.py
--rw-r--r--   0        0        0     2419 2023-06-27 05:37:44.441128 django_restit-4.1.7/location/providers/iplookup/abstractapi.py
--rw-r--r--   0        0        0     1345 2023-06-27 05:37:44.441192 django_restit-4.1.7/location/providers/iplookup/extremeip.py
--rw-r--r--   0        0        0     2121 2023-06-27 05:37:44.441260 django_restit-4.1.7/location/providers/iplookup/geoplugin.py
--rw-r--r--   0        0        0     1797 2023-06-27 05:37:44.441325 django_restit-4.1.7/location/providers/iplookup/ipapi.py
--rw-r--r--   0        0        0     1265 2023-06-27 05:37:44.441395 django_restit-4.1.7/location/providers/iplookup/ipinfo.py
--rw-r--r--   0        0        0      937 2023-06-27 05:37:44.441463 django_restit-4.1.7/location/providers/iplookup/restit.py
--rw-r--r--   0        0        0       42 2023-06-27 05:37:44.441569 django_restit-4.1.7/location/providers/location/__init__.py
--rw-r--r--   0        0        0     2860 2023-06-27 05:37:44.441653 django_restit-4.1.7/location/providers/location/google.py
--rw-r--r--   0        0        0       46 2023-06-27 05:37:44.441777 django_restit-4.1.7/location/providers/timezones/__init__.py
--rw-r--r--   0        0        0      619 2023-06-27 05:37:44.441855 django_restit-4.1.7/location/providers/timezones/google.py
--rw-r--r--   0        0        0     1935 2023-06-27 05:37:44.441924 django_restit-4.1.7/location/providers/zillow.py
--rw-r--r--   0        0        0      123 2023-06-27 05:37:44.442046 django_restit-4.1.7/location/rpc/__init__.py
--rw-r--r--   0        0        0      875 2023-07-03 18:37:00.843398 django_restit-4.1.7/location/rpc/ip.py
--rw-r--r--   0        0        0      779 2023-06-27 05:37:44.442183 django_restit-4.1.7/location/rpc/location.py
--rw-r--r--   0        0        0     3735 2023-06-27 05:37:44.442254 django_restit-4.1.7/location/rpc/track.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.442312 django_restit-4.1.7/medialib/__init__.py
--rw-r--r--   0        0        0     2261 2023-06-27 05:37:44.442393 django_restit-4.1.7/medialib/admin.py
--rw-r--r--   0        0        0       27 2023-06-27 05:37:44.442482 django_restit-4.1.7/medialib/cvutil/__init__.py
--rw-r--r--   0        0        0     4269 2023-06-27 05:37:44.442556 django_restit-4.1.7/medialib/cvutil/contours.py
--rw-r--r--   0        0        0    12649 2023-06-27 05:37:44.442653 django_restit-4.1.7/medialib/cvutil/images.py
--rw-r--r--   0        0        0     9586 2023-06-27 05:37:44.442744 django_restit-4.1.7/medialib/cvutil/misc.py
--rw-r--r--   0        0        0     5824 2023-06-27 05:37:44.442838 django_restit-4.1.7/medialib/cvutil/text.py
--rw-r--r--   0        0        0    48442 2023-06-27 05:37:44.443047 django_restit-4.1.7/medialib/fixtures/initial_data.json
--rw-r--r--   0        0        0    31978 2023-06-27 05:37:44.443182 django_restit-4.1.7/medialib/fixtures/medialib.json
--rw-r--r--   0        0        0    16989 2023-06-27 05:37:44.443279 django_restit-4.1.7/medialib/fixtures/medialib_test_fixture.json
--rw-r--r--   0        0        0     5442 2023-06-27 05:37:44.443362 django_restit-4.1.7/medialib/forms.py
--rw-r--r--   0        0        0    20518 2023-06-27 05:37:44.443459 django_restit-4.1.7/medialib/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.443499 django_restit-4.1.7/medialib/migrations/__init__.py
--rw-r--r--   0        0        0    52121 2023-06-27 05:37:44.443702 django_restit-4.1.7/medialib/models.py
--rw-r--r--   0        0        0     1189 2023-06-27 05:37:44.443785 django_restit-4.1.7/medialib/ocr.py
--rw-r--r--   0        0        0     1275 2023-06-27 05:37:44.443858 django_restit-4.1.7/medialib/pdf.py
--rw-r--r--   0        0        0      545 2023-06-27 05:37:44.443925 django_restit-4.1.7/medialib/qrcode.py
--rw-r--r--   0        0        0    10312 2023-06-27 05:37:44.444059 django_restit-4.1.7/medialib/render/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444125 django_restit-4.1.7/medialib/render/engines/__init__.py
--rw-r--r--   0        0        0     3531 2023-06-27 05:37:44.444213 django_restit-4.1.7/medialib/render/engines/anigif.py
--rw-r--r--   0        0        0     6881 2023-06-27 05:37:44.444291 django_restit-4.1.7/medialib/render/engines/ffmpeg.py
--rw-r--r--   0        0        0      792 2023-06-27 05:37:44.444369 django_restit-4.1.7/medialib/render/engines/gifsicle.py
--rw-r--r--   0        0        0     3436 2023-06-27 05:37:44.444438 django_restit-4.1.7/medialib/render/engines/hls.py
--rw-r--r--   0        0        0      983 2023-06-27 05:37:44.444498 django_restit-4.1.7/medialib/render/engines/mp4box.py
--rw-r--r--   0        0        0      397 2023-06-27 05:37:44.444604 django_restit-4.1.7/medialib/render/engines/rtmp/Makefile
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444636 django_restit-4.1.7/medialib/render/engines/rtmp/__init__.py
--rw-r--r--   0        0        0     4026 2023-06-27 05:37:44.444726 django_restit-4.1.7/medialib/render/engines/rtmp/rtmp.i
--rw-r--r--   0        0        0      699 2023-06-27 05:37:44.444798 django_restit-4.1.7/medialib/render/engines/rtmpdump.py
--rw-r--r--   0        0        0     1017 2023-06-27 05:37:44.444865 django_restit-4.1.7/medialib/render/engines/rtmpsink.py
--rw-r--r--   0        0        0     3466 2023-06-27 05:37:44.444941 django_restit-4.1.7/medialib/render/engines/video_getinfo.py
--rw-r--r--   0        0        0      809 2023-06-27 05:37:44.445017 django_restit-4.1.7/medialib/render/engines/websnap.py
--rw-r--r--   0        0        0     2193 2023-06-27 05:37:44.445078 django_restit-4.1.7/medialib/render/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.445133 django_restit-4.1.7/medialib/render/presets/__init__.py
--rw-r--r--   0        0        0     4179 2023-06-27 05:37:44.445227 django_restit-4.1.7/medialib/render/presets/akamai.py
--rw-r--r--   0        0        0     3284 2023-06-27 05:37:44.445306 django_restit-4.1.7/medialib/render/presets/animated_thumbnail.py
--rw-r--r--   0        0        0     4004 2023-06-27 05:37:44.445394 django_restit-4.1.7/medialib/render/presets/ffmpeg.py
--rw-r--r--   0        0        0     2087 2023-06-27 05:37:44.445469 django_restit-4.1.7/medialib/render/presets/flv.py
--rw-r--r--   0        0        0     6567 2023-06-27 05:37:44.445567 django_restit-4.1.7/medialib/render/presets/hls.py
--rw-r--r--   0        0        0     6955 2023-06-27 05:37:44.445668 django_restit-4.1.7/medialib/render/presets/image_transcode.py
--rw-r--r--   0        0        0     1094 2023-06-27 05:37:44.445750 django_restit-4.1.7/medialib/render/presets/image_validate.py
--rw-r--r--   0        0        0     2423 2023-06-27 05:37:44.445825 django_restit-4.1.7/medialib/render/presets/mp4.py
--rw-r--r--   0        0        0     4997 2023-06-27 05:37:44.445908 django_restit-4.1.7/medialib/render/presets/video_still.py
--rw-r--r--   0        0        0     3228 2023-06-27 05:37:44.445986 django_restit-4.1.7/medialib/render/presets/video_validate.py
--rw-r--r--   0        0        0      863 2023-06-27 05:37:44.446101 django_restit-4.1.7/medialib/render/presets/websnap.py
--rw-r--r--   0        0        0     2282 2023-06-27 05:37:44.446183 django_restit-4.1.7/medialib/render/presets/youtube.py
--rw-r--r--   0        0        0    16451 2023-06-27 05:37:44.446294 django_restit-4.1.7/medialib/render/render_utils.py
--rw-r--r--   0        0        0      370 2023-06-27 05:37:44.446381 django_restit-4.1.7/medialib/render/schedule.py
--rw-r--r--   0        0        0       82 2023-06-27 05:37:44.446525 django_restit-4.1.7/medialib/rpc/__init__.py
--rw-r--r--   0        0        0    37925 2023-06-27 05:37:44.446687 django_restit-4.1.7/medialib/rpc/legacy.py
--rw-r--r--   0        0        0      617 2023-06-27 05:37:44.446776 django_restit-4.1.7/medialib/rpc/media.py
--rw-r--r--   0        0        0      956 2023-06-27 05:37:44.446852 django_restit-4.1.7/medialib/rpc/tools.py
--rwxr-xr-x   0        0        0     7875 2023-06-27 05:37:44.446994 django_restit-4.1.7/medialib/scripts/init_config
--rw-r--r--   0        0        0     4499 2023-06-27 05:37:44.447158 django_restit-4.1.7/medialib/static/css/base_medialibui.css
--rw-r--r--   0        0        0     3128 2023-06-27 05:37:44.447238 django_restit-4.1.7/medialib/static/css/base_widgets.css
--rw-r--r--   0        0        0     3263 2023-06-27 05:37:44.447311 django_restit-4.1.7/medialib/static/css/jquery.jcrop.css
--rw-r--r--   0        0        0      193 2023-06-27 05:37:44.447412 django_restit-4.1.7/medialib/static/img/arrow-down-white.png
--rw-r--r--   0        0        0     4589 2023-06-27 05:37:44.447507 django_restit-4.1.7/medialib/static/img/bg-body.gif
--rw-r--r--   0        0        0      441 2023-06-27 05:37:44.447579 django_restit-4.1.7/medialib/static/img/cancel.gif
--rw-r--r--   0        0        0      341 2023-06-27 05:37:44.447648 django_restit-4.1.7/medialib/static/img/icon-generic.gif
--rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447712 django_restit-4.1.7/medialib/static/img/icon-image.gif
--rw-r--r--   0        0        0      359 2023-06-27 05:37:44.447775 django_restit-4.1.7/medialib/static/img/icon-media.gif
--rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447850 django_restit-4.1.7/medialib/static/img/icon-zip.gif
--rw-r--r--   0        0        0     3208 2023-06-27 05:37:44.447934 django_restit-4.1.7/medialib/static/img/loading.gif
--rw-r--r--   0        0        0     2537 2023-06-27 05:37:44.448000 django_restit-4.1.7/medialib/static/img/noimage.gif
--rw-r--r--   0        0        0     1057 2023-06-27 05:37:44.448065 django_restit-4.1.7/medialib/static/img/render_err.gif
--rw-r--r--   0        0        0     6716 2023-06-27 05:37:44.448158 django_restit-4.1.7/medialib/static/img/rendering.gif
--rw-r--r--   0        0        0      292 2023-06-27 05:37:44.448225 django_restit-4.1.7/medialib/static/img/star_off.png
--rw-r--r--   0        0        0      297 2023-06-27 05:37:44.448287 django_restit-4.1.7/medialib/static/img/star_on.png
--rw-r--r--   0        0        0     1130 2023-06-27 05:37:44.448351 django_restit-4.1.7/medialib/static/img/unknown.gif
--rwxr-xr-x   0        0        0    74054 2023-06-27 05:37:44.448677 django_restit-4.1.7/medialib/static/lib/caman.full.js
--rw-r--r--   0        0        0    17360 2023-06-27 05:37:44.448823 django_restit-4.1.7/medialib/static/lib/hammer.min.js
--rwxr-xr-x   0        0        0    42434 2023-06-27 05:37:44.449017 django_restit-4.1.7/medialib/static/lib/jquery.Jcrop.js
--rw-r--r--   0        0        0      743 2023-06-27 05:37:44.449098 django_restit-4.1.7/medialib/static/lib/jquery.hammer.js
--rw-r--r--   0        0        0    16587 2023-06-27 05:37:44.449224 django_restit-4.1.7/medialib/static/lib/load-image.min.js
--rwxr-xr-x   0        0        0   111779 2023-06-27 05:37:44.449542 django_restit-4.1.7/medialib/static/lib/swiper.js
--rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449771 django_restit-4.1.7/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js
--rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449850 django_restit-4.1.7/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js
--rw-r--r--   0        0        0     5708 2023-06-27 05:37:44.449979 django_restit-4.1.7/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js
--rw-r--r--   0        0        0     3502 2023-06-27 05:37:44.450059 django_restit-4.1.7/medialib/static/lib/tinymce/plugins/medialib/medialib.html
--rw-r--r--   0        0        0     5876 2023-06-27 05:37:44.450187 django_restit-4.1.7/medialib/stores/__init__.py
--rw-r--r--   0        0        0      601 2023-06-27 05:37:44.450314 django_restit-4.1.7/medialib/stores/apiclient/__init__.py
--rw-r--r--   0        0        0     9852 2023-06-27 05:37:44.450415 django_restit-4.1.7/medialib/stores/apiclient/channel.py
--rw-r--r--   0        0        0    35929 2023-06-27 05:37:44.450591 django_restit-4.1.7/medialib/stores/apiclient/discovery.py
--rw-r--r--   0        0        0     3516 2023-06-27 05:37:44.450684 django_restit-4.1.7/medialib/stores/apiclient/errors.py
--rw-r--r--   0        0        0    52911 2023-06-27 05:37:44.450906 django_restit-4.1.7/medialib/stores/apiclient/http.py
--rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.451002 django_restit-4.1.7/medialib/stores/apiclient/mimeparse.py
--rw-r--r--   0        0        0    11761 2023-06-27 05:37:44.451111 django_restit-4.1.7/medialib/stores/apiclient/model.py
--rw-r--r--   0        0        0     3528 2023-06-27 05:37:44.451205 django_restit-4.1.7/medialib/stores/apiclient/sample_tools.py
--rw-r--r--   0        0        0     9293 2023-06-27 05:37:44.451302 django_restit-4.1.7/medialib/stores/apiclient/schema.py
--rw-r--r--   0        0        0     1592 2023-06-27 05:37:44.451390 django_restit-4.1.7/medialib/stores/filestore.py
--rw-r--r--   0        0        0    69575 2023-06-27 05:37:44.451712 django_restit-4.1.7/medialib/stores/httplib2/__init__.py
--rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.451937 django_restit-4.1.7/medialib/stores/httplib2/cacerts.txt
--rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.452031 django_restit-4.1.7/medialib/stores/httplib2/iri2uri.py
--rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.452160 django_restit-4.1.7/medialib/stores/httplib2/socks.py
--rw-r--r--   0        0        0      706 2023-06-27 05:37:44.452238 django_restit-4.1.7/medialib/stores/httpstore.py
--rw-r--r--   0        0        0      304 2023-06-27 05:37:44.452325 django_restit-4.1.7/medialib/stores/nullstore.py
--rw-r--r--   0        0        0      213 2023-06-27 05:37:44.452492 django_restit-4.1.7/medialib/stores/oauth2client/__init__.py
--rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.452598 django_restit-4.1.7/medialib/stores/oauth2client/anyjson.py
--rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.452767 django_restit-4.1.7/medialib/stores/oauth2client/appengine.py
--rw-r--r--   0        0        0    44346 2023-06-27 05:37:44.452995 django_restit-4.1.7/medialib/stores/oauth2client/client.py
--rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.453091 django_restit-4.1.7/medialib/stores/oauth2client/clientsecrets.py
--rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.453196 django_restit-4.1.7/medialib/stores/oauth2client/crypt.py
--rw-r--r--   0        0        0     3755 2023-06-27 05:37:44.453276 django_restit-4.1.7/medialib/stores/oauth2client/django_orm.py
--rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.453391 django_restit-4.1.7/medialib/stores/oauth2client/file.py
--rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.453451 django_restit-4.1.7/medialib/stores/oauth2client/gce.py
--rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.453541 django_restit-4.1.7/medialib/stores/oauth2client/keyring_storage.py
--rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.453634 django_restit-4.1.7/medialib/stores/oauth2client/locked_file.py
--rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.453698 django_restit-4.1.7/medialib/stores/oauth2client/multistore_file.py
--rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.453764 django_restit-4.1.7/medialib/stores/oauth2client/old_run.py
--rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.453855 django_restit-4.1.7/medialib/stores/oauth2client/tools.py
--rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.453938 django_restit-4.1.7/medialib/stores/oauth2client/util.py
--rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.454013 django_restit-4.1.7/medialib/stores/oauth2client/xsrfutil.py
--rw-r--r--   0        0        0      500 2023-06-27 05:37:44.454077 django_restit-4.1.7/medialib/stores/rtmpstore.py
--rw-r--r--   0        0        0     4583 2023-06-27 05:37:44.454163 django_restit-4.1.7/medialib/stores/s3store.py
--rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.454272 django_restit-4.1.7/medialib/stores/uritemplate/__init__.py
--rw-r--r--   0        0        0      406 2023-06-27 05:37:44.454334 django_restit-4.1.7/medialib/stores/youtubestore.py
--rw-r--r--   0        0        0     3691 2023-06-27 05:37:44.454500 django_restit-4.1.7/medialib/templates/medialib/base.html
--rw-r--r--   0        0        0     1277 2023-06-27 05:37:44.454591 django_restit-4.1.7/medialib/templates/medialib/instances.html
--rw-r--r--   0        0        0     1170 2023-06-27 05:37:44.454657 django_restit-4.1.7/medialib/templates/medialib/items.html
--rw-r--r--   0        0        0     8194 2023-06-27 05:37:44.454746 django_restit-4.1.7/medialib/templates/medialib/library.html
--rw-r--r--   0        0        0       65 2023-06-27 05:37:44.454810 django_restit-4.1.7/medialib/templates/medialib/notify_error.subject
--rw-r--r--   0        0        0       49 2023-06-27 05:37:44.454869 django_restit-4.1.7/medialib/templates/medialib/notify_error.to
--rw-r--r--   0        0        0      272 2023-06-27 05:37:44.454932 django_restit-4.1.7/medialib/templates/medialib/notify_error.txt
--rw-r--r--   0        0        0       71 2023-06-27 05:37:44.454996 django_restit-4.1.7/medialib/templates/medialib/notify_ready.subject
--rw-r--r--   0        0        0       49 2023-06-27 05:37:44.455056 django_restit-4.1.7/medialib/templates/medialib/notify_ready.to
--rw-r--r--   0        0        0      298 2023-06-27 05:37:44.455113 django_restit-4.1.7/medialib/templates/medialib/notify_ready.txt
--rw-r--r--   0        0        0       64 2023-06-27 05:37:44.455175 django_restit-4.1.7/medialib/templates/medialib/notify_render_error.subject
--rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455232 django_restit-4.1.7/medialib/templates/medialib/notify_render_error.to
--rw-r--r--   0        0        0      271 2023-06-27 05:37:44.455301 django_restit-4.1.7/medialib/templates/medialib/notify_render_error.txt
--rw-r--r--   0        0        0       68 2023-06-27 05:37:44.455380 django_restit-4.1.7/medialib/templates/medialib/notify_validate_error.subject
--rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455452 django_restit-4.1.7/medialib/templates/medialib/notify_validate_error.to
--rw-r--r--   0        0        0      275 2023-06-27 05:37:44.455521 django_restit-4.1.7/medialib/templates/medialib/notify_validate_error.txt
--rw-r--r--   0        0        0      206 2023-06-27 05:37:44.455593 django_restit-4.1.7/medialib/templates/medialib/smil
--rw-r--r--   0        0        0     1177 2023-06-27 05:37:44.455665 django_restit-4.1.7/medialib/templates/medialib/test.html
--rw-r--r--   0        0        0     1549 2023-06-27 05:37:44.455737 django_restit-4.1.7/medialib/templates/medialib/testpicker.html
--rw-r--r--   0        0        0     6045 2023-06-27 05:37:44.455814 django_restit-4.1.7/medialib/tests.py
--rw-r--r--   0        0        0      544 2023-06-27 05:37:44.455873 django_restit-4.1.7/medialib/tq.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.455894 django_restit-4.1.7/medialib/urls.py
--rw-r--r--   0        0        0     3756 2023-06-27 05:37:44.455970 django_restit-4.1.7/medialib/utils.py
--rw-r--r--   0        0        0     4321 2023-06-27 05:37:44.456050 django_restit-4.1.7/medialib/views.py
--rw-r--r--   0        0        0     4303 2023-06-27 05:37:44.456166 django_restit-4.1.7/medialib/youtube/__init__.py
--rw-r--r--   0        0        0      601 2023-06-27 05:37:44.456272 django_restit-4.1.7/medialib/youtube/apiclient/__init__.py
--rw-r--r--   0        0        0     9886 2023-06-27 05:37:44.456332 django_restit-4.1.7/medialib/youtube/apiclient/channel.py
--rw-r--r--   0        0        0    35907 2023-06-27 05:37:44.456516 django_restit-4.1.7/medialib/youtube/apiclient/discovery.py
--rw-r--r--   0        0        0     3550 2023-06-27 05:37:44.456592 django_restit-4.1.7/medialib/youtube/apiclient/errors.py
--rw-r--r--   0        0        0    52945 2023-06-27 05:37:44.456694 django_restit-4.1.7/medialib/youtube/apiclient/http.py
--rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.456785 django_restit-4.1.7/medialib/youtube/apiclient/mimeparse.py
--rw-r--r--   0        0        0    11795 2023-06-27 05:37:44.456835 django_restit-4.1.7/medialib/youtube/apiclient/model.py
--rw-r--r--   0        0        0     3596 2023-06-27 05:37:44.456895 django_restit-4.1.7/medialib/youtube/apiclient/sample_tools.py
--rw-r--r--   0        0        0     9327 2023-06-27 05:37:44.456959 django_restit-4.1.7/medialib/youtube/apiclient/schema.py
--rw-r--r--   0        0        0    69581 2023-06-27 05:37:44.457093 django_restit-4.1.7/medialib/youtube/httplib2/__init__.py
--rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.457310 django_restit-4.1.7/medialib/youtube/httplib2/cacerts.txt
--rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.457412 django_restit-4.1.7/medialib/youtube/httplib2/iri2uri.py
--rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.457533 django_restit-4.1.7/medialib/youtube/httplib2/socks.py
--rw-r--r--   0        0        0      213 2023-06-27 05:37:44.457629 django_restit-4.1.7/medialib/youtube/oauth2client/__init__.py
--rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.457687 django_restit-4.1.7/medialib/youtube/oauth2client/anyjson.py
--rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.457830 django_restit-4.1.7/medialib/youtube/oauth2client/appengine.py
--rw-r--r--   0        0        0    44431 2023-06-27 05:37:44.457905 django_restit-4.1.7/medialib/youtube/oauth2client/client.py
--rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.457990 django_restit-4.1.7/medialib/youtube/oauth2client/clientsecrets.py
--rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.458075 django_restit-4.1.7/medialib/youtube/oauth2client/crypt.py
--rw-r--r--   0        0        0     3753 2023-06-27 05:37:44.458140 django_restit-4.1.7/medialib/youtube/oauth2client/django_orm.py
--rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.458204 django_restit-4.1.7/medialib/youtube/oauth2client/file.py
--rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.458255 django_restit-4.1.7/medialib/youtube/oauth2client/gce.py
--rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.458323 django_restit-4.1.7/medialib/youtube/oauth2client/keyring_storage.py
--rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.458399 django_restit-4.1.7/medialib/youtube/oauth2client/locked_file.py
--rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.458454 django_restit-4.1.7/medialib/youtube/oauth2client/multistore_file.py
--rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.458510 django_restit-4.1.7/medialib/youtube/oauth2client/old_run.py
--rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.458604 django_restit-4.1.7/medialib/youtube/oauth2client/tools.py
--rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.458680 django_restit-4.1.7/medialib/youtube/oauth2client/util.py
--rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.458745 django_restit-4.1.7/medialib/youtube/oauth2client/xsrfutil.py
--rw-r--r--   0        0        0     2849 2023-06-27 05:37:44.458806 django_restit-4.1.7/medialib/youtube/upload.py
--rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.458902 django_restit-4.1.7/medialib/youtube/uritemplate/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-27 05:37:44.459001 django_restit-4.1.7/metrics/README.md
--rw-r--r--   0        0        0       90 2023-06-27 05:37:44.459061 django_restit-4.1.7/metrics/__init__.py
--rw-r--r--   0        0        0    23460 2023-06-27 05:37:44.459219 django_restit-4.1.7/metrics/client.py
--rw-r--r--   0        0        0     9182 2023-06-27 05:37:44.459333 django_restit-4.1.7/metrics/eod.py
--rw-r--r--   0        0        0     1664 2023-06-27 05:37:44.459430 django_restit-4.1.7/metrics/examples/eod_example.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459493 django_restit-4.1.7/metrics/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459564 django_restit-4.1.7/metrics/management/commands/__init__.py
--rw-r--r--   0        0        0      429 2023-06-27 05:37:44.459636 django_restit-4.1.7/metrics/management/commands/delete_gauge.py
--rw-r--r--   0        0        0      464 2023-06-27 05:37:44.459697 django_restit-4.1.7/metrics/management/commands/delete_metric.py
--rw-r--r--   0        0        0     2801 2023-06-27 05:37:44.459766 django_restit-4.1.7/metrics/management/commands/fix_redis_metrics_keys.py
--rw-r--r--   0        0        0     1928 2023-06-27 05:37:44.459829 django_restit-4.1.7/metrics/management/commands/generate_test_metrics.py
--rw-r--r--   0        0        0     1742 2023-06-27 05:37:44.459896 django_restit-4.1.7/metrics/management/commands/redis_metrics_send_mail.py
--rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.459957 django_restit-4.1.7/metrics/management/commands/reset_weekly_metrics.py
--rw-r--r--   0        0        0     4343 2023-06-27 05:37:44.460023 django_restit-4.1.7/metrics/management/commands/system_metric.py
--rw-r--r--   0        0        0     2399 2023-06-27 05:37:44.460109 django_restit-4.1.7/metrics/migrations/0001_initial.py
--rw-r--r--   0        0        0     1510 2023-06-27 05:37:44.460172 django_restit-4.1.7/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py
--rw-r--r--   0        0        0      453 2023-06-27 05:37:44.460231 django_restit-4.1.7/metrics/migrations/0003_metrics_expires.py
--rw-r--r--   0        0        0     3271 2023-06-27 05:37:44.460284 django_restit-4.1.7/metrics/migrations/0004_eodmetrics.py
--rw-r--r--   0        0        0     2358 2023-06-27 05:37:44.460347 django_restit-4.1.7/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460367 django_restit-4.1.7/metrics/migrations/__init__.py
--rw-r--r--   0        0        0    11540 2023-07-14 20:40:49.561768 django_restit-4.1.7/metrics/models.py
--rw-r--r--   0        0        0      480 2023-06-27 05:37:44.460528 django_restit-4.1.7/metrics/periodic.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460587 django_restit-4.1.7/metrics/providers/__init__.py
--rw-r--r--   0        0        0     7335 2023-06-27 05:37:44.460691 django_restit-4.1.7/metrics/providers/aws.py
--rw-r--r--   0        0        0    14827 2023-07-11 15:48:34.905677 django_restit-4.1.7/metrics/rpc.py
--rw-r--r--   0        0        0      132 2023-06-27 05:37:44.460832 django_restit-4.1.7/metrics/settings.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460855 django_restit-4.1.7/metrics/tq.py
--rw-r--r--   0        0        0    11508 2023-07-14 00:37:57.980977 django_restit-4.1.7/metrics/utils.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461016 django_restit-4.1.7/pushit/__init__.py
--rw-r--r--   0        0        0      451 2023-06-27 05:37:44.461079 django_restit-4.1.7/pushit/admin.py
--rw-r--r--   0        0        0     4555 2023-06-27 05:37:44.461167 django_restit-4.1.7/pushit/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461190 django_restit-4.1.7/pushit/migrations/__init__.py
--rw-r--r--   0        0        0     5066 2023-07-11 15:47:46.945937 django_restit-4.1.7/pushit/models.py
--rw-r--r--   0        0        0       88 2023-06-27 05:37:44.461351 django_restit-4.1.7/pushit/rpc/__init__.py
--rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.461414 django_restit-4.1.7/pushit/rpc/githooks.py
--rw-r--r--   0        0        0     5028 2023-06-27 05:37:44.461473 django_restit-4.1.7/pushit/rpc/legacy.py
--rw-r--r--   0        0        0      378 2023-06-27 05:37:44.461520 django_restit-4.1.7/pushit/rpc/products.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461605 django_restit-4.1.7/pushit/static/js/models_pushit.js
--rw-r--r--   0        0        0      131 2023-06-27 05:37:44.461676 django_restit-4.1.7/pushit/tq.py
--rw-r--r--   0        0        0     1966 2023-06-27 05:37:44.461734 django_restit-4.1.7/pushit/utils.py
--rw-r--r--   0        0        0     1167 2023-07-16 05:53:03.706046 django_restit-4.1.7/pyproject.toml
--rw-r--r--   0        0        0      118 2023-06-27 05:37:44.461884 django_restit-4.1.7/rest/.gitignore
--rw-r--r--   0        0        0     5460 2023-06-27 05:37:44.461959 django_restit-4.1.7/rest/README.md
--rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462010 django_restit-4.1.7/rest/RemoteEvents.py
--rw-r--r--   0        0        0      120 2023-07-16 05:53:03.730182 django_restit-4.1.7/rest/__init__.py
--rw-r--r--   0        0        0     1967 2023-06-27 05:37:44.462114 django_restit-4.1.7/rest/arc4.py
--rw-r--r--   0        0        0       83 2023-06-27 05:37:44.462161 django_restit-4.1.7/rest/cache.py
--rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462295 django_restit-4.1.7/rest/crypto/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-27 05:37:44.462374 django_restit-4.1.7/rest/crypto/aes.py
--rw-r--r--   0        0        0     4082 2023-06-27 05:37:44.462442 django_restit-4.1.7/rest/crypto/privpub.py
--rw-r--r--   0        0        0     4514 2023-07-11 15:29:38.508089 django_restit-4.1.7/rest/crypto/util.py
--rw-r--r--   0        0        0     7548 2023-07-12 19:54:30.986685 django_restit-4.1.7/rest/datem.py
--rw-r--r--   0        0        0    15573 2023-07-11 15:46:20.585526 django_restit-4.1.7/rest/decorators.py
--rw-r--r--   0        0        0      788 2023-06-27 05:37:44.462816 django_restit-4.1.7/rest/encryption.py
--rw-r--r--   0        0        0      501 2023-07-11 15:16:32.180675 django_restit-4.1.7/rest/errors.py
--rw-r--r--   0        0        0       54 2023-06-27 05:37:44.462913 django_restit-4.1.7/rest/extra/__init__.py
--rw-r--r--   0        0        0     1078 2023-06-27 05:37:44.462982 django_restit-4.1.7/rest/extra/json_metadata.py
--rw-r--r--   0        0        0     9719 2023-06-27 05:37:44.463072 django_restit-4.1.7/rest/fields.py
--rw-r--r--   0        0        0     6316 2023-06-27 05:37:44.463145 django_restit-4.1.7/rest/forms.py
--rw-r--r--   0        0        0    24650 2023-07-11 15:25:55.654664 django_restit-4.1.7/rest/helpers.py
--rw-r--r--   0        0        0      260 2023-06-27 05:37:44.463338 django_restit-4.1.7/rest/joke.py
--rw-r--r--   0        0        0     2298 2023-06-27 05:37:44.463411 django_restit-4.1.7/rest/jwtoken.py
--rw-r--r--   0        0        0    20930 2023-06-27 15:33:50.289063 django_restit-4.1.7/rest/log.py
--rw-r--r--   0        0        0     7754 2023-06-27 05:37:44.463623 django_restit-4.1.7/rest/mail.py
--rw-r--r--   0        0        0     9174 2023-06-27 05:37:44.463711 django_restit-4.1.7/rest/mailman.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463776 django_restit-4.1.7/rest/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463861 django_restit-4.1.7/rest/management/commands/__init__.py
--rw-r--r--   0        0        0      389 2023-06-27 05:37:44.463942 django_restit-4.1.7/rest/management/commands/rpc.py
--rw-r--r--   0        0        0       33 2023-06-27 05:37:44.464028 django_restit-4.1.7/rest/middleware/__init__.py
--rw-r--r--   0        0        0     3513 2023-06-27 05:37:44.464096 django_restit-4.1.7/rest/middleware/cors.py
--rw-r--r--   0        0        0     2345 2023-06-27 05:37:44.464159 django_restit-4.1.7/rest/middleware/db_router.py
--rw-r--r--   0        0        0     5395 2023-06-27 05:37:44.464226 django_restit-4.1.7/rest/middleware/jwt.py
--rw-r--r--   0        0        0     4127 2023-06-27 05:37:44.464313 django_restit-4.1.7/rest/middleware/request.py
--rw-r--r--   0        0        0     9015 2023-06-27 05:37:44.464386 django_restit-4.1.7/rest/middleware/session.py
--rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.464450 django_restit-4.1.7/rest/middleware/session_store.py
--rw-r--r--   0        0        0      130 2023-07-11 15:56:36.722347 django_restit-4.1.7/rest/models/__init__.py
--rw-r--r--   0        0        0    62288 2023-07-12 19:45:09.742630 django_restit-4.1.7/rest/models/base.py
--rw-r--r--   0        0        0      578 2023-07-11 16:03:40.953305 django_restit-4.1.7/rest/models/cacher.py
--rw-r--r--   0        0        0    11606 2023-07-11 15:42:46.818779 django_restit-4.1.7/rest/models/metadata.py
--rw-r--r--   0        0        0   149463 2023-06-27 05:37:44.465139 django_restit-4.1.7/rest/regexes.yaml
--rw-r--r--   0        0        0    15248 2023-07-11 22:23:29.744915 django_restit-4.1.7/rest/requestex.py
--rw-r--r--   0        0        0     3713 2023-06-27 15:25:34.225162 django_restit-4.1.7/rest/rpc.py
--rw-r--r--   0        0        0     7645 2023-06-27 05:37:44.465350 django_restit-4.1.7/rest/search.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.465410 django_restit-4.1.7/rest/serializers/__init__.py
--rw-r--r--   0        0        0     2015 2023-07-12 03:00:36.470673 django_restit-4.1.7/rest/serializers/collection.py
--rw-r--r--   0        0        0     2975 2023-06-27 05:37:44.465556 django_restit-4.1.7/rest/serializers/csv.py
--rw-r--r--   0        0        0     1077 2023-06-27 05:37:44.465616 django_restit-4.1.7/rest/serializers/excel.py
--rw-r--r--   0        0        0     1736 2023-06-27 05:37:44.465675 django_restit-4.1.7/rest/serializers/json.py
--rw-r--r--   0        0        0    61795 2023-07-11 16:27:26.664542 django_restit-4.1.7/rest/serializers/legacy.py
--rw-r--r--   0        0        0     7320 2023-07-14 00:32:10.541201 django_restit-4.1.7/rest/serializers/model.py
--rw-r--r--   0        0        0      997 2023-07-06 18:50:18.372944 django_restit-4.1.7/rest/serializers/profiler.py
--rw-r--r--   0        0        0     6509 2023-07-11 20:46:40.798160 django_restit-4.1.7/rest/serializers/response.py
--rw-r--r--   0        0        0     2734 2023-06-27 05:37:44.466139 django_restit-4.1.7/rest/serializers/util.py
--rw-r--r--   0        0        0     1532 2023-06-27 05:37:44.466216 django_restit-4.1.7/rest/settings_helper.py
--rw-r--r--   0        0        0    95786 2023-06-27 05:37:44.466685 django_restit-4.1.7/rest/static/lib/jquery.js
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466742 django_restit-4.1.7/rest/static/rest/app.css
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466776 django_restit-4.1.7/rest/static/rest/app.js
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466808 django_restit-4.1.7/rest/static/rest/rest.js
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466846 django_restit-4.1.7/rest/static/rest/rest.scss
--rw-r--r--   0        0        0      529 2023-06-27 05:37:44.466992 django_restit-4.1.7/rest/templates/email/error.html
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.467020 django_restit-4.1.7/rest/templates/email/error.subject
--rw-r--r--   0        0        0     7148 2023-06-27 05:37:44.467101 django_restit-4.1.7/rest/templates/rest_docs.html
--rw-r--r--   0        0        0    10880 2023-06-27 05:37:44.467182 django_restit-4.1.7/rest/templates/rest_html.html
--rw-r--r--   0        0        0   185122 2023-06-27 05:37:44.467607 django_restit-4.1.7/rest/ua.py
--rw-r--r--   0        0        0    17064 2023-06-27 05:37:44.467734 django_restit-4.1.7/rest/uberdict.py
--rw-r--r--   0        0        0    11881 2023-06-27 05:37:44.467820 django_restit-4.1.7/rest/url_docs.py
--rw-r--r--   0        0        0     1787 2023-06-27 05:37:44.467877 django_restit-4.1.7/rest/urls.py
--rw-r--r--   0        0        0     1056 2023-06-27 05:37:44.467929 django_restit-4.1.7/rest/views.py
--rw-r--r--   0        0        0      118 2023-06-27 05:37:44.468007 django_restit-4.1.7/sessionlog/.gitignore
--rw-r--r--   0        0        0       62 2023-06-27 05:37:44.468062 django_restit-4.1.7/sessionlog/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468086 django_restit-4.1.7/sessionlog/__init__.py
--rw-r--r--   0        0        0      245 2023-06-27 05:37:44.468153 django_restit-4.1.7/sessionlog/admin.py
--rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.468231 django_restit-4.1.7/sessionlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468261 django_restit-4.1.7/sessionlog/migrations/__init__.py
--rw-r--r--   0        0        0     3978 2023-07-05 22:43:30.431976 django_restit-4.1.7/sessionlog/models.py
--rw-r--r--   0        0        0      383 2023-06-27 05:37:44.468400 django_restit-4.1.7/sessionlog/tests.py
--rw-r--r--   0        0        0       26 2023-06-27 05:37:44.468451 django_restit-4.1.7/sessionlog/views.py
--rw-r--r--   0        0        0     2196 2023-06-27 05:37:44.468543 django_restit-4.1.7/taskqueue/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468569 django_restit-4.1.7/taskqueue/__init__.py
--rw-r--r--   0        0        0      208 2023-06-27 05:37:44.468635 django_restit-4.1.7/taskqueue/admin.py
--rw-r--r--   0        0        0     4738 2023-06-27 05:37:44.468730 django_restit-4.1.7/taskqueue/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468758 django_restit-4.1.7/taskqueue/migrations/__init__.py
--rw-r--r--   0        0        0    16531 2023-06-27 05:37:44.468876 django_restit-4.1.7/taskqueue/models.py
--rw-r--r--   0        0        0     3072 2023-06-27 05:37:44.468952 django_restit-4.1.7/taskqueue/periodic.py
--rw-r--r--   0        0        0     5326 2023-06-27 05:37:44.469019 django_restit-4.1.7/taskqueue/rpc.py
--rw-r--r--   0        0        0      942 2023-06-27 05:37:44.469073 django_restit-4.1.7/taskqueue/tq.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469126 django_restit-4.1.7/taskqueue/transports/__init__.py
--rw-r--r--   0        0        0      623 2023-06-27 05:37:44.469185 django_restit-4.1.7/taskqueue/transports/email.py
--rw-r--r--   0        0        0     2409 2023-06-27 05:37:44.469240 django_restit-4.1.7/taskqueue/transports/http.py
--rw-r--r--   0        0        0     1099 2023-06-27 05:37:44.469291 django_restit-4.1.7/taskqueue/transports/s3.py
--rw-r--r--   0        0        0     1891 2023-06-27 05:37:44.469341 django_restit-4.1.7/taskqueue/transports/sftp.py
--rw-r--r--   0        0        0      142 2023-06-27 05:37:44.469388 django_restit-4.1.7/taskqueue/transports/sms.py
--rw-r--r--   0        0        0    13660 2023-06-27 05:37:44.469465 django_restit-4.1.7/taskqueue/worker.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469517 django_restit-4.1.7/telephony/__init__.py
--rw-r--r--   0        0        0      243 2023-06-27 05:37:44.469571 django_restit-4.1.7/telephony/admin.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469591 django_restit-4.1.7/telephony/decorators.py
--rw-r--r--   0        0        0     3030 2023-06-27 05:37:44.469692 django_restit-4.1.7/telephony/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469714 django_restit-4.1.7/telephony/migrations/__init__.py
--rw-r--r--   0        0        0     7753 2023-06-27 05:37:44.469796 django_restit-4.1.7/telephony/models.py
--rw-r--r--   0        0        0     2126 2023-06-27 05:37:44.469861 django_restit-4.1.7/telephony/phone_util.py
--rw-r--r--   0        0        0     2659 2023-06-27 05:37:44.469923 django_restit-4.1.7/telephony/rpc.py
--rw-r--r--   0        0        0     3624 2023-06-27 05:37:44.470008 django_restit-4.1.7/ws4redis/README.md
--rwxr-xr-x   0        0        0       46 2023-06-27 05:37:44.470065 django_restit-4.1.7/ws4redis/__init__.py
--rw-r--r--   0        0        0     4942 2023-06-27 05:37:44.470133 django_restit-4.1.7/ws4redis/client.py
--rw-r--r--   0        0        0    13110 2023-07-08 23:34:53.804529 django_restit-4.1.7/ws4redis/connection.py
--rwxr-xr-x   0        0        0      636 2023-06-27 05:37:44.470295 django_restit-4.1.7/ws4redis/exceptions.py
--rw-r--r--   0        0        0     5561 2023-07-08 23:30:25.146274 django_restit-4.1.7/ws4redis/redis.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.470422 django_restit-4.1.7/ws4redis/servers/__init__.py
--rw-r--r--   0        0        0     3747 2023-06-27 05:37:44.470507 django_restit-4.1.7/ws4redis/servers/base.py
--rw-r--r--   0        0        0     4329 2023-06-27 05:37:44.470582 django_restit-4.1.7/ws4redis/servers/django.py
--rw-r--r--   0        0        0     1723 2023-06-27 05:37:44.470638 django_restit-4.1.7/ws4redis/servers/uwsgi.py
--rwxr-xr-x   0        0        0     1411 2023-06-27 05:37:44.470697 django_restit-4.1.7/ws4redis/settings.py
--rwxr-xr-x   0        0        0     5122 2023-06-27 05:37:44.470772 django_restit-4.1.7/ws4redis/utf8validator.py
--rwxr-xr-x   0        0        0    14848 2023-06-27 05:37:44.470868 django_restit-4.1.7/ws4redis/websocket.py
--rw-r--r--   0        0        0     7531 1970-01-01 00:00:00.000000 django_restit-4.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-27 05:37:44.430230 django_restit-4.1.8/LICENSE.md
+-rw-r--r--   0        0        0     6240 2023-06-30 17:03:51.486194 django_restit-4.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.430501 django_restit-4.1.8/account/__init__.py
+-rw-r--r--   0        0        0     1839 2023-06-27 05:37:44.430617 django_restit-4.1.8/account/admin.py
+-rw-r--r--   0        0        0      980 2023-06-27 05:37:44.430754 django_restit-4.1.8/account/fcm/__init__.py
+-rw-r--r--   0        0        0    15894 2023-06-27 05:37:44.430954 django_restit-4.1.8/account/migrations/0001_initial.py
+-rw-r--r--   0        0        0      738 2023-06-27 05:37:44.431054 django_restit-4.1.8/account/migrations/0003_member_phone_number.py
+-rw-r--r--   0        0        0      551 2023-06-27 05:37:44.431131 django_restit-4.1.8/account/migrations/0004_group_modified_alter_group_created.py
+-rw-r--r--   0        0        0      437 2023-06-27 05:37:44.431211 django_restit-4.1.8/account/migrations/0005_member_auth_code_expires.py
+-rw-r--r--   0        0        0      450 2023-06-27 05:37:44.431293 django_restit-4.1.8/account/migrations/0006_member_security_token.py
+-rw-r--r--   0        0        0     1654 2023-06-27 05:37:44.431375 django_restit-4.1.8/account/migrations/0007_authtoken_signature_authsession.py
+-rw-r--r--   0        0        0     2379 2023-06-27 05:37:44.431464 django_restit-4.1.8/account/migrations/0008_memberdevice_memberdevicemetadata.py
+-rw-r--r--   0        0        0      468 2023-06-27 05:37:44.431538 django_restit-4.1.8/account/migrations/0009_alter_member_phone_number.py
+-rw-r--r--   0        0        0      305 2023-06-27 05:37:44.431613 django_restit-4.1.8/account/migrations/0010_delete_authtoken.py
+-rw-r--r--   0        0        0     1062 2023-06-27 05:37:44.431685 django_restit-4.1.8/account/migrations/0011_authtoken.py
+-rw-r--r--   0        0        0     2043 2023-06-27 05:37:44.431755 django_restit-4.1.8/account/migrations/0012_settings_settingsmetadata.py
+-rw-r--r--   0        0        0      418 2023-07-13 15:44:27.208937 django_restit-4.1.8/account/migrations/0013_memberdevice_ip.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.431784 django_restit-4.1.8/account/migrations/__init__.py
+-rw-r--r--   0        0        0      341 2023-06-27 05:37:44.431899 django_restit-4.1.8/account/models/__init__.py
+-rw-r--r--   0        0        0     3680 2023-07-13 15:49:05.899210 django_restit-4.1.8/account/models/device.py
+-rw-r--r--   0        0        0     1437 2023-06-27 05:37:44.432051 django_restit-4.1.8/account/models/feeds.py
+-rw-r--r--   0        0        0    18212 2023-07-15 18:26:26.310351 django_restit-4.1.8/account/models/group.py
+-rw-r--r--   0        0        0     2720 2023-06-27 05:37:44.432315 django_restit-4.1.8/account/models/legacy.py
+-rw-r--r--   0        0        0    46833 2023-07-16 20:13:04.054844 django_restit-4.1.8/account/models/member.py
+-rw-r--r--   0        0        0     6842 2023-06-27 05:37:44.432689 django_restit-4.1.8/account/models/membership.py
+-rw-r--r--   0        0        0    10739 2023-06-27 05:37:44.432797 django_restit-4.1.8/account/models/notify.py
+-rw-r--r--   0        0        0     3345 2023-06-27 05:37:44.432886 django_restit-4.1.8/account/models/session.py
+-rw-r--r--   0        0        0     2137 2023-06-27 05:37:44.432966 django_restit-4.1.8/account/models/settings.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.433042 django_restit-4.1.8/account/oauth/__init__.py
+-rw-r--r--   0        0        0     2078 2023-06-27 05:37:44.433131 django_restit-4.1.8/account/oauth/google.py
+-rw-r--r--   0        0        0      578 2023-06-27 05:37:44.433195 django_restit-4.1.8/account/periodic.py
+-rw-r--r--   0        0        0      152 2023-06-27 05:37:44.433297 django_restit-4.1.8/account/rpc/__init__.py
+-rw-r--r--   0        0        0    12428 2023-06-27 05:37:44.433416 django_restit-4.1.8/account/rpc/auth.py
+-rw-r--r--   0        0        0     2852 2023-07-13 15:33:42.583999 django_restit-4.1.8/account/rpc/device.py
+-rw-r--r--   0        0        0     3078 2023-06-27 05:37:44.433585 django_restit-4.1.8/account/rpc/group.py
+-rw-r--r--   0        0        0     1150 2023-06-27 05:37:44.433650 django_restit-4.1.8/account/rpc/member.py
+-rw-r--r--   0        0        0     3344 2023-06-27 05:37:44.433726 django_restit-4.1.8/account/rpc/notify.py
+-rw-r--r--   0        0        0     2610 2023-06-27 05:37:44.433805 django_restit-4.1.8/account/rpc/oauth.py
+-rw-r--r--   0        0        0      271 2023-06-27 05:37:44.433874 django_restit-4.1.8/account/rpc/settings.py
+-rw-r--r--   0        0        0       53 2023-06-27 05:37:44.433934 django_restit-4.1.8/account/settings.py
+-rw-r--r--   0        0        0     9709 2023-06-27 05:37:44.434095 django_restit-4.1.8/account/templates/email/base.html
+-rw-r--r--   0        0        0    10567 2023-06-27 05:37:44.434205 django_restit-4.1.8/account/templates/email/invite.html
+-rw-r--r--   0        0        0    15185 2023-06-27 05:37:44.434344 django_restit-4.1.8/account/templates/email/plain/invite.html
+-rw-r--r--   0        0        0    13954 2023-06-27 05:37:44.434450 django_restit-4.1.8/account/templates/email/plain/reset_code.html
+-rw-r--r--   0        0        0    10261 2023-06-27 05:37:44.434528 django_restit-4.1.8/account/templates/email/reset_code.html
+-rw-r--r--   0        0        0    15163 2023-06-27 05:37:44.434627 django_restit-4.1.8/account/templates/email/simple/invite.html
+-rw-r--r--   0        0        0    13944 2023-06-27 05:37:44.434713 django_restit-4.1.8/account/templates/email/simple/reset_code.html
+-rw-r--r--   0        0        0      520 2023-06-27 05:37:44.434828 django_restit-4.1.8/auditlog/README
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.434859 django_restit-4.1.8/auditlog/__init__.py
+-rw-r--r--   0        0        0     1006 2023-06-27 05:37:44.434933 django_restit-4.1.8/auditlog/admin.py
+-rw-r--r--   0        0        0     6553 2023-06-27 05:37:44.435019 django_restit-4.1.8/auditlog/decorators.py
+-rw-r--r--   0        0        0     1329 2023-06-27 05:37:44.435081 django_restit-4.1.8/auditlog/middleware.py
+-rw-r--r--   0        0        0     3309 2023-06-27 05:37:44.435191 django_restit-4.1.8/auditlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435224 django_restit-4.1.8/auditlog/migrations/__init__.py
+-rw-r--r--   0        0        0    16051 2023-06-27 16:49:06.686531 django_restit-4.1.8/auditlog/models.py
+-rw-r--r--   0        0        0      264 2023-06-27 05:37:44.435414 django_restit-4.1.8/auditlog/periodic.py
+-rw-r--r--   0        0        0     3591 2023-06-27 05:37:44.435492 django_restit-4.1.8/auditlog/rpc.py
+-rw-r--r--   0        0        0     2019 2023-06-27 05:37:44.435560 django_restit-4.1.8/auditlog/tq.py
+-rw-r--r--   0        0        0      163 2023-06-27 05:37:44.435623 django_restit-4.1.8/auditlog/urls.py
+-rw-r--r--   0        0        0     2169 2023-06-27 05:37:44.435745 django_restit-4.1.8/inbox/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435775 django_restit-4.1.8/inbox/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-27 05:37:44.435850 django_restit-4.1.8/inbox/admin.py
+-rw-r--r--   0        0        0     5621 2023-06-27 05:37:44.435936 django_restit-4.1.8/inbox/handlers.py
+-rw-r--r--   0        0        0     6429 2023-06-27 05:37:44.436034 django_restit-4.1.8/inbox/migrations/0001_initial.py
+-rw-r--r--   0        0        0      380 2023-06-27 05:37:44.436102 django_restit-4.1.8/inbox/migrations/0002_alter_message_cc.py
+-rw-r--r--   0        0        0      416 2023-06-27 05:37:44.436177 django_restit-4.1.8/inbox/migrations/0003_attachment_content_type.py
+-rw-r--r--   0        0        0     1140 2023-06-27 05:37:44.436249 django_restit-4.1.8/inbox/migrations/0004_mailtemplate.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.436274 django_restit-4.1.8/inbox/migrations/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-27 05:37:44.436383 django_restit-4.1.8/inbox/models/__init__.py
+-rw-r--r--   0        0        0     2832 2023-06-27 05:37:44.436463 django_restit-4.1.8/inbox/models/bounce.py
+-rw-r--r--   0        0        0     2468 2023-06-27 05:37:44.436568 django_restit-4.1.8/inbox/models/complaint.py
+-rw-r--r--   0        0        0     2879 2023-06-27 05:37:44.436797 django_restit-4.1.8/inbox/models/message.py
+-rw-r--r--   0        0        0     1013 2023-06-27 05:37:44.436870 django_restit-4.1.8/inbox/models/template.py
+-rw-r--r--   0        0        0     1534 2023-06-27 05:37:44.436956 django_restit-4.1.8/inbox/rpc.py
+-rw-r--r--   0        0        0       89 2023-06-27 05:37:44.437057 django_restit-4.1.8/inbox/utils/__init__.py
+-rw-r--r--   0        0        0     4366 2023-06-27 05:37:44.437161 django_restit-4.1.8/inbox/utils/parsing.py
+-rw-r--r--   0        0        0     4098 2023-06-27 05:37:44.437260 django_restit-4.1.8/inbox/utils/render.py
+-rw-r--r--   0        0        0     2109 2023-06-27 05:37:44.437361 django_restit-4.1.8/inbox/utils/sending.py
+-rw-r--r--   0        0        0     1114 2023-06-27 05:37:44.437469 django_restit-4.1.8/incident/README.md
+-rw-r--r--   0        0        0     1468 2023-06-27 22:00:18.628468 django_restit-4.1.8/incident/__init__.py
+-rw-r--r--   0        0        0     9720 2023-06-27 05:37:44.437670 django_restit-4.1.8/incident/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2023-06-27 05:37:44.437757 django_restit-4.1.8/incident/migrations/0002_event_component_event_component_id.py
+-rw-r--r--   0        0        0      425 2023-06-27 05:37:44.437826 django_restit-4.1.8/incident/migrations/0003_rule_action.py
+-rw-r--r--   0        0        0      662 2023-06-27 05:37:44.437890 django_restit-4.1.8/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py
+-rw-r--r--   0        0        0      698 2023-06-27 05:37:44.437964 django_restit-4.1.8/incident/migrations/0005_incident_component_alter_incident_state.py
+-rw-r--r--   0        0        0      324 2023-06-27 05:37:44.438034 django_restit-4.1.8/incident/migrations/0006_delete_eventmetadata.py
+-rw-r--r--   0        0        0      414 2023-06-27 05:37:44.438100 django_restit-4.1.8/incident/migrations/0007_event_metadata.py
+-rw-r--r--   0        0        0      903 2023-06-27 05:37:44.438184 django_restit-4.1.8/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438214 django_restit-4.1.8/incident/migrations/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-27 05:37:44.438331 django_restit-4.1.8/incident/models/__init__.py
+-rw-r--r--   0        0        0     5068 2023-06-27 22:00:18.628641 django_restit-4.1.8/incident/models/event.py
+-rw-r--r--   0        0        0    10022 2023-06-27 05:37:44.438560 django_restit-4.1.8/incident/models/incident.py
+-rw-r--r--   0        0        0     2187 2023-06-27 05:37:44.438718 django_restit-4.1.8/incident/models/ossec.py
+-rw-r--r--   0        0        0     5300 2023-06-27 05:37:44.438826 django_restit-4.1.8/incident/models/rules.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438911 django_restit-4.1.8/incident/parsers/__init__.py
+-rw-r--r--   0        0        0     5289 2023-06-27 05:37:44.439057 django_restit-4.1.8/incident/parsers/ossec.py
+-rw-r--r--   0        0        0      723 2023-06-27 05:37:44.439158 django_restit-4.1.8/incident/periodic.py
+-rw-r--r--   0        0        0     2831 2023-06-27 05:37:44.439252 django_restit-4.1.8/incident/rpc.py
+-rw-r--r--   0        0        0    12732 2023-06-27 05:37:44.439416 django_restit-4.1.8/incident/templates/email/incident_change.html
+-rw-r--r--   0        0        0    15173 2023-06-27 05:37:44.439515 django_restit-4.1.8/incident/templates/email/incident_new.html
+-rw-r--r--   0        0        0    13208 2023-06-27 05:37:44.439626 django_restit-4.1.8/incident/templates/email/incident_plain.html
+-rw-r--r--   0        0        0      796 2023-06-27 05:37:44.439700 django_restit-4.1.8/incident/tq.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.439791 django_restit-4.1.8/location/__init__.py
+-rw-r--r--   0        0        0      297 2023-06-27 05:37:44.439885 django_restit-4.1.8/location/admin.py
+-rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.440042 django_restit-4.1.8/location/geolocate.py
+-rw-r--r--   0        0        0     7000 2023-06-27 05:37:44.440236 django_restit-4.1.8/location/migrations/0001_initial.py
+-rw-r--r--   0        0        0      576 2023-06-27 05:37:44.440313 django_restit-4.1.8/location/migrations/0002_geoip_subnet_alter_geoip_ip.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440339 django_restit-4.1.8/location/migrations/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-27 05:37:44.440480 django_restit-4.1.8/location/models/__init__.py
+-rw-r--r--   0        0        0     2028 2023-06-27 05:37:44.440559 django_restit-4.1.8/location/models/address.py
+-rw-r--r--   0        0        0     3500 2023-06-27 05:37:44.440656 django_restit-4.1.8/location/models/ip.py
+-rw-r--r--   0        0        0     1994 2023-06-27 05:37:44.440722 django_restit-4.1.8/location/models/legacy.py
+-rw-r--r--   0        0        0     2316 2023-06-27 05:37:44.440785 django_restit-4.1.8/location/models/location.py
+-rw-r--r--   0        0        0     1474 2023-06-27 05:37:44.440843 django_restit-4.1.8/location/models/track.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440920 django_restit-4.1.8/location/providers/__init__.py
+-rw-r--r--   0        0        0      730 2023-06-27 05:37:44.441046 django_restit-4.1.8/location/providers/iplookup/__init__.py
+-rw-r--r--   0        0        0     2419 2023-06-27 05:37:44.441128 django_restit-4.1.8/location/providers/iplookup/abstractapi.py
+-rw-r--r--   0        0        0     1345 2023-06-27 05:37:44.441192 django_restit-4.1.8/location/providers/iplookup/extremeip.py
+-rw-r--r--   0        0        0     2121 2023-06-27 05:37:44.441260 django_restit-4.1.8/location/providers/iplookup/geoplugin.py
+-rw-r--r--   0        0        0     1797 2023-06-27 05:37:44.441325 django_restit-4.1.8/location/providers/iplookup/ipapi.py
+-rw-r--r--   0        0        0     1265 2023-06-27 05:37:44.441395 django_restit-4.1.8/location/providers/iplookup/ipinfo.py
+-rw-r--r--   0        0        0      937 2023-06-27 05:37:44.441463 django_restit-4.1.8/location/providers/iplookup/restit.py
+-rw-r--r--   0        0        0       42 2023-06-27 05:37:44.441569 django_restit-4.1.8/location/providers/location/__init__.py
+-rw-r--r--   0        0        0     2860 2023-06-27 05:37:44.441653 django_restit-4.1.8/location/providers/location/google.py
+-rw-r--r--   0        0        0       46 2023-06-27 05:37:44.441777 django_restit-4.1.8/location/providers/timezones/__init__.py
+-rw-r--r--   0        0        0      619 2023-06-27 05:37:44.441855 django_restit-4.1.8/location/providers/timezones/google.py
+-rw-r--r--   0        0        0     1935 2023-06-27 05:37:44.441924 django_restit-4.1.8/location/providers/zillow.py
+-rw-r--r--   0        0        0      123 2023-06-27 05:37:44.442046 django_restit-4.1.8/location/rpc/__init__.py
+-rw-r--r--   0        0        0      875 2023-07-03 18:37:00.843398 django_restit-4.1.8/location/rpc/ip.py
+-rw-r--r--   0        0        0      779 2023-06-27 05:37:44.442183 django_restit-4.1.8/location/rpc/location.py
+-rw-r--r--   0        0        0     3735 2023-06-27 05:37:44.442254 django_restit-4.1.8/location/rpc/track.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.442312 django_restit-4.1.8/medialib/__init__.py
+-rw-r--r--   0        0        0     2261 2023-06-27 05:37:44.442393 django_restit-4.1.8/medialib/admin.py
+-rw-r--r--   0        0        0       27 2023-06-27 05:37:44.442482 django_restit-4.1.8/medialib/cvutil/__init__.py
+-rw-r--r--   0        0        0     4269 2023-06-27 05:37:44.442556 django_restit-4.1.8/medialib/cvutil/contours.py
+-rw-r--r--   0        0        0    12649 2023-06-27 05:37:44.442653 django_restit-4.1.8/medialib/cvutil/images.py
+-rw-r--r--   0        0        0     9586 2023-06-27 05:37:44.442744 django_restit-4.1.8/medialib/cvutil/misc.py
+-rw-r--r--   0        0        0     5824 2023-06-27 05:37:44.442838 django_restit-4.1.8/medialib/cvutil/text.py
+-rw-r--r--   0        0        0    48442 2023-06-27 05:37:44.443047 django_restit-4.1.8/medialib/fixtures/initial_data.json
+-rw-r--r--   0        0        0    31978 2023-06-27 05:37:44.443182 django_restit-4.1.8/medialib/fixtures/medialib.json
+-rw-r--r--   0        0        0    16989 2023-06-27 05:37:44.443279 django_restit-4.1.8/medialib/fixtures/medialib_test_fixture.json
+-rw-r--r--   0        0        0     5442 2023-06-27 05:37:44.443362 django_restit-4.1.8/medialib/forms.py
+-rw-r--r--   0        0        0    20518 2023-06-27 05:37:44.443459 django_restit-4.1.8/medialib/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.443499 django_restit-4.1.8/medialib/migrations/__init__.py
+-rw-r--r--   0        0        0    52121 2023-06-27 05:37:44.443702 django_restit-4.1.8/medialib/models.py
+-rw-r--r--   0        0        0     1189 2023-06-27 05:37:44.443785 django_restit-4.1.8/medialib/ocr.py
+-rw-r--r--   0        0        0     1275 2023-06-27 05:37:44.443858 django_restit-4.1.8/medialib/pdf.py
+-rw-r--r--   0        0        0      545 2023-06-27 05:37:44.443925 django_restit-4.1.8/medialib/qrcode.py
+-rw-r--r--   0        0        0    10312 2023-06-27 05:37:44.444059 django_restit-4.1.8/medialib/render/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444125 django_restit-4.1.8/medialib/render/engines/__init__.py
+-rw-r--r--   0        0        0     3531 2023-06-27 05:37:44.444213 django_restit-4.1.8/medialib/render/engines/anigif.py
+-rw-r--r--   0        0        0     6881 2023-06-27 05:37:44.444291 django_restit-4.1.8/medialib/render/engines/ffmpeg.py
+-rw-r--r--   0        0        0      792 2023-06-27 05:37:44.444369 django_restit-4.1.8/medialib/render/engines/gifsicle.py
+-rw-r--r--   0        0        0     3436 2023-06-27 05:37:44.444438 django_restit-4.1.8/medialib/render/engines/hls.py
+-rw-r--r--   0        0        0      983 2023-06-27 05:37:44.444498 django_restit-4.1.8/medialib/render/engines/mp4box.py
+-rw-r--r--   0        0        0      397 2023-06-27 05:37:44.444604 django_restit-4.1.8/medialib/render/engines/rtmp/Makefile
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444636 django_restit-4.1.8/medialib/render/engines/rtmp/__init__.py
+-rw-r--r--   0        0        0     4026 2023-06-27 05:37:44.444726 django_restit-4.1.8/medialib/render/engines/rtmp/rtmp.i
+-rw-r--r--   0        0        0      699 2023-06-27 05:37:44.444798 django_restit-4.1.8/medialib/render/engines/rtmpdump.py
+-rw-r--r--   0        0        0     1017 2023-06-27 05:37:44.444865 django_restit-4.1.8/medialib/render/engines/rtmpsink.py
+-rw-r--r--   0        0        0     3466 2023-06-27 05:37:44.444941 django_restit-4.1.8/medialib/render/engines/video_getinfo.py
+-rw-r--r--   0        0        0      809 2023-06-27 05:37:44.445017 django_restit-4.1.8/medialib/render/engines/websnap.py
+-rw-r--r--   0        0        0     2193 2023-06-27 05:37:44.445078 django_restit-4.1.8/medialib/render/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.445133 django_restit-4.1.8/medialib/render/presets/__init__.py
+-rw-r--r--   0        0        0     4179 2023-06-27 05:37:44.445227 django_restit-4.1.8/medialib/render/presets/akamai.py
+-rw-r--r--   0        0        0     3284 2023-06-27 05:37:44.445306 django_restit-4.1.8/medialib/render/presets/animated_thumbnail.py
+-rw-r--r--   0        0        0     4004 2023-06-27 05:37:44.445394 django_restit-4.1.8/medialib/render/presets/ffmpeg.py
+-rw-r--r--   0        0        0     2087 2023-06-27 05:37:44.445469 django_restit-4.1.8/medialib/render/presets/flv.py
+-rw-r--r--   0        0        0     6567 2023-06-27 05:37:44.445567 django_restit-4.1.8/medialib/render/presets/hls.py
+-rw-r--r--   0        0        0     6955 2023-06-27 05:37:44.445668 django_restit-4.1.8/medialib/render/presets/image_transcode.py
+-rw-r--r--   0        0        0     1094 2023-06-27 05:37:44.445750 django_restit-4.1.8/medialib/render/presets/image_validate.py
+-rw-r--r--   0        0        0     2423 2023-06-27 05:37:44.445825 django_restit-4.1.8/medialib/render/presets/mp4.py
+-rw-r--r--   0        0        0     4997 2023-06-27 05:37:44.445908 django_restit-4.1.8/medialib/render/presets/video_still.py
+-rw-r--r--   0        0        0     3228 2023-06-27 05:37:44.445986 django_restit-4.1.8/medialib/render/presets/video_validate.py
+-rw-r--r--   0        0        0      863 2023-06-27 05:37:44.446101 django_restit-4.1.8/medialib/render/presets/websnap.py
+-rw-r--r--   0        0        0     2282 2023-06-27 05:37:44.446183 django_restit-4.1.8/medialib/render/presets/youtube.py
+-rw-r--r--   0        0        0    16451 2023-06-27 05:37:44.446294 django_restit-4.1.8/medialib/render/render_utils.py
+-rw-r--r--   0        0        0      370 2023-06-27 05:37:44.446381 django_restit-4.1.8/medialib/render/schedule.py
+-rw-r--r--   0        0        0       82 2023-06-27 05:37:44.446525 django_restit-4.1.8/medialib/rpc/__init__.py
+-rw-r--r--   0        0        0    37925 2023-06-27 05:37:44.446687 django_restit-4.1.8/medialib/rpc/legacy.py
+-rw-r--r--   0        0        0      617 2023-06-27 05:37:44.446776 django_restit-4.1.8/medialib/rpc/media.py
+-rw-r--r--   0        0        0      956 2023-06-27 05:37:44.446852 django_restit-4.1.8/medialib/rpc/tools.py
+-rwxr-xr-x   0        0        0     7875 2023-06-27 05:37:44.446994 django_restit-4.1.8/medialib/scripts/init_config
+-rw-r--r--   0        0        0     4499 2023-06-27 05:37:44.447158 django_restit-4.1.8/medialib/static/css/base_medialibui.css
+-rw-r--r--   0        0        0     3128 2023-06-27 05:37:44.447238 django_restit-4.1.8/medialib/static/css/base_widgets.css
+-rw-r--r--   0        0        0     3263 2023-06-27 05:37:44.447311 django_restit-4.1.8/medialib/static/css/jquery.jcrop.css
+-rw-r--r--   0        0        0      193 2023-06-27 05:37:44.447412 django_restit-4.1.8/medialib/static/img/arrow-down-white.png
+-rw-r--r--   0        0        0     4589 2023-06-27 05:37:44.447507 django_restit-4.1.8/medialib/static/img/bg-body.gif
+-rw-r--r--   0        0        0      441 2023-06-27 05:37:44.447579 django_restit-4.1.8/medialib/static/img/cancel.gif
+-rw-r--r--   0        0        0      341 2023-06-27 05:37:44.447648 django_restit-4.1.8/medialib/static/img/icon-generic.gif
+-rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447712 django_restit-4.1.8/medialib/static/img/icon-image.gif
+-rw-r--r--   0        0        0      359 2023-06-27 05:37:44.447775 django_restit-4.1.8/medialib/static/img/icon-media.gif
+-rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447850 django_restit-4.1.8/medialib/static/img/icon-zip.gif
+-rw-r--r--   0        0        0     3208 2023-06-27 05:37:44.447934 django_restit-4.1.8/medialib/static/img/loading.gif
+-rw-r--r--   0        0        0     2537 2023-06-27 05:37:44.448000 django_restit-4.1.8/medialib/static/img/noimage.gif
+-rw-r--r--   0        0        0     1057 2023-06-27 05:37:44.448065 django_restit-4.1.8/medialib/static/img/render_err.gif
+-rw-r--r--   0        0        0     6716 2023-06-27 05:37:44.448158 django_restit-4.1.8/medialib/static/img/rendering.gif
+-rw-r--r--   0        0        0      292 2023-06-27 05:37:44.448225 django_restit-4.1.8/medialib/static/img/star_off.png
+-rw-r--r--   0        0        0      297 2023-06-27 05:37:44.448287 django_restit-4.1.8/medialib/static/img/star_on.png
+-rw-r--r--   0        0        0     1130 2023-06-27 05:37:44.448351 django_restit-4.1.8/medialib/static/img/unknown.gif
+-rwxr-xr-x   0        0        0    74054 2023-06-27 05:37:44.448677 django_restit-4.1.8/medialib/static/lib/caman.full.js
+-rw-r--r--   0        0        0    17360 2023-06-27 05:37:44.448823 django_restit-4.1.8/medialib/static/lib/hammer.min.js
+-rwxr-xr-x   0        0        0    42434 2023-06-27 05:37:44.449017 django_restit-4.1.8/medialib/static/lib/jquery.Jcrop.js
+-rw-r--r--   0        0        0      743 2023-06-27 05:37:44.449098 django_restit-4.1.8/medialib/static/lib/jquery.hammer.js
+-rw-r--r--   0        0        0    16587 2023-06-27 05:37:44.449224 django_restit-4.1.8/medialib/static/lib/load-image.min.js
+-rwxr-xr-x   0        0        0   111779 2023-06-27 05:37:44.449542 django_restit-4.1.8/medialib/static/lib/swiper.js
+-rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449771 django_restit-4.1.8/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js
+-rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449850 django_restit-4.1.8/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js
+-rw-r--r--   0        0        0     5708 2023-06-27 05:37:44.449979 django_restit-4.1.8/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js
+-rw-r--r--   0        0        0     3502 2023-06-27 05:37:44.450059 django_restit-4.1.8/medialib/static/lib/tinymce/plugins/medialib/medialib.html
+-rw-r--r--   0        0        0     5876 2023-06-27 05:37:44.450187 django_restit-4.1.8/medialib/stores/__init__.py
+-rw-r--r--   0        0        0      601 2023-06-27 05:37:44.450314 django_restit-4.1.8/medialib/stores/apiclient/__init__.py
+-rw-r--r--   0        0        0     9852 2023-06-27 05:37:44.450415 django_restit-4.1.8/medialib/stores/apiclient/channel.py
+-rw-r--r--   0        0        0    35929 2023-06-27 05:37:44.450591 django_restit-4.1.8/medialib/stores/apiclient/discovery.py
+-rw-r--r--   0        0        0     3516 2023-06-27 05:37:44.450684 django_restit-4.1.8/medialib/stores/apiclient/errors.py
+-rw-r--r--   0        0        0    52911 2023-06-27 05:37:44.450906 django_restit-4.1.8/medialib/stores/apiclient/http.py
+-rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.451002 django_restit-4.1.8/medialib/stores/apiclient/mimeparse.py
+-rw-r--r--   0        0        0    11761 2023-06-27 05:37:44.451111 django_restit-4.1.8/medialib/stores/apiclient/model.py
+-rw-r--r--   0        0        0     3528 2023-06-27 05:37:44.451205 django_restit-4.1.8/medialib/stores/apiclient/sample_tools.py
+-rw-r--r--   0        0        0     9293 2023-06-27 05:37:44.451302 django_restit-4.1.8/medialib/stores/apiclient/schema.py
+-rw-r--r--   0        0        0     1592 2023-06-27 05:37:44.451390 django_restit-4.1.8/medialib/stores/filestore.py
+-rw-r--r--   0        0        0    69575 2023-06-27 05:37:44.451712 django_restit-4.1.8/medialib/stores/httplib2/__init__.py
+-rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.451937 django_restit-4.1.8/medialib/stores/httplib2/cacerts.txt
+-rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.452031 django_restit-4.1.8/medialib/stores/httplib2/iri2uri.py
+-rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.452160 django_restit-4.1.8/medialib/stores/httplib2/socks.py
+-rw-r--r--   0        0        0      706 2023-06-27 05:37:44.452238 django_restit-4.1.8/medialib/stores/httpstore.py
+-rw-r--r--   0        0        0      304 2023-06-27 05:37:44.452325 django_restit-4.1.8/medialib/stores/nullstore.py
+-rw-r--r--   0        0        0      213 2023-06-27 05:37:44.452492 django_restit-4.1.8/medialib/stores/oauth2client/__init__.py
+-rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.452598 django_restit-4.1.8/medialib/stores/oauth2client/anyjson.py
+-rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.452767 django_restit-4.1.8/medialib/stores/oauth2client/appengine.py
+-rw-r--r--   0        0        0    44346 2023-06-27 05:37:44.452995 django_restit-4.1.8/medialib/stores/oauth2client/client.py
+-rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.453091 django_restit-4.1.8/medialib/stores/oauth2client/clientsecrets.py
+-rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.453196 django_restit-4.1.8/medialib/stores/oauth2client/crypt.py
+-rw-r--r--   0        0        0     3755 2023-06-27 05:37:44.453276 django_restit-4.1.8/medialib/stores/oauth2client/django_orm.py
+-rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.453391 django_restit-4.1.8/medialib/stores/oauth2client/file.py
+-rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.453451 django_restit-4.1.8/medialib/stores/oauth2client/gce.py
+-rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.453541 django_restit-4.1.8/medialib/stores/oauth2client/keyring_storage.py
+-rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.453634 django_restit-4.1.8/medialib/stores/oauth2client/locked_file.py
+-rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.453698 django_restit-4.1.8/medialib/stores/oauth2client/multistore_file.py
+-rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.453764 django_restit-4.1.8/medialib/stores/oauth2client/old_run.py
+-rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.453855 django_restit-4.1.8/medialib/stores/oauth2client/tools.py
+-rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.453938 django_restit-4.1.8/medialib/stores/oauth2client/util.py
+-rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.454013 django_restit-4.1.8/medialib/stores/oauth2client/xsrfutil.py
+-rw-r--r--   0        0        0      500 2023-06-27 05:37:44.454077 django_restit-4.1.8/medialib/stores/rtmpstore.py
+-rw-r--r--   0        0        0     4583 2023-06-27 05:37:44.454163 django_restit-4.1.8/medialib/stores/s3store.py
+-rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.454272 django_restit-4.1.8/medialib/stores/uritemplate/__init__.py
+-rw-r--r--   0        0        0      406 2023-06-27 05:37:44.454334 django_restit-4.1.8/medialib/stores/youtubestore.py
+-rw-r--r--   0        0        0     3691 2023-06-27 05:37:44.454500 django_restit-4.1.8/medialib/templates/medialib/base.html
+-rw-r--r--   0        0        0     1277 2023-06-27 05:37:44.454591 django_restit-4.1.8/medialib/templates/medialib/instances.html
+-rw-r--r--   0        0        0     1170 2023-06-27 05:37:44.454657 django_restit-4.1.8/medialib/templates/medialib/items.html
+-rw-r--r--   0        0        0     8194 2023-06-27 05:37:44.454746 django_restit-4.1.8/medialib/templates/medialib/library.html
+-rw-r--r--   0        0        0       65 2023-06-27 05:37:44.454810 django_restit-4.1.8/medialib/templates/medialib/notify_error.subject
+-rw-r--r--   0        0        0       49 2023-06-27 05:37:44.454869 django_restit-4.1.8/medialib/templates/medialib/notify_error.to
+-rw-r--r--   0        0        0      272 2023-06-27 05:37:44.454932 django_restit-4.1.8/medialib/templates/medialib/notify_error.txt
+-rw-r--r--   0        0        0       71 2023-06-27 05:37:44.454996 django_restit-4.1.8/medialib/templates/medialib/notify_ready.subject
+-rw-r--r--   0        0        0       49 2023-06-27 05:37:44.455056 django_restit-4.1.8/medialib/templates/medialib/notify_ready.to
+-rw-r--r--   0        0        0      298 2023-06-27 05:37:44.455113 django_restit-4.1.8/medialib/templates/medialib/notify_ready.txt
+-rw-r--r--   0        0        0       64 2023-06-27 05:37:44.455175 django_restit-4.1.8/medialib/templates/medialib/notify_render_error.subject
+-rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455232 django_restit-4.1.8/medialib/templates/medialib/notify_render_error.to
+-rw-r--r--   0        0        0      271 2023-06-27 05:37:44.455301 django_restit-4.1.8/medialib/templates/medialib/notify_render_error.txt
+-rw-r--r--   0        0        0       68 2023-06-27 05:37:44.455380 django_restit-4.1.8/medialib/templates/medialib/notify_validate_error.subject
+-rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455452 django_restit-4.1.8/medialib/templates/medialib/notify_validate_error.to
+-rw-r--r--   0        0        0      275 2023-06-27 05:37:44.455521 django_restit-4.1.8/medialib/templates/medialib/notify_validate_error.txt
+-rw-r--r--   0        0        0      206 2023-06-27 05:37:44.455593 django_restit-4.1.8/medialib/templates/medialib/smil
+-rw-r--r--   0        0        0     1177 2023-06-27 05:37:44.455665 django_restit-4.1.8/medialib/templates/medialib/test.html
+-rw-r--r--   0        0        0     1549 2023-06-27 05:37:44.455737 django_restit-4.1.8/medialib/templates/medialib/testpicker.html
+-rw-r--r--   0        0        0     6045 2023-06-27 05:37:44.455814 django_restit-4.1.8/medialib/tests.py
+-rw-r--r--   0        0        0      544 2023-06-27 05:37:44.455873 django_restit-4.1.8/medialib/tq.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.455894 django_restit-4.1.8/medialib/urls.py
+-rw-r--r--   0        0        0     3756 2023-06-27 05:37:44.455970 django_restit-4.1.8/medialib/utils.py
+-rw-r--r--   0        0        0     4321 2023-06-27 05:37:44.456050 django_restit-4.1.8/medialib/views.py
+-rw-r--r--   0        0        0     4303 2023-06-27 05:37:44.456166 django_restit-4.1.8/medialib/youtube/__init__.py
+-rw-r--r--   0        0        0      601 2023-06-27 05:37:44.456272 django_restit-4.1.8/medialib/youtube/apiclient/__init__.py
+-rw-r--r--   0        0        0     9886 2023-06-27 05:37:44.456332 django_restit-4.1.8/medialib/youtube/apiclient/channel.py
+-rw-r--r--   0        0        0    35907 2023-06-27 05:37:44.456516 django_restit-4.1.8/medialib/youtube/apiclient/discovery.py
+-rw-r--r--   0        0        0     3550 2023-06-27 05:37:44.456592 django_restit-4.1.8/medialib/youtube/apiclient/errors.py
+-rw-r--r--   0        0        0    52945 2023-06-27 05:37:44.456694 django_restit-4.1.8/medialib/youtube/apiclient/http.py
+-rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.456785 django_restit-4.1.8/medialib/youtube/apiclient/mimeparse.py
+-rw-r--r--   0        0        0    11795 2023-06-27 05:37:44.456835 django_restit-4.1.8/medialib/youtube/apiclient/model.py
+-rw-r--r--   0        0        0     3596 2023-06-27 05:37:44.456895 django_restit-4.1.8/medialib/youtube/apiclient/sample_tools.py
+-rw-r--r--   0        0        0     9327 2023-06-27 05:37:44.456959 django_restit-4.1.8/medialib/youtube/apiclient/schema.py
+-rw-r--r--   0        0        0    69581 2023-06-27 05:37:44.457093 django_restit-4.1.8/medialib/youtube/httplib2/__init__.py
+-rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.457310 django_restit-4.1.8/medialib/youtube/httplib2/cacerts.txt
+-rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.457412 django_restit-4.1.8/medialib/youtube/httplib2/iri2uri.py
+-rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.457533 django_restit-4.1.8/medialib/youtube/httplib2/socks.py
+-rw-r--r--   0        0        0      213 2023-06-27 05:37:44.457629 django_restit-4.1.8/medialib/youtube/oauth2client/__init__.py
+-rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.457687 django_restit-4.1.8/medialib/youtube/oauth2client/anyjson.py
+-rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.457830 django_restit-4.1.8/medialib/youtube/oauth2client/appengine.py
+-rw-r--r--   0        0        0    44431 2023-06-27 05:37:44.457905 django_restit-4.1.8/medialib/youtube/oauth2client/client.py
+-rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.457990 django_restit-4.1.8/medialib/youtube/oauth2client/clientsecrets.py
+-rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.458075 django_restit-4.1.8/medialib/youtube/oauth2client/crypt.py
+-rw-r--r--   0        0        0     3753 2023-06-27 05:37:44.458140 django_restit-4.1.8/medialib/youtube/oauth2client/django_orm.py
+-rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.458204 django_restit-4.1.8/medialib/youtube/oauth2client/file.py
+-rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.458255 django_restit-4.1.8/medialib/youtube/oauth2client/gce.py
+-rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.458323 django_restit-4.1.8/medialib/youtube/oauth2client/keyring_storage.py
+-rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.458399 django_restit-4.1.8/medialib/youtube/oauth2client/locked_file.py
+-rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.458454 django_restit-4.1.8/medialib/youtube/oauth2client/multistore_file.py
+-rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.458510 django_restit-4.1.8/medialib/youtube/oauth2client/old_run.py
+-rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.458604 django_restit-4.1.8/medialib/youtube/oauth2client/tools.py
+-rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.458680 django_restit-4.1.8/medialib/youtube/oauth2client/util.py
+-rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.458745 django_restit-4.1.8/medialib/youtube/oauth2client/xsrfutil.py
+-rw-r--r--   0        0        0     2849 2023-06-27 05:37:44.458806 django_restit-4.1.8/medialib/youtube/upload.py
+-rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.458902 django_restit-4.1.8/medialib/youtube/uritemplate/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-27 05:37:44.459001 django_restit-4.1.8/metrics/README.md
+-rw-r--r--   0        0        0       90 2023-06-27 05:37:44.459061 django_restit-4.1.8/metrics/__init__.py
+-rw-r--r--   0        0        0    23460 2023-06-27 05:37:44.459219 django_restit-4.1.8/metrics/client.py
+-rw-r--r--   0        0        0     9182 2023-06-27 05:37:44.459333 django_restit-4.1.8/metrics/eod.py
+-rw-r--r--   0        0        0     1664 2023-06-27 05:37:44.459430 django_restit-4.1.8/metrics/examples/eod_example.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459493 django_restit-4.1.8/metrics/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459564 django_restit-4.1.8/metrics/management/commands/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-27 05:37:44.459636 django_restit-4.1.8/metrics/management/commands/delete_gauge.py
+-rw-r--r--   0        0        0      464 2023-06-27 05:37:44.459697 django_restit-4.1.8/metrics/management/commands/delete_metric.py
+-rw-r--r--   0        0        0     2801 2023-06-27 05:37:44.459766 django_restit-4.1.8/metrics/management/commands/fix_redis_metrics_keys.py
+-rw-r--r--   0        0        0     1928 2023-06-27 05:37:44.459829 django_restit-4.1.8/metrics/management/commands/generate_test_metrics.py
+-rw-r--r--   0        0        0     1742 2023-06-27 05:37:44.459896 django_restit-4.1.8/metrics/management/commands/redis_metrics_send_mail.py
+-rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.459957 django_restit-4.1.8/metrics/management/commands/reset_weekly_metrics.py
+-rw-r--r--   0        0        0     4343 2023-06-27 05:37:44.460023 django_restit-4.1.8/metrics/management/commands/system_metric.py
+-rw-r--r--   0        0        0     2399 2023-06-27 05:37:44.460109 django_restit-4.1.8/metrics/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1510 2023-06-27 05:37:44.460172 django_restit-4.1.8/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py
+-rw-r--r--   0        0        0      453 2023-06-27 05:37:44.460231 django_restit-4.1.8/metrics/migrations/0003_metrics_expires.py
+-rw-r--r--   0        0        0     3271 2023-06-27 05:37:44.460284 django_restit-4.1.8/metrics/migrations/0004_eodmetrics.py
+-rw-r--r--   0        0        0     2358 2023-06-27 05:37:44.460347 django_restit-4.1.8/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460367 django_restit-4.1.8/metrics/migrations/__init__.py
+-rw-r--r--   0        0        0    11540 2023-07-14 20:40:49.561768 django_restit-4.1.8/metrics/models.py
+-rw-r--r--   0        0        0      480 2023-06-27 05:37:44.460528 django_restit-4.1.8/metrics/periodic.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460587 django_restit-4.1.8/metrics/providers/__init__.py
+-rw-r--r--   0        0        0     7335 2023-06-27 05:37:44.460691 django_restit-4.1.8/metrics/providers/aws.py
+-rw-r--r--   0        0        0    14827 2023-07-11 15:48:34.905677 django_restit-4.1.8/metrics/rpc.py
+-rw-r--r--   0        0        0      132 2023-06-27 05:37:44.460832 django_restit-4.1.8/metrics/settings.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460855 django_restit-4.1.8/metrics/tq.py
+-rw-r--r--   0        0        0    11508 2023-07-14 00:37:57.980977 django_restit-4.1.8/metrics/utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461016 django_restit-4.1.8/pushit/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-27 05:37:44.461079 django_restit-4.1.8/pushit/admin.py
+-rw-r--r--   0        0        0     4555 2023-06-27 05:37:44.461167 django_restit-4.1.8/pushit/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461190 django_restit-4.1.8/pushit/migrations/__init__.py
+-rw-r--r--   0        0        0     5066 2023-07-11 15:47:46.945937 django_restit-4.1.8/pushit/models.py
+-rw-r--r--   0        0        0       88 2023-06-27 05:37:44.461351 django_restit-4.1.8/pushit/rpc/__init__.py
+-rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.461414 django_restit-4.1.8/pushit/rpc/githooks.py
+-rw-r--r--   0        0        0     5028 2023-06-27 05:37:44.461473 django_restit-4.1.8/pushit/rpc/legacy.py
+-rw-r--r--   0        0        0      378 2023-06-27 05:37:44.461520 django_restit-4.1.8/pushit/rpc/products.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461605 django_restit-4.1.8/pushit/static/js/models_pushit.js
+-rw-r--r--   0        0        0      131 2023-06-27 05:37:44.461676 django_restit-4.1.8/pushit/tq.py
+-rw-r--r--   0        0        0     1966 2023-06-27 05:37:44.461734 django_restit-4.1.8/pushit/utils.py
+-rw-r--r--   0        0        0     1167 2023-07-17 18:51:59.744740 django_restit-4.1.8/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-06-27 05:37:44.461884 django_restit-4.1.8/rest/.gitignore
+-rw-r--r--   0        0        0     5460 2023-06-27 05:37:44.461959 django_restit-4.1.8/rest/README.md
+-rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462010 django_restit-4.1.8/rest/RemoteEvents.py
+-rw-r--r--   0        0        0      120 2023-07-17 18:51:59.769118 django_restit-4.1.8/rest/__init__.py
+-rw-r--r--   0        0        0     1967 2023-06-27 05:37:44.462114 django_restit-4.1.8/rest/arc4.py
+-rw-r--r--   0        0        0       83 2023-06-27 05:37:44.462161 django_restit-4.1.8/rest/cache.py
+-rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462295 django_restit-4.1.8/rest/crypto/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-27 05:37:44.462374 django_restit-4.1.8/rest/crypto/aes.py
+-rw-r--r--   0        0        0     4082 2023-06-27 05:37:44.462442 django_restit-4.1.8/rest/crypto/privpub.py
+-rw-r--r--   0        0        0     4514 2023-07-11 15:29:38.508089 django_restit-4.1.8/rest/crypto/util.py
+-rw-r--r--   0        0        0     7548 2023-07-12 19:54:30.986685 django_restit-4.1.8/rest/datem.py
+-rw-r--r--   0        0        0    15590 2023-07-17 18:49:05.153834 django_restit-4.1.8/rest/decorators.py
+-rw-r--r--   0        0        0      788 2023-06-27 05:37:44.462816 django_restit-4.1.8/rest/encryption.py
+-rw-r--r--   0        0        0      501 2023-07-11 15:16:32.180675 django_restit-4.1.8/rest/errors.py
+-rw-r--r--   0        0        0       54 2023-06-27 05:37:44.462913 django_restit-4.1.8/rest/extra/__init__.py
+-rw-r--r--   0        0        0     1078 2023-06-27 05:37:44.462982 django_restit-4.1.8/rest/extra/json_metadata.py
+-rw-r--r--   0        0        0     9719 2023-06-27 05:37:44.463072 django_restit-4.1.8/rest/fields.py
+-rw-r--r--   0        0        0     6316 2023-06-27 05:37:44.463145 django_restit-4.1.8/rest/forms.py
+-rw-r--r--   0        0        0    24650 2023-07-11 15:25:55.654664 django_restit-4.1.8/rest/helpers.py
+-rw-r--r--   0        0        0      260 2023-06-27 05:37:44.463338 django_restit-4.1.8/rest/joke.py
+-rw-r--r--   0        0        0     2298 2023-06-27 05:37:44.463411 django_restit-4.1.8/rest/jwtoken.py
+-rw-r--r--   0        0        0    20930 2023-06-27 15:33:50.289063 django_restit-4.1.8/rest/log.py
+-rw-r--r--   0        0        0     7754 2023-06-27 05:37:44.463623 django_restit-4.1.8/rest/mail.py
+-rw-r--r--   0        0        0     9174 2023-06-27 05:37:44.463711 django_restit-4.1.8/rest/mailman.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463776 django_restit-4.1.8/rest/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463861 django_restit-4.1.8/rest/management/commands/__init__.py
+-rw-r--r--   0        0        0      389 2023-06-27 05:37:44.463942 django_restit-4.1.8/rest/management/commands/rpc.py
+-rw-r--r--   0        0        0       33 2023-06-27 05:37:44.464028 django_restit-4.1.8/rest/middleware/__init__.py
+-rw-r--r--   0        0        0     3513 2023-06-27 05:37:44.464096 django_restit-4.1.8/rest/middleware/cors.py
+-rw-r--r--   0        0        0     2345 2023-06-27 05:37:44.464159 django_restit-4.1.8/rest/middleware/db_router.py
+-rw-r--r--   0        0        0     5395 2023-06-27 05:37:44.464226 django_restit-4.1.8/rest/middleware/jwt.py
+-rw-r--r--   0        0        0     4127 2023-06-27 05:37:44.464313 django_restit-4.1.8/rest/middleware/request.py
+-rw-r--r--   0        0        0     9015 2023-06-27 05:37:44.464386 django_restit-4.1.8/rest/middleware/session.py
+-rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.464450 django_restit-4.1.8/rest/middleware/session_store.py
+-rw-r--r--   0        0        0      130 2023-07-11 15:56:36.722347 django_restit-4.1.8/rest/models/__init__.py
+-rw-r--r--   0        0        0    62288 2023-07-12 19:45:09.742630 django_restit-4.1.8/rest/models/base.py
+-rw-r--r--   0        0        0      578 2023-07-11 16:03:40.953305 django_restit-4.1.8/rest/models/cacher.py
+-rw-r--r--   0        0        0    11894 2023-07-17 18:46:38.869722 django_restit-4.1.8/rest/models/metadata.py
+-rw-r--r--   0        0        0   149463 2023-06-27 05:37:44.465139 django_restit-4.1.8/rest/regexes.yaml
+-rw-r--r--   0        0        0    15248 2023-07-11 22:23:29.744915 django_restit-4.1.8/rest/requestex.py
+-rw-r--r--   0        0        0     3713 2023-06-27 15:25:34.225162 django_restit-4.1.8/rest/rpc.py
+-rw-r--r--   0        0        0     7645 2023-06-27 05:37:44.465350 django_restit-4.1.8/rest/search.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.465410 django_restit-4.1.8/rest/serializers/__init__.py
+-rw-r--r--   0        0        0     2015 2023-07-12 03:00:36.470673 django_restit-4.1.8/rest/serializers/collection.py
+-rw-r--r--   0        0        0     2975 2023-06-27 05:37:44.465556 django_restit-4.1.8/rest/serializers/csv.py
+-rw-r--r--   0        0        0     1077 2023-06-27 05:37:44.465616 django_restit-4.1.8/rest/serializers/excel.py
+-rw-r--r--   0        0        0     1736 2023-06-27 05:37:44.465675 django_restit-4.1.8/rest/serializers/json.py
+-rw-r--r--   0        0        0    61795 2023-07-11 16:27:26.664542 django_restit-4.1.8/rest/serializers/legacy.py
+-rw-r--r--   0        0        0     7320 2023-07-14 00:32:10.541201 django_restit-4.1.8/rest/serializers/model.py
+-rw-r--r--   0        0        0      997 2023-07-06 18:50:18.372944 django_restit-4.1.8/rest/serializers/profiler.py
+-rw-r--r--   0        0        0     6509 2023-07-11 20:46:40.798160 django_restit-4.1.8/rest/serializers/response.py
+-rw-r--r--   0        0        0     2734 2023-06-27 05:37:44.466139 django_restit-4.1.8/rest/serializers/util.py
+-rw-r--r--   0        0        0     1532 2023-06-27 05:37:44.466216 django_restit-4.1.8/rest/settings_helper.py
+-rw-r--r--   0        0        0    95786 2023-06-27 05:37:44.466685 django_restit-4.1.8/rest/static/lib/jquery.js
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466742 django_restit-4.1.8/rest/static/rest/app.css
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466776 django_restit-4.1.8/rest/static/rest/app.js
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466808 django_restit-4.1.8/rest/static/rest/rest.js
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466846 django_restit-4.1.8/rest/static/rest/rest.scss
+-rw-r--r--   0        0        0      529 2023-06-27 05:37:44.466992 django_restit-4.1.8/rest/templates/email/error.html
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.467020 django_restit-4.1.8/rest/templates/email/error.subject
+-rw-r--r--   0        0        0     7148 2023-06-27 05:37:44.467101 django_restit-4.1.8/rest/templates/rest_docs.html
+-rw-r--r--   0        0        0    10880 2023-06-27 05:37:44.467182 django_restit-4.1.8/rest/templates/rest_html.html
+-rw-r--r--   0        0        0   185122 2023-06-27 05:37:44.467607 django_restit-4.1.8/rest/ua.py
+-rw-r--r--   0        0        0    17064 2023-06-27 05:37:44.467734 django_restit-4.1.8/rest/uberdict.py
+-rw-r--r--   0        0        0    11881 2023-06-27 05:37:44.467820 django_restit-4.1.8/rest/url_docs.py
+-rw-r--r--   0        0        0     1787 2023-06-27 05:37:44.467877 django_restit-4.1.8/rest/urls.py
+-rw-r--r--   0        0        0     1056 2023-06-27 05:37:44.467929 django_restit-4.1.8/rest/views.py
+-rw-r--r--   0        0        0      118 2023-06-27 05:37:44.468007 django_restit-4.1.8/sessionlog/.gitignore
+-rw-r--r--   0        0        0       62 2023-06-27 05:37:44.468062 django_restit-4.1.8/sessionlog/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468086 django_restit-4.1.8/sessionlog/__init__.py
+-rw-r--r--   0        0        0      245 2023-06-27 05:37:44.468153 django_restit-4.1.8/sessionlog/admin.py
+-rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.468231 django_restit-4.1.8/sessionlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468261 django_restit-4.1.8/sessionlog/migrations/__init__.py
+-rw-r--r--   0        0        0     3978 2023-07-05 22:43:30.431976 django_restit-4.1.8/sessionlog/models.py
+-rw-r--r--   0        0        0      383 2023-06-27 05:37:44.468400 django_restit-4.1.8/sessionlog/tests.py
+-rw-r--r--   0        0        0       26 2023-06-27 05:37:44.468451 django_restit-4.1.8/sessionlog/views.py
+-rw-r--r--   0        0        0     2196 2023-06-27 05:37:44.468543 django_restit-4.1.8/taskqueue/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468569 django_restit-4.1.8/taskqueue/__init__.py
+-rw-r--r--   0        0        0      208 2023-06-27 05:37:44.468635 django_restit-4.1.8/taskqueue/admin.py
+-rw-r--r--   0        0        0     4738 2023-06-27 05:37:44.468730 django_restit-4.1.8/taskqueue/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468758 django_restit-4.1.8/taskqueue/migrations/__init__.py
+-rw-r--r--   0        0        0    16531 2023-06-27 05:37:44.468876 django_restit-4.1.8/taskqueue/models.py
+-rw-r--r--   0        0        0     3072 2023-06-27 05:37:44.468952 django_restit-4.1.8/taskqueue/periodic.py
+-rw-r--r--   0        0        0     5326 2023-06-27 05:37:44.469019 django_restit-4.1.8/taskqueue/rpc.py
+-rw-r--r--   0        0        0      942 2023-06-27 05:37:44.469073 django_restit-4.1.8/taskqueue/tq.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469126 django_restit-4.1.8/taskqueue/transports/__init__.py
+-rw-r--r--   0        0        0      623 2023-06-27 05:37:44.469185 django_restit-4.1.8/taskqueue/transports/email.py
+-rw-r--r--   0        0        0     2409 2023-06-27 05:37:44.469240 django_restit-4.1.8/taskqueue/transports/http.py
+-rw-r--r--   0        0        0     1099 2023-06-27 05:37:44.469291 django_restit-4.1.8/taskqueue/transports/s3.py
+-rw-r--r--   0        0        0     1891 2023-06-27 05:37:44.469341 django_restit-4.1.8/taskqueue/transports/sftp.py
+-rw-r--r--   0        0        0      142 2023-06-27 05:37:44.469388 django_restit-4.1.8/taskqueue/transports/sms.py
+-rw-r--r--   0        0        0    13660 2023-06-27 05:37:44.469465 django_restit-4.1.8/taskqueue/worker.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469517 django_restit-4.1.8/telephony/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-27 05:37:44.469571 django_restit-4.1.8/telephony/admin.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469591 django_restit-4.1.8/telephony/decorators.py
+-rw-r--r--   0        0        0     3030 2023-06-27 05:37:44.469692 django_restit-4.1.8/telephony/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469714 django_restit-4.1.8/telephony/migrations/__init__.py
+-rw-r--r--   0        0        0     7753 2023-06-27 05:37:44.469796 django_restit-4.1.8/telephony/models.py
+-rw-r--r--   0        0        0     2126 2023-06-27 05:37:44.469861 django_restit-4.1.8/telephony/phone_util.py
+-rw-r--r--   0        0        0     2659 2023-06-27 05:37:44.469923 django_restit-4.1.8/telephony/rpc.py
+-rw-r--r--   0        0        0     3624 2023-06-27 05:37:44.470008 django_restit-4.1.8/ws4redis/README.md
+-rwxr-xr-x   0        0        0       46 2023-06-27 05:37:44.470065 django_restit-4.1.8/ws4redis/__init__.py
+-rw-r--r--   0        0        0     4942 2023-06-27 05:37:44.470133 django_restit-4.1.8/ws4redis/client.py
+-rw-r--r--   0        0        0    13110 2023-07-08 23:34:53.804529 django_restit-4.1.8/ws4redis/connection.py
+-rwxr-xr-x   0        0        0      636 2023-06-27 05:37:44.470295 django_restit-4.1.8/ws4redis/exceptions.py
+-rw-r--r--   0        0        0     5561 2023-07-08 23:30:25.146274 django_restit-4.1.8/ws4redis/redis.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.470422 django_restit-4.1.8/ws4redis/servers/__init__.py
+-rw-r--r--   0        0        0     3747 2023-06-27 05:37:44.470507 django_restit-4.1.8/ws4redis/servers/base.py
+-rw-r--r--   0        0        0     4329 2023-06-27 05:37:44.470582 django_restit-4.1.8/ws4redis/servers/django.py
+-rw-r--r--   0        0        0     1723 2023-06-27 05:37:44.470638 django_restit-4.1.8/ws4redis/servers/uwsgi.py
+-rwxr-xr-x   0        0        0     1411 2023-06-27 05:37:44.470697 django_restit-4.1.8/ws4redis/settings.py
+-rwxr-xr-x   0        0        0     5122 2023-06-27 05:37:44.470772 django_restit-4.1.8/ws4redis/utf8validator.py
+-rwxr-xr-x   0        0        0    14848 2023-06-27 05:37:44.470868 django_restit-4.1.8/ws4redis/websocket.py
+-rw-r--r--   0        0        0     7531 1970-01-01 00:00:00.000000 django_restit-4.1.8/PKG-INFO
```

### Comparing `django_restit-4.1.7/LICENSE.md` & `django_restit-4.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/README.md` & `django_restit-4.1.8/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/admin.py` & `django_restit-4.1.8/account/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/fcm/__init__.py` & `django_restit-4.1.8/account/fcm/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/migrations/0001_initial.py` & `django_restit-4.1.8/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/migrations/0003_member_phone_number.py` & `django_restit-4.1.8/account/migrations/0003_member_phone_number.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/migrations/0004_group_modified_alter_group_created.py` & `django_restit-4.1.8/account/migrations/0004_group_modified_alter_group_created.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/migrations/0007_authtoken_signature_authsession.py` & `django_restit-4.1.8/account/migrations/0007_authtoken_signature_authsession.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/migrations/0008_memberdevice_memberdevicemetadata.py` & `django_restit-4.1.8/account/migrations/0008_memberdevice_memberdevicemetadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/migrations/0011_authtoken.py` & `django_restit-4.1.8/account/migrations/0011_authtoken.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/migrations/0012_settings_settingsmetadata.py` & `django_restit-4.1.8/account/migrations/0012_settings_settingsmetadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/models/device.py` & `django_restit-4.1.8/account/models/device.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/models/feeds.py` & `django_restit-4.1.8/account/models/feeds.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/models/group.py` & `django_restit-4.1.8/account/models/group.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/models/legacy.py` & `django_restit-4.1.8/account/models/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/models/member.py` & `django_restit-4.1.8/account/models/member.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,14 +508,16 @@
         NotificationRecord = RestModel.getModel("account", "NotificationRecord")
         NotificationRecord.notify(
             [self], subject=subject, message=body,
             template=template, context=context,
             email_only=True, attachments=attachments)
 
     def sendInvite(self, subject, group=None, url=None, msg=None, **kwargs):
+        if url[:4] != "http":
+            url = f"https://{url}"
         context = rh.getContext(
             self.getActiveRequest(),
             member=self,
             group=group,
             url=url,
             msg=msg, **kwargs)
         rest_mail.send(self.email, subject, template=settings.get("EMAIL_TEMPLATE_INVITE", "email/invite.html"), context=context)
```

### Comparing `django_restit-4.1.7/account/models/membership.py` & `django_restit-4.1.8/account/models/membership.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/models/notify.py` & `django_restit-4.1.8/account/models/notify.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/models/session.py` & `django_restit-4.1.8/account/models/session.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/models/settings.py` & `django_restit-4.1.8/account/models/settings.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/oauth/google.py` & `django_restit-4.1.8/account/oauth/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/periodic.py` & `django_restit-4.1.8/account/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/rpc/auth.py` & `django_restit-4.1.8/account/rpc/auth.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/rpc/device.py` & `django_restit-4.1.8/account/rpc/device.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/rpc/group.py` & `django_restit-4.1.8/account/rpc/group.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/rpc/member.py` & `django_restit-4.1.8/account/rpc/member.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/rpc/notify.py` & `django_restit-4.1.8/account/rpc/notify.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/rpc/oauth.py` & `django_restit-4.1.8/account/rpc/oauth.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/templates/email/base.html` & `django_restit-4.1.8/account/templates/email/base.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/templates/email/invite.html` & `django_restit-4.1.8/account/templates/email/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/templates/email/plain/invite.html` & `django_restit-4.1.8/account/templates/email/plain/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/templates/email/plain/reset_code.html` & `django_restit-4.1.8/account/templates/email/plain/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/templates/email/reset_code.html` & `django_restit-4.1.8/account/templates/email/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/templates/email/simple/invite.html` & `django_restit-4.1.8/account/templates/email/simple/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/account/templates/email/simple/reset_code.html` & `django_restit-4.1.8/account/templates/email/simple/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/auditlog/README` & `django_restit-4.1.8/auditlog/README`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/auditlog/admin.py` & `django_restit-4.1.8/auditlog/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/auditlog/decorators.py` & `django_restit-4.1.8/auditlog/decorators.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/auditlog/middleware.py` & `django_restit-4.1.8/auditlog/middleware.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/auditlog/migrations/0001_initial.py` & `django_restit-4.1.8/auditlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/auditlog/models.py` & `django_restit-4.1.8/auditlog/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/auditlog/rpc.py` & `django_restit-4.1.8/auditlog/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/auditlog/tq.py` & `django_restit-4.1.8/auditlog/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/inbox/README.md` & `django_restit-4.1.8/inbox/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/inbox/handlers.py` & `django_restit-4.1.8/inbox/handlers.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/inbox/migrations/0001_initial.py` & `django_restit-4.1.8/inbox/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/inbox/migrations/0004_mailtemplate.py` & `django_restit-4.1.8/inbox/migrations/0004_mailtemplate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/inbox/models/bounce.py` & `django_restit-4.1.8/inbox/models/bounce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/inbox/models/complaint.py` & `django_restit-4.1.8/inbox/models/complaint.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/inbox/models/message.py` & `django_restit-4.1.8/inbox/models/message.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/inbox/models/template.py` & `django_restit-4.1.8/inbox/models/template.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/inbox/rpc.py` & `django_restit-4.1.8/inbox/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/inbox/utils/parsing.py` & `django_restit-4.1.8/inbox/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/inbox/utils/render.py` & `django_restit-4.1.8/inbox/utils/render.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/inbox/utils/sending.py` & `django_restit-4.1.8/inbox/utils/sending.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/README.md` & `django_restit-4.1.8/incident/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/__init__.py` & `django_restit-4.1.8/incident/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/migrations/0001_initial.py` & `django_restit-4.1.8/incident/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/migrations/0002_event_component_event_component_id.py` & `django_restit-4.1.8/incident/migrations/0002_event_component_event_component_id.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py` & `django_restit-4.1.8/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/migrations/0005_incident_component_alter_incident_state.py` & `django_restit-4.1.8/incident/migrations/0005_incident_component_alter_incident_state.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py` & `django_restit-4.1.8/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/models/event.py` & `django_restit-4.1.8/incident/models/event.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/models/incident.py` & `django_restit-4.1.8/incident/models/incident.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/models/ossec.py` & `django_restit-4.1.8/incident/models/ossec.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/models/rules.py` & `django_restit-4.1.8/incident/models/rules.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/parsers/ossec.py` & `django_restit-4.1.8/incident/parsers/ossec.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/periodic.py` & `django_restit-4.1.8/incident/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/rpc.py` & `django_restit-4.1.8/incident/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/templates/email/incident_change.html` & `django_restit-4.1.8/incident/templates/email/incident_change.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/templates/email/incident_new.html` & `django_restit-4.1.8/incident/templates/email/incident_new.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/templates/email/incident_plain.html` & `django_restit-4.1.8/incident/templates/email/incident_plain.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/incident/tq.py` & `django_restit-4.1.8/incident/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/geolocate.py` & `django_restit-4.1.8/location/geolocate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/migrations/0001_initial.py` & `django_restit-4.1.8/location/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/migrations/0002_geoip_subnet_alter_geoip_ip.py` & `django_restit-4.1.8/location/migrations/0002_geoip_subnet_alter_geoip_ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/models/address.py` & `django_restit-4.1.8/location/models/address.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/models/ip.py` & `django_restit-4.1.8/location/models/ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/models/legacy.py` & `django_restit-4.1.8/location/models/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/models/location.py` & `django_restit-4.1.8/location/models/location.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/models/track.py` & `django_restit-4.1.8/location/models/track.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/providers/iplookup/__init__.py` & `django_restit-4.1.8/location/providers/iplookup/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/providers/iplookup/abstractapi.py` & `django_restit-4.1.8/location/providers/iplookup/abstractapi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/providers/iplookup/extremeip.py` & `django_restit-4.1.8/location/providers/iplookup/extremeip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/providers/iplookup/geoplugin.py` & `django_restit-4.1.8/location/providers/iplookup/geoplugin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/providers/iplookup/ipapi.py` & `django_restit-4.1.8/location/providers/iplookup/ipapi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/providers/iplookup/ipinfo.py` & `django_restit-4.1.8/location/providers/iplookup/ipinfo.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/providers/iplookup/restit.py` & `django_restit-4.1.8/location/providers/iplookup/restit.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/providers/location/google.py` & `django_restit-4.1.8/location/providers/location/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/providers/timezones/google.py` & `django_restit-4.1.8/location/providers/timezones/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/providers/zillow.py` & `django_restit-4.1.8/location/providers/zillow.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/rpc/ip.py` & `django_restit-4.1.8/location/rpc/ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/rpc/location.py` & `django_restit-4.1.8/location/rpc/location.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/location/rpc/track.py` & `django_restit-4.1.8/location/rpc/track.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/admin.py` & `django_restit-4.1.8/medialib/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/cvutil/contours.py` & `django_restit-4.1.8/medialib/cvutil/contours.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/cvutil/images.py` & `django_restit-4.1.8/medialib/cvutil/images.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/cvutil/misc.py` & `django_restit-4.1.8/medialib/cvutil/misc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/cvutil/text.py` & `django_restit-4.1.8/medialib/cvutil/text.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/fixtures/initial_data.json` & `django_restit-4.1.8/medialib/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/fixtures/medialib.json` & `django_restit-4.1.8/medialib/fixtures/medialib.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/fixtures/medialib_test_fixture.json` & `django_restit-4.1.8/medialib/fixtures/medialib_test_fixture.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/forms.py` & `django_restit-4.1.8/medialib/forms.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/migrations/0001_initial.py` & `django_restit-4.1.8/medialib/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/models.py` & `django_restit-4.1.8/medialib/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/ocr.py` & `django_restit-4.1.8/medialib/ocr.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/pdf.py` & `django_restit-4.1.8/medialib/pdf.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/qrcode.py` & `django_restit-4.1.8/medialib/qrcode.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/__init__.py` & `django_restit-4.1.8/medialib/render/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/engines/anigif.py` & `django_restit-4.1.8/medialib/render/engines/anigif.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/engines/ffmpeg.py` & `django_restit-4.1.8/medialib/render/engines/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/engines/gifsicle.py` & `django_restit-4.1.8/medialib/render/engines/gifsicle.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/engines/hls.py` & `django_restit-4.1.8/medialib/render/engines/hls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/engines/mp4box.py` & `django_restit-4.1.8/medialib/render/engines/mp4box.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/engines/rtmp/rtmp.i` & `django_restit-4.1.8/medialib/render/engines/rtmp/rtmp.i`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/engines/rtmpdump.py` & `django_restit-4.1.8/medialib/render/engines/rtmpdump.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/engines/rtmpsink.py` & `django_restit-4.1.8/medialib/render/engines/rtmpsink.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/engines/video_getinfo.py` & `django_restit-4.1.8/medialib/render/engines/video_getinfo.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/engines/websnap.py` & `django_restit-4.1.8/medialib/render/engines/websnap.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/exceptions.py` & `django_restit-4.1.8/medialib/render/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/presets/akamai.py` & `django_restit-4.1.8/medialib/render/presets/akamai.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/presets/animated_thumbnail.py` & `django_restit-4.1.8/medialib/render/presets/animated_thumbnail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/presets/ffmpeg.py` & `django_restit-4.1.8/medialib/render/presets/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/presets/flv.py` & `django_restit-4.1.8/medialib/render/presets/flv.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/presets/hls.py` & `django_restit-4.1.8/medialib/render/presets/hls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/presets/image_transcode.py` & `django_restit-4.1.8/medialib/render/presets/image_transcode.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/presets/image_validate.py` & `django_restit-4.1.8/medialib/render/presets/image_validate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/presets/mp4.py` & `django_restit-4.1.8/medialib/render/presets/mp4.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/presets/video_still.py` & `django_restit-4.1.8/medialib/render/presets/video_still.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/presets/video_validate.py` & `django_restit-4.1.8/medialib/render/presets/video_validate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/presets/websnap.py` & `django_restit-4.1.8/medialib/render/presets/websnap.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/presets/youtube.py` & `django_restit-4.1.8/medialib/render/presets/youtube.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/render/render_utils.py` & `django_restit-4.1.8/medialib/render/render_utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/rpc/legacy.py` & `django_restit-4.1.8/medialib/rpc/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/rpc/media.py` & `django_restit-4.1.8/medialib/rpc/media.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/rpc/tools.py` & `django_restit-4.1.8/medialib/rpc/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/scripts/init_config` & `django_restit-4.1.8/medialib/scripts/init_config`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/css/base_medialibui.css` & `django_restit-4.1.8/medialib/static/css/base_medialibui.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/css/base_widgets.css` & `django_restit-4.1.8/medialib/static/css/base_widgets.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/css/jquery.jcrop.css` & `django_restit-4.1.8/medialib/static/css/jquery.jcrop.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/img/bg-body.gif` & `django_restit-4.1.8/medialib/static/img/bg-body.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/img/loading.gif` & `django_restit-4.1.8/medialib/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/img/noimage.gif` & `django_restit-4.1.8/medialib/static/img/noimage.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/img/render_err.gif` & `django_restit-4.1.8/medialib/static/img/render_err.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/img/rendering.gif` & `django_restit-4.1.8/medialib/static/img/rendering.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/img/unknown.gif` & `django_restit-4.1.8/medialib/static/img/unknown.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/lib/caman.full.js` & `django_restit-4.1.8/medialib/static/lib/caman.full.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/lib/hammer.min.js` & `django_restit-4.1.8/medialib/static/lib/hammer.min.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/lib/jquery.Jcrop.js` & `django_restit-4.1.8/medialib/static/lib/jquery.Jcrop.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/lib/jquery.hammer.js` & `django_restit-4.1.8/medialib/static/lib/jquery.hammer.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/lib/load-image.min.js` & `django_restit-4.1.8/medialib/static/lib/load-image.min.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/lib/swiper.js` & `django_restit-4.1.8/medialib/static/lib/swiper.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js` & `django_restit-4.1.8/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js` & `django_restit-4.1.8/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js` & `django_restit-4.1.8/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/static/lib/tinymce/plugins/medialib/medialib.html` & `django_restit-4.1.8/medialib/static/lib/tinymce/plugins/medialib/medialib.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/__init__.py` & `django_restit-4.1.8/medialib/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/apiclient/__init__.py` & `django_restit-4.1.8/medialib/stores/apiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/apiclient/channel.py` & `django_restit-4.1.8/medialib/stores/apiclient/channel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/apiclient/discovery.py` & `django_restit-4.1.8/medialib/stores/apiclient/discovery.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/apiclient/errors.py` & `django_restit-4.1.8/medialib/stores/apiclient/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/apiclient/http.py` & `django_restit-4.1.8/medialib/stores/apiclient/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/apiclient/mimeparse.py` & `django_restit-4.1.8/medialib/stores/apiclient/mimeparse.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/apiclient/model.py` & `django_restit-4.1.8/medialib/stores/apiclient/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/apiclient/sample_tools.py` & `django_restit-4.1.8/medialib/stores/apiclient/sample_tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/apiclient/schema.py` & `django_restit-4.1.8/medialib/stores/apiclient/schema.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/filestore.py` & `django_restit-4.1.8/medialib/stores/filestore.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/httplib2/__init__.py` & `django_restit-4.1.8/medialib/stores/httplib2/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/httplib2/cacerts.txt` & `django_restit-4.1.8/medialib/stores/httplib2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/httplib2/iri2uri.py` & `django_restit-4.1.8/medialib/stores/httplib2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/httplib2/socks.py` & `django_restit-4.1.8/medialib/stores/httplib2/socks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/httpstore.py` & `django_restit-4.1.8/medialib/stores/httpstore.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/anyjson.py` & `django_restit-4.1.8/medialib/stores/oauth2client/anyjson.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/appengine.py` & `django_restit-4.1.8/medialib/stores/oauth2client/appengine.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/client.py` & `django_restit-4.1.8/medialib/stores/oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/clientsecrets.py` & `django_restit-4.1.8/medialib/stores/oauth2client/clientsecrets.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/crypt.py` & `django_restit-4.1.8/medialib/stores/oauth2client/crypt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/django_orm.py` & `django_restit-4.1.8/medialib/stores/oauth2client/django_orm.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/file.py` & `django_restit-4.1.8/medialib/stores/oauth2client/file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/gce.py` & `django_restit-4.1.8/medialib/stores/oauth2client/gce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/keyring_storage.py` & `django_restit-4.1.8/medialib/stores/oauth2client/keyring_storage.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/locked_file.py` & `django_restit-4.1.8/medialib/stores/oauth2client/locked_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/multistore_file.py` & `django_restit-4.1.8/medialib/stores/oauth2client/multistore_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/old_run.py` & `django_restit-4.1.8/medialib/stores/oauth2client/old_run.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/tools.py` & `django_restit-4.1.8/medialib/stores/oauth2client/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/util.py` & `django_restit-4.1.8/medialib/stores/oauth2client/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/oauth2client/xsrfutil.py` & `django_restit-4.1.8/medialib/stores/oauth2client/xsrfutil.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/s3store.py` & `django_restit-4.1.8/medialib/stores/s3store.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/stores/uritemplate/__init__.py` & `django_restit-4.1.8/medialib/stores/uritemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/templates/medialib/base.html` & `django_restit-4.1.8/medialib/templates/medialib/base.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/templates/medialib/instances.html` & `django_restit-4.1.8/medialib/templates/medialib/instances.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/templates/medialib/items.html` & `django_restit-4.1.8/medialib/templates/medialib/items.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/templates/medialib/library.html` & `django_restit-4.1.8/medialib/templates/medialib/library.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/templates/medialib/test.html` & `django_restit-4.1.8/medialib/templates/medialib/test.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/templates/medialib/testpicker.html` & `django_restit-4.1.8/medialib/templates/medialib/testpicker.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/tests.py` & `django_restit-4.1.8/medialib/tests.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/tq.py` & `django_restit-4.1.8/medialib/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/utils.py` & `django_restit-4.1.8/medialib/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/views.py` & `django_restit-4.1.8/medialib/views.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/__init__.py` & `django_restit-4.1.8/medialib/youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/apiclient/__init__.py` & `django_restit-4.1.8/medialib/youtube/apiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/apiclient/channel.py` & `django_restit-4.1.8/medialib/youtube/apiclient/channel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/apiclient/discovery.py` & `django_restit-4.1.8/medialib/youtube/apiclient/discovery.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/apiclient/errors.py` & `django_restit-4.1.8/medialib/youtube/apiclient/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/apiclient/http.py` & `django_restit-4.1.8/medialib/youtube/apiclient/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/apiclient/mimeparse.py` & `django_restit-4.1.8/medialib/youtube/apiclient/mimeparse.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/apiclient/model.py` & `django_restit-4.1.8/medialib/youtube/apiclient/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/apiclient/sample_tools.py` & `django_restit-4.1.8/medialib/youtube/apiclient/sample_tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/apiclient/schema.py` & `django_restit-4.1.8/medialib/youtube/apiclient/schema.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/httplib2/__init__.py` & `django_restit-4.1.8/medialib/youtube/httplib2/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/httplib2/cacerts.txt` & `django_restit-4.1.8/medialib/youtube/httplib2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/httplib2/iri2uri.py` & `django_restit-4.1.8/medialib/youtube/httplib2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/httplib2/socks.py` & `django_restit-4.1.8/medialib/youtube/httplib2/socks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/anyjson.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/anyjson.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/appengine.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/appengine.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/client.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/clientsecrets.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/clientsecrets.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/crypt.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/crypt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/django_orm.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/django_orm.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/file.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/gce.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/gce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/keyring_storage.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/keyring_storage.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/locked_file.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/locked_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/multistore_file.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/multistore_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/old_run.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/old_run.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/tools.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/util.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/oauth2client/xsrfutil.py` & `django_restit-4.1.8/medialib/youtube/oauth2client/xsrfutil.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/upload.py` & `django_restit-4.1.8/medialib/youtube/upload.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/medialib/youtube/uritemplate/__init__.py` & `django_restit-4.1.8/medialib/youtube/uritemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/README.md` & `django_restit-4.1.8/metrics/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/client.py` & `django_restit-4.1.8/metrics/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/eod.py` & `django_restit-4.1.8/metrics/eod.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/examples/eod_example.py` & `django_restit-4.1.8/metrics/examples/eod_example.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/management/commands/fix_redis_metrics_keys.py` & `django_restit-4.1.8/metrics/management/commands/fix_redis_metrics_keys.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/management/commands/generate_test_metrics.py` & `django_restit-4.1.8/metrics/management/commands/generate_test_metrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/management/commands/redis_metrics_send_mail.py` & `django_restit-4.1.8/metrics/management/commands/redis_metrics_send_mail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/management/commands/reset_weekly_metrics.py` & `django_restit-4.1.8/metrics/management/commands/reset_weekly_metrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/management/commands/system_metric.py` & `django_restit-4.1.8/metrics/management/commands/system_metric.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/migrations/0001_initial.py` & `django_restit-4.1.8/metrics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py` & `django_restit-4.1.8/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/migrations/0004_eodmetrics.py` & `django_restit-4.1.8/metrics/migrations/0004_eodmetrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py` & `django_restit-4.1.8/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/models.py` & `django_restit-4.1.8/metrics/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/providers/aws.py` & `django_restit-4.1.8/metrics/providers/aws.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/rpc.py` & `django_restit-4.1.8/metrics/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/metrics/utils.py` & `django_restit-4.1.8/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/pushit/migrations/0001_initial.py` & `django_restit-4.1.8/pushit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/pushit/models.py` & `django_restit-4.1.8/pushit/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/pushit/rpc/githooks.py` & `django_restit-4.1.8/pushit/rpc/githooks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/pushit/rpc/legacy.py` & `django_restit-4.1.8/pushit/rpc/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/pushit/utils.py` & `django_restit-4.1.8/pushit/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/pyproject.toml` & `django_restit-4.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-restit"
-version = "4.1.7"
+version = "4.1.8"
 description = "A Rest Framework for DJANGO"
 authors = ["Ian Starnes <ians@311labs.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     {include = "account"},
```

### Comparing `django_restit-4.1.7/rest/README.md` & `django_restit-4.1.8/rest/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/arc4.py` & `django_restit-4.1.8/rest/arc4.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/crypto/aes.py` & `django_restit-4.1.8/rest/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/crypto/privpub.py` & `django_restit-4.1.8/rest/crypto/privpub.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/crypto/util.py` & `django_restit-4.1.8/rest/crypto/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/datem.py` & `django_restit-4.1.8/rest/datem.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/decorators.py` & `django_restit-4.1.8/rest/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
         if hasattr(request, "_log_component"):
             metadata["component"] = request._log_component
             metadata["pkey"] = request._log_pk
 
         incident.event_now(
             "rest_errors", description=subject, level=1, hostname=host,
-            details=stack, reporter_ip=request.ip,
+            details=stack, reporter_ip=request.ip, request=request,
             metadata=metadata)
 
         return restStatus(request, False, error=str(err), stack=stack)
     return restStatus(request, False)
 
 
 def dispatcher(request, *args, **kwargs):
```

### Comparing `django_restit-4.1.7/rest/encryption.py` & `django_restit-4.1.8/rest/encryption.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/extra/json_metadata.py` & `django_restit-4.1.8/rest/extra/json_metadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/fields.py` & `django_restit-4.1.8/rest/fields.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/forms.py` & `django_restit-4.1.8/rest/forms.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/helpers.py` & `django_restit-4.1.8/rest/helpers.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/jwtoken.py` & `django_restit-4.1.8/rest/jwtoken.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/log.py` & `django_restit-4.1.8/rest/log.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/mail.py` & `django_restit-4.1.8/rest/mail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/mailman.py` & `django_restit-4.1.8/rest/mailman.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/middleware/cors.py` & `django_restit-4.1.8/rest/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/middleware/db_router.py` & `django_restit-4.1.8/rest/middleware/db_router.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/middleware/jwt.py` & `django_restit-4.1.8/rest/middleware/jwt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/middleware/request.py` & `django_restit-4.1.8/rest/middleware/request.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/middleware/session.py` & `django_restit-4.1.8/rest/middleware/session.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/middleware/session_store.py` & `django_restit-4.1.8/rest/middleware/session_store.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/models/base.py` & `django_restit-4.1.8/rest/models/base.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/models/cacher.py` & `django_restit-4.1.8/rest/models/cacher.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/models/metadata.py` & `django_restit-4.1.8/rest/models/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,22 @@
         if not self.id:
             self.save()
 
         if values is None:
             values = request
             request = None
 
+        if isinstance(values, list):
+            # bug fix probably for odd browser handling of certain form data
+            output = objict()
+            for item in values:
+                if isinstance(item, dict):
+                    output.update(item)
+            values = output
+
         if not isinstance(values, dict):
             raise Exception("invalid metadata: {}".format(values))
 
         for key, value in list(values.items()):
             cat = None
             if "." in key:
                 cat, key = key.split('.')
```

### Comparing `django_restit-4.1.7/rest/regexes.yaml` & `django_restit-4.1.8/rest/regexes.yaml`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/requestex.py` & `django_restit-4.1.8/rest/requestex.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/rpc.py` & `django_restit-4.1.8/rest/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/search.py` & `django_restit-4.1.8/rest/search.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/serializers/collection.py` & `django_restit-4.1.8/rest/serializers/collection.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/serializers/csv.py` & `django_restit-4.1.8/rest/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/serializers/excel.py` & `django_restit-4.1.8/rest/serializers/excel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/serializers/json.py` & `django_restit-4.1.8/rest/serializers/json.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/serializers/legacy.py` & `django_restit-4.1.8/rest/serializers/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/serializers/model.py` & `django_restit-4.1.8/rest/serializers/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/serializers/profiler.py` & `django_restit-4.1.8/rest/serializers/profiler.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/serializers/response.py` & `django_restit-4.1.8/rest/serializers/response.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/serializers/util.py` & `django_restit-4.1.8/rest/serializers/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/settings_helper.py` & `django_restit-4.1.8/rest/settings_helper.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/static/lib/jquery.js` & `django_restit-4.1.8/rest/static/lib/jquery.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/templates/email/error.html` & `django_restit-4.1.8/rest/templates/email/error.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/templates/rest_docs.html` & `django_restit-4.1.8/rest/templates/rest_docs.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/templates/rest_html.html` & `django_restit-4.1.8/rest/templates/rest_html.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/ua.py` & `django_restit-4.1.8/rest/ua.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/uberdict.py` & `django_restit-4.1.8/rest/uberdict.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/url_docs.py` & `django_restit-4.1.8/rest/url_docs.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/urls.py` & `django_restit-4.1.8/rest/urls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/rest/views.py` & `django_restit-4.1.8/rest/views.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/sessionlog/migrations/0001_initial.py` & `django_restit-4.1.8/sessionlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/sessionlog/models.py` & `django_restit-4.1.8/sessionlog/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/taskqueue/README.md` & `django_restit-4.1.8/taskqueue/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/taskqueue/migrations/0001_initial.py` & `django_restit-4.1.8/taskqueue/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/taskqueue/models.py` & `django_restit-4.1.8/taskqueue/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/taskqueue/periodic.py` & `django_restit-4.1.8/taskqueue/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/taskqueue/rpc.py` & `django_restit-4.1.8/taskqueue/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/taskqueue/tq.py` & `django_restit-4.1.8/taskqueue/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/taskqueue/transports/email.py` & `django_restit-4.1.8/taskqueue/transports/email.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/taskqueue/transports/http.py` & `django_restit-4.1.8/taskqueue/transports/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/taskqueue/transports/s3.py` & `django_restit-4.1.8/taskqueue/transports/s3.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/taskqueue/transports/sftp.py` & `django_restit-4.1.8/taskqueue/transports/sftp.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/taskqueue/worker.py` & `django_restit-4.1.8/taskqueue/worker.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/telephony/migrations/0001_initial.py` & `django_restit-4.1.8/telephony/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/telephony/models.py` & `django_restit-4.1.8/telephony/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/telephony/phone_util.py` & `django_restit-4.1.8/telephony/phone_util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/telephony/rpc.py` & `django_restit-4.1.8/telephony/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/ws4redis/README.md` & `django_restit-4.1.8/ws4redis/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/ws4redis/client.py` & `django_restit-4.1.8/ws4redis/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/ws4redis/connection.py` & `django_restit-4.1.8/ws4redis/connection.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/ws4redis/exceptions.py` & `django_restit-4.1.8/ws4redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/ws4redis/redis.py` & `django_restit-4.1.8/ws4redis/redis.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/ws4redis/servers/base.py` & `django_restit-4.1.8/ws4redis/servers/base.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/ws4redis/servers/django.py` & `django_restit-4.1.8/ws4redis/servers/django.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/ws4redis/servers/uwsgi.py` & `django_restit-4.1.8/ws4redis/servers/uwsgi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/ws4redis/settings.py` & `django_restit-4.1.8/ws4redis/settings.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/ws4redis/utf8validator.py` & `django_restit-4.1.8/ws4redis/utf8validator.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/ws4redis/websocket.py` & `django_restit-4.1.8/ws4redis/websocket.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.1.7/PKG-INFO` & `django_restit-4.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-restit
-Version: 4.1.7
+Version: 4.1.8
 Summary: A Rest Framework for DJANGO
 License: MIT
 Author: Ian Starnes
 Author-email: ians@311labs.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

