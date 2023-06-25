# Comparing `tmp/django_restit-4.0.1.tar.gz` & `tmp/django_restit-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_restit-4.0.1.tar", max compression
+gzip compressed data, was "django_restit-4.0.2.tar", max compression
```

## Comparing `django_restit-4.0.1.tar` & `django_restit-4.0.2.tar`

### file list

```diff
@@ -1,447 +1,447 @@
--rw-r--r--   0        0        0     1068 2023-06-23 21:15:35.136818 django_restit-4.0.1/LICENSE.md
--rw-r--r--   0        0        0     6234 2023-06-23 21:15:35.136901 django_restit-4.0.1/README.md
--rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.1/account/__init__.py
--rw-r--r--   0        0        0     1839 2023-06-23 21:15:35.137029 django_restit-4.0.1/account/admin.py
--rw-r--r--   0        0        0      980 2023-06-23 21:15:35.137125 django_restit-4.0.1/account/fcm/__init__.py
--rw-r--r--   0        0        0    15894 2022-09-27 04:43:03.000000 django_restit-4.0.1/account/migrations/0001_initial.py
--rw-r--r--   0        0        0      738 2023-06-23 21:15:35.137234 django_restit-4.0.1/account/migrations/0003_member_phone_number.py
--rw-r--r--   0        0        0      551 2022-07-28 20:16:05.000000 django_restit-4.0.1/account/migrations/0004_group_modified_alter_group_created.py
--rw-r--r--   0        0        0      437 2022-07-28 20:16:05.000000 django_restit-4.0.1/account/migrations/0005_member_auth_code_expires.py
--rw-r--r--   0        0        0      450 2022-07-28 20:16:05.000000 django_restit-4.0.1/account/migrations/0006_member_security_token.py
--rw-r--r--   0        0        0     1654 2022-09-24 21:52:53.000000 django_restit-4.0.1/account/migrations/0007_authtoken_signature_authsession.py
--rw-r--r--   0        0        0     2379 2022-08-11 21:50:51.000000 django_restit-4.0.1/account/migrations/0008_memberdevice_memberdevicemetadata.py
--rw-r--r--   0        0        0      468 2022-09-24 21:54:39.000000 django_restit-4.0.1/account/migrations/0009_alter_member_phone_number.py
--rw-r--r--   0        0        0      305 2022-09-24 21:54:43.000000 django_restit-4.0.1/account/migrations/0010_delete_authtoken.py
--rw-r--r--   0        0        0     1062 2022-09-24 21:56:14.000000 django_restit-4.0.1/account/migrations/0011_authtoken.py
--rw-r--r--   0        0        0     2043 2023-06-23 21:15:35.137371 django_restit-4.0.1/account/migrations/0012_settings_settingsmetadata.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.1/account/migrations/__init__.py
--rw-r--r--   0        0        0      341 2023-06-23 21:15:35.137581 django_restit-4.0.1/account/models/__init__.py
--rw-r--r--   0        0        0     3070 2022-11-13 00:07:37.000000 django_restit-4.0.1/account/models/device.py
--rw-r--r--   0        0        0     1437 2022-07-28 20:16:05.000000 django_restit-4.0.1/account/models/feeds.py
--rw-r--r--   0        0        0    18161 2023-06-23 21:15:35.137723 django_restit-4.0.1/account/models/group.py
--rw-r--r--   0        0        0     2720 2022-09-24 05:45:19.000000 django_restit-4.0.1/account/models/legacy.py
--rw-r--r--   0        0        0    45805 2023-06-23 21:15:35.137966 django_restit-4.0.1/account/models/member.py
--rw-r--r--   0        0        0     6842 2023-06-23 21:15:35.138172 django_restit-4.0.1/account/models/membership.py
--rw-r--r--   0        0        0    10739 2023-06-23 21:15:35.138283 django_restit-4.0.1/account/models/notify.py
--rw-r--r--   0        0        0     3345 2023-06-23 21:15:35.138374 django_restit-4.0.1/account/models/session.py
--rw-r--r--   0        0        0     2137 2023-06-23 21:15:35.138434 django_restit-4.0.1/account/models/settings.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.138485 django_restit-4.0.1/account/oauth/__init__.py
--rw-r--r--   0        0        0     2078 2023-06-23 21:15:35.138691 django_restit-4.0.1/account/oauth/google.py
--rw-r--r--   0        0        0      578 2023-06-23 21:15:35.138771 django_restit-4.0.1/account/periodic.py
--rw-r--r--   0        0        0      152 2023-06-23 21:15:35.138965 django_restit-4.0.1/account/rpc/__init__.py
--rw-r--r--   0        0        0    12428 2023-06-23 21:15:35.139084 django_restit-4.0.1/account/rpc/auth.py
--rw-r--r--   0        0        0     2104 2022-11-13 00:14:42.000000 django_restit-4.0.1/account/rpc/device.py
--rw-r--r--   0        0        0     3078 2023-06-23 21:15:35.139179 django_restit-4.0.1/account/rpc/group.py
--rw-r--r--   0        0        0     1150 2022-10-30 01:24:30.000000 django_restit-4.0.1/account/rpc/member.py
--rw-r--r--   0        0        0     3344 2022-10-04 17:23:13.000000 django_restit-4.0.1/account/rpc/notify.py
--rw-r--r--   0        0        0     2610 2023-06-23 21:15:35.139259 django_restit-4.0.1/account/rpc/oauth.py
--rw-r--r--   0        0        0      271 2023-06-23 21:15:35.139434 django_restit-4.0.1/account/rpc/settings.py
--rw-r--r--   0        0        0       53 2023-06-23 21:15:35.139504 django_restit-4.0.1/account/settings.py
--rw-r--r--   0        0        0     9709 2022-07-28 20:16:05.000000 django_restit-4.0.1/account/templates/email/base.html
--rw-r--r--   0        0        0    10567 2022-07-28 20:16:05.000000 django_restit-4.0.1/account/templates/email/invite.html
--rw-r--r--   0        0        0    15185 2023-06-23 21:15:35.139631 django_restit-4.0.1/account/templates/email/plain/invite.html
--rw-r--r--   0        0        0    13954 2023-06-23 21:15:35.139720 django_restit-4.0.1/account/templates/email/plain/reset_code.html
--rw-r--r--   0        0        0    10261 2022-07-28 20:16:05.000000 django_restit-4.0.1/account/templates/email/reset_code.html
--rw-r--r--   0        0        0    15163 2023-06-23 21:15:35.139805 django_restit-4.0.1/account/templates/email/simple/invite.html
--rw-r--r--   0        0        0    13944 2023-06-23 21:15:35.139868 django_restit-4.0.1/account/templates/email/simple/reset_code.html
--rw-r--r--   0        0        0      520 2022-07-29 02:52:46.000000 django_restit-4.0.1/auditlog/README
--rw-r--r--   0        0        0        0 2022-07-29 02:52:46.000000 django_restit-4.0.1/auditlog/__init__.py
--rw-r--r--   0        0        0     1006 2022-09-24 03:15:33.000000 django_restit-4.0.1/auditlog/admin.py
--rw-r--r--   0        0        0     6553 2022-09-24 03:15:33.000000 django_restit-4.0.1/auditlog/decorators.py
--rw-r--r--   0        0        0     1329 2023-06-23 21:15:35.139991 django_restit-4.0.1/auditlog/middleware.py
--rw-r--r--   0        0        0     3309 2022-09-24 03:15:33.000000 django_restit-4.0.1/auditlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-07-29 02:52:46.000000 django_restit-4.0.1/auditlog/migrations/__init__.py
--rw-r--r--   0        0        0    16043 2023-06-23 21:15:35.140513 django_restit-4.0.1/auditlog/models.py
--rw-r--r--   0        0        0      264 2023-06-23 21:15:35.140617 django_restit-4.0.1/auditlog/periodic.py
--rw-r--r--   0        0        0     3591 2022-10-03 03:50:26.000000 django_restit-4.0.1/auditlog/rpc.py
--rw-r--r--   0        0        0     2019 2023-06-23 21:15:35.140714 django_restit-4.0.1/auditlog/tq.py
--rw-r--r--   0        0        0      163 2022-07-29 02:52:46.000000 django_restit-4.0.1/auditlog/urls.py
--rw-r--r--   0        0        0     2169 2023-06-23 21:15:35.140811 django_restit-4.0.1/inbox/README.md
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.140833 django_restit-4.0.1/inbox/__init__.py
--rw-r--r--   0        0        0      243 2023-06-23 21:15:35.140908 django_restit-4.0.1/inbox/admin.py
--rw-r--r--   0        0        0     5621 2023-06-23 21:15:35.140972 django_restit-4.0.1/inbox/handlers.py
--rw-r--r--   0        0        0     6429 2023-06-23 21:15:35.141059 django_restit-4.0.1/inbox/migrations/0001_initial.py
--rw-r--r--   0        0        0      380 2023-06-23 21:15:35.141115 django_restit-4.0.1/inbox/migrations/0002_alter_message_cc.py
--rw-r--r--   0        0        0      416 2023-06-23 21:15:35.141178 django_restit-4.0.1/inbox/migrations/0003_attachment_content_type.py
--rw-r--r--   0        0        0     1140 2023-06-23 21:15:35.141236 django_restit-4.0.1/inbox/migrations/0004_mailtemplate.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.141260 django_restit-4.0.1/inbox/migrations/__init__.py
--rw-r--r--   0        0        0      174 2023-06-23 21:15:35.141369 django_restit-4.0.1/inbox/models/__init__.py
--rw-r--r--   0        0        0     2832 2023-06-23 21:15:35.141433 django_restit-4.0.1/inbox/models/bounce.py
--rw-r--r--   0        0        0     2468 2023-06-23 21:15:35.141520 django_restit-4.0.1/inbox/models/complaint.py
--rw-r--r--   0        0        0     2879 2023-06-23 21:15:35.141710 django_restit-4.0.1/inbox/models/message.py
--rw-r--r--   0        0        0     1013 2023-06-23 21:15:35.141770 django_restit-4.0.1/inbox/models/template.py
--rw-r--r--   0        0        0     1534 2023-06-23 21:15:35.141837 django_restit-4.0.1/inbox/rpc.py
--rw-r--r--   0        0        0       89 2023-06-23 21:15:35.141924 django_restit-4.0.1/inbox/utils/__init__.py
--rw-r--r--   0        0        0     4366 2023-06-23 21:15:35.142001 django_restit-4.0.1/inbox/utils/parsing.py
--rw-r--r--   0        0        0     4098 2023-06-23 21:15:35.142066 django_restit-4.0.1/inbox/utils/render.py
--rw-r--r--   0        0        0     2109 2023-06-23 21:15:35.142125 django_restit-4.0.1/inbox/utils/sending.py
--rw-r--r--   0        0        0     1114 2023-06-23 21:15:35.142232 django_restit-4.0.1/incident/README.md
--rw-r--r--   0        0        0      988 2023-06-23 21:15:35.142301 django_restit-4.0.1/incident/__init__.py
--rw-r--r--   0        0        0     9720 2023-06-23 21:15:35.142408 django_restit-4.0.1/incident/migrations/0001_initial.py
--rw-r--r--   0        0        0      595 2023-06-23 21:15:35.142478 django_restit-4.0.1/incident/migrations/0002_event_component_event_component_id.py
--rw-r--r--   0        0        0      425 2023-06-23 21:15:35.142525 django_restit-4.0.1/incident/migrations/0003_rule_action.py
--rw-r--r--   0        0        0      662 2023-06-23 21:15:35.142574 django_restit-4.0.1/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py
--rw-r--r--   0        0        0      698 2023-06-23 21:15:35.142626 django_restit-4.0.1/incident/migrations/0005_incident_component_alter_incident_state.py
--rw-r--r--   0        0        0      324 2023-06-23 21:15:35.142680 django_restit-4.0.1/incident/migrations/0006_delete_eventmetadata.py
--rw-r--r--   0        0        0      414 2023-06-23 21:15:35.142730 django_restit-4.0.1/incident/migrations/0007_event_metadata.py
--rw-r--r--   0        0        0      903 2023-06-23 21:15:35.142784 django_restit-4.0.1/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.142804 django_restit-4.0.1/incident/migrations/__init__.py
--rw-r--r--   0        0        0      167 2023-06-23 21:15:35.142905 django_restit-4.0.1/incident/models/__init__.py
--rw-r--r--   0        0        0     4976 2023-06-23 21:15:35.142969 django_restit-4.0.1/incident/models/event.py
--rw-r--r--   0        0        0    10022 2023-06-23 21:15:35.143045 django_restit-4.0.1/incident/models/incident.py
--rw-r--r--   0        0        0     2187 2023-06-23 21:15:35.143123 django_restit-4.0.1/incident/models/ossec.py
--rw-r--r--   0        0        0     5300 2023-06-23 21:15:35.143181 django_restit-4.0.1/incident/models/rules.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.143230 django_restit-4.0.1/incident/parsers/__init__.py
--rw-r--r--   0        0        0     5289 2023-06-23 21:15:35.143323 django_restit-4.0.1/incident/parsers/ossec.py
--rw-r--r--   0        0        0      723 2023-06-23 21:15:35.143378 django_restit-4.0.1/incident/periodic.py
--rw-r--r--   0        0        0     2831 2023-06-23 21:15:35.143434 django_restit-4.0.1/incident/rpc.py
--rw-r--r--   0        0        0    12732 2023-06-23 21:15:35.143576 django_restit-4.0.1/incident/templates/email/incident_change.html
--rw-r--r--   0        0        0    15173 2023-06-23 21:15:35.143659 django_restit-4.0.1/incident/templates/email/incident_new.html
--rw-r--r--   0        0        0    13208 2023-06-23 21:15:35.143748 django_restit-4.0.1/incident/templates/email/incident_plain.html
--rw-r--r--   0        0        0      796 2023-06-23 21:15:35.143887 django_restit-4.0.1/incident/tq.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.1/location/__init__.py
--rw-r--r--   0        0        0      297 2023-06-23 21:15:35.143952 django_restit-4.0.1/location/admin.py
--rw-r--r--   0        0        0     1694 2023-06-23 21:15:35.144111 django_restit-4.0.1/location/geolocate.py
--rw-r--r--   0        0        0     7000 2022-07-28 20:16:05.000000 django_restit-4.0.1/location/migrations/0001_initial.py
--rw-r--r--   0        0        0      576 2023-06-23 21:15:35.144178 django_restit-4.0.1/location/migrations/0002_geoip_subnet_alter_geoip_ip.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.1/location/migrations/__init__.py
--rw-r--r--   0        0        0      230 2023-06-23 21:15:35.144260 django_restit-4.0.1/location/models/__init__.py
--rw-r--r--   0        0        0     2028 2023-06-23 21:15:35.144322 django_restit-4.0.1/location/models/address.py
--rw-r--r--   0        0        0     3500 2023-06-23 21:15:35.144407 django_restit-4.0.1/location/models/ip.py
--rw-r--r--   0        0        0     1994 2023-06-23 21:15:35.144467 django_restit-4.0.1/location/models/legacy.py
--rw-r--r--   0        0        0     2316 2023-06-23 21:15:35.144520 django_restit-4.0.1/location/models/location.py
--rw-r--r--   0        0        0     1474 2023-06-23 21:15:35.144569 django_restit-4.0.1/location/models/track.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.144628 django_restit-4.0.1/location/providers/__init__.py
--rw-r--r--   0        0        0      730 2023-06-23 21:15:35.144750 django_restit-4.0.1/location/providers/iplookup/__init__.py
--rw-r--r--   0        0        0     2419 2023-06-23 21:15:35.144808 django_restit-4.0.1/location/providers/iplookup/abstractapi.py
--rw-r--r--   0        0        0     1345 2023-06-23 21:15:35.144857 django_restit-4.0.1/location/providers/iplookup/extremeip.py
--rw-r--r--   0        0        0     2121 2023-06-23 21:15:35.144909 django_restit-4.0.1/location/providers/iplookup/geoplugin.py
--rw-r--r--   0        0        0     1797 2023-06-23 21:15:35.144963 django_restit-4.0.1/location/providers/iplookup/ipapi.py
--rw-r--r--   0        0        0     1265 2023-06-23 21:15:35.145020 django_restit-4.0.1/location/providers/iplookup/ipinfo.py
--rw-r--r--   0        0        0      937 2023-06-23 21:15:35.145073 django_restit-4.0.1/location/providers/iplookup/restit.py
--rw-r--r--   0        0        0       42 2023-06-23 21:15:35.145153 django_restit-4.0.1/location/providers/location/__init__.py
--rw-r--r--   0        0        0     2860 2023-06-23 21:15:35.145211 django_restit-4.0.1/location/providers/location/google.py
--rw-r--r--   0        0        0       46 2023-06-23 21:15:35.145290 django_restit-4.0.1/location/providers/timezones/__init__.py
--rw-r--r--   0        0        0      619 2023-06-23 21:15:35.145347 django_restit-4.0.1/location/providers/timezones/google.py
--rw-r--r--   0        0        0     1935 2023-06-23 21:15:35.145739 django_restit-4.0.1/location/providers/zillow.py
--rw-r--r--   0        0        0      123 2023-06-23 21:15:35.145822 django_restit-4.0.1/location/rpc/__init__.py
--rw-r--r--   0        0        0      782 2023-06-23 21:15:35.145877 django_restit-4.0.1/location/rpc/ip.py
--rw-r--r--   0        0        0      779 2023-06-23 21:15:35.145928 django_restit-4.0.1/location/rpc/location.py
--rw-r--r--   0        0        0     3735 2023-06-23 21:15:35.145987 django_restit-4.0.1/location/rpc/track.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.1/medialib/__init__.py
--rw-r--r--   0        0        0     2261 2022-07-28 20:16:05.000000 django_restit-4.0.1/medialib/admin.py
--rw-r--r--   0        0        0       27 2022-07-28 20:16:05.000000 django_restit-4.0.1/medialib/cvutil/__init__.py
--rw-r--r--   0        0        0     4269 2022-07-28 20:16:05.000000 django_restit-4.0.1/medialib/cvutil/contours.py
--rw-r--r--   0        0        0    12649 2022-07-28 20:16:05.000000 django_restit-4.0.1/medialib/cvutil/images.py
--rw-r--r--   0        0        0     9586 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/cvutil/misc.py
--rw-r--r--   0        0        0     5824 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/cvutil/text.py
--rw-r--r--   0        0        0    48442 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/fixtures/initial_data.json
--rw-r--r--   0        0        0    31978 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/fixtures/medialib.json
--rw-r--r--   0        0        0    16989 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/fixtures/medialib_test_fixture.json
--rw-r--r--   0        0        0     5442 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/forms.py
--rw-r--r--   0        0        0    20518 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/migrations/__init__.py
--rw-r--r--   0        0        0    52121 2023-06-23 21:15:35.146207 django_restit-4.0.1/medialib/models.py
--rw-r--r--   0        0        0     1189 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/ocr.py
--rw-r--r--   0        0        0     1275 2023-06-23 21:15:35.146396 django_restit-4.0.1/medialib/pdf.py
--rw-r--r--   0        0        0      545 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/qrcode.py
--rw-r--r--   0        0        0    10312 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/__init__.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/engines/__init__.py
--rw-r--r--   0        0        0     3531 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/engines/anigif.py
--rw-r--r--   0        0        0     6881 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/engines/ffmpeg.py
--rw-r--r--   0        0        0      792 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/engines/gifsicle.py
--rw-r--r--   0        0        0     3436 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/engines/hls.py
--rw-r--r--   0        0        0      983 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/engines/mp4box.py
--rw-r--r--   0        0        0      397 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/engines/rtmp/Makefile
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/engines/rtmp/__init__.py
--rw-r--r--   0        0        0     4026 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/engines/rtmp/rtmp.i
--rw-r--r--   0        0        0      699 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/engines/rtmpdump.py
--rw-r--r--   0        0        0     1017 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/engines/rtmpsink.py
--rw-r--r--   0        0        0     3466 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/engines/video_getinfo.py
--rw-r--r--   0        0        0      809 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/engines/websnap.py
--rw-r--r--   0        0        0     2193 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/exceptions.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/presets/__init__.py
--rw-r--r--   0        0        0     4179 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/presets/akamai.py
--rw-r--r--   0        0        0     3284 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/presets/animated_thumbnail.py
--rw-r--r--   0        0        0     4004 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/presets/ffmpeg.py
--rw-r--r--   0        0        0     2087 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/presets/flv.py
--rw-r--r--   0        0        0     6567 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/presets/hls.py
--rw-r--r--   0        0        0     6955 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/presets/image_transcode.py
--rw-r--r--   0        0        0     1094 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/presets/image_validate.py
--rw-r--r--   0        0        0     2423 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/presets/mp4.py
--rw-r--r--   0        0        0     4997 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/presets/video_still.py
--rw-r--r--   0        0        0     3228 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/presets/video_validate.py
--rw-r--r--   0        0        0      863 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/presets/websnap.py
--rw-r--r--   0        0        0     2282 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/presets/youtube.py
--rw-r--r--   0        0        0    16451 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/render_utils.py
--rw-r--r--   0        0        0      370 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/render/schedule.py
--rw-r--r--   0        0        0       82 2022-10-20 05:50:28.000000 django_restit-4.0.1/medialib/rpc/__init__.py
--rw-r--r--   0        0        0    37925 2022-10-20 05:55:31.000000 django_restit-4.0.1/medialib/rpc/legacy.py
--rw-r--r--   0        0        0      617 2022-10-20 06:03:18.000000 django_restit-4.0.1/medialib/rpc/media.py
--rw-r--r--   0        0        0      956 2022-10-20 05:51:56.000000 django_restit-4.0.1/medialib/rpc/tools.py
--rwxr-xr-x   0        0        0     7875 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/scripts/init_config
--rw-r--r--   0        0        0     4499 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/css/base_medialibui.css
--rw-r--r--   0        0        0     3128 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/css/base_widgets.css
--rw-r--r--   0        0        0     3263 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/css/jquery.jcrop.css
--rw-r--r--   0        0        0      193 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/arrow-down-white.png
--rw-r--r--   0        0        0     4589 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/bg-body.gif
--rw-r--r--   0        0        0      441 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/cancel.gif
--rw-r--r--   0        0        0      341 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/icon-generic.gif
--rw-r--r--   0        0        0      355 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/icon-image.gif
--rw-r--r--   0        0        0      359 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/icon-media.gif
--rw-r--r--   0        0        0      355 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/icon-zip.gif
--rw-r--r--   0        0        0     3208 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/loading.gif
--rw-r--r--   0        0        0     2537 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/noimage.gif
--rw-r--r--   0        0        0     1057 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/render_err.gif
--rw-r--r--   0        0        0     6716 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/rendering.gif
--rw-r--r--   0        0        0      292 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/star_off.png
--rw-r--r--   0        0        0      297 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/star_on.png
--rw-r--r--   0        0        0     1130 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/img/unknown.gif
--rwxr-xr-x   0        0        0    74054 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/lib/caman.full.js
--rw-r--r--   0        0        0    17360 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/lib/hammer.min.js
--rwxr-xr-x   0        0        0    42434 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/lib/jquery.Jcrop.js
--rw-r--r--   0        0        0      743 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/lib/jquery.hammer.js
--rw-r--r--   0        0        0    16587 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/lib/load-image.min.js
--rwxr-xr-x   0        0        0   111779 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/lib/swiper.js
--rw-r--r--   0        0        0     1163 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js
--rw-r--r--   0        0        0     1163 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js
--rw-r--r--   0        0        0     5708 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js
--rw-r--r--   0        0        0     3502 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/static/lib/tinymce/plugins/medialib/medialib.html
--rw-r--r--   0        0        0     5876 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/__init__.py
--rw-r--r--   0        0        0      601 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/apiclient/__init__.py
--rw-r--r--   0        0        0     9852 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/apiclient/channel.py
--rw-r--r--   0        0        0    35929 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/apiclient/discovery.py
--rw-r--r--   0        0        0     3516 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/apiclient/errors.py
--rw-r--r--   0        0        0    52911 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/apiclient/http.py
--rw-r--r--   0        0        0     6505 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/apiclient/mimeparse.py
--rw-r--r--   0        0        0    11761 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/apiclient/model.py
--rw-r--r--   0        0        0     3528 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/apiclient/sample_tools.py
--rw-r--r--   0        0        0     9293 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/apiclient/schema.py
--rw-r--r--   0        0        0     1592 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/filestore.py
--rw-r--r--   0        0        0    69575 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/httplib2/__init__.py
--rw-r--r--   0        0        0    39670 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/httplib2/cacerts.txt
--rw-r--r--   0        0        0     3821 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/httplib2/iri2uri.py
--rw-r--r--   0        0        0    18452 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/httplib2/socks.py
--rw-r--r--   0        0        0      706 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/httpstore.py
--rw-r--r--   0        0        0      304 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/nullstore.py
--rw-r--r--   0        0        0      213 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/__init__.py
--rw-r--r--   0        0        0     1044 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/anyjson.py
--rw-r--r--   0        0        0    32534 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/appengine.py
--rw-r--r--   0        0        0    44346 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/client.py
--rw-r--r--   0        0        0     4425 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/clientsecrets.py
--rw-r--r--   0        0        0    10239 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/crypt.py
--rw-r--r--   0        0        0     3755 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/django_orm.py
--rw-r--r--   0        0        0     3164 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/file.py
--rw-r--r--   0        0        0     3036 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/gce.py
--rw-r--r--   0        0        0     3229 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/keyring_storage.py
--rw-r--r--   0        0        0    11393 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/locked_file.py
--rw-r--r--   0        0        0    13950 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/multistore_file.py
--rw-r--r--   0        0        0     5588 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/old_run.py
--rw-r--r--   0        0        0     8379 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/tools.py
--rw-r--r--   0        0        0     5706 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/util.py
--rw-r--r--   0        0        0     3367 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/oauth2client/xsrfutil.py
--rw-r--r--   0        0        0      500 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/rtmpstore.py
--rw-r--r--   0        0        0     4583 2023-06-23 21:15:35.146572 django_restit-4.0.1/medialib/stores/s3store.py
--rw-r--r--   0        0        0     4996 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/uritemplate/__init__.py
--rw-r--r--   0        0        0      406 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/stores/youtubestore.py
--rw-r--r--   0        0        0     3691 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/base.html
--rw-r--r--   0        0        0     1277 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/instances.html
--rw-r--r--   0        0        0     1170 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/items.html
--rw-r--r--   0        0        0     8194 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/library.html
--rw-r--r--   0        0        0       65 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/notify_error.subject
--rw-r--r--   0        0        0       49 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/notify_error.to
--rw-r--r--   0        0        0      272 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/notify_error.txt
--rw-r--r--   0        0        0       71 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/notify_ready.subject
--rw-r--r--   0        0        0       49 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/notify_ready.to
--rw-r--r--   0        0        0      298 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/notify_ready.txt
--rw-r--r--   0        0        0       64 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/notify_render_error.subject
--rw-r--r--   0        0        0       48 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/notify_render_error.to
--rw-r--r--   0        0        0      271 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/notify_render_error.txt
--rw-r--r--   0        0        0       68 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/notify_validate_error.subject
--rw-r--r--   0        0        0       48 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/notify_validate_error.to
--rw-r--r--   0        0        0      275 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/notify_validate_error.txt
--rw-r--r--   0        0        0      206 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/smil
--rw-r--r--   0        0        0     1177 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/test.html
--rw-r--r--   0        0        0     1549 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/templates/medialib/testpicker.html
--rw-r--r--   0        0        0     6045 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/tests.py
--rw-r--r--   0        0        0      544 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/tq.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/urls.py
--rw-r--r--   0        0        0     3756 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/utils.py
--rw-r--r--   0        0        0     4321 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/views.py
--rw-r--r--   0        0        0     4303 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/__init__.py
--rw-r--r--   0        0        0      601 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/apiclient/__init__.py
--rw-r--r--   0        0        0     9886 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/apiclient/channel.py
--rw-r--r--   0        0        0    35907 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/apiclient/discovery.py
--rw-r--r--   0        0        0     3550 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/apiclient/errors.py
--rw-r--r--   0        0        0    52945 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/apiclient/http.py
--rw-r--r--   0        0        0     6505 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/apiclient/mimeparse.py
--rw-r--r--   0        0        0    11795 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/apiclient/model.py
--rw-r--r--   0        0        0     3596 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/apiclient/sample_tools.py
--rw-r--r--   0        0        0     9327 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/apiclient/schema.py
--rw-r--r--   0        0        0    69581 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/httplib2/__init__.py
--rw-r--r--   0        0        0    39670 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/httplib2/cacerts.txt
--rw-r--r--   0        0        0     3821 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/httplib2/iri2uri.py
--rw-r--r--   0        0        0    18452 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/httplib2/socks.py
--rw-r--r--   0        0        0      213 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/__init__.py
--rw-r--r--   0        0        0     1044 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/anyjson.py
--rw-r--r--   0        0        0    32534 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/appengine.py
--rw-r--r--   0        0        0    44431 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/client.py
--rw-r--r--   0        0        0     4425 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/clientsecrets.py
--rw-r--r--   0        0        0    10239 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/crypt.py
--rw-r--r--   0        0        0     3753 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/django_orm.py
--rw-r--r--   0        0        0     3164 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/file.py
--rw-r--r--   0        0        0     3036 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/gce.py
--rw-r--r--   0        0        0     3229 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/keyring_storage.py
--rw-r--r--   0        0        0    11393 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/locked_file.py
--rw-r--r--   0        0        0    13950 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/multistore_file.py
--rw-r--r--   0        0        0     5588 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/old_run.py
--rw-r--r--   0        0        0     8379 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/tools.py
--rw-r--r--   0        0        0     5706 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/util.py
--rw-r--r--   0        0        0     3367 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/oauth2client/xsrfutil.py
--rw-r--r--   0        0        0     2849 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/upload.py
--rw-r--r--   0        0        0     4996 2022-07-28 20:16:06.000000 django_restit-4.0.1/medialib/youtube/uritemplate/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-23 21:15:35.146800 django_restit-4.0.1/metrics/README.md
--rw-r--r--   0        0        0       90 2023-06-23 21:15:35.146848 django_restit-4.0.1/metrics/__init__.py
--rw-r--r--   0        0        0    23460 2023-06-23 21:15:35.146988 django_restit-4.0.1/metrics/client.py
--rw-r--r--   0        0        0     9182 2023-06-23 21:15:35.147084 django_restit-4.0.1/metrics/eod.py
--rw-r--r--   0        0        0     1664 2023-06-23 21:15:35.147166 django_restit-4.0.1/metrics/examples/eod_example.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.147220 django_restit-4.0.1/metrics/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.147298 django_restit-4.0.1/metrics/management/commands/__init__.py
--rw-r--r--   0        0        0      429 2023-06-23 21:15:35.147527 django_restit-4.0.1/metrics/management/commands/delete_gauge.py
--rw-r--r--   0        0        0      464 2023-06-23 21:15:35.147736 django_restit-4.0.1/metrics/management/commands/delete_metric.py
--rw-r--r--   0        0        0     2801 2023-06-23 21:15:35.147974 django_restit-4.0.1/metrics/management/commands/fix_redis_metrics_keys.py
--rw-r--r--   0        0        0     1928 2023-06-23 21:15:35.148212 django_restit-4.0.1/metrics/management/commands/generate_test_metrics.py
--rw-r--r--   0        0        0     1742 2023-06-23 21:15:35.148371 django_restit-4.0.1/metrics/management/commands/redis_metrics_send_mail.py
--rw-r--r--   0        0        0     1874 2023-06-23 21:15:35.148601 django_restit-4.0.1/metrics/management/commands/reset_weekly_metrics.py
--rw-r--r--   0        0        0     4343 2023-06-23 21:15:35.148742 django_restit-4.0.1/metrics/management/commands/system_metric.py
--rw-r--r--   0        0        0     2399 2023-06-23 21:15:35.148840 django_restit-4.0.1/metrics/migrations/0001_initial.py
--rw-r--r--   0        0        0     1510 2023-06-23 21:15:35.148905 django_restit-4.0.1/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py
--rw-r--r--   0        0        0      453 2023-06-23 21:15:35.148960 django_restit-4.0.1/metrics/migrations/0003_metrics_expires.py
--rw-r--r--   0        0        0     3271 2023-06-23 21:15:35.149017 django_restit-4.0.1/metrics/migrations/0004_eodmetrics.py
--rw-r--r--   0        0        0     2358 2023-06-24 01:15:03.076316 django_restit-4.0.1/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.149043 django_restit-4.0.1/metrics/migrations/__init__.py
--rw-r--r--   0        0        0    10599 2023-06-24 01:15:03.076758 django_restit-4.0.1/metrics/models.py
--rw-r--r--   0        0        0      480 2023-06-23 21:15:35.149225 django_restit-4.0.1/metrics/periodic.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.149281 django_restit-4.0.1/metrics/providers/__init__.py
--rw-r--r--   0        0        0     7335 2023-06-23 21:15:35.149411 django_restit-4.0.1/metrics/providers/aws.py
--rw-r--r--   0        0        0    14826 2023-06-23 21:15:35.149500 django_restit-4.0.1/metrics/rpc.py
--rw-r--r--   0        0        0      132 2023-06-23 21:15:35.149570 django_restit-4.0.1/metrics/settings.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.149594 django_restit-4.0.1/metrics/tq.py
--rw-r--r--   0        0        0    10490 2023-06-23 21:15:35.149712 django_restit-4.0.1/metrics/utils.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/pushit/__init__.py
--rw-r--r--   0        0        0      451 2022-07-28 20:16:06.000000 django_restit-4.0.1/pushit/admin.py
--rw-r--r--   0        0        0     4555 2022-07-28 20:16:06.000000 django_restit-4.0.1/pushit/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/pushit/migrations/__init__.py
--rw-r--r--   0        0        0     5076 2022-07-28 20:16:06.000000 django_restit-4.0.1/pushit/models.py
--rw-r--r--   0        0        0    12431 2023-06-23 21:15:35.150053 django_restit-4.0.1/pushit/rpc.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.150246 django_restit-4.0.1/pushit/static/js/models_pushit.js
--rw-r--r--   0        0        0     1382 2023-06-24 01:15:43.215992 django_restit-4.0.1/pyproject.toml
--rw-r--r--   0        0        0      118 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/.gitignore
--rw-r--r--   0        0        0     5460 2022-10-30 01:29:56.000000 django_restit-4.0.1/rest/README.md
--rw-r--r--   0        0        0       72 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/RemoteEvents.py
--rw-r--r--   0        0        0      120 2022-11-13 00:23:18.000000 django_restit-4.0.1/rest/__init__.py
--rw-r--r--   0        0        0     1967 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/arc4.py
--rw-r--r--   0        0        0       83 2023-06-23 21:15:35.150349 django_restit-4.0.1/rest/cache.py
--rw-r--r--   0        0        0       72 2023-06-23 21:15:35.150496 django_restit-4.0.1/rest/crypto/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-23 21:15:35.150606 django_restit-4.0.1/rest/crypto/aes.py
--rw-r--r--   0        0        0     4082 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/crypto/privpub.py
--rw-r--r--   0        0        0     3955 2022-10-28 22:27:17.000000 django_restit-4.0.1/rest/crypto/util.py
--rw-r--r--   0        0        0     7784 2023-06-23 21:15:35.150736 django_restit-4.0.1/rest/datem.py
--rw-r--r--   0        0        0    15213 2023-06-23 21:15:35.150865 django_restit-4.0.1/rest/decorators.py
--rw-r--r--   0        0        0      788 2023-06-23 21:15:35.150965 django_restit-4.0.1/rest/encryption.py
--rw-r--r--   0        0        0       54 2023-06-23 21:15:35.151052 django_restit-4.0.1/rest/extra/__init__.py
--rw-r--r--   0        0        0     1078 2023-06-23 21:15:35.151114 django_restit-4.0.1/rest/extra/json_metadata.py
--rw-r--r--   0        0        0     9719 2023-06-23 21:15:35.151226 django_restit-4.0.1/rest/fields.py
--rw-r--r--   0        0        0     6316 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/forms.py
--rw-r--r--   0        0        0    23837 2023-06-23 21:15:35.151406 django_restit-4.0.1/rest/helpers.py
--rw-r--r--   0        0        0      260 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/joke.py
--rw-r--r--   0        0        0     2298 2023-06-23 21:15:35.151515 django_restit-4.0.1/rest/jwtoken.py
--rw-r--r--   0        0        0    21139 2023-06-23 21:15:35.151666 django_restit-4.0.1/rest/log.py
--rw-r--r--   0        0        0     7754 2023-06-23 21:15:35.151788 django_restit-4.0.1/rest/mail.py
--rw-r--r--   0        0        0     9174 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/mailman.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/management/__init__.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/management/commands/__init__.py
--rw-r--r--   0        0        0      389 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/management/commands/rpc.py
--rw-r--r--   0        0        0       33 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/middleware/__init__.py
--rw-r--r--   0        0        0     3513 2022-07-30 23:06:28.000000 django_restit-4.0.1/rest/middleware/cors.py
--rw-r--r--   0        0        0     2345 2023-06-23 21:15:35.151948 django_restit-4.0.1/rest/middleware/db_router.py
--rw-r--r--   0        0        0     5395 2023-06-23 21:15:35.152061 django_restit-4.0.1/rest/middleware/jwt.py
--rw-r--r--   0        0        0     4127 2023-06-23 21:15:35.152179 django_restit-4.0.1/rest/middleware/request.py
--rw-r--r--   0        0        0     9015 2023-06-23 21:15:35.152293 django_restit-4.0.1/rest/middleware/session.py
--rw-r--r--   0        0        0     1874 2023-06-23 21:15:35.152353 django_restit-4.0.1/rest/middleware/session_store.py
--rw-r--r--   0        0        0    76845 2023-06-23 21:15:35.152636 django_restit-4.0.1/rest/models.py
--rw-r--r--   0        0        0   149463 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/regexes.yaml
--rw-r--r--   0        0        0    14894 2023-06-23 21:15:35.152738 django_restit-4.0.1/rest/requestex.py
--rw-r--r--   0        0        0     3480 2022-09-29 05:47:59.000000 django_restit-4.0.1/rest/rpc.py
--rw-r--r--   0        0        0     7645 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/search.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.152794 django_restit-4.0.1/rest/serializers/__init__.py
--rw-r--r--   0        0        0     1644 2023-06-23 21:15:35.152880 django_restit-4.0.1/rest/serializers/collection.py
--rw-r--r--   0        0        0     2975 2023-06-23 21:15:35.152935 django_restit-4.0.1/rest/serializers/csv.py
--rw-r--r--   0        0        0     1077 2023-06-23 21:15:35.152983 django_restit-4.0.1/rest/serializers/excel.py
--rw-r--r--   0        0        0     1736 2023-06-23 21:15:35.153036 django_restit-4.0.1/rest/serializers/json.py
--rw-r--r--   0        0        0    61738 2023-06-23 21:15:35.153260 django_restit-4.0.1/rest/serializers/legacy.py
--rw-r--r--   0        0        0     4887 2023-06-23 21:15:35.153339 django_restit-4.0.1/rest/serializers/model.py
--rw-r--r--   0        0        0     6162 2023-06-23 21:15:35.153411 django_restit-4.0.1/rest/serializers/response.py
--rw-r--r--   0        0        0     2734 2023-06-23 21:15:35.153507 django_restit-4.0.1/rest/serializers/util.py
--rw-r--r--   0        0        0     1532 2023-06-23 21:15:35.153605 django_restit-4.0.1/rest/settings_helper.py
--rw-r--r--   0        0        0    95786 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/static/lib/jquery.js
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.153689 django_restit-4.0.1/rest/static/rest/app.css
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.153786 django_restit-4.0.1/rest/static/rest/app.js
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/static/rest/rest.js
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/static/rest/rest.scss
--rw-r--r--   0        0        0      529 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/templates/email/error.html
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/templates/email/error.subject
--rw-r--r--   0        0        0     7148 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/templates/rest_docs.html
--rw-r--r--   0        0        0    10880 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/templates/rest_html.html
--rw-r--r--   0        0        0   185122 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/ua.py
--rw-r--r--   0        0        0    17064 2023-06-23 21:15:35.153956 django_restit-4.0.1/rest/uberdict.py
--rw-r--r--   0        0        0    11881 2022-07-28 20:16:06.000000 django_restit-4.0.1/rest/url_docs.py
--rw-r--r--   0        0        0     1713 2023-06-23 21:15:35.154058 django_restit-4.0.1/rest/urls.py
--rw-r--r--   0        0        0     1056 2023-06-23 21:15:35.154155 django_restit-4.0.1/rest/views.py
--rw-r--r--   0        0        0      118 2022-07-28 20:16:06.000000 django_restit-4.0.1/sessionlog/.gitignore
--rw-r--r--   0        0        0       62 2022-07-28 20:16:06.000000 django_restit-4.0.1/sessionlog/README.md
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/sessionlog/__init__.py
--rw-r--r--   0        0        0      245 2023-06-23 21:15:35.154256 django_restit-4.0.1/sessionlog/admin.py
--rw-r--r--   0        0        0     1694 2022-07-28 20:16:06.000000 django_restit-4.0.1/sessionlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/sessionlog/migrations/__init__.py
--rw-r--r--   0        0        0     3922 2023-06-23 21:15:35.154359 django_restit-4.0.1/sessionlog/models.py
--rw-r--r--   0        0        0      383 2022-07-28 20:16:06.000000 django_restit-4.0.1/sessionlog/tests.py
--rw-r--r--   0        0        0       26 2022-07-28 20:16:06.000000 django_restit-4.0.1/sessionlog/views.py
--rw-r--r--   0        0        0     2196 2022-07-28 20:16:06.000000 django_restit-4.0.1/taskqueue/README.md
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/taskqueue/__init__.py
--rw-r--r--   0        0        0      208 2023-06-23 21:15:35.154426 django_restit-4.0.1/taskqueue/admin.py
--rw-r--r--   0        0        0     4738 2022-07-28 20:16:06.000000 django_restit-4.0.1/taskqueue/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/taskqueue/migrations/__init__.py
--rw-r--r--   0        0        0    16531 2023-06-23 21:15:35.154590 django_restit-4.0.1/taskqueue/models.py
--rw-r--r--   0        0        0     3072 2023-06-23 21:15:35.154789 django_restit-4.0.1/taskqueue/periodic.py
--rw-r--r--   0        0        0     5326 2023-06-23 21:15:35.154903 django_restit-4.0.1/taskqueue/rpc.py
--rw-r--r--   0        0        0      942 2022-07-28 20:16:06.000000 django_restit-4.0.1/taskqueue/tq.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/taskqueue/transports/__init__.py
--rw-r--r--   0        0        0      623 2022-07-28 20:16:06.000000 django_restit-4.0.1/taskqueue/transports/email.py
--rw-r--r--   0        0        0     2409 2022-07-28 20:16:06.000000 django_restit-4.0.1/taskqueue/transports/http.py
--rw-r--r--   0        0        0     1099 2022-07-28 20:16:06.000000 django_restit-4.0.1/taskqueue/transports/s3.py
--rw-r--r--   0        0        0     1891 2022-07-28 20:16:06.000000 django_restit-4.0.1/taskqueue/transports/sftp.py
--rw-r--r--   0        0        0      142 2022-07-28 20:16:06.000000 django_restit-4.0.1/taskqueue/transports/sms.py
--rw-r--r--   0        0        0    13660 2023-06-23 21:15:35.155056 django_restit-4.0.1/taskqueue/worker.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/telephony/__init__.py
--rw-r--r--   0        0        0      243 2023-06-23 21:15:35.155115 django_restit-4.0.1/telephony/admin.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/telephony/decorators.py
--rw-r--r--   0        0        0     3030 2022-07-28 20:16:06.000000 django_restit-4.0.1/telephony/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/telephony/migrations/__init__.py
--rw-r--r--   0        0        0     7753 2022-07-28 20:16:06.000000 django_restit-4.0.1/telephony/models.py
--rw-r--r--   0        0        0     2126 2022-07-28 20:16:06.000000 django_restit-4.0.1/telephony/phone_util.py
--rw-r--r--   0        0        0     2659 2022-11-04 18:26:58.000000 django_restit-4.0.1/telephony/rpc.py
--rw-r--r--   0        0        0     3624 2023-06-23 21:15:35.155183 django_restit-4.0.1/ws4redis/README.md
--rwxr-xr-x   0        0        0       46 2022-07-28 20:16:06.000000 django_restit-4.0.1/ws4redis/__init__.py
--rw-r--r--   0        0        0     4942 2023-06-23 21:15:35.155467 django_restit-4.0.1/ws4redis/client.py
--rw-r--r--   0        0        0    13026 2023-06-23 21:15:35.155574 django_restit-4.0.1/ws4redis/connection.py
--rwxr-xr-x   0        0        0      636 2022-07-28 20:16:06.000000 django_restit-4.0.1/ws4redis/exceptions.py
--rw-r--r--   0        0        0     5548 2023-06-23 21:15:35.155756 django_restit-4.0.1/ws4redis/redis.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.1/ws4redis/servers/__init__.py
--rw-r--r--   0        0        0     3747 2023-06-23 21:15:35.155987 django_restit-4.0.1/ws4redis/servers/base.py
--rw-r--r--   0        0        0     4329 2022-07-28 20:16:06.000000 django_restit-4.0.1/ws4redis/servers/django.py
--rw-r--r--   0        0        0     1723 2022-07-28 20:16:06.000000 django_restit-4.0.1/ws4redis/servers/uwsgi.py
--rwxr-xr-x   0        0        0     1411 2023-06-23 21:15:35.156079 django_restit-4.0.1/ws4redis/settings.py
--rwxr-xr-x   0        0        0     5122 2022-07-28 20:16:06.000000 django_restit-4.0.1/ws4redis/utf8validator.py
--rwxr-xr-x   0        0        0    14848 2023-06-23 21:15:35.156205 django_restit-4.0.1/ws4redis/websocket.py
--rw-r--r--   0        0        0     7382 1970-01-01 00:00:00.000000 django_restit-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-23 21:15:35.136818 django_restit-4.0.2/LICENSE.md
+-rw-r--r--   0        0        0     6234 2023-06-23 21:15:35.136901 django_restit-4.0.2/README.md
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/__init__.py
+-rw-r--r--   0        0        0     1839 2023-06-23 21:15:35.137029 django_restit-4.0.2/account/admin.py
+-rw-r--r--   0        0        0      980 2023-06-23 21:15:35.137125 django_restit-4.0.2/account/fcm/__init__.py
+-rw-r--r--   0        0        0    15894 2022-09-27 04:43:03.000000 django_restit-4.0.2/account/migrations/0001_initial.py
+-rw-r--r--   0        0        0      738 2023-06-23 21:15:35.137234 django_restit-4.0.2/account/migrations/0003_member_phone_number.py
+-rw-r--r--   0        0        0      551 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/migrations/0004_group_modified_alter_group_created.py
+-rw-r--r--   0        0        0      437 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/migrations/0005_member_auth_code_expires.py
+-rw-r--r--   0        0        0      450 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/migrations/0006_member_security_token.py
+-rw-r--r--   0        0        0     1654 2022-09-24 21:52:53.000000 django_restit-4.0.2/account/migrations/0007_authtoken_signature_authsession.py
+-rw-r--r--   0        0        0     2379 2022-08-11 21:50:51.000000 django_restit-4.0.2/account/migrations/0008_memberdevice_memberdevicemetadata.py
+-rw-r--r--   0        0        0      468 2022-09-24 21:54:39.000000 django_restit-4.0.2/account/migrations/0009_alter_member_phone_number.py
+-rw-r--r--   0        0        0      305 2022-09-24 21:54:43.000000 django_restit-4.0.2/account/migrations/0010_delete_authtoken.py
+-rw-r--r--   0        0        0     1062 2022-09-24 21:56:14.000000 django_restit-4.0.2/account/migrations/0011_authtoken.py
+-rw-r--r--   0        0        0     2043 2023-06-23 21:15:35.137371 django_restit-4.0.2/account/migrations/0012_settings_settingsmetadata.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/migrations/__init__.py
+-rw-r--r--   0        0        0      341 2023-06-23 21:15:35.137581 django_restit-4.0.2/account/models/__init__.py
+-rw-r--r--   0        0        0     3070 2022-11-13 00:07:37.000000 django_restit-4.0.2/account/models/device.py
+-rw-r--r--   0        0        0     1437 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/models/feeds.py
+-rw-r--r--   0        0        0    18161 2023-06-23 21:15:35.137723 django_restit-4.0.2/account/models/group.py
+-rw-r--r--   0        0        0     2720 2022-09-24 05:45:19.000000 django_restit-4.0.2/account/models/legacy.py
+-rw-r--r--   0        0        0    45805 2023-06-23 21:15:35.137966 django_restit-4.0.2/account/models/member.py
+-rw-r--r--   0        0        0     6842 2023-06-23 21:15:35.138172 django_restit-4.0.2/account/models/membership.py
+-rw-r--r--   0        0        0    10739 2023-06-23 21:15:35.138283 django_restit-4.0.2/account/models/notify.py
+-rw-r--r--   0        0        0     3345 2023-06-23 21:15:35.138374 django_restit-4.0.2/account/models/session.py
+-rw-r--r--   0        0        0     2137 2023-06-23 21:15:35.138434 django_restit-4.0.2/account/models/settings.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.138485 django_restit-4.0.2/account/oauth/__init__.py
+-rw-r--r--   0        0        0     2078 2023-06-23 21:15:35.138691 django_restit-4.0.2/account/oauth/google.py
+-rw-r--r--   0        0        0      578 2023-06-23 21:15:35.138771 django_restit-4.0.2/account/periodic.py
+-rw-r--r--   0        0        0      152 2023-06-23 21:15:35.138965 django_restit-4.0.2/account/rpc/__init__.py
+-rw-r--r--   0        0        0    12428 2023-06-23 21:15:35.139084 django_restit-4.0.2/account/rpc/auth.py
+-rw-r--r--   0        0        0     2104 2022-11-13 00:14:42.000000 django_restit-4.0.2/account/rpc/device.py
+-rw-r--r--   0        0        0     3078 2023-06-23 21:15:35.139179 django_restit-4.0.2/account/rpc/group.py
+-rw-r--r--   0        0        0     1150 2022-10-30 01:24:30.000000 django_restit-4.0.2/account/rpc/member.py
+-rw-r--r--   0        0        0     3344 2022-10-04 17:23:13.000000 django_restit-4.0.2/account/rpc/notify.py
+-rw-r--r--   0        0        0     2610 2023-06-23 21:15:35.139259 django_restit-4.0.2/account/rpc/oauth.py
+-rw-r--r--   0        0        0      271 2023-06-23 21:15:35.139434 django_restit-4.0.2/account/rpc/settings.py
+-rw-r--r--   0        0        0       53 2023-06-23 21:15:35.139504 django_restit-4.0.2/account/settings.py
+-rw-r--r--   0        0        0     9709 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/templates/email/base.html
+-rw-r--r--   0        0        0    10567 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/templates/email/invite.html
+-rw-r--r--   0        0        0    15185 2023-06-23 21:15:35.139631 django_restit-4.0.2/account/templates/email/plain/invite.html
+-rw-r--r--   0        0        0    13954 2023-06-23 21:15:35.139720 django_restit-4.0.2/account/templates/email/plain/reset_code.html
+-rw-r--r--   0        0        0    10261 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/templates/email/reset_code.html
+-rw-r--r--   0        0        0    15163 2023-06-23 21:15:35.139805 django_restit-4.0.2/account/templates/email/simple/invite.html
+-rw-r--r--   0        0        0    13944 2023-06-23 21:15:35.139868 django_restit-4.0.2/account/templates/email/simple/reset_code.html
+-rw-r--r--   0        0        0      520 2022-07-29 02:52:46.000000 django_restit-4.0.2/auditlog/README
+-rw-r--r--   0        0        0        0 2022-07-29 02:52:46.000000 django_restit-4.0.2/auditlog/__init__.py
+-rw-r--r--   0        0        0     1006 2022-09-24 03:15:33.000000 django_restit-4.0.2/auditlog/admin.py
+-rw-r--r--   0        0        0     6553 2022-09-24 03:15:33.000000 django_restit-4.0.2/auditlog/decorators.py
+-rw-r--r--   0        0        0     1329 2023-06-23 21:15:35.139991 django_restit-4.0.2/auditlog/middleware.py
+-rw-r--r--   0        0        0     3309 2022-09-24 03:15:33.000000 django_restit-4.0.2/auditlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-07-29 02:52:46.000000 django_restit-4.0.2/auditlog/migrations/__init__.py
+-rw-r--r--   0        0        0    16043 2023-06-23 21:15:35.140513 django_restit-4.0.2/auditlog/models.py
+-rw-r--r--   0        0        0      264 2023-06-23 21:15:35.140617 django_restit-4.0.2/auditlog/periodic.py
+-rw-r--r--   0        0        0     3591 2022-10-03 03:50:26.000000 django_restit-4.0.2/auditlog/rpc.py
+-rw-r--r--   0        0        0     2019 2023-06-23 21:15:35.140714 django_restit-4.0.2/auditlog/tq.py
+-rw-r--r--   0        0        0      163 2022-07-29 02:52:46.000000 django_restit-4.0.2/auditlog/urls.py
+-rw-r--r--   0        0        0     2169 2023-06-23 21:15:35.140811 django_restit-4.0.2/inbox/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.140833 django_restit-4.0.2/inbox/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-23 21:15:35.140908 django_restit-4.0.2/inbox/admin.py
+-rw-r--r--   0        0        0     5621 2023-06-23 21:15:35.140972 django_restit-4.0.2/inbox/handlers.py
+-rw-r--r--   0        0        0     6429 2023-06-23 21:15:35.141059 django_restit-4.0.2/inbox/migrations/0001_initial.py
+-rw-r--r--   0        0        0      380 2023-06-23 21:15:35.141115 django_restit-4.0.2/inbox/migrations/0002_alter_message_cc.py
+-rw-r--r--   0        0        0      416 2023-06-23 21:15:35.141178 django_restit-4.0.2/inbox/migrations/0003_attachment_content_type.py
+-rw-r--r--   0        0        0     1140 2023-06-23 21:15:35.141236 django_restit-4.0.2/inbox/migrations/0004_mailtemplate.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.141260 django_restit-4.0.2/inbox/migrations/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-23 21:15:35.141369 django_restit-4.0.2/inbox/models/__init__.py
+-rw-r--r--   0        0        0     2832 2023-06-23 21:15:35.141433 django_restit-4.0.2/inbox/models/bounce.py
+-rw-r--r--   0        0        0     2468 2023-06-23 21:15:35.141520 django_restit-4.0.2/inbox/models/complaint.py
+-rw-r--r--   0        0        0     2879 2023-06-23 21:15:35.141710 django_restit-4.0.2/inbox/models/message.py
+-rw-r--r--   0        0        0     1013 2023-06-23 21:15:35.141770 django_restit-4.0.2/inbox/models/template.py
+-rw-r--r--   0        0        0     1534 2023-06-23 21:15:35.141837 django_restit-4.0.2/inbox/rpc.py
+-rw-r--r--   0        0        0       89 2023-06-23 21:15:35.141924 django_restit-4.0.2/inbox/utils/__init__.py
+-rw-r--r--   0        0        0     4366 2023-06-23 21:15:35.142001 django_restit-4.0.2/inbox/utils/parsing.py
+-rw-r--r--   0        0        0     4098 2023-06-23 21:15:35.142066 django_restit-4.0.2/inbox/utils/render.py
+-rw-r--r--   0        0        0     2109 2023-06-23 21:15:35.142125 django_restit-4.0.2/inbox/utils/sending.py
+-rw-r--r--   0        0        0     1114 2023-06-23 21:15:35.142232 django_restit-4.0.2/incident/README.md
+-rw-r--r--   0        0        0      988 2023-06-23 21:15:35.142301 django_restit-4.0.2/incident/__init__.py
+-rw-r--r--   0        0        0     9720 2023-06-23 21:15:35.142408 django_restit-4.0.2/incident/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2023-06-23 21:15:35.142478 django_restit-4.0.2/incident/migrations/0002_event_component_event_component_id.py
+-rw-r--r--   0        0        0      425 2023-06-23 21:15:35.142525 django_restit-4.0.2/incident/migrations/0003_rule_action.py
+-rw-r--r--   0        0        0      662 2023-06-23 21:15:35.142574 django_restit-4.0.2/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py
+-rw-r--r--   0        0        0      698 2023-06-23 21:15:35.142626 django_restit-4.0.2/incident/migrations/0005_incident_component_alter_incident_state.py
+-rw-r--r--   0        0        0      324 2023-06-23 21:15:35.142680 django_restit-4.0.2/incident/migrations/0006_delete_eventmetadata.py
+-rw-r--r--   0        0        0      414 2023-06-23 21:15:35.142730 django_restit-4.0.2/incident/migrations/0007_event_metadata.py
+-rw-r--r--   0        0        0      903 2023-06-23 21:15:35.142784 django_restit-4.0.2/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.142804 django_restit-4.0.2/incident/migrations/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-23 21:15:35.142905 django_restit-4.0.2/incident/models/__init__.py
+-rw-r--r--   0        0        0     4976 2023-06-23 21:15:35.142969 django_restit-4.0.2/incident/models/event.py
+-rw-r--r--   0        0        0    10022 2023-06-23 21:15:35.143045 django_restit-4.0.2/incident/models/incident.py
+-rw-r--r--   0        0        0     2187 2023-06-23 21:15:35.143123 django_restit-4.0.2/incident/models/ossec.py
+-rw-r--r--   0        0        0     5300 2023-06-23 21:15:35.143181 django_restit-4.0.2/incident/models/rules.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.143230 django_restit-4.0.2/incident/parsers/__init__.py
+-rw-r--r--   0        0        0     5289 2023-06-23 21:15:35.143323 django_restit-4.0.2/incident/parsers/ossec.py
+-rw-r--r--   0        0        0      723 2023-06-23 21:15:35.143378 django_restit-4.0.2/incident/periodic.py
+-rw-r--r--   0        0        0     2831 2023-06-23 21:15:35.143434 django_restit-4.0.2/incident/rpc.py
+-rw-r--r--   0        0        0    12732 2023-06-23 21:15:35.143576 django_restit-4.0.2/incident/templates/email/incident_change.html
+-rw-r--r--   0        0        0    15173 2023-06-23 21:15:35.143659 django_restit-4.0.2/incident/templates/email/incident_new.html
+-rw-r--r--   0        0        0    13208 2023-06-23 21:15:35.143748 django_restit-4.0.2/incident/templates/email/incident_plain.html
+-rw-r--r--   0        0        0      796 2023-06-23 21:15:35.143887 django_restit-4.0.2/incident/tq.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.2/location/__init__.py
+-rw-r--r--   0        0        0      297 2023-06-23 21:15:35.143952 django_restit-4.0.2/location/admin.py
+-rw-r--r--   0        0        0     1694 2023-06-23 21:15:35.144111 django_restit-4.0.2/location/geolocate.py
+-rw-r--r--   0        0        0     7000 2022-07-28 20:16:05.000000 django_restit-4.0.2/location/migrations/0001_initial.py
+-rw-r--r--   0        0        0      576 2023-06-23 21:15:35.144178 django_restit-4.0.2/location/migrations/0002_geoip_subnet_alter_geoip_ip.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.2/location/migrations/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-23 21:15:35.144260 django_restit-4.0.2/location/models/__init__.py
+-rw-r--r--   0        0        0     2028 2023-06-23 21:15:35.144322 django_restit-4.0.2/location/models/address.py
+-rw-r--r--   0        0        0     3500 2023-06-23 21:15:35.144407 django_restit-4.0.2/location/models/ip.py
+-rw-r--r--   0        0        0     1994 2023-06-23 21:15:35.144467 django_restit-4.0.2/location/models/legacy.py
+-rw-r--r--   0        0        0     2316 2023-06-23 21:15:35.144520 django_restit-4.0.2/location/models/location.py
+-rw-r--r--   0        0        0     1474 2023-06-23 21:15:35.144569 django_restit-4.0.2/location/models/track.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.144628 django_restit-4.0.2/location/providers/__init__.py
+-rw-r--r--   0        0        0      730 2023-06-23 21:15:35.144750 django_restit-4.0.2/location/providers/iplookup/__init__.py
+-rw-r--r--   0        0        0     2419 2023-06-23 21:15:35.144808 django_restit-4.0.2/location/providers/iplookup/abstractapi.py
+-rw-r--r--   0        0        0     1345 2023-06-23 21:15:35.144857 django_restit-4.0.2/location/providers/iplookup/extremeip.py
+-rw-r--r--   0        0        0     2121 2023-06-23 21:15:35.144909 django_restit-4.0.2/location/providers/iplookup/geoplugin.py
+-rw-r--r--   0        0        0     1797 2023-06-23 21:15:35.144963 django_restit-4.0.2/location/providers/iplookup/ipapi.py
+-rw-r--r--   0        0        0     1265 2023-06-23 21:15:35.145020 django_restit-4.0.2/location/providers/iplookup/ipinfo.py
+-rw-r--r--   0        0        0      937 2023-06-23 21:15:35.145073 django_restit-4.0.2/location/providers/iplookup/restit.py
+-rw-r--r--   0        0        0       42 2023-06-23 21:15:35.145153 django_restit-4.0.2/location/providers/location/__init__.py
+-rw-r--r--   0        0        0     2860 2023-06-23 21:15:35.145211 django_restit-4.0.2/location/providers/location/google.py
+-rw-r--r--   0        0        0       46 2023-06-23 21:15:35.145290 django_restit-4.0.2/location/providers/timezones/__init__.py
+-rw-r--r--   0        0        0      619 2023-06-23 21:15:35.145347 django_restit-4.0.2/location/providers/timezones/google.py
+-rw-r--r--   0        0        0     1935 2023-06-23 21:15:35.145739 django_restit-4.0.2/location/providers/zillow.py
+-rw-r--r--   0        0        0      123 2023-06-23 21:15:35.145822 django_restit-4.0.2/location/rpc/__init__.py
+-rw-r--r--   0        0        0      782 2023-06-23 21:15:35.145877 django_restit-4.0.2/location/rpc/ip.py
+-rw-r--r--   0        0        0      779 2023-06-23 21:15:35.145928 django_restit-4.0.2/location/rpc/location.py
+-rw-r--r--   0        0        0     3735 2023-06-23 21:15:35.145987 django_restit-4.0.2/location/rpc/track.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.2/medialib/__init__.py
+-rw-r--r--   0        0        0     2261 2022-07-28 20:16:05.000000 django_restit-4.0.2/medialib/admin.py
+-rw-r--r--   0        0        0       27 2022-07-28 20:16:05.000000 django_restit-4.0.2/medialib/cvutil/__init__.py
+-rw-r--r--   0        0        0     4269 2022-07-28 20:16:05.000000 django_restit-4.0.2/medialib/cvutil/contours.py
+-rw-r--r--   0        0        0    12649 2022-07-28 20:16:05.000000 django_restit-4.0.2/medialib/cvutil/images.py
+-rw-r--r--   0        0        0     9586 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/cvutil/misc.py
+-rw-r--r--   0        0        0     5824 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/cvutil/text.py
+-rw-r--r--   0        0        0    48442 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/fixtures/initial_data.json
+-rw-r--r--   0        0        0    31978 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/fixtures/medialib.json
+-rw-r--r--   0        0        0    16989 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/fixtures/medialib_test_fixture.json
+-rw-r--r--   0        0        0     5442 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/forms.py
+-rw-r--r--   0        0        0    20518 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/migrations/__init__.py
+-rw-r--r--   0        0        0    52121 2023-06-23 21:15:35.146207 django_restit-4.0.2/medialib/models.py
+-rw-r--r--   0        0        0     1189 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/ocr.py
+-rw-r--r--   0        0        0     1275 2023-06-23 21:15:35.146396 django_restit-4.0.2/medialib/pdf.py
+-rw-r--r--   0        0        0      545 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/qrcode.py
+-rw-r--r--   0        0        0    10312 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/__init__.py
+-rw-r--r--   0        0        0     3531 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/anigif.py
+-rw-r--r--   0        0        0     6881 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/ffmpeg.py
+-rw-r--r--   0        0        0      792 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/gifsicle.py
+-rw-r--r--   0        0        0     3436 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/hls.py
+-rw-r--r--   0        0        0      983 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/mp4box.py
+-rw-r--r--   0        0        0      397 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/rtmp/Makefile
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/rtmp/__init__.py
+-rw-r--r--   0        0        0     4026 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/rtmp/rtmp.i
+-rw-r--r--   0        0        0      699 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/rtmpdump.py
+-rw-r--r--   0        0        0     1017 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/rtmpsink.py
+-rw-r--r--   0        0        0     3466 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/video_getinfo.py
+-rw-r--r--   0        0        0      809 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/websnap.py
+-rw-r--r--   0        0        0     2193 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/exceptions.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/__init__.py
+-rw-r--r--   0        0        0     4179 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/akamai.py
+-rw-r--r--   0        0        0     3284 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/animated_thumbnail.py
+-rw-r--r--   0        0        0     4004 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/ffmpeg.py
+-rw-r--r--   0        0        0     2087 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/flv.py
+-rw-r--r--   0        0        0     6567 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/hls.py
+-rw-r--r--   0        0        0     6955 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/image_transcode.py
+-rw-r--r--   0        0        0     1094 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/image_validate.py
+-rw-r--r--   0        0        0     2423 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/mp4.py
+-rw-r--r--   0        0        0     4997 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/video_still.py
+-rw-r--r--   0        0        0     3228 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/video_validate.py
+-rw-r--r--   0        0        0      863 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/websnap.py
+-rw-r--r--   0        0        0     2282 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/youtube.py
+-rw-r--r--   0        0        0    16451 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/render_utils.py
+-rw-r--r--   0        0        0      370 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/schedule.py
+-rw-r--r--   0        0        0       82 2022-10-20 05:50:28.000000 django_restit-4.0.2/medialib/rpc/__init__.py
+-rw-r--r--   0        0        0    37925 2022-10-20 05:55:31.000000 django_restit-4.0.2/medialib/rpc/legacy.py
+-rw-r--r--   0        0        0      617 2022-10-20 06:03:18.000000 django_restit-4.0.2/medialib/rpc/media.py
+-rw-r--r--   0        0        0      956 2022-10-20 05:51:56.000000 django_restit-4.0.2/medialib/rpc/tools.py
+-rwxr-xr-x   0        0        0     7875 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/scripts/init_config
+-rw-r--r--   0        0        0     4499 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/css/base_medialibui.css
+-rw-r--r--   0        0        0     3128 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/css/base_widgets.css
+-rw-r--r--   0        0        0     3263 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/css/jquery.jcrop.css
+-rw-r--r--   0        0        0      193 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/arrow-down-white.png
+-rw-r--r--   0        0        0     4589 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/bg-body.gif
+-rw-r--r--   0        0        0      441 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/cancel.gif
+-rw-r--r--   0        0        0      341 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/icon-generic.gif
+-rw-r--r--   0        0        0      355 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/icon-image.gif
+-rw-r--r--   0        0        0      359 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/icon-media.gif
+-rw-r--r--   0        0        0      355 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/icon-zip.gif
+-rw-r--r--   0        0        0     3208 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/loading.gif
+-rw-r--r--   0        0        0     2537 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/noimage.gif
+-rw-r--r--   0        0        0     1057 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/render_err.gif
+-rw-r--r--   0        0        0     6716 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/rendering.gif
+-rw-r--r--   0        0        0      292 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/star_off.png
+-rw-r--r--   0        0        0      297 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/star_on.png
+-rw-r--r--   0        0        0     1130 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/unknown.gif
+-rwxr-xr-x   0        0        0    74054 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/caman.full.js
+-rw-r--r--   0        0        0    17360 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/hammer.min.js
+-rwxr-xr-x   0        0        0    42434 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/jquery.Jcrop.js
+-rw-r--r--   0        0        0      743 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/jquery.hammer.js
+-rw-r--r--   0        0        0    16587 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/load-image.min.js
+-rwxr-xr-x   0        0        0   111779 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/swiper.js
+-rw-r--r--   0        0        0     1163 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js
+-rw-r--r--   0        0        0     1163 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js
+-rw-r--r--   0        0        0     5708 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js
+-rw-r--r--   0        0        0     3502 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/medialib.html
+-rw-r--r--   0        0        0     5876 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/__init__.py
+-rw-r--r--   0        0        0      601 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/__init__.py
+-rw-r--r--   0        0        0     9852 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/channel.py
+-rw-r--r--   0        0        0    35929 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/discovery.py
+-rw-r--r--   0        0        0     3516 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/errors.py
+-rw-r--r--   0        0        0    52911 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/http.py
+-rw-r--r--   0        0        0     6505 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/mimeparse.py
+-rw-r--r--   0        0        0    11761 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/model.py
+-rw-r--r--   0        0        0     3528 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/sample_tools.py
+-rw-r--r--   0        0        0     9293 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/schema.py
+-rw-r--r--   0        0        0     1592 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/filestore.py
+-rw-r--r--   0        0        0    69575 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/httplib2/__init__.py
+-rw-r--r--   0        0        0    39670 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/httplib2/cacerts.txt
+-rw-r--r--   0        0        0     3821 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/httplib2/iri2uri.py
+-rw-r--r--   0        0        0    18452 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/httplib2/socks.py
+-rw-r--r--   0        0        0      706 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/httpstore.py
+-rw-r--r--   0        0        0      304 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/nullstore.py
+-rw-r--r--   0        0        0      213 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/__init__.py
+-rw-r--r--   0        0        0     1044 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/anyjson.py
+-rw-r--r--   0        0        0    32534 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/appengine.py
+-rw-r--r--   0        0        0    44346 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/client.py
+-rw-r--r--   0        0        0     4425 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/clientsecrets.py
+-rw-r--r--   0        0        0    10239 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/crypt.py
+-rw-r--r--   0        0        0     3755 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/django_orm.py
+-rw-r--r--   0        0        0     3164 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/file.py
+-rw-r--r--   0        0        0     3036 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/gce.py
+-rw-r--r--   0        0        0     3229 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/keyring_storage.py
+-rw-r--r--   0        0        0    11393 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/locked_file.py
+-rw-r--r--   0        0        0    13950 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/multistore_file.py
+-rw-r--r--   0        0        0     5588 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/old_run.py
+-rw-r--r--   0        0        0     8379 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/tools.py
+-rw-r--r--   0        0        0     5706 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/util.py
+-rw-r--r--   0        0        0     3367 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/xsrfutil.py
+-rw-r--r--   0        0        0      500 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/rtmpstore.py
+-rw-r--r--   0        0        0     4583 2023-06-23 21:15:35.146572 django_restit-4.0.2/medialib/stores/s3store.py
+-rw-r--r--   0        0        0     4996 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/uritemplate/__init__.py
+-rw-r--r--   0        0        0      406 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/youtubestore.py
+-rw-r--r--   0        0        0     3691 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/base.html
+-rw-r--r--   0        0        0     1277 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/instances.html
+-rw-r--r--   0        0        0     1170 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/items.html
+-rw-r--r--   0        0        0     8194 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/library.html
+-rw-r--r--   0        0        0       65 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_error.subject
+-rw-r--r--   0        0        0       49 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_error.to
+-rw-r--r--   0        0        0      272 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_error.txt
+-rw-r--r--   0        0        0       71 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_ready.subject
+-rw-r--r--   0        0        0       49 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_ready.to
+-rw-r--r--   0        0        0      298 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_ready.txt
+-rw-r--r--   0        0        0       64 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_render_error.subject
+-rw-r--r--   0        0        0       48 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_render_error.to
+-rw-r--r--   0        0        0      271 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_render_error.txt
+-rw-r--r--   0        0        0       68 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_validate_error.subject
+-rw-r--r--   0        0        0       48 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_validate_error.to
+-rw-r--r--   0        0        0      275 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_validate_error.txt
+-rw-r--r--   0        0        0      206 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/smil
+-rw-r--r--   0        0        0     1177 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/test.html
+-rw-r--r--   0        0        0     1549 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/testpicker.html
+-rw-r--r--   0        0        0     6045 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/tests.py
+-rw-r--r--   0        0        0      544 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/tq.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/urls.py
+-rw-r--r--   0        0        0     3756 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/utils.py
+-rw-r--r--   0        0        0     4321 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/views.py
+-rw-r--r--   0        0        0     4303 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/__init__.py
+-rw-r--r--   0        0        0      601 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/__init__.py
+-rw-r--r--   0        0        0     9886 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/channel.py
+-rw-r--r--   0        0        0    35907 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/discovery.py
+-rw-r--r--   0        0        0     3550 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/errors.py
+-rw-r--r--   0        0        0    52945 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/http.py
+-rw-r--r--   0        0        0     6505 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/mimeparse.py
+-rw-r--r--   0        0        0    11795 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/model.py
+-rw-r--r--   0        0        0     3596 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/sample_tools.py
+-rw-r--r--   0        0        0     9327 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/schema.py
+-rw-r--r--   0        0        0    69581 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/httplib2/__init__.py
+-rw-r--r--   0        0        0    39670 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/httplib2/cacerts.txt
+-rw-r--r--   0        0        0     3821 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/httplib2/iri2uri.py
+-rw-r--r--   0        0        0    18452 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/httplib2/socks.py
+-rw-r--r--   0        0        0      213 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/__init__.py
+-rw-r--r--   0        0        0     1044 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/anyjson.py
+-rw-r--r--   0        0        0    32534 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/appengine.py
+-rw-r--r--   0        0        0    44431 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/client.py
+-rw-r--r--   0        0        0     4425 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/clientsecrets.py
+-rw-r--r--   0        0        0    10239 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/crypt.py
+-rw-r--r--   0        0        0     3753 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/django_orm.py
+-rw-r--r--   0        0        0     3164 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/file.py
+-rw-r--r--   0        0        0     3036 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/gce.py
+-rw-r--r--   0        0        0     3229 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/keyring_storage.py
+-rw-r--r--   0        0        0    11393 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/locked_file.py
+-rw-r--r--   0        0        0    13950 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/multistore_file.py
+-rw-r--r--   0        0        0     5588 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/old_run.py
+-rw-r--r--   0        0        0     8379 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/tools.py
+-rw-r--r--   0        0        0     5706 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/util.py
+-rw-r--r--   0        0        0     3367 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/xsrfutil.py
+-rw-r--r--   0        0        0     2849 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/upload.py
+-rw-r--r--   0        0        0     4996 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/uritemplate/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-23 21:15:35.146800 django_restit-4.0.2/metrics/README.md
+-rw-r--r--   0        0        0       90 2023-06-23 21:15:35.146848 django_restit-4.0.2/metrics/__init__.py
+-rw-r--r--   0        0        0    23460 2023-06-23 21:15:35.146988 django_restit-4.0.2/metrics/client.py
+-rw-r--r--   0        0        0     9182 2023-06-23 21:15:35.147084 django_restit-4.0.2/metrics/eod.py
+-rw-r--r--   0        0        0     1664 2023-06-23 21:15:35.147166 django_restit-4.0.2/metrics/examples/eod_example.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.147220 django_restit-4.0.2/metrics/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.147298 django_restit-4.0.2/metrics/management/commands/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-23 21:15:35.147527 django_restit-4.0.2/metrics/management/commands/delete_gauge.py
+-rw-r--r--   0        0        0      464 2023-06-23 21:15:35.147736 django_restit-4.0.2/metrics/management/commands/delete_metric.py
+-rw-r--r--   0        0        0     2801 2023-06-23 21:15:35.147974 django_restit-4.0.2/metrics/management/commands/fix_redis_metrics_keys.py
+-rw-r--r--   0        0        0     1928 2023-06-23 21:15:35.148212 django_restit-4.0.2/metrics/management/commands/generate_test_metrics.py
+-rw-r--r--   0        0        0     1742 2023-06-23 21:15:35.148371 django_restit-4.0.2/metrics/management/commands/redis_metrics_send_mail.py
+-rw-r--r--   0        0        0     1874 2023-06-23 21:15:35.148601 django_restit-4.0.2/metrics/management/commands/reset_weekly_metrics.py
+-rw-r--r--   0        0        0     4343 2023-06-23 21:15:35.148742 django_restit-4.0.2/metrics/management/commands/system_metric.py
+-rw-r--r--   0        0        0     2399 2023-06-23 21:15:35.148840 django_restit-4.0.2/metrics/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1510 2023-06-23 21:15:35.148905 django_restit-4.0.2/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py
+-rw-r--r--   0        0        0      453 2023-06-23 21:15:35.148960 django_restit-4.0.2/metrics/migrations/0003_metrics_expires.py
+-rw-r--r--   0        0        0     3271 2023-06-23 21:15:35.149017 django_restit-4.0.2/metrics/migrations/0004_eodmetrics.py
+-rw-r--r--   0        0        0     2358 2023-06-24 01:15:03.076316 django_restit-4.0.2/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.149043 django_restit-4.0.2/metrics/migrations/__init__.py
+-rw-r--r--   0        0        0    10599 2023-06-24 01:15:03.076758 django_restit-4.0.2/metrics/models.py
+-rw-r--r--   0        0        0      480 2023-06-23 21:15:35.149225 django_restit-4.0.2/metrics/periodic.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.149281 django_restit-4.0.2/metrics/providers/__init__.py
+-rw-r--r--   0        0        0     7335 2023-06-23 21:15:35.149411 django_restit-4.0.2/metrics/providers/aws.py
+-rw-r--r--   0        0        0    14826 2023-06-23 21:15:35.149500 django_restit-4.0.2/metrics/rpc.py
+-rw-r--r--   0        0        0      132 2023-06-23 21:15:35.149570 django_restit-4.0.2/metrics/settings.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.149594 django_restit-4.0.2/metrics/tq.py
+-rw-r--r--   0        0        0    10490 2023-06-23 21:15:35.149712 django_restit-4.0.2/metrics/utils.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/pushit/__init__.py
+-rw-r--r--   0        0        0      451 2022-07-28 20:16:06.000000 django_restit-4.0.2/pushit/admin.py
+-rw-r--r--   0        0        0     4555 2022-07-28 20:16:06.000000 django_restit-4.0.2/pushit/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/pushit/migrations/__init__.py
+-rw-r--r--   0        0        0     5076 2022-07-28 20:16:06.000000 django_restit-4.0.2/pushit/models.py
+-rw-r--r--   0        0        0    12431 2023-06-23 21:15:35.150053 django_restit-4.0.2/pushit/rpc.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.150246 django_restit-4.0.2/pushit/static/js/models_pushit.js
+-rw-r--r--   0        0        0     1462 2023-06-25 17:36:11.934754 django_restit-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0      118 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/.gitignore
+-rw-r--r--   0        0        0     5460 2022-10-30 01:29:56.000000 django_restit-4.0.2/rest/README.md
+-rw-r--r--   0        0        0       72 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/RemoteEvents.py
+-rw-r--r--   0        0        0      120 2022-11-13 00:23:18.000000 django_restit-4.0.2/rest/__init__.py
+-rw-r--r--   0        0        0     1967 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/arc4.py
+-rw-r--r--   0        0        0       83 2023-06-23 21:15:35.150349 django_restit-4.0.2/rest/cache.py
+-rw-r--r--   0        0        0       72 2023-06-23 21:15:35.150496 django_restit-4.0.2/rest/crypto/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-23 21:15:35.150606 django_restit-4.0.2/rest/crypto/aes.py
+-rw-r--r--   0        0        0     4082 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/crypto/privpub.py
+-rw-r--r--   0        0        0     3955 2022-10-28 22:27:17.000000 django_restit-4.0.2/rest/crypto/util.py
+-rw-r--r--   0        0        0     7784 2023-06-23 21:15:35.150736 django_restit-4.0.2/rest/datem.py
+-rw-r--r--   0        0        0    15213 2023-06-23 21:15:35.150865 django_restit-4.0.2/rest/decorators.py
+-rw-r--r--   0        0        0      788 2023-06-23 21:15:35.150965 django_restit-4.0.2/rest/encryption.py
+-rw-r--r--   0        0        0       54 2023-06-23 21:15:35.151052 django_restit-4.0.2/rest/extra/__init__.py
+-rw-r--r--   0        0        0     1078 2023-06-23 21:15:35.151114 django_restit-4.0.2/rest/extra/json_metadata.py
+-rw-r--r--   0        0        0     9719 2023-06-23 21:15:35.151226 django_restit-4.0.2/rest/fields.py
+-rw-r--r--   0        0        0     6316 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/forms.py
+-rw-r--r--   0        0        0    23837 2023-06-23 21:15:35.151406 django_restit-4.0.2/rest/helpers.py
+-rw-r--r--   0        0        0      260 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/joke.py
+-rw-r--r--   0        0        0     2298 2023-06-23 21:15:35.151515 django_restit-4.0.2/rest/jwtoken.py
+-rw-r--r--   0        0        0    21139 2023-06-23 21:15:35.151666 django_restit-4.0.2/rest/log.py
+-rw-r--r--   0        0        0     7754 2023-06-23 21:15:35.151788 django_restit-4.0.2/rest/mail.py
+-rw-r--r--   0        0        0     9174 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/mailman.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/management/commands/__init__.py
+-rw-r--r--   0        0        0      389 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/management/commands/rpc.py
+-rw-r--r--   0        0        0       33 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/middleware/__init__.py
+-rw-r--r--   0        0        0     3513 2022-07-30 23:06:28.000000 django_restit-4.0.2/rest/middleware/cors.py
+-rw-r--r--   0        0        0     2345 2023-06-23 21:15:35.151948 django_restit-4.0.2/rest/middleware/db_router.py
+-rw-r--r--   0        0        0     5395 2023-06-23 21:15:35.152061 django_restit-4.0.2/rest/middleware/jwt.py
+-rw-r--r--   0        0        0     4127 2023-06-23 21:15:35.152179 django_restit-4.0.2/rest/middleware/request.py
+-rw-r--r--   0        0        0     9015 2023-06-23 21:15:35.152293 django_restit-4.0.2/rest/middleware/session.py
+-rw-r--r--   0        0        0     1874 2023-06-23 21:15:35.152353 django_restit-4.0.2/rest/middleware/session_store.py
+-rw-r--r--   0        0        0    76845 2023-06-23 21:15:35.152636 django_restit-4.0.2/rest/models.py
+-rw-r--r--   0        0        0   149463 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/regexes.yaml
+-rw-r--r--   0        0        0    14894 2023-06-23 21:15:35.152738 django_restit-4.0.2/rest/requestex.py
+-rw-r--r--   0        0        0     3480 2022-09-29 05:47:59.000000 django_restit-4.0.2/rest/rpc.py
+-rw-r--r--   0        0        0     7645 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/search.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.152794 django_restit-4.0.2/rest/serializers/__init__.py
+-rw-r--r--   0        0        0     1644 2023-06-23 21:15:35.152880 django_restit-4.0.2/rest/serializers/collection.py
+-rw-r--r--   0        0        0     2975 2023-06-23 21:15:35.152935 django_restit-4.0.2/rest/serializers/csv.py
+-rw-r--r--   0        0        0     1077 2023-06-23 21:15:35.152983 django_restit-4.0.2/rest/serializers/excel.py
+-rw-r--r--   0        0        0     1736 2023-06-23 21:15:35.153036 django_restit-4.0.2/rest/serializers/json.py
+-rw-r--r--   0        0        0    61738 2023-06-23 21:15:35.153260 django_restit-4.0.2/rest/serializers/legacy.py
+-rw-r--r--   0        0        0     4943 2023-06-25 17:36:11.924423 django_restit-4.0.2/rest/serializers/model.py
+-rw-r--r--   0        0        0     6162 2023-06-23 21:15:35.153411 django_restit-4.0.2/rest/serializers/response.py
+-rw-r--r--   0        0        0     2734 2023-06-23 21:15:35.153507 django_restit-4.0.2/rest/serializers/util.py
+-rw-r--r--   0        0        0     1532 2023-06-23 21:15:35.153605 django_restit-4.0.2/rest/settings_helper.py
+-rw-r--r--   0        0        0    95786 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/static/lib/jquery.js
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.153689 django_restit-4.0.2/rest/static/rest/app.css
+-rw-r--r--   0        0        0        0 2023-06-23 21:15:35.153786 django_restit-4.0.2/rest/static/rest/app.js
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/static/rest/rest.js
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/static/rest/rest.scss
+-rw-r--r--   0        0        0      529 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/templates/email/error.html
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/templates/email/error.subject
+-rw-r--r--   0        0        0     7148 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/templates/rest_docs.html
+-rw-r--r--   0        0        0    10880 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/templates/rest_html.html
+-rw-r--r--   0        0        0   185122 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/ua.py
+-rw-r--r--   0        0        0    17064 2023-06-23 21:15:35.153956 django_restit-4.0.2/rest/uberdict.py
+-rw-r--r--   0        0        0    11881 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/url_docs.py
+-rw-r--r--   0        0        0     1713 2023-06-23 21:15:35.154058 django_restit-4.0.2/rest/urls.py
+-rw-r--r--   0        0        0     1056 2023-06-23 21:15:35.154155 django_restit-4.0.2/rest/views.py
+-rw-r--r--   0        0        0      118 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/.gitignore
+-rw-r--r--   0        0        0       62 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/README.md
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/__init__.py
+-rw-r--r--   0        0        0      245 2023-06-23 21:15:35.154256 django_restit-4.0.2/sessionlog/admin.py
+-rw-r--r--   0        0        0     1694 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/migrations/__init__.py
+-rw-r--r--   0        0        0     3922 2023-06-23 21:15:35.154359 django_restit-4.0.2/sessionlog/models.py
+-rw-r--r--   0        0        0      383 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/tests.py
+-rw-r--r--   0        0        0       26 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/views.py
+-rw-r--r--   0        0        0     2196 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/README.md
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/__init__.py
+-rw-r--r--   0        0        0      208 2023-06-23 21:15:35.154426 django_restit-4.0.2/taskqueue/admin.py
+-rw-r--r--   0        0        0     4738 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/migrations/__init__.py
+-rw-r--r--   0        0        0    16531 2023-06-23 21:15:35.154590 django_restit-4.0.2/taskqueue/models.py
+-rw-r--r--   0        0        0     3072 2023-06-23 21:15:35.154789 django_restit-4.0.2/taskqueue/periodic.py
+-rw-r--r--   0        0        0     5326 2023-06-23 21:15:35.154903 django_restit-4.0.2/taskqueue/rpc.py
+-rw-r--r--   0        0        0      942 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/tq.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/transports/__init__.py
+-rw-r--r--   0        0        0      623 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/transports/email.py
+-rw-r--r--   0        0        0     2409 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/transports/http.py
+-rw-r--r--   0        0        0     1099 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/transports/s3.py
+-rw-r--r--   0        0        0     1891 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/transports/sftp.py
+-rw-r--r--   0        0        0      142 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/transports/sms.py
+-rw-r--r--   0        0        0    13660 2023-06-23 21:15:35.155056 django_restit-4.0.2/taskqueue/worker.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/telephony/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-23 21:15:35.155115 django_restit-4.0.2/telephony/admin.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/telephony/decorators.py
+-rw-r--r--   0        0        0     3030 2022-07-28 20:16:06.000000 django_restit-4.0.2/telephony/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/telephony/migrations/__init__.py
+-rw-r--r--   0        0        0     7753 2022-07-28 20:16:06.000000 django_restit-4.0.2/telephony/models.py
+-rw-r--r--   0        0        0     2126 2022-07-28 20:16:06.000000 django_restit-4.0.2/telephony/phone_util.py
+-rw-r--r--   0        0        0     2659 2022-11-04 18:26:58.000000 django_restit-4.0.2/telephony/rpc.py
+-rw-r--r--   0        0        0     3624 2023-06-23 21:15:35.155183 django_restit-4.0.2/ws4redis/README.md
+-rwxr-xr-x   0        0        0       46 2022-07-28 20:16:06.000000 django_restit-4.0.2/ws4redis/__init__.py
+-rw-r--r--   0        0        0     4942 2023-06-23 21:15:35.155467 django_restit-4.0.2/ws4redis/client.py
+-rw-r--r--   0        0        0    13026 2023-06-23 21:15:35.155574 django_restit-4.0.2/ws4redis/connection.py
+-rwxr-xr-x   0        0        0      636 2022-07-28 20:16:06.000000 django_restit-4.0.2/ws4redis/exceptions.py
+-rw-r--r--   0        0        0     5548 2023-06-23 21:15:35.155756 django_restit-4.0.2/ws4redis/redis.py
+-rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/ws4redis/servers/__init__.py
+-rw-r--r--   0        0        0     3747 2023-06-23 21:15:35.155987 django_restit-4.0.2/ws4redis/servers/base.py
+-rw-r--r--   0        0        0     4329 2022-07-28 20:16:06.000000 django_restit-4.0.2/ws4redis/servers/django.py
+-rw-r--r--   0        0        0     1723 2022-07-28 20:16:06.000000 django_restit-4.0.2/ws4redis/servers/uwsgi.py
+-rwxr-xr-x   0        0        0     1411 2023-06-23 21:15:35.156079 django_restit-4.0.2/ws4redis/settings.py
+-rwxr-xr-x   0        0        0     5122 2022-07-28 20:16:06.000000 django_restit-4.0.2/ws4redis/utf8validator.py
+-rwxr-xr-x   0        0        0    14848 2023-06-23 21:15:35.156205 django_restit-4.0.2/ws4redis/websocket.py
+-rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 django_restit-4.0.2/PKG-INFO
```

### Comparing `django_restit-4.0.1/LICENSE.md` & `django_restit-4.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/README.md` & `django_restit-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/admin.py` & `django_restit-4.0.2/account/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/fcm/__init__.py` & `django_restit-4.0.2/account/fcm/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/migrations/0001_initial.py` & `django_restit-4.0.2/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/migrations/0003_member_phone_number.py` & `django_restit-4.0.2/account/migrations/0003_member_phone_number.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/migrations/0004_group_modified_alter_group_created.py` & `django_restit-4.0.2/account/migrations/0004_group_modified_alter_group_created.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/migrations/0007_authtoken_signature_authsession.py` & `django_restit-4.0.2/account/migrations/0007_authtoken_signature_authsession.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/migrations/0008_memberdevice_memberdevicemetadata.py` & `django_restit-4.0.2/account/migrations/0008_memberdevice_memberdevicemetadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/migrations/0011_authtoken.py` & `django_restit-4.0.2/account/migrations/0011_authtoken.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/migrations/0012_settings_settingsmetadata.py` & `django_restit-4.0.2/account/migrations/0012_settings_settingsmetadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/models/device.py` & `django_restit-4.0.2/account/models/device.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/models/feeds.py` & `django_restit-4.0.2/account/models/feeds.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/models/group.py` & `django_restit-4.0.2/account/models/group.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/models/legacy.py` & `django_restit-4.0.2/account/models/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/models/member.py` & `django_restit-4.0.2/account/models/member.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/models/membership.py` & `django_restit-4.0.2/account/models/membership.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/models/notify.py` & `django_restit-4.0.2/account/models/notify.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/models/session.py` & `django_restit-4.0.2/account/models/session.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/models/settings.py` & `django_restit-4.0.2/account/models/settings.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/oauth/google.py` & `django_restit-4.0.2/account/oauth/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/periodic.py` & `django_restit-4.0.2/account/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/rpc/auth.py` & `django_restit-4.0.2/account/rpc/auth.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/rpc/device.py` & `django_restit-4.0.2/account/rpc/device.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/rpc/group.py` & `django_restit-4.0.2/account/rpc/group.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/rpc/member.py` & `django_restit-4.0.2/account/rpc/member.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/rpc/notify.py` & `django_restit-4.0.2/account/rpc/notify.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/rpc/oauth.py` & `django_restit-4.0.2/account/rpc/oauth.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/templates/email/base.html` & `django_restit-4.0.2/account/templates/email/base.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/templates/email/invite.html` & `django_restit-4.0.2/account/templates/email/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/templates/email/plain/invite.html` & `django_restit-4.0.2/account/templates/email/plain/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/templates/email/plain/reset_code.html` & `django_restit-4.0.2/account/templates/email/plain/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/templates/email/reset_code.html` & `django_restit-4.0.2/account/templates/email/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/templates/email/simple/invite.html` & `django_restit-4.0.2/account/templates/email/simple/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/account/templates/email/simple/reset_code.html` & `django_restit-4.0.2/account/templates/email/simple/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/auditlog/README` & `django_restit-4.0.2/auditlog/README`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/auditlog/admin.py` & `django_restit-4.0.2/auditlog/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/auditlog/decorators.py` & `django_restit-4.0.2/auditlog/decorators.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/auditlog/middleware.py` & `django_restit-4.0.2/auditlog/middleware.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/auditlog/migrations/0001_initial.py` & `django_restit-4.0.2/auditlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/auditlog/models.py` & `django_restit-4.0.2/auditlog/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/auditlog/rpc.py` & `django_restit-4.0.2/auditlog/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/auditlog/tq.py` & `django_restit-4.0.2/auditlog/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/inbox/README.md` & `django_restit-4.0.2/inbox/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/inbox/handlers.py` & `django_restit-4.0.2/inbox/handlers.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/inbox/migrations/0001_initial.py` & `django_restit-4.0.2/inbox/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/inbox/migrations/0004_mailtemplate.py` & `django_restit-4.0.2/inbox/migrations/0004_mailtemplate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/inbox/models/bounce.py` & `django_restit-4.0.2/inbox/models/bounce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/inbox/models/complaint.py` & `django_restit-4.0.2/inbox/models/complaint.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/inbox/models/message.py` & `django_restit-4.0.2/inbox/models/message.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/inbox/models/template.py` & `django_restit-4.0.2/inbox/models/template.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/inbox/rpc.py` & `django_restit-4.0.2/inbox/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/inbox/utils/parsing.py` & `django_restit-4.0.2/inbox/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/inbox/utils/render.py` & `django_restit-4.0.2/inbox/utils/render.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/inbox/utils/sending.py` & `django_restit-4.0.2/inbox/utils/sending.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/README.md` & `django_restit-4.0.2/incident/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/__init__.py` & `django_restit-4.0.2/incident/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/migrations/0001_initial.py` & `django_restit-4.0.2/incident/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/migrations/0002_event_component_event_component_id.py` & `django_restit-4.0.2/incident/migrations/0002_event_component_event_component_id.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py` & `django_restit-4.0.2/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/migrations/0005_incident_component_alter_incident_state.py` & `django_restit-4.0.2/incident/migrations/0005_incident_component_alter_incident_state.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py` & `django_restit-4.0.2/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/models/event.py` & `django_restit-4.0.2/incident/models/event.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/models/incident.py` & `django_restit-4.0.2/incident/models/incident.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/models/ossec.py` & `django_restit-4.0.2/incident/models/ossec.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/models/rules.py` & `django_restit-4.0.2/incident/models/rules.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/parsers/ossec.py` & `django_restit-4.0.2/incident/parsers/ossec.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/periodic.py` & `django_restit-4.0.2/incident/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/rpc.py` & `django_restit-4.0.2/incident/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/templates/email/incident_change.html` & `django_restit-4.0.2/incident/templates/email/incident_change.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/templates/email/incident_new.html` & `django_restit-4.0.2/incident/templates/email/incident_new.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/templates/email/incident_plain.html` & `django_restit-4.0.2/incident/templates/email/incident_plain.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/incident/tq.py` & `django_restit-4.0.2/incident/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/geolocate.py` & `django_restit-4.0.2/location/geolocate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/migrations/0001_initial.py` & `django_restit-4.0.2/location/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/migrations/0002_geoip_subnet_alter_geoip_ip.py` & `django_restit-4.0.2/location/migrations/0002_geoip_subnet_alter_geoip_ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/models/address.py` & `django_restit-4.0.2/location/models/address.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/models/ip.py` & `django_restit-4.0.2/location/models/ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/models/legacy.py` & `django_restit-4.0.2/location/models/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/models/location.py` & `django_restit-4.0.2/location/models/location.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/models/track.py` & `django_restit-4.0.2/location/models/track.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/providers/iplookup/__init__.py` & `django_restit-4.0.2/location/providers/iplookup/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/providers/iplookup/abstractapi.py` & `django_restit-4.0.2/location/providers/iplookup/abstractapi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/providers/iplookup/extremeip.py` & `django_restit-4.0.2/location/providers/iplookup/extremeip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/providers/iplookup/geoplugin.py` & `django_restit-4.0.2/location/providers/iplookup/geoplugin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/providers/iplookup/ipapi.py` & `django_restit-4.0.2/location/providers/iplookup/ipapi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/providers/iplookup/ipinfo.py` & `django_restit-4.0.2/location/providers/iplookup/ipinfo.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/providers/iplookup/restit.py` & `django_restit-4.0.2/location/providers/iplookup/restit.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/providers/location/google.py` & `django_restit-4.0.2/location/providers/location/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/providers/timezones/google.py` & `django_restit-4.0.2/location/providers/timezones/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/providers/zillow.py` & `django_restit-4.0.2/location/providers/zillow.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/rpc/ip.py` & `django_restit-4.0.2/location/rpc/ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/rpc/location.py` & `django_restit-4.0.2/location/rpc/location.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/location/rpc/track.py` & `django_restit-4.0.2/location/rpc/track.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/admin.py` & `django_restit-4.0.2/medialib/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/cvutil/contours.py` & `django_restit-4.0.2/medialib/cvutil/contours.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/cvutil/images.py` & `django_restit-4.0.2/medialib/cvutil/images.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/cvutil/misc.py` & `django_restit-4.0.2/medialib/cvutil/misc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/cvutil/text.py` & `django_restit-4.0.2/medialib/cvutil/text.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/fixtures/initial_data.json` & `django_restit-4.0.2/medialib/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/fixtures/medialib.json` & `django_restit-4.0.2/medialib/fixtures/medialib.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/fixtures/medialib_test_fixture.json` & `django_restit-4.0.2/medialib/fixtures/medialib_test_fixture.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/forms.py` & `django_restit-4.0.2/medialib/forms.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/migrations/0001_initial.py` & `django_restit-4.0.2/medialib/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/models.py` & `django_restit-4.0.2/medialib/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/ocr.py` & `django_restit-4.0.2/medialib/ocr.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/pdf.py` & `django_restit-4.0.2/medialib/pdf.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/qrcode.py` & `django_restit-4.0.2/medialib/qrcode.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/__init__.py` & `django_restit-4.0.2/medialib/render/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/engines/anigif.py` & `django_restit-4.0.2/medialib/render/engines/anigif.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/engines/ffmpeg.py` & `django_restit-4.0.2/medialib/render/engines/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/engines/gifsicle.py` & `django_restit-4.0.2/medialib/render/engines/gifsicle.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/engines/hls.py` & `django_restit-4.0.2/medialib/render/engines/hls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/engines/mp4box.py` & `django_restit-4.0.2/medialib/render/engines/mp4box.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/engines/rtmp/rtmp.i` & `django_restit-4.0.2/medialib/render/engines/rtmp/rtmp.i`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/engines/rtmpdump.py` & `django_restit-4.0.2/medialib/render/engines/rtmpdump.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/engines/rtmpsink.py` & `django_restit-4.0.2/medialib/render/engines/rtmpsink.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/engines/video_getinfo.py` & `django_restit-4.0.2/medialib/render/engines/video_getinfo.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/engines/websnap.py` & `django_restit-4.0.2/medialib/render/engines/websnap.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/exceptions.py` & `django_restit-4.0.2/medialib/render/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/presets/akamai.py` & `django_restit-4.0.2/medialib/render/presets/akamai.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/presets/animated_thumbnail.py` & `django_restit-4.0.2/medialib/render/presets/animated_thumbnail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/presets/ffmpeg.py` & `django_restit-4.0.2/medialib/render/presets/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/presets/flv.py` & `django_restit-4.0.2/medialib/render/presets/flv.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/presets/hls.py` & `django_restit-4.0.2/medialib/render/presets/hls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/presets/image_transcode.py` & `django_restit-4.0.2/medialib/render/presets/image_transcode.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/presets/image_validate.py` & `django_restit-4.0.2/medialib/render/presets/image_validate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/presets/mp4.py` & `django_restit-4.0.2/medialib/render/presets/mp4.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/presets/video_still.py` & `django_restit-4.0.2/medialib/render/presets/video_still.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/presets/video_validate.py` & `django_restit-4.0.2/medialib/render/presets/video_validate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/presets/websnap.py` & `django_restit-4.0.2/medialib/render/presets/websnap.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/presets/youtube.py` & `django_restit-4.0.2/medialib/render/presets/youtube.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/render/render_utils.py` & `django_restit-4.0.2/medialib/render/render_utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/rpc/legacy.py` & `django_restit-4.0.2/medialib/rpc/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/rpc/media.py` & `django_restit-4.0.2/medialib/rpc/media.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/rpc/tools.py` & `django_restit-4.0.2/medialib/rpc/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/scripts/init_config` & `django_restit-4.0.2/medialib/scripts/init_config`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/css/base_medialibui.css` & `django_restit-4.0.2/medialib/static/css/base_medialibui.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/css/base_widgets.css` & `django_restit-4.0.2/medialib/static/css/base_widgets.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/css/jquery.jcrop.css` & `django_restit-4.0.2/medialib/static/css/jquery.jcrop.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/img/bg-body.gif` & `django_restit-4.0.2/medialib/static/img/bg-body.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/img/loading.gif` & `django_restit-4.0.2/medialib/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/img/noimage.gif` & `django_restit-4.0.2/medialib/static/img/noimage.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/img/render_err.gif` & `django_restit-4.0.2/medialib/static/img/render_err.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/img/rendering.gif` & `django_restit-4.0.2/medialib/static/img/rendering.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/img/unknown.gif` & `django_restit-4.0.2/medialib/static/img/unknown.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/lib/caman.full.js` & `django_restit-4.0.2/medialib/static/lib/caman.full.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/lib/hammer.min.js` & `django_restit-4.0.2/medialib/static/lib/hammer.min.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/lib/jquery.Jcrop.js` & `django_restit-4.0.2/medialib/static/lib/jquery.Jcrop.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/lib/jquery.hammer.js` & `django_restit-4.0.2/medialib/static/lib/jquery.hammer.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/lib/load-image.min.js` & `django_restit-4.0.2/medialib/static/lib/load-image.min.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/lib/swiper.js` & `django_restit-4.0.2/medialib/static/lib/swiper.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js` & `django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js` & `django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js` & `django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/static/lib/tinymce/plugins/medialib/medialib.html` & `django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/medialib.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/__init__.py` & `django_restit-4.0.2/medialib/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/apiclient/__init__.py` & `django_restit-4.0.2/medialib/stores/apiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/apiclient/channel.py` & `django_restit-4.0.2/medialib/stores/apiclient/channel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/apiclient/discovery.py` & `django_restit-4.0.2/medialib/stores/apiclient/discovery.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/apiclient/errors.py` & `django_restit-4.0.2/medialib/stores/apiclient/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/apiclient/http.py` & `django_restit-4.0.2/medialib/stores/apiclient/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/apiclient/mimeparse.py` & `django_restit-4.0.2/medialib/stores/apiclient/mimeparse.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/apiclient/model.py` & `django_restit-4.0.2/medialib/stores/apiclient/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/apiclient/sample_tools.py` & `django_restit-4.0.2/medialib/stores/apiclient/sample_tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/apiclient/schema.py` & `django_restit-4.0.2/medialib/stores/apiclient/schema.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/filestore.py` & `django_restit-4.0.2/medialib/stores/filestore.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/httplib2/__init__.py` & `django_restit-4.0.2/medialib/stores/httplib2/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/httplib2/cacerts.txt` & `django_restit-4.0.2/medialib/stores/httplib2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/httplib2/iri2uri.py` & `django_restit-4.0.2/medialib/stores/httplib2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/httplib2/socks.py` & `django_restit-4.0.2/medialib/stores/httplib2/socks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/httpstore.py` & `django_restit-4.0.2/medialib/stores/httpstore.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/anyjson.py` & `django_restit-4.0.2/medialib/stores/oauth2client/anyjson.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/appengine.py` & `django_restit-4.0.2/medialib/stores/oauth2client/appengine.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/client.py` & `django_restit-4.0.2/medialib/stores/oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/clientsecrets.py` & `django_restit-4.0.2/medialib/stores/oauth2client/clientsecrets.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/crypt.py` & `django_restit-4.0.2/medialib/stores/oauth2client/crypt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/django_orm.py` & `django_restit-4.0.2/medialib/stores/oauth2client/django_orm.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/file.py` & `django_restit-4.0.2/medialib/stores/oauth2client/file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/gce.py` & `django_restit-4.0.2/medialib/stores/oauth2client/gce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/keyring_storage.py` & `django_restit-4.0.2/medialib/stores/oauth2client/keyring_storage.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/locked_file.py` & `django_restit-4.0.2/medialib/stores/oauth2client/locked_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/multistore_file.py` & `django_restit-4.0.2/medialib/stores/oauth2client/multistore_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/old_run.py` & `django_restit-4.0.2/medialib/stores/oauth2client/old_run.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/tools.py` & `django_restit-4.0.2/medialib/stores/oauth2client/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/util.py` & `django_restit-4.0.2/medialib/stores/oauth2client/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/oauth2client/xsrfutil.py` & `django_restit-4.0.2/medialib/stores/oauth2client/xsrfutil.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/s3store.py` & `django_restit-4.0.2/medialib/stores/s3store.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/stores/uritemplate/__init__.py` & `django_restit-4.0.2/medialib/stores/uritemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/templates/medialib/base.html` & `django_restit-4.0.2/medialib/templates/medialib/base.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/templates/medialib/instances.html` & `django_restit-4.0.2/medialib/templates/medialib/instances.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/templates/medialib/items.html` & `django_restit-4.0.2/medialib/templates/medialib/items.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/templates/medialib/library.html` & `django_restit-4.0.2/medialib/templates/medialib/library.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/templates/medialib/test.html` & `django_restit-4.0.2/medialib/templates/medialib/test.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/templates/medialib/testpicker.html` & `django_restit-4.0.2/medialib/templates/medialib/testpicker.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/tests.py` & `django_restit-4.0.2/medialib/tests.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/tq.py` & `django_restit-4.0.2/medialib/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/utils.py` & `django_restit-4.0.2/medialib/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/views.py` & `django_restit-4.0.2/medialib/views.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/__init__.py` & `django_restit-4.0.2/medialib/youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/apiclient/__init__.py` & `django_restit-4.0.2/medialib/youtube/apiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/apiclient/channel.py` & `django_restit-4.0.2/medialib/youtube/apiclient/channel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/apiclient/discovery.py` & `django_restit-4.0.2/medialib/youtube/apiclient/discovery.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/apiclient/errors.py` & `django_restit-4.0.2/medialib/youtube/apiclient/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/apiclient/http.py` & `django_restit-4.0.2/medialib/youtube/apiclient/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/apiclient/mimeparse.py` & `django_restit-4.0.2/medialib/youtube/apiclient/mimeparse.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/apiclient/model.py` & `django_restit-4.0.2/medialib/youtube/apiclient/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/apiclient/sample_tools.py` & `django_restit-4.0.2/medialib/youtube/apiclient/sample_tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/apiclient/schema.py` & `django_restit-4.0.2/medialib/youtube/apiclient/schema.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/httplib2/__init__.py` & `django_restit-4.0.2/medialib/youtube/httplib2/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/httplib2/cacerts.txt` & `django_restit-4.0.2/medialib/youtube/httplib2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/httplib2/iri2uri.py` & `django_restit-4.0.2/medialib/youtube/httplib2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/httplib2/socks.py` & `django_restit-4.0.2/medialib/youtube/httplib2/socks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/anyjson.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/anyjson.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/appengine.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/appengine.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/client.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/clientsecrets.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/clientsecrets.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/crypt.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/crypt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/django_orm.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/django_orm.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/file.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/gce.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/gce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/keyring_storage.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/keyring_storage.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/locked_file.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/locked_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/multistore_file.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/multistore_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/old_run.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/old_run.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/tools.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/util.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/oauth2client/xsrfutil.py` & `django_restit-4.0.2/medialib/youtube/oauth2client/xsrfutil.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/upload.py` & `django_restit-4.0.2/medialib/youtube/upload.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/medialib/youtube/uritemplate/__init__.py` & `django_restit-4.0.2/medialib/youtube/uritemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/README.md` & `django_restit-4.0.2/metrics/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/client.py` & `django_restit-4.0.2/metrics/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/eod.py` & `django_restit-4.0.2/metrics/eod.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/examples/eod_example.py` & `django_restit-4.0.2/metrics/examples/eod_example.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/management/commands/fix_redis_metrics_keys.py` & `django_restit-4.0.2/metrics/management/commands/fix_redis_metrics_keys.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/management/commands/generate_test_metrics.py` & `django_restit-4.0.2/metrics/management/commands/generate_test_metrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/management/commands/redis_metrics_send_mail.py` & `django_restit-4.0.2/metrics/management/commands/redis_metrics_send_mail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/management/commands/reset_weekly_metrics.py` & `django_restit-4.0.2/metrics/management/commands/reset_weekly_metrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/management/commands/system_metric.py` & `django_restit-4.0.2/metrics/management/commands/system_metric.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/migrations/0001_initial.py` & `django_restit-4.0.2/metrics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py` & `django_restit-4.0.2/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/migrations/0004_eodmetrics.py` & `django_restit-4.0.2/metrics/migrations/0004_eodmetrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py` & `django_restit-4.0.2/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/models.py` & `django_restit-4.0.2/metrics/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/providers/aws.py` & `django_restit-4.0.2/metrics/providers/aws.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/rpc.py` & `django_restit-4.0.2/metrics/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/metrics/utils.py` & `django_restit-4.0.2/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/pushit/migrations/0001_initial.py` & `django_restit-4.0.2/pushit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/pushit/models.py` & `django_restit-4.0.2/pushit/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/pushit/rpc.py` & `django_restit-4.0.2/pushit/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/pyproject.toml` & `django_restit-4.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-restit"
-version = "4.0.1"
+version = "4.0.2"
 description = "A Rest Framework for DJANGO"
 authors = ["Ian Starnes <ians@311labs.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     {include = "account"},
@@ -42,14 +42,17 @@
 mistune = "*"
 inlinestyler = "*"
 python-dateutil = "^2.8.2"
 hashids = "^1.3.1"
 boto3 = "^1.26.160"
 pyotp = "^2.8.0"
 pyqrcode = "^1.2.1"
+redis = "^3.0.1"
+django-redis-cache = "^3.0.1"
+django-redis-sessions = "^0.6.2"
 
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 bumpver = "^2023.1124"
 
 [tool.bumpver]
```

### Comparing `django_restit-4.0.1/rest/README.md` & `django_restit-4.0.2/rest/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/arc4.py` & `django_restit-4.0.2/rest/arc4.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/crypto/aes.py` & `django_restit-4.0.2/rest/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/crypto/privpub.py` & `django_restit-4.0.2/rest/crypto/privpub.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/crypto/util.py` & `django_restit-4.0.2/rest/crypto/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/datem.py` & `django_restit-4.0.2/rest/datem.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/decorators.py` & `django_restit-4.0.2/rest/decorators.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/encryption.py` & `django_restit-4.0.2/rest/encryption.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/extra/json_metadata.py` & `django_restit-4.0.2/rest/extra/json_metadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/fields.py` & `django_restit-4.0.2/rest/fields.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/forms.py` & `django_restit-4.0.2/rest/forms.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/helpers.py` & `django_restit-4.0.2/rest/helpers.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/jwtoken.py` & `django_restit-4.0.2/rest/jwtoken.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/log.py` & `django_restit-4.0.2/rest/log.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/mail.py` & `django_restit-4.0.2/rest/mail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/mailman.py` & `django_restit-4.0.2/rest/mailman.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/middleware/cors.py` & `django_restit-4.0.2/rest/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/middleware/db_router.py` & `django_restit-4.0.2/rest/middleware/db_router.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/middleware/jwt.py` & `django_restit-4.0.2/rest/middleware/jwt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/middleware/request.py` & `django_restit-4.0.2/rest/middleware/request.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/middleware/session.py` & `django_restit-4.0.2/rest/middleware/session.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/middleware/session_store.py` & `django_restit-4.0.2/rest/middleware/session_store.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/models.py` & `django_restit-4.0.2/rest/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/regexes.yaml` & `django_restit-4.0.2/rest/regexes.yaml`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/requestex.py` & `django_restit-4.0.2/rest/requestex.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/rpc.py` & `django_restit-4.0.2/rest/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/search.py` & `django_restit-4.0.2/rest/search.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/serializers/collection.py` & `django_restit-4.0.2/rest/serializers/collection.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/serializers/csv.py` & `django_restit-4.0.2/rest/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/serializers/excel.py` & `django_restit-4.0.2/rest/serializers/excel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/serializers/json.py` & `django_restit-4.0.2/rest/serializers/json.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/serializers/legacy.py` & `django_restit-4.0.2/rest/serializers/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/serializers/model.py` & `django_restit-4.0.2/rest/serializers/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,26 +46,26 @@
                 if id_key in data:
                     del data[id_key]
             continue
         value = get_field_value(instance, fin)
         if isinstance(value, models.Model):
             if fin not in recursed:
                 recursed.append(fin)
-            sfields = get_model_fields(fin, fields)
+            sfields = get_model_fields(fin, chain(fields, extra, recurse_into))
             if sfields:
                 data[fout] = to_dict(value, sfields)
             elif hasattr(value, "pk"):
                 data[fout] = value.pk
                 # FIXME we should use _id when not showing full model
                 # data[f"{fout}_id"] = value.pk
             continue
         if isinstance(value, models.Manager):
             if fin not in recursed:
                 recursed.append(fin)
-            sfields = get_model_fields(fin, fields)
+            sfields = get_model_fields(fin, chain(fields, extra, recurse_into))
             if __MY_CACHE__.cs is None:
                 __MY_CACHE__.cs = helpers.importModule("rest.serializers.collection")
             data[fout] = __MY_CACHE__.cs.to_list(value.all(), fields=sfields)["data"]
             continue
         try:
             data[fout] = serialize_value(value if not callable(value) else value())
         except Exception as err:
```

### Comparing `django_restit-4.0.1/rest/serializers/response.py` & `django_restit-4.0.2/rest/serializers/response.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/serializers/util.py` & `django_restit-4.0.2/rest/serializers/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/settings_helper.py` & `django_restit-4.0.2/rest/settings_helper.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/static/lib/jquery.js` & `django_restit-4.0.2/rest/static/lib/jquery.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/templates/email/error.html` & `django_restit-4.0.2/rest/templates/email/error.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/templates/rest_docs.html` & `django_restit-4.0.2/rest/templates/rest_docs.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/templates/rest_html.html` & `django_restit-4.0.2/rest/templates/rest_html.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/ua.py` & `django_restit-4.0.2/rest/ua.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/uberdict.py` & `django_restit-4.0.2/rest/uberdict.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/url_docs.py` & `django_restit-4.0.2/rest/url_docs.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/urls.py` & `django_restit-4.0.2/rest/urls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/rest/views.py` & `django_restit-4.0.2/rest/views.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/sessionlog/migrations/0001_initial.py` & `django_restit-4.0.2/sessionlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/sessionlog/models.py` & `django_restit-4.0.2/sessionlog/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/taskqueue/README.md` & `django_restit-4.0.2/taskqueue/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/taskqueue/migrations/0001_initial.py` & `django_restit-4.0.2/taskqueue/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/taskqueue/models.py` & `django_restit-4.0.2/taskqueue/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/taskqueue/periodic.py` & `django_restit-4.0.2/taskqueue/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/taskqueue/rpc.py` & `django_restit-4.0.2/taskqueue/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/taskqueue/tq.py` & `django_restit-4.0.2/taskqueue/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/taskqueue/transports/email.py` & `django_restit-4.0.2/taskqueue/transports/email.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/taskqueue/transports/http.py` & `django_restit-4.0.2/taskqueue/transports/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/taskqueue/transports/s3.py` & `django_restit-4.0.2/taskqueue/transports/s3.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/taskqueue/transports/sftp.py` & `django_restit-4.0.2/taskqueue/transports/sftp.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/taskqueue/worker.py` & `django_restit-4.0.2/taskqueue/worker.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/telephony/migrations/0001_initial.py` & `django_restit-4.0.2/telephony/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/telephony/models.py` & `django_restit-4.0.2/telephony/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/telephony/phone_util.py` & `django_restit-4.0.2/telephony/phone_util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/telephony/rpc.py` & `django_restit-4.0.2/telephony/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/ws4redis/README.md` & `django_restit-4.0.2/ws4redis/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/ws4redis/client.py` & `django_restit-4.0.2/ws4redis/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/ws4redis/connection.py` & `django_restit-4.0.2/ws4redis/connection.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/ws4redis/exceptions.py` & `django_restit-4.0.2/ws4redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/ws4redis/redis.py` & `django_restit-4.0.2/ws4redis/redis.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/ws4redis/servers/base.py` & `django_restit-4.0.2/ws4redis/servers/base.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/ws4redis/servers/django.py` & `django_restit-4.0.2/ws4redis/servers/django.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/ws4redis/servers/uwsgi.py` & `django_restit-4.0.2/ws4redis/servers/uwsgi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/ws4redis/settings.py` & `django_restit-4.0.2/ws4redis/settings.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/ws4redis/utf8validator.py` & `django_restit-4.0.2/ws4redis/utf8validator.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/ws4redis/websocket.py` & `django_restit-4.0.2/ws4redis/websocket.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.1/PKG-INFO` & `django_restit-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: django-restit
-Version: 4.0.1
+Version: 4.0.2
 Summary: A Rest Framework for DJANGO
 License: MIT
 Author: Ian Starnes
 Author-email: ians@311labs.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.160,<2.0.0)
 Requires-Dist: django
+Requires-Dist: django-redis-cache (>=3.0.1,<4.0.0)
+Requires-Dist: django-redis-sessions (>=0.6.2,<0.7.0)
 Requires-Dist: hashids (>=1.3.1,<2.0.0)
 Requires-Dist: inlinestyler
 Requires-Dist: mistune
 Requires-Dist: phonenumbers
 Requires-Dist: pillow
 Requires-Dist: psutil
 Requires-Dist: pycountry
@@ -25,14 +27,15 @@
 Requires-Dist: pygments
 Requires-Dist: pyjwt
 Requires-Dist: pyobjict (>=1.1.6,<2.0.0)
 Requires-Dist: pyotp (>=2.8.0,<3.0.0)
 Requires-Dist: pypng
 Requires-Dist: pyqrcode (>=1.2.1,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: redis (>=3.0.1,<4.0.0)
 Requires-Dist: six
 Requires-Dist: twilio
 Requires-Dist: ujson
 Requires-Dist: uwsgi
 Requires-Dist: wsaccel
 Description-Content-Type: text/markdown
```

