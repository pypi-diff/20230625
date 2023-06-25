# Comparing `tmp/origamibot-2.3.4.tar.gz` & `tmp/origamibot-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "origamibot-2.3.4.tar", max compression
+gzip compressed data, was "origamibot-2.3.6.tar", max compression
```

## Comparing `origamibot-2.3.4.tar` & `origamibot-2.3.6.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0     1076 2022-12-15 18:14:26.870587 origamibot-2.3.4/LICENSE
--rw-r--r--   0        0        0     4295 2022-12-15 18:14:26.870587 origamibot-2.3.4/README.md
--rw-r--r--   0        0        0       41 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/__init__.py
--rw-r--r--   0        0        0        0 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/__init__.py
--rw-r--r--   0        0        0    47428 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/api_request.py
--rw-r--r--   0        0        0    54663 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/bot.py
--rw-r--r--   0        0        0     1130 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/callbacks.py
--rw-r--r--   0        0        0     2621 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/commands.py
--rw-r--r--   0        0        0       43 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/exceptions.py
--rw-r--r--   0        0        0      592 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/sthread.py
--rw-r--r--   0        0        0     3250 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/__init__.py
--rw-r--r--   0        0        0     1487 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/animation.py
--rw-r--r--   0        0        0     1259 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/audio.py
--rw-r--r--   0        0        0      228 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/base/__init__.py
--rw-r--r--   0        0        0     4644 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/base/field.py
--rw-r--r--   0        0        0      358 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/base/inline_query_result.py
--rw-r--r--   0        0        0      414 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/base/input_media.py
--rw-r--r--   0        0        0      840 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/base/input_message_content.py
--rw-r--r--   0        0        0     3955 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/base/telegram_structure.py
--rw-r--r--   0        0        0      382 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/bot_command.py
--rw-r--r--   0        0        0     1081 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/callback_query.py
--rw-r--r--   0        0        0     2355 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/chat.py
--rw-r--r--   0        0        0     3094 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/chat_member.py
--rw-r--r--   0        0        0     1478 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/chat_permissions.py
--rw-r--r--   0        0        0      714 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/chat_photo.py
--rw-r--r--   0        0        0      835 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/chosen_inline_result.py
--rw-r--r--   0        0        0     1516 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/command_scope.py
--rw-r--r--   0        0        0      796 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/contact.py
--rw-r--r--   0        0        0      329 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/dice.py
--rw-r--r--   0        0        0     1034 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/document.py
--rw-r--r--   0        0        0      447 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/encrypted_credentials.py
--rw-r--r--   0        0        0     1473 2022-12-15 18:14:26.958587 origamibot-2.3.4/origamibot/core/teletypes/encrypted_passport_element.py
--rw-r--r--   0        0        0      946 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/file.py
--rw-r--r--   0        0        0      735 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/force_reply.py
--rw-r--r--   0        0        0     1189 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/game.py
--rw-r--r--   0        0        0     1367 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_keyboard_button.py
--rw-r--r--   0        0        0      537 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_keyboard_markup.py
--rw-r--r--   0        0        0      745 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query.py
--rw-r--r--   0        0        0     1472 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/__init__.py
--rw-r--r--   0        0        0     1537 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/article.py
--rw-r--r--   0        0        0     1419 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/audio.py
--rw-r--r--   0        0        0     1060 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_audio.py
--rw-r--r--   0        0        0     1319 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_document.py
--rw-r--r--   0        0        0     1159 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_gif.py
--rw-r--r--   0        0        0     1179 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_mpeg4_gif.py
--rw-r--r--   0        0        0      820 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_sticker.py
--rw-r--r--   0        0        0     1301 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_video.py
--rw-r--r--   0        0        0     1165 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_voice.py
--rw-r--r--   0        0        0     1571 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/contact.py
--rw-r--r--   0        0        0     1822 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/document.py
--rw-r--r--   0        0        0      599 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/game.py
--rw-r--r--   0        0        0     1811 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/gif.py
--rw-r--r--   0        0        0     1545 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/location.py
--rw-r--r--   0        0        0     1854 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/mpeg4gif.py
--rw-r--r--   0        0        0     1543 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/photo.py
--rw-r--r--   0        0        0     1833 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/venue.py
--rw-r--r--   0        0        0     1945 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/video.py
--rw-r--r--   0        0        0     1291 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/voice.py
--rw-r--r--   0        0        0      643 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/input_contact_message_content.py
--rw-r--r--   0        0        0       53 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/input_file.py
--rw-r--r--   0        0        0      528 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/input_location_message_content.py
--rw-r--r--   0        0        0      994 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/input_media_animation.py
--rw-r--r--   0        0        0      997 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/input_media_audio.py
--rw-r--r--   0        0        0      646 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/input_media_document.py
--rw-r--r--   0        0        0      425 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/input_media_photo.py
--rw-r--r--   0        0        0     1151 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/input_media_video.py
--rw-r--r--   0        0        0      597 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/input_text_message_content.py
--rw-r--r--   0        0        0     1011 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/input_venue_message_content.py
--rw-r--r--   0        0        0      751 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/invoice.py
--rw-r--r--   0        0        0      765 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/keyboard_button.py
--rw-r--r--   0        0        0      203 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/keyboard_button_poll_type.py
--rw-r--r--   0        0        0      341 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/labeled_price.py
--rw-r--r--   0        0        0      429 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/location.py
--rw-r--r--   0        0        0      675 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/login_url.py
--rw-r--r--   0        0        0      575 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/mask_position.py
--rw-r--r--   0        0        0     8420 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/message.py
--rw-r--r--   0        0        0      942 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/message_entity.py
--rw-r--r--   0        0        0      711 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/order_info.py
--rw-r--r--   0        0        0      554 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/passport_data.py
--rw-r--r--   0        0        0      624 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/passport_file.py
--rw-r--r--   0        0        0      815 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/photo_size.py
--rw-r--r--   0        0        0     1985 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/poll.py
--rw-r--r--   0        0        0      491 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/poll_answer.py
--rw-r--r--   0        0        0      355 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/poll_option.py
--rw-r--r--   0        0        0     1108 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/pre_checkout_query.py
--rw-r--r--   0        0        0      949 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/reply_keyboard_markup.py
--rw-r--r--   0        0        0      803 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/reply_keyboard_remove.py
--rw-r--r--   0        0        0      434 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/responce_parameters.py
--rw-r--r--   0        0        0      856 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/shipping_address.py
--rw-r--r--   0        0        0      541 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/shipping_option.py
--rw-r--r--   0        0        0      732 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/shipping_query.py
--rw-r--r--   0        0        0     1904 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/sticker.py
--rw-r--r--   0        0        0      925 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/sticker_set.py
--rw-r--r--   0        0        0     1247 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/successful_payment.py
--rw-r--r--   0        0        0     2307 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/update.py
--rw-r--r--   0        0        0     1591 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/user.py
--rw-r--r--   0        0        0      534 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/user_profile_photos.py
--rw-r--r--   0        0        0      689 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/venue.py
--rw-r--r--   0        0        0     1300 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/video.py
--rw-r--r--   0        0        0      968 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/video_note.py
--rw-r--r--   0        0        0      801 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/voice.py
--rw-r--r--   0        0        0     1195 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/teletypes/webhook_info.py
--rw-r--r--   0        0        0     1285 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/core/util.py
--rw-r--r--   0        0        0     1678 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/listener.py
--rw-r--r--   0        0        0      316 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/logutil.py
--rw-r--r--   0        0        0       61 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/text.py
--rw-r--r--   0        0        0     1173 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/types.py
--rw-r--r--   0        0        0      357 2022-12-15 18:14:26.962587 origamibot-2.3.4/origamibot/util.py
--rw-r--r--   0        0        0      640 2022-12-15 18:14:29.066593 origamibot-2.3.4/pyproject.toml
--rw-r--r--   0        0        0     5345 1970-01-01 00:00:00.000000 origamibot-2.3.4/setup.py
--rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 origamibot-2.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-25 07:23:19.162273 origamibot-2.3.6/LICENSE
+-rw-r--r--   0        0        0     4296 2023-06-25 07:23:19.162273 origamibot-2.3.6/README.md
+-rw-r--r--   0        0        0       41 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/__init__.py
+-rw-r--r--   0        0        0    47641 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/api_request.py
+-rw-r--r--   0        0        0    54663 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/bot.py
+-rw-r--r--   0        0        0     1130 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/callbacks.py
+-rw-r--r--   0        0        0     2621 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/commands.py
+-rw-r--r--   0        0        0       43 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/exceptions.py
+-rw-r--r--   0        0        0      592 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/sthread.py
+-rw-r--r--   0        0        0     3250 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/__init__.py
+-rw-r--r--   0        0        0     1487 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/animation.py
+-rw-r--r--   0        0        0     1259 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/audio.py
+-rw-r--r--   0        0        0      228 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/base/__init__.py
+-rw-r--r--   0        0        0     4645 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/base/field.py
+-rw-r--r--   0        0        0      358 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/base/inline_query_result.py
+-rw-r--r--   0        0        0      414 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/base/input_media.py
+-rw-r--r--   0        0        0      840 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/base/input_message_content.py
+-rw-r--r--   0        0        0     3955 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/base/telegram_structure.py
+-rw-r--r--   0        0        0      382 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/bot_command.py
+-rw-r--r--   0        0        0     1081 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/callback_query.py
+-rw-r--r--   0        0        0     2355 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/chat.py
+-rw-r--r--   0        0        0     3094 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/chat_member.py
+-rw-r--r--   0        0        0     1478 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/chat_permissions.py
+-rw-r--r--   0        0        0      714 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/chat_photo.py
+-rw-r--r--   0        0        0      835 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/chosen_inline_result.py
+-rw-r--r--   0        0        0     1516 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/command_scope.py
+-rw-r--r--   0        0        0      796 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/contact.py
+-rw-r--r--   0        0        0      329 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/dice.py
+-rw-r--r--   0        0        0     1034 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/document.py
+-rw-r--r--   0        0        0      447 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/encrypted_credentials.py
+-rw-r--r--   0        0        0     1473 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/encrypted_passport_element.py
+-rw-r--r--   0        0        0      946 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/file.py
+-rw-r--r--   0        0        0      735 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/force_reply.py
+-rw-r--r--   0        0        0     1189 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/game.py
+-rw-r--r--   0        0        0     1367 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_keyboard_button.py
+-rw-r--r--   0        0        0      537 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_keyboard_markup.py
+-rw-r--r--   0        0        0      745 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query.py
+-rw-r--r--   0        0        0     1472 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/__init__.py
+-rw-r--r--   0        0        0     1537 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/article.py
+-rw-r--r--   0        0        0     1419 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/audio.py
+-rw-r--r--   0        0        0     1060 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_audio.py
+-rw-r--r--   0        0        0     1319 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_document.py
+-rw-r--r--   0        0        0     1159 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_gif.py
+-rw-r--r--   0        0        0     1179 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_mpeg4_gif.py
+-rw-r--r--   0        0        0      820 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_sticker.py
+-rw-r--r--   0        0        0     1301 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_video.py
+-rw-r--r--   0        0        0     1165 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_voice.py
+-rw-r--r--   0        0        0     1571 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/contact.py
+-rw-r--r--   0        0        0     1822 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/document.py
+-rw-r--r--   0        0        0      599 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/game.py
+-rw-r--r--   0        0        0     1811 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/gif.py
+-rw-r--r--   0        0        0     1545 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/location.py
+-rw-r--r--   0        0        0     1854 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/mpeg4gif.py
+-rw-r--r--   0        0        0     1543 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/photo.py
+-rw-r--r--   0        0        0     1833 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/venue.py
+-rw-r--r--   0        0        0     1945 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/video.py
+-rw-r--r--   0        0        0     1291 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/voice.py
+-rw-r--r--   0        0        0      643 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/input_contact_message_content.py
+-rw-r--r--   0        0        0       53 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/input_file.py
+-rw-r--r--   0        0        0      528 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/input_location_message_content.py
+-rw-r--r--   0        0        0      994 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/input_media_animation.py
+-rw-r--r--   0        0        0      997 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/input_media_audio.py
+-rw-r--r--   0        0        0      646 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/input_media_document.py
+-rw-r--r--   0        0        0      425 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/input_media_photo.py
+-rw-r--r--   0        0        0     1151 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/input_media_video.py
+-rw-r--r--   0        0        0      597 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/input_text_message_content.py
+-rw-r--r--   0        0        0     1011 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/input_venue_message_content.py
+-rw-r--r--   0        0        0      751 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/invoice.py
+-rw-r--r--   0        0        0      765 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/keyboard_button.py
+-rw-r--r--   0        0        0      203 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/keyboard_button_poll_type.py
+-rw-r--r--   0        0        0      341 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/labeled_price.py
+-rw-r--r--   0        0        0      429 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/location.py
+-rw-r--r--   0        0        0      675 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/login_url.py
+-rw-r--r--   0        0        0      575 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/mask_position.py
+-rw-r--r--   0        0        0     8420 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/message.py
+-rw-r--r--   0        0        0      942 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/message_entity.py
+-rw-r--r--   0        0        0      711 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/order_info.py
+-rw-r--r--   0        0        0      554 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/passport_data.py
+-rw-r--r--   0        0        0      624 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/passport_file.py
+-rw-r--r--   0        0        0      815 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/photo_size.py
+-rw-r--r--   0        0        0     1985 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/poll.py
+-rw-r--r--   0        0        0      491 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/poll_answer.py
+-rw-r--r--   0        0        0      355 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/poll_option.py
+-rw-r--r--   0        0        0     1108 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/pre_checkout_query.py
+-rw-r--r--   0        0        0      949 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/reply_keyboard_markup.py
+-rw-r--r--   0        0        0      803 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/reply_keyboard_remove.py
+-rw-r--r--   0        0        0      434 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/responce_parameters.py
+-rw-r--r--   0        0        0      856 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/shipping_address.py
+-rw-r--r--   0        0        0      541 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/shipping_option.py
+-rw-r--r--   0        0        0      732 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/shipping_query.py
+-rw-r--r--   0        0        0     1904 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/sticker.py
+-rw-r--r--   0        0        0      925 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/sticker_set.py
+-rw-r--r--   0        0        0     1247 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/successful_payment.py
+-rw-r--r--   0        0        0     2307 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/update.py
+-rw-r--r--   0        0        0     1591 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/user.py
+-rw-r--r--   0        0        0      534 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/user_profile_photos.py
+-rw-r--r--   0        0        0      689 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/venue.py
+-rw-r--r--   0        0        0     1300 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/video.py
+-rw-r--r--   0        0        0      968 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/video_note.py
+-rw-r--r--   0        0        0      801 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/voice.py
+-rw-r--r--   0        0        0     1195 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/teletypes/webhook_info.py
+-rw-r--r--   0        0        0     1285 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/core/util.py
+-rw-r--r--   0        0        0     1678 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/listener.py
+-rw-r--r--   0        0        0      316 2023-06-25 07:23:19.678286 origamibot-2.3.6/origamibot/logutil.py
+-rw-r--r--   0        0        0       61 2023-06-25 07:23:19.682286 origamibot-2.3.6/origamibot/text.py
+-rw-r--r--   0        0        0     1173 2023-06-25 07:23:19.682286 origamibot-2.3.6/origamibot/types.py
+-rw-r--r--   0        0        0      357 2023-06-25 07:23:19.682286 origamibot-2.3.6/origamibot/util.py
+-rw-r--r--   0        0        0      639 2023-06-25 07:23:19.682286 origamibot-2.3.6/pyproject.toml
+-rw-r--r--   0        0        0     5346 1970-01-01 00:00:00.000000 origamibot-2.3.6/setup.py
+-rw-r--r--   0        0        0     5166 1970-01-01 00:00:00.000000 origamibot-2.3.6/PKG-INFO
```

### Comparing `origamibot-2.3.4/LICENSE` & `origamibot-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/README.md` & `origamibot-2.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     def on_command_failure(self, message, err=None):  # When command fails
         if err is None:
             self.bot.send_message(message.chat.id,
                                   'Command failed to bind arguments!')
         else:
             self.bot.send_message(message.chat.id,
-                                  'Error in command:\n{err}')
+                                  f'Error in command:\n{err}')
 
 
 if __name__ == '__main__':
     token = (argv[1] if len(argv) > 1 else input('Enter bot token: '))
     bot = Bot(token)   # Create instance of OrigamiBot class
 
     # Add an event listener
```

### Comparing `origamibot-2.3.4/origamibot/core/api_request.py` & `origamibot-2.3.6/origamibot/core/api_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,28 +66,34 @@
     url = api_url.format(token=token, method=method)
 
     data = {
         key: value
         for key, value in data.items()
         if value is not None
     }
-  
+    timeout_connect = 5
+    timeout_read = data.get('timeout', 0)
+    if timeout_read is not None:
+        timeout_read += timeout_connect
+    timeout = (timeout_connect, timeout_read)
+
     convert_elements_to_str(data)
 
     files = {
         key: value
         for key, value in files.items()
         if value is not None
     }
     if files:
         response = requests.post(url, params=data, files=files)
     else:
         json_data = json.dumps(data, ensure_ascii=True)
         headers = {'Content-type': 'application/json'}
-        response = requests.post(url, data=json_data, headers=headers)
+        response = requests.post(
+            url, data=json_data, headers=headers, timeout=timeout)
 
     if response.status_code != 200:
         description = \
             json.loads(response.text).get('description', 'No description')
         raise TelegramAPIError(f'[{response.status_code}] {description}')
 
     data = json.loads(response.text)['result']
```

### Comparing `origamibot-2.3.4/origamibot/core/bot.py` & `origamibot-2.3.6/origamibot/core/bot.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/callbacks.py` & `origamibot-2.3.6/origamibot/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/commands.py` & `origamibot-2.3.6/origamibot/core/commands.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/sthread.py` & `origamibot-2.3.6/origamibot/core/sthread.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/__init__.py` & `origamibot-2.3.6/origamibot/core/teletypes/__init__.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/animation.py` & `origamibot-2.3.6/origamibot/core/teletypes/animation.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/audio.py` & `origamibot-2.3.6/origamibot/core/teletypes/audio.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/base/field.py` & `origamibot-2.3.6/origamibot/core/teletypes/base/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
             elif item_type == list:
                 # Convert nested lists
                 value[i] = self.validate_value(item)
             else:
                 raise FieldTypeError(
                     f'''Wrong type in list {
                         item}, excpected one of {
-                            self.datatypes}'''
+                            self.data_types}'''
                     )
 
         return value
 
 
 
 from .telegram_structure import TelegramStructure  # NOQA
```

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/base/input_message_content.py` & `origamibot-2.3.6/origamibot/core/teletypes/base/input_message_content.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/base/telegram_structure.py` & `origamibot-2.3.6/origamibot/core/teletypes/base/telegram_structure.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/callback_query.py` & `origamibot-2.3.6/origamibot/core/teletypes/callback_query.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/chat.py` & `origamibot-2.3.6/origamibot/core/teletypes/chat.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/chat_member.py` & `origamibot-2.3.6/origamibot/core/teletypes/chat_member.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/chat_permissions.py` & `origamibot-2.3.6/origamibot/core/teletypes/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/chat_photo.py` & `origamibot-2.3.6/origamibot/core/teletypes/chat_photo.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/chosen_inline_result.py` & `origamibot-2.3.6/origamibot/core/teletypes/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/command_scope.py` & `origamibot-2.3.6/origamibot/core/teletypes/command_scope.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/contact.py` & `origamibot-2.3.6/origamibot/core/teletypes/contact.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/document.py` & `origamibot-2.3.6/origamibot/core/teletypes/document.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/encrypted_passport_element.py` & `origamibot-2.3.6/origamibot/core/teletypes/encrypted_passport_element.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/file.py` & `origamibot-2.3.6/origamibot/core/teletypes/file.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/force_reply.py` & `origamibot-2.3.6/origamibot/core/teletypes/force_reply.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/game.py` & `origamibot-2.3.6/origamibot/core/teletypes/game.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_keyboard_button.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_keyboard_markup.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/__init__.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/__init__.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/article.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/article.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/audio.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/audio.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_audio.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_audio.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_document.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_document.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_gif.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_gif.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_mpeg4_gif.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_mpeg4_gif.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_sticker.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_sticker.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_video.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_video.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/cached_voice.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/cached_voice.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/contact.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/contact.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/document.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/document.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/game.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/game.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/gif.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/gif.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/location.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/location.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/mpeg4gif.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/mpeg4gif.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/photo.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/photo.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/venue.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/venue.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/video.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/video.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/inline_query_result/voice.py` & `origamibot-2.3.6/origamibot/core/teletypes/inline_query_result/voice.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/input_contact_message_content.py` & `origamibot-2.3.6/origamibot/core/teletypes/input_contact_message_content.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/input_location_message_content.py` & `origamibot-2.3.6/origamibot/core/teletypes/input_location_message_content.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/input_media_animation.py` & `origamibot-2.3.6/origamibot/core/teletypes/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/input_media_audio.py` & `origamibot-2.3.6/origamibot/core/teletypes/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/input_media_document.py` & `origamibot-2.3.6/origamibot/core/teletypes/input_media_document.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/input_media_video.py` & `origamibot-2.3.6/origamibot/core/teletypes/input_media_video.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/input_text_message_content.py` & `origamibot-2.3.6/origamibot/core/teletypes/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/input_venue_message_content.py` & `origamibot-2.3.6/origamibot/core/teletypes/input_venue_message_content.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/invoice.py` & `origamibot-2.3.6/origamibot/core/teletypes/invoice.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/keyboard_button.py` & `origamibot-2.3.6/origamibot/core/teletypes/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/login_url.py` & `origamibot-2.3.6/origamibot/core/teletypes/login_url.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/mask_position.py` & `origamibot-2.3.6/origamibot/core/teletypes/mask_position.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/message.py` & `origamibot-2.3.6/origamibot/core/teletypes/message.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/message_entity.py` & `origamibot-2.3.6/origamibot/core/teletypes/message_entity.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/order_info.py` & `origamibot-2.3.6/origamibot/core/teletypes/order_info.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/passport_data.py` & `origamibot-2.3.6/origamibot/core/teletypes/passport_data.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/passport_file.py` & `origamibot-2.3.6/origamibot/core/teletypes/passport_file.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/photo_size.py` & `origamibot-2.3.6/origamibot/core/teletypes/photo_size.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/poll.py` & `origamibot-2.3.6/origamibot/core/teletypes/poll.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/pre_checkout_query.py` & `origamibot-2.3.6/origamibot/core/teletypes/pre_checkout_query.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/reply_keyboard_markup.py` & `origamibot-2.3.6/origamibot/core/teletypes/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/reply_keyboard_remove.py` & `origamibot-2.3.6/origamibot/core/teletypes/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/shipping_address.py` & `origamibot-2.3.6/origamibot/core/teletypes/shipping_address.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/shipping_option.py` & `origamibot-2.3.6/origamibot/core/teletypes/shipping_option.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/shipping_query.py` & `origamibot-2.3.6/origamibot/core/teletypes/shipping_query.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/sticker.py` & `origamibot-2.3.6/origamibot/core/teletypes/sticker.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/sticker_set.py` & `origamibot-2.3.6/origamibot/core/teletypes/sticker_set.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/successful_payment.py` & `origamibot-2.3.6/origamibot/core/teletypes/successful_payment.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/update.py` & `origamibot-2.3.6/origamibot/core/teletypes/update.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/user.py` & `origamibot-2.3.6/origamibot/core/teletypes/user.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/user_profile_photos.py` & `origamibot-2.3.6/origamibot/core/teletypes/user_profile_photos.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/venue.py` & `origamibot-2.3.6/origamibot/core/teletypes/venue.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/video.py` & `origamibot-2.3.6/origamibot/core/teletypes/video.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/video_note.py` & `origamibot-2.3.6/origamibot/core/teletypes/video_note.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/voice.py` & `origamibot-2.3.6/origamibot/core/teletypes/voice.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/teletypes/webhook_info.py` & `origamibot-2.3.6/origamibot/core/teletypes/webhook_info.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/core/util.py` & `origamibot-2.3.6/origamibot/core/util.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/listener.py` & `origamibot-2.3.6/origamibot/listener.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/origamibot/types.py` & `origamibot-2.3.6/origamibot/types.py`

 * *Files identical despite different names*

### Comparing `origamibot-2.3.4/pyproject.toml` & `origamibot-2.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "origamibot"
-version = "v2.3.4"
+version = "2.3.6"
 description = "Library for creating bots for telegram with Python."
 authors = ["Crystal Melting Dot <stresspassing@gmail.com>"]
 license = "MIT"
 repository = 'https://github.com/cmd410/OrigamiBot'
 readme = 'README.md'
 
 [tool.poetry.dependencies]
```

### Comparing `origamibot-2.3.4/setup.py` & `origamibot-2.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 ['requests>=2.25.1,<3.0.0']
 
 extras_require = \
 {'telegram-text': ['telegram-text>=0.1.0,<0.2.0']}
 
 setup_kwargs = {
     'name': 'origamibot',
-    'version': '2.3.4',
+    'version': '2.3.6',
     'description': 'Library for creating bots for telegram with Python.',
-    'long_description': "\n\n\n\n![](https://media.githubusercontent.com/media/cmd410/OrigamiBot/master/imgs/logo.png)\n\nLibrary for creating bots for telegram with [Python](https://www.python.org/). \n\n**OrigamiBot** aims to make development of Telegram bots as easy and flexible as possible.\n\n![Upload Python Package](https://github.com/cmd410/OrigamiBot/workflows/Upload%20Python%20Package/badge.svg)\n\n## Installation\n\nOrigamibot is published in [PyPI](https://pypi.org/project/origamibot/), so it can be installed with one simple command:\n\n```\npip install origamibot\n```\n\n## Basic concepts\n\n**OrigamiBot** class is thing that will get updates form the server and dispatch them to your **command holders** and **event listeners**.\n\n- **Command Holder** is a custom class that you create that exposes its methods as commands for bot\n  command holder can be attached to bot using `bot.add_commands(your_command_holder_class())`\n- **Event listener** is a class that inherits from `origamibot.util.Listener` and performs some actions on certain events(when its `on_<something>` methods are called from **OrigamiBot**). Event listener can be added to bot with `bot.add_listener(your_listener_object)` \n\n## Usage example\n\nHere goes a simple example of a bot:\n\n```python\nfrom sys import argv\nfrom time import sleep\n\nfrom origamibot import OrigamiBot as Bot\nfrom origamibot.listener import Listener\n\n\nclass BotsCommands:\n    def __init__(self, bot: Bot):  # Can initialize however you like\n        self.bot = bot\n\n    def start(self, message):   # /start command\n        self.bot.send_message(\n            message.chat.id,\n            'Hello user!\\nThis is an example bot.')\n\n    def echo(self, message, value: str):  # /echo [value: str] command\n        self.bot.send_message(\n            message.chat.id,\n            value\n            )\n\n    def add(self, message, a: float, b: float):  # /add [a: float] [b: float]\n        self.bot.send_message(\n            message.chat.id,\n            str(a + b)\n            )\n\n    def _not_a_command(self):   # This method not considered a command\n        print('I am not a command')\n\n\nclass MessageListener(Listener):  # Event listener must inherit Listener\n    def __init__(self, bot):\n        self.bot = bot\n        self.m_count = 0\n\n    def on_message(self, message):   # called on every message\n        self.m_count += 1\n        print(f'Total messages: {self.m_count}')\n\n    def on_command_failure(self, message, err=None):  # When command fails\n        if err is None:\n            self.bot.send_message(message.chat.id,\n                                  'Command failed to bind arguments!')\n        else:\n            self.bot.send_message(message.chat.id,\n                                  'Error in command:\\n{err}')\n\n\nif __name__ == '__main__':\n    token = (argv[1] if len(argv) > 1 else input('Enter bot token: '))\n    bot = Bot(token)   # Create instance of OrigamiBot class\n\n    # Add an event listener\n    bot.add_listener(MessageListener(bot))\n\n    # Add a command holder\n    bot.add_commands(BotsCommands(bot))\n\n    # We can add as many command holders\n    # and event listeners as we like\n\n    bot.start()   # start bot's threads\n    while True:\n        sleep(1)\n        # Can also do some useful work i main thread\n        # Like autoposting to channels for example\n```\n\nCommands are added as methods of an object(be it class or instance of it), if their names don't start with `_` which makes it possible to also contain some utility functions inside command container. \n\nFor the command to be called two conditions must be met:\n\n1. command name must match with method name\n2. command's arguments must match signature of a method\n\nMethod signature supports any number of arguments with simple typing(`str`, `int`, `float`, `bool`) or without a typing(in this case all arguments are strings by default), as well as variable number of arguments `*args`. More complex types(as lists, tuples, custom object classes) are not supported, as bot does not know how to parse them, and I don't want to enforce my own parsing algorithm, but bot will still attempt to convert it like `cls(argument)`, but a correct result is not guaranteed.\n\n> **Boolean** values are considered True if their string representation is in `{'True', 'true', '1'}`, and False if in `{'False', 'false', '0'}`\n\n",
+    'long_description': "\n\n\n\n![](https://media.githubusercontent.com/media/cmd410/OrigamiBot/master/imgs/logo.png)\n\nLibrary for creating bots for telegram with [Python](https://www.python.org/). \n\n**OrigamiBot** aims to make development of Telegram bots as easy and flexible as possible.\n\n![Upload Python Package](https://github.com/cmd410/OrigamiBot/workflows/Upload%20Python%20Package/badge.svg)\n\n## Installation\n\nOrigamibot is published in [PyPI](https://pypi.org/project/origamibot/), so it can be installed with one simple command:\n\n```\npip install origamibot\n```\n\n## Basic concepts\n\n**OrigamiBot** class is thing that will get updates form the server and dispatch them to your **command holders** and **event listeners**.\n\n- **Command Holder** is a custom class that you create that exposes its methods as commands for bot\n  command holder can be attached to bot using `bot.add_commands(your_command_holder_class())`\n- **Event listener** is a class that inherits from `origamibot.util.Listener` and performs some actions on certain events(when its `on_<something>` methods are called from **OrigamiBot**). Event listener can be added to bot with `bot.add_listener(your_listener_object)` \n\n## Usage example\n\nHere goes a simple example of a bot:\n\n```python\nfrom sys import argv\nfrom time import sleep\n\nfrom origamibot import OrigamiBot as Bot\nfrom origamibot.listener import Listener\n\n\nclass BotsCommands:\n    def __init__(self, bot: Bot):  # Can initialize however you like\n        self.bot = bot\n\n    def start(self, message):   # /start command\n        self.bot.send_message(\n            message.chat.id,\n            'Hello user!\\nThis is an example bot.')\n\n    def echo(self, message, value: str):  # /echo [value: str] command\n        self.bot.send_message(\n            message.chat.id,\n            value\n            )\n\n    def add(self, message, a: float, b: float):  # /add [a: float] [b: float]\n        self.bot.send_message(\n            message.chat.id,\n            str(a + b)\n            )\n\n    def _not_a_command(self):   # This method not considered a command\n        print('I am not a command')\n\n\nclass MessageListener(Listener):  # Event listener must inherit Listener\n    def __init__(self, bot):\n        self.bot = bot\n        self.m_count = 0\n\n    def on_message(self, message):   # called on every message\n        self.m_count += 1\n        print(f'Total messages: {self.m_count}')\n\n    def on_command_failure(self, message, err=None):  # When command fails\n        if err is None:\n            self.bot.send_message(message.chat.id,\n                                  'Command failed to bind arguments!')\n        else:\n            self.bot.send_message(message.chat.id,\n                                  f'Error in command:\\n{err}')\n\n\nif __name__ == '__main__':\n    token = (argv[1] if len(argv) > 1 else input('Enter bot token: '))\n    bot = Bot(token)   # Create instance of OrigamiBot class\n\n    # Add an event listener\n    bot.add_listener(MessageListener(bot))\n\n    # Add a command holder\n    bot.add_commands(BotsCommands(bot))\n\n    # We can add as many command holders\n    # and event listeners as we like\n\n    bot.start()   # start bot's threads\n    while True:\n        sleep(1)\n        # Can also do some useful work i main thread\n        # Like autoposting to channels for example\n```\n\nCommands are added as methods of an object(be it class or instance of it), if their names don't start with `_` which makes it possible to also contain some utility functions inside command container. \n\nFor the command to be called two conditions must be met:\n\n1. command name must match with method name\n2. command's arguments must match signature of a method\n\nMethod signature supports any number of arguments with simple typing(`str`, `int`, `float`, `bool`) or without a typing(in this case all arguments are strings by default), as well as variable number of arguments `*args`. More complex types(as lists, tuples, custom object classes) are not supported, as bot does not know how to parse them, and I don't want to enforce my own parsing algorithm, but bot will still attempt to convert it like `cls(argument)`, but a correct result is not guaranteed.\n\n> **Boolean** values are considered True if their string representation is in `{'True', 'true', '1'}`, and False if in `{'False', 'false', '0'}`\n\n",
     'author': 'Crystal Melting Dot',
     'author_email': 'stresspassing@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cmd410/OrigamiBot',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `origamibot-2.3.4/PKG-INFO` & `origamibot-2.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: origamibot
-Version: 2.3.4
+Version: 2.3.6
 Summary: Library for creating bots for telegram with Python.
 Home-page: https://github.com/cmd410/OrigamiBot
 License: MIT
 Author: Crystal Melting Dot
 Author-email: stresspassing@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -96,15 +96,15 @@
 
     def on_command_failure(self, message, err=None):  # When command fails
         if err is None:
             self.bot.send_message(message.chat.id,
                                   'Command failed to bind arguments!')
         else:
             self.bot.send_message(message.chat.id,
-                                  'Error in command:\n{err}')
+                                  f'Error in command:\n{err}')
 
 
 if __name__ == '__main__':
     token = (argv[1] if len(argv) > 1 else input('Enter bot token: '))
     bot = Bot(token)   # Create instance of OrigamiBot class
 
     # Add an event listener
```

