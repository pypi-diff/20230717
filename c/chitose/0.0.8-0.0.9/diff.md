# Comparing `tmp/chitose-0.0.8.tar.gz` & `tmp/chitose-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chitose-0.0.8.tar", max compression
+gzip compressed data, was "chitose-0.0.9.tar", max compression
```

## Comparing `chitose-0.0.8.tar` & `chitose-0.0.9.tar`

### file list

```diff
@@ -1,145 +1,145 @@
--rw-r--r--   0        0        0     1073 2023-06-04 10:04:22.655807 chitose-0.0.8/LICENSE
--rw-r--r--   0        0        0     3643 2023-06-04 10:04:22.655807 chitose-0.0.8/README.md
--rw-r--r--   0        0        0      221 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/__init__.py
--rw-r--r--   0        0        0     9519 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/agent.py
--rw-r--r--   0        0        0      551 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/__init__.py
--rw-r--r--   0        0        0     1274 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/__init__.py
--rw-r--r--   0        0        0     2153 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0     5314 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      272 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/get_preferences.py
--rw-r--r--   0        0        0      244 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      255 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0      411 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      682 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/profile.py
--rw-r--r--   0        0        0      424 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/put_preferences.py
--rw-r--r--   0        0        0      425 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      393 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      446 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0     1717 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/embed/external.py
--rw-r--r--   0        0        0     1343 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/embed/images.py
--rw-r--r--   0        0        0     2511 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/embed/record.py
--rw-r--r--   0        0        0     1145 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0     3640 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0     6930 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/defs.py
--rw-r--r--   0        0        0      995 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/describe_feed_generator.py
--rw-r--r--   0        0        0      926 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/generator.py
--rw-r--r--   0        0        0      420 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_actor_feeds.py
--rw-r--r--   0        0        0      397 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0      419 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_feed.py
--rw-r--r--   0        0        0      345 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_feed_generator.py
--rw-r--r--   0        0        0      311 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_feed_generators.py
--rw-r--r--   0        0        0      421 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_feed_skeleton.py
--rw-r--r--   0        0        0      860 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0      385 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      268 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0      411 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0      435 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      480 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/like.py
--rw-r--r--   0        0        0     2470 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/post.py
--rw-r--r--   0        0        0      484 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/feed/repost.py
--rw-r--r--   0        0        0     2981 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      398 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/block.py
--rw-r--r--   0        0        0     2642 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/defs.py
--rw-r--r--   0        0        0      400 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/follow.py
--rw-r--r--   0        0        0      373 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0      395 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0      391 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0      378 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_list.py
--rw-r--r--   0        0        0      386 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_list_mutes.py
--rw-r--r--   0        0        0      406 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_lists.py
--rw-r--r--   0        0        0      356 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0      969 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/list.py
--rw-r--r--   0        0        0      459 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/listitem.py
--rw-r--r--   0        0        0      303 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      300 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/mute_actor_list.py
--rw-r--r--   0        0        0      309 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0      306 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/graph/unmute_actor_list.py
--rw-r--r--   0        0        0     1150 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      301 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1599 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      337 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      449 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0     1327 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0     1022 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0      455 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      303 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/app/bsky/unspecced/get_popular_feed_generators.py
--rw-r--r--   0        0        0      373 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/blob.py
--rw-r--r--   0        0        0      563 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/__init__.py
--rw-r--r--   0        0        0     1253 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/__init__.py
--rw-r--r--   0        0        0     6382 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0    13162 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      396 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/disable_account_invites.py
--rw-r--r--   0        0        0      474 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0      357 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/enable_account_invites.py
--rw-r--r--   0        0        0      452 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      296 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0      462 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      296 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0     1009 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      327 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      267 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      534 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/rebase_repo.py
--rw-r--r--   0        0        0      447 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      396 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0      496 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0     1019 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      436 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      372 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      886 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      335 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      320 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0     1434 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/label/__init__.py
--rw-r--r--   0        0        0     1096 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/label/defs.py
--rw-r--r--   0        0        0      768 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0     1145 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      988 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0      693 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      740 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0     5608 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0     1892 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0      881 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      842 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0      368 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0      651 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1376 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0     1024 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      526 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/rebase_repo.py
--rw-r--r--   0        0        0      392 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      313 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0     4353 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/__init__.py
--rw-r--r--   0        0        0      565 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/create_account.py
--rw-r--r--   0        0        0      725 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      405 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0      785 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0      479 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/create_session.py
--rw-r--r--   0        0        0     1191 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/defs.py
--rw-r--r--   0        0        0      391 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      251 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0      740 2023-06-04 10:04:22.655807 chitose-0.0.8/chitose/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0      454 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      262 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/get_session.py
--rw-r--r--   0        0        0      592 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      260 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      282 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      348 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      365 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      330 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0     4579 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      388 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      345 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      458 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      549 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      314 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      532 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      576 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      551 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0      644 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      488 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      398 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     3266 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0      170 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/link.py
--rw-r--r--   0        0        0      136 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/object.py
--rw-r--r--   0        0        0      136 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/record.py
--rw-r--r--   0        0        0     2206 2023-06-04 10:04:22.659807 chitose-0.0.8/chitose/xrpc.py
--rw-r--r--   0        0        0      823 2023-06-04 10:04:22.659807 chitose-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4481 1970-01-01 00:00:00.000000 chitose-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-10 22:58:32.999990 chitose-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3643 2023-06-10 22:58:32.999990 chitose-0.0.9/README.md
+-rw-r--r--   0        0        0      221 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/__init__.py
+-rw-r--r--   0        0        0     9950 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/agent.py
+-rw-r--r--   0        0        0      560 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/__init__.py
+-rw-r--r--   0        0        0     2153 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     5433 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      272 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/actor/get_preferences.py
+-rw-r--r--   0        0        0      244 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      255 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0      411 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      699 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      424 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/actor/put_preferences.py
+-rw-r--r--   0        0        0      425 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      393 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      446 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1785 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1425 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2596 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1179 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0     3640 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     7134 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0     1029 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/describe_feed_generator.py
+-rw-r--r--   0        0        0      943 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/generator.py
+-rw-r--r--   0        0        0      420 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/get_actor_feeds.py
+-rw-r--r--   0        0        0      397 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0      419 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/get_feed.py
+-rw-r--r--   0        0        0      345 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/get_feed_generator.py
+-rw-r--r--   0        0        0      311 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/get_feed_generators.py
+-rw-r--r--   0        0        0      421 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/get_feed_skeleton.py
+-rw-r--r--   0        0        0      877 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0      385 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      268 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0      411 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0      435 2023-06-10 22:58:32.999990 chitose-0.0.9/chitose/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      511 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2538 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      515 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0     2981 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/block.py
+-rw-r--r--   0        0        0     2710 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/defs.py
+-rw-r--r--   0        0        0      431 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0      373 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0      395 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0      391 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      378 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/get_list.py
+-rw-r--r--   0        0        0      386 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/get_list_mutes.py
+-rw-r--r--   0        0        0      406 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/get_lists.py
+-rw-r--r--   0        0        0      356 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0      986 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/list.py
+-rw-r--r--   0        0        0      490 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/listitem.py
+-rw-r--r--   0        0        0      303 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      300 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/mute_actor_list.py
+-rw-r--r--   0        0        0      309 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      306 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/graph/unmute_actor_list.py
+-rw-r--r--   0        0        0     1150 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1616 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      337 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      449 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1395 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0     1022 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0      455 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      303 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/app/bsky/unspecced/get_popular_feed_generators.py
+-rw-r--r--   0        0        0      407 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/blob.py
+-rw-r--r--   0        0        0      575 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/__init__.py
+-rw-r--r--   0        0        0     1330 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/__init__.py
+-rw-r--r--   0        0        0     6504 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0    13618 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      396 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/disable_account_invites.py
+-rw-r--r--   0        0        0      474 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      357 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/enable_account_invites.py
+-rw-r--r--   0        0        0      452 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      296 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0      462 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      296 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0     1142 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      327 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      267 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      534 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/rebase_repo.py
+-rw-r--r--   0        0        0      447 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      396 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0      496 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0     1019 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      436 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      372 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      886 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      335 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      320 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0     1434 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0     1113 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/label/defs.py
+-rw-r--r--   0        0        0      768 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0     1179 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      988 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0      693 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      740 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0     5608 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     1943 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0      881 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      842 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0      368 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0      651 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1393 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1024 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      526 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/repo/rebase_repo.py
+-rw-r--r--   0        0        0      423 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      313 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0     4353 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0      565 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0      756 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      405 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0      802 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0      479 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1239 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      391 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      251 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0      757 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0      454 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      262 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0      623 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      260 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      282 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      348 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      365 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      330 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0     4579 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      388 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      345 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      458 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      549 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      314 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      532 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      576 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      551 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0      661 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      488 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      398 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     3368 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      205 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/link.py
+-rw-r--r--   0        0        0      169 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/object.py
+-rw-r--r--   0        0        0      169 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/record.py
+-rw-r--r--   0        0        0     2237 2023-06-10 22:58:33.003991 chitose-0.0.9/chitose/xrpc.py
+-rw-r--r--   0        0        0      823 2023-06-10 22:58:33.007991 chitose-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4481 1970-01-01 00:00:00.000000 chitose-0.0.9/PKG-INFO
```

### Comparing `chitose-0.0.8/LICENSE` & `chitose-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/README.md` & `chitose-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/agent.py` & `chitose-0.0.9/chitose/agent.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,33 +22,33 @@
 
 
 class BskyAgent:
     def __init__(self, service: str) -> None:
         self.service = service
         self.session: dict[str, str] = {}
 
-    def _add_auth_header(self, headers: dict[str, str]):
+    def _add_auth_header(self, headers: dict[str, str]) -> dict[str, str]:
         if 'authorization' not in headers and 'accessJwt' in self.session:
             return headers | {
                 'authorization': f'Bearer {self.session["accessJwt"]}'
             }
 
         return headers
 
-    def _refresh_session(self, e: urllib.error.HTTPError):
+    def _refresh_session(self, e: urllib.error.HTTPError) -> None:
         if e.code != 400 or 'refreshJwt' not in self.session:
             raise e
 
         try:
             obj = json.loads(e.read())
         except json.JSONDecodeError:
             raise e
 
         if 'error' not in obj:
-            return e
+            raise e
 
         error = obj['error']
         if error != 'ExpiredToken':
             raise e
 
         self.session = json.loads(
             call('com.atproto.server.refreshSession',
@@ -72,80 +72,80 @@
                    handler: XrpcHandler) -> None:
         # https -> wss
         scheme = urllib.parse.urlparse(self.service).scheme
         service = self.service.replace(scheme, 'wss', 1)
         subscribe(method, params, service, handler)
 
     @property
-    def app(self):
+    def app(self) -> App_:
         return App_(self._call, self._subscribe)
 
     @property
-    def com(self):
+    def com(self) -> Com_:
         return Com_(self._call, self._subscribe)
 
     def get_timeline(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.feed` for available arguments."""
-        return self.app.bsky.feed.get_timeline(**kwargs)
+        return self.app.bsky.feed.get_timeline(**kwargs)  # type: ignore[arg-type]
 
     def get_author_feed(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.feed` for available arguments."""
-        return self.app.bsky.feed.get_author_feed(**kwargs)
+        return self.app.bsky.feed.get_author_feed(**kwargs)  # type: ignore[arg-type]
 
     def get_post_thread(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.feed` for available arguments."""
-        return self.app.bsky.feed.get_post_thread(**kwargs)
+        return self.app.bsky.feed.get_post_thread(**kwargs)  # type: ignore[arg-type]
 
     def get_posts(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.feed` for available arguments."""
-        return self.app.bsky.feed.get_posts(**kwargs)
+        return self.app.bsky.feed.get_posts(**kwargs)  # type: ignore[arg-type]
 
     def get_likes(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.feed` for available arguments."""
-        return self.app.bsky.feed.get_likes(**kwargs)
+        return self.app.bsky.feed.get_likes(**kwargs)  # type: ignore[arg-type]
 
     def get_reposted_by(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.feed` for available arguments."""
-        return self.app.bsky.feed.get_reposted_by(**kwargs)
+        return self.app.bsky.feed.get_reposted_by(**kwargs)  # type: ignore[arg-type]
 
     def get_follows(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.graph` for available arguments."""
-        return self.app.bsky.graph.get_follows(**kwargs)
+        return self.app.bsky.graph.get_follows(**kwargs)  # type: ignore[arg-type]
 
     def get_followers(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.graph` for available arguments."""
-        return self.app.bsky.graph.get_followers(**kwargs)
+        return self.app.bsky.graph.get_followers(**kwargs)  # type: ignore[arg-type]
 
     def get_profile(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.actor` for available arguments."""
-        return self.app.bsky.actor.get_profile(**kwargs)
+        return self.app.bsky.actor.get_profile(**kwargs)  # type: ignore[arg-type]
 
     def get_profiles(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.actor` for available arguments."""
-        return self.app.bsky.actor.get_profiles(**kwargs)
+        return self.app.bsky.actor.get_profiles(**kwargs)  # type: ignore[arg-type]
 
     def get_suggestions(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.actor` for available arguments."""
-        return self.app.bsky.actor.get_suggestions(**kwargs)
+        return self.app.bsky.actor.get_suggestions(**kwargs)  # type: ignore[arg-type]
 
     def search_actors(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.actor` for available arguments."""
-        return self.app.bsky.actor.search_actors(**kwargs)
+        return self.app.bsky.actor.search_actors(**kwargs)  # type: ignore[arg-type]
 
     def search_actors_typeahead(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.actor` for available arguments."""
-        return self.app.bsky.actor.search_actors_typeahead(**kwargs)
+        return self.app.bsky.actor.search_actors_typeahead(**kwargs)  # type: ignore[arg-type]
 
     def list_notifications(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See :doc:`chitose.app.bsky.notification` for available arguments."""
-        return self.app.bsky.notification.list_notifications(**kwargs)
+        return self.app.bsky.notification.list_notifications(**kwargs)  # type: ignore[arg-type]
 
     def count_unread_notifications(self, **kwargs: dict[str, typing.Any]) -> bytes:
         """See `get_unread_count()` in :doc:`chitose.app.bsky.notification` for available arguments."""
-        return self.app.bsky.notification.get_unread_count(**kwargs)
+        return self.app.bsky.notification.get_unread_count(**kwargs)  # type: ignore[arg-type]
 
     def post(self, record: Post) -> bytes:
         if not self.session:
             raise Exception('Not logged in')
 
         return self.com.atproto.repo.create_record(
             repo=self.session['did'],
```

### Comparing `chitose-0.0.8/chitose/app/__init__.py` & `chitose-0.0.9/chitose/app/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,9 +8,9 @@
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
     def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
         self.subscribe = subscribe
 
     @property
-    def bsky(self):
+    def bsky(self) -> Bsky_:
         return Bsky_(self.call, self.subscribe)
```

### Comparing `chitose-0.0.8/chitose/app/bsky/__init__.py` & `chitose-0.0.9/chitose/com/atproto/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 # GENERATED CODE - DO NOT MODIFY
 from __future__ import annotations
 from chitose.xrpc import XrpcCall
 from chitose.xrpc import XrpcSubscribe
-from .actor import Actor_
-from .embed import Embed_
-from .feed import Feed_
-from .graph import Graph_
-from .notification import Notification_
-from .richtext import Richtext_
-from .unspecced import Unspecced_
+from .admin import Admin_
+from .identity import Identity_
+from .label import Label_
+from .moderation import Moderation_
+from .repo import Repo_
+from .server import Server_
+from .sync import Sync_
 
-class Bsky_:
+class Atproto_:
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
     def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
         self.subscribe = subscribe
 
     @property
-    def actor(self):
-        return Actor_(self.call, self.subscribe)
+    def admin(self) -> Admin_:
+        return Admin_(self.call, self.subscribe)
 
     @property
-    def embed(self):
-        return Embed_(self.call, self.subscribe)
+    def identity(self) -> Identity_:
+        return Identity_(self.call, self.subscribe)
 
     @property
-    def feed(self):
-        return Feed_(self.call, self.subscribe)
+    def label(self) -> Label_:
+        return Label_(self.call, self.subscribe)
 
     @property
-    def graph(self):
-        return Graph_(self.call, self.subscribe)
+    def moderation(self) -> Moderation_:
+        return Moderation_(self.call, self.subscribe)
 
     @property
-    def notification(self):
-        return Notification_(self.call, self.subscribe)
+    def repo(self) -> Repo_:
+        return Repo_(self.call, self.subscribe)
 
     @property
-    def richtext(self):
-        return Richtext_(self.call, self.subscribe)
+    def server(self) -> Server_:
+        return Server_(self.call, self.subscribe)
 
     @property
-    def unspecced(self):
-        return Unspecced_(self.call, self.subscribe)
+    def sync(self) -> Sync_:
+        return Sync_(self.call, self.subscribe)
```

### Comparing `chitose-0.0.8/chitose/app/bsky/actor/__init__.py` & `chitose-0.0.9/chitose/app/bsky/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/app/bsky/actor/defs.py` & `chitose-0.0.9/chitose/app/bsky/actor/defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.did = did
         self.handle = handle
         self.display_name = display_name
         self.avatar = avatar
         self.viewer = viewer
         self.labels = labels
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'did': self.did, 'handle': self.handle, 'displayName': self.display_name, 'avatar': self.avatar, 'viewer': self.viewer, 'labels': self.labels, '$type': 'app.bsky.actor.defs#profileViewBasic'}
 
 class ProfileView(chitose.Object):
     """"""
 
     def __init__(self, did: str, handle: str, display_name: typing.Optional[str]=None, description: typing.Optional[str]=None, avatar: typing.Optional[str]=None, indexed_at: typing.Optional[str]=None, viewer: typing.Optional[chitose.app.bsky.actor.defs.ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.did = did
@@ -30,15 +30,15 @@
         self.display_name = display_name
         self.description = description
         self.avatar = avatar
         self.indexed_at = indexed_at
         self.viewer = viewer
         self.labels = labels
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'did': self.did, 'handle': self.handle, 'displayName': self.display_name, 'description': self.description, 'avatar': self.avatar, 'indexedAt': self.indexed_at, 'viewer': self.viewer, 'labels': self.labels, '$type': 'app.bsky.actor.defs#profileView'}
 
 class ProfileViewDetailed(chitose.Object):
     """"""
 
     def __init__(self, did: str, handle: str, display_name: typing.Optional[str]=None, description: typing.Optional[str]=None, avatar: typing.Optional[str]=None, banner: typing.Optional[str]=None, followers_count: typing.Optional[int]=None, follows_count: typing.Optional[int]=None, posts_count: typing.Optional[int]=None, indexed_at: typing.Optional[str]=None, viewer: typing.Optional[chitose.app.bsky.actor.defs.ViewerState]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.did = did
@@ -50,53 +50,53 @@
         self.followers_count = followers_count
         self.follows_count = follows_count
         self.posts_count = posts_count
         self.indexed_at = indexed_at
         self.viewer = viewer
         self.labels = labels
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'did': self.did, 'handle': self.handle, 'displayName': self.display_name, 'description': self.description, 'avatar': self.avatar, 'banner': self.banner, 'followersCount': self.followers_count, 'followsCount': self.follows_count, 'postsCount': self.posts_count, 'indexedAt': self.indexed_at, 'viewer': self.viewer, 'labels': self.labels, '$type': 'app.bsky.actor.defs#profileViewDetailed'}
 
 class ViewerState(chitose.Object):
     """"""
 
     def __init__(self, muted: typing.Optional[bool]=None, muted_by_list: typing.Optional[chitose.app.bsky.graph.defs.ListViewBasic]=None, blocked_by: typing.Optional[bool]=None, blocking: typing.Optional[str]=None, following: typing.Optional[str]=None, followed_by: typing.Optional[str]=None) -> None:
         self.muted = muted
         self.muted_by_list = muted_by_list
         self.blocked_by = blocked_by
         self.blocking = blocking
         self.following = following
         self.followed_by = followed_by
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'muted': self.muted, 'mutedByList': self.muted_by_list, 'blockedBy': self.blocked_by, 'blocking': self.blocking, 'following': self.following, 'followedBy': self.followed_by, '$type': 'app.bsky.actor.defs#viewerState'}
 Preferences = list[typing.Union['chitose.app.bsky.actor.defs.AdultContentPref', 'chitose.app.bsky.actor.defs.ContentLabelPref', 'chitose.app.bsky.actor.defs.SavedFeedsPref']]
 
 class AdultContentPref(chitose.Object):
     """"""
 
     def __init__(self, enabled: bool) -> None:
         self.enabled = enabled
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'enabled': self.enabled, '$type': 'app.bsky.actor.defs#adultContentPref'}
 
 class ContentLabelPref(chitose.Object):
     """"""
 
     def __init__(self, label: str, visibility: typing.Literal['show', 'warn', 'hide']) -> None:
         self.label = label
         self.visibility = visibility
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'label': self.label, 'visibility': self.visibility, '$type': 'app.bsky.actor.defs#contentLabelPref'}
 
 class SavedFeedsPref(chitose.Object):
     """"""
 
     def __init__(self, pinned: list[str], saved: list[str]) -> None:
         self.pinned = pinned
         self.saved = saved
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'pinned': self.pinned, 'saved': self.saved, '$type': 'app.bsky.actor.defs#savedFeedsPref'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/actor/profile.py` & `chitose-0.0.9/chitose/app/bsky/actor/profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
     def __init__(self, display_name: typing.Optional[str]=None, description: typing.Optional[str]=None, avatar: typing.Optional[chitose.Blob]=None, banner: typing.Optional[chitose.Blob]=None) -> None:
         self.display_name = display_name
         self.description = description
         self.avatar = avatar
         self.banner = banner
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'displayName': self.display_name, 'description': self.description, 'avatar': self.avatar, 'banner': self.banner, '$type': 'app.bsky.actor.profile'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/embed/external.py` & `chitose-0.0.9/chitose/app/bsky/embed/external.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,42 +7,42 @@
 
 class External(chitose.Object):
     """"""
 
     def __init__(self, external: chitose.app.bsky.embed.external.ExternalExternal) -> None:
         self.external = external
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'external': self.external, '$type': 'app.bsky.embed.external'}
 
 class ExternalExternal(chitose.Object):
     """"""
 
     def __init__(self, uri: str, title: str, description: str, thumb: typing.Optional[chitose.Blob]=None) -> None:
         self.uri = uri
         self.title = title
         self.description = description
         self.thumb = thumb
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, 'title': self.title, 'description': self.description, 'thumb': self.thumb, '$type': 'app.bsky.embed.external#external'}
 
 class View(chitose.Object):
     """"""
 
     def __init__(self, external: chitose.app.bsky.embed.external.ViewExternal) -> None:
         self.external = external
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'external': self.external, '$type': 'app.bsky.embed.external#view'}
 
 class ViewExternal(chitose.Object):
     """"""
 
     def __init__(self, uri: str, title: str, description: str, thumb: typing.Optional[str]=None) -> None:
         self.uri = uri
         self.title = title
         self.description = description
         self.thumb = thumb
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, 'title': self.title, 'description': self.description, 'thumb': self.thumb, '$type': 'app.bsky.embed.external#viewExternal'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/embed/images.py` & `chitose-0.0.9/chitose/app/bsky/embed/images.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 # GENERATED CODE - DO NOT MODIFY
 """A set of images embedded in some other form of content"""
 from __future__ import annotations
 import chitose
 import chitose.app.bsky.embed.images
+import typing
 
 class Images(chitose.Object):
     """"""
 
     def __init__(self, images: list[chitose.app.bsky.embed.images.Image]) -> None:
         self.images = images
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'images': self.images, '$type': 'app.bsky.embed.images'}
 
 class Image(chitose.Object):
     """"""
 
     def __init__(self, image: chitose.Blob, alt: str) -> None:
         self.image = image
         self.alt = alt
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'image': self.image, 'alt': self.alt, '$type': 'app.bsky.embed.images#image'}
 
 class View(chitose.Object):
     """"""
 
     def __init__(self, images: list[chitose.app.bsky.embed.images.ViewImage]) -> None:
         self.images = images
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'images': self.images, '$type': 'app.bsky.embed.images#view'}
 
 class ViewImage(chitose.Object):
     """"""
 
     def __init__(self, thumb: str, fullsize: str, alt: str) -> None:
         self.thumb = thumb
         self.fullsize = fullsize
         self.alt = alt
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'thumb': self.thumb, 'fullsize': self.fullsize, 'alt': self.alt, '$type': 'app.bsky.embed.images#viewImage'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/embed/record.py` & `chitose-0.0.9/chitose/app/bsky/embed/record.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,51 +14,51 @@
 
 class Record(chitose.Object):
     """"""
 
     def __init__(self, record: chitose.com.atproto.repo.strong_ref.StrongRef) -> None:
         self.record = record
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'record': self.record, '$type': 'app.bsky.embed.record'}
 
 class View(chitose.Object):
     """"""
 
     def __init__(self, record: typing.Union[chitose.app.bsky.embed.record.ViewRecord, chitose.app.bsky.embed.record.ViewNotFound, chitose.app.bsky.embed.record.ViewBlocked, chitose.app.bsky.feed.defs.GeneratorView]) -> None:
         self.record = record
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'record': self.record, '$type': 'app.bsky.embed.record#view'}
 
 class ViewRecord(chitose.Object):
     """"""
 
     def __init__(self, uri: str, cid: str, author: chitose.app.bsky.actor.defs.ProfileViewBasic, value: typing.Any, indexed_at: str, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None, embeds: typing.Optional[list[typing.Union[chitose.app.bsky.embed.images.View, chitose.app.bsky.embed.external.View, chitose.app.bsky.embed.record.View, chitose.app.bsky.embed.record_with_media.View]]]=None) -> None:
         self.uri = uri
         self.cid = cid
         self.author = author
         self.value = value
         self.indexed_at = indexed_at
         self.labels = labels
         self.embeds = embeds
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, 'cid': self.cid, 'author': self.author, 'value': self.value, 'indexedAt': self.indexed_at, 'labels': self.labels, 'embeds': self.embeds, '$type': 'app.bsky.embed.record#viewRecord'}
 
 class ViewNotFound(chitose.Object):
     """"""
 
     def __init__(self, uri: str) -> None:
         self.uri = uri
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, '$type': 'app.bsky.embed.record#viewNotFound'}
 
 class ViewBlocked(chitose.Object):
     """"""
 
     def __init__(self, uri: str) -> None:
         self.uri = uri
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, '$type': 'app.bsky.embed.record#viewBlocked'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/embed/record_with_media.py` & `chitose-0.0.9/chitose/app/bsky/embed/record_with_media.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 class RecordWithMedia(chitose.Object):
     """"""
 
     def __init__(self, record: chitose.app.bsky.embed.record.Record, media: typing.Union[chitose.app.bsky.embed.images.Images, chitose.app.bsky.embed.external.External]) -> None:
         self.record = record
         self.media = media
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'record': self.record, 'media': self.media, '$type': 'app.bsky.embed.recordWithMedia'}
 
 class View(chitose.Object):
     """"""
 
     def __init__(self, record: chitose.app.bsky.embed.record.View, media: typing.Union[chitose.app.bsky.embed.images.View, chitose.app.bsky.embed.external.View]) -> None:
         self.record = record
         self.media = media
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'record': self.record, 'media': self.media, '$type': 'app.bsky.embed.recordWithMedia#view'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/feed/__init__.py` & `chitose-0.0.9/chitose/app/bsky/feed/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/app/bsky/feed/defs.py` & `chitose-0.0.9/chitose/app/bsky/feed/defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,87 +24,87 @@
         self.embed = embed
         self.reply_count = reply_count
         self.repost_count = repost_count
         self.like_count = like_count
         self.viewer = viewer
         self.labels = labels
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, 'cid': self.cid, 'author': self.author, 'record': self.record, 'indexedAt': self.indexed_at, 'embed': self.embed, 'replyCount': self.reply_count, 'repostCount': self.repost_count, 'likeCount': self.like_count, 'viewer': self.viewer, 'labels': self.labels, '$type': 'app.bsky.feed.defs#postView'}
 
 class ViewerState(chitose.Object):
     """"""
 
     def __init__(self, repost: typing.Optional[str]=None, like: typing.Optional[str]=None) -> None:
         self.repost = repost
         self.like = like
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'repost': self.repost, 'like': self.like, '$type': 'app.bsky.feed.defs#viewerState'}
 
 class FeedViewPost(chitose.Object):
     """"""
 
     def __init__(self, post: chitose.app.bsky.feed.defs.PostView, reply: typing.Optional[chitose.app.bsky.feed.defs.ReplyRef]=None, reason: typing.Optional[chitose.app.bsky.feed.defs.ReasonRepost]=None) -> None:
         self.post = post
         self.reply = reply
         self.reason = reason
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'post': self.post, 'reply': self.reply, 'reason': self.reason, '$type': 'app.bsky.feed.defs#feedViewPost'}
 
 class ReplyRef(chitose.Object):
     """"""
 
     def __init__(self, root: typing.Union[chitose.app.bsky.feed.defs.PostView, chitose.app.bsky.feed.defs.NotFoundPost, chitose.app.bsky.feed.defs.BlockedPost], parent: typing.Union[chitose.app.bsky.feed.defs.PostView, chitose.app.bsky.feed.defs.NotFoundPost, chitose.app.bsky.feed.defs.BlockedPost]) -> None:
         self.root = root
         self.parent = parent
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'root': self.root, 'parent': self.parent, '$type': 'app.bsky.feed.defs#replyRef'}
 
 class ReasonRepost(chitose.Object):
     """"""
 
     def __init__(self, by: chitose.app.bsky.actor.defs.ProfileViewBasic, indexed_at: str) -> None:
         self.by = by
         self.indexed_at = indexed_at
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'by': self.by, 'indexedAt': self.indexed_at, '$type': 'app.bsky.feed.defs#reasonRepost'}
 
 class ThreadViewPost(chitose.Object):
     """"""
 
     def __init__(self, post: chitose.app.bsky.feed.defs.PostView, parent: typing.Optional[typing.Union[chitose.app.bsky.feed.defs.ThreadViewPost, chitose.app.bsky.feed.defs.NotFoundPost, chitose.app.bsky.feed.defs.BlockedPost]]=None, replies: typing.Optional[list[typing.Union[chitose.app.bsky.feed.defs.ThreadViewPost, chitose.app.bsky.feed.defs.NotFoundPost, chitose.app.bsky.feed.defs.BlockedPost]]]=None) -> None:
         self.post = post
         self.parent = parent
         self.replies = replies
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'post': self.post, 'parent': self.parent, 'replies': self.replies, '$type': 'app.bsky.feed.defs#threadViewPost'}
 
 class NotFoundPost(chitose.Object):
     """"""
 
     def __init__(self, uri: str, not_found: bool) -> None:
         self.uri = uri
         self.not_found = not_found
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, 'notFound': self.not_found, '$type': 'app.bsky.feed.defs#notFoundPost'}
 
 class BlockedPost(chitose.Object):
     """"""
 
     def __init__(self, uri: str, blocked: bool) -> None:
         self.uri = uri
         self.blocked = blocked
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, 'blocked': self.blocked, '$type': 'app.bsky.feed.defs#blockedPost'}
 
 class GeneratorView(chitose.Object):
     """"""
 
     def __init__(self, uri: str, cid: str, creator: chitose.app.bsky.actor.defs.ProfileView, display_name: str, indexed_at: str, did: typing.Optional[str]=None, description: typing.Optional[str]=None, description_facets: typing.Optional[list[chitose.app.bsky.richtext.facet.Facet]]=None, avatar: typing.Optional[str]=None, like_count: typing.Optional[int]=None, viewer: typing.Optional[chitose.app.bsky.feed.defs.GeneratorViewerState]=None) -> None:
         self.uri = uri
@@ -115,37 +115,37 @@
         self.did = did
         self.description = description
         self.description_facets = description_facets
         self.avatar = avatar
         self.like_count = like_count
         self.viewer = viewer
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, 'cid': self.cid, 'creator': self.creator, 'displayName': self.display_name, 'indexedAt': self.indexed_at, 'did': self.did, 'description': self.description, 'descriptionFacets': self.description_facets, 'avatar': self.avatar, 'likeCount': self.like_count, 'viewer': self.viewer, '$type': 'app.bsky.feed.defs#generatorView'}
 
 class GeneratorViewerState(chitose.Object):
     """"""
 
     def __init__(self, like: typing.Optional[str]=None) -> None:
         self.like = like
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'like': self.like, '$type': 'app.bsky.feed.defs#generatorViewerState'}
 
 class SkeletonFeedPost(chitose.Object):
     """"""
 
     def __init__(self, post: str, reason: typing.Optional[chitose.app.bsky.feed.defs.SkeletonReasonRepost]=None) -> None:
         self.post = post
         self.reason = reason
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'post': self.post, 'reason': self.reason, '$type': 'app.bsky.feed.defs#skeletonFeedPost'}
 
 class SkeletonReasonRepost(chitose.Object):
     """"""
 
     def __init__(self, repost: str) -> None:
         self.repost = repost
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'repost': self.repost, '$type': 'app.bsky.feed.defs#skeletonReasonRepost'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/feed/describe_feed_generator.py` & `chitose-0.0.9/chitose/com/atproto/server/describe_server.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _describe_feed_generator(call: chitose.xrpc.XrpcCall) -> bytes:
-    """Returns information about a given feed generator including TOS & offered feed URIs"""
-    return call('app.bsky.feed.describeFeedGenerator', [], None, {})
-
-class Feed(chitose.Object):
-    """"""
-
-    def __init__(self, uri: str) -> None:
-        self.uri = uri
-
-    def to_dict(self) -> dict:
-        return {'uri': self.uri, '$type': 'app.bsky.feed.describeFeedGenerator#feed'}
+def _describe_server(call: chitose.xrpc.XrpcCall) -> bytes:
+    """Get a document describing the service's accounts configuration."""
+    return call('com.atproto.server.describeServer', [], None, {})
 
 class Links(chitose.Object):
     """"""
 
     def __init__(self, privacy_policy: typing.Optional[str]=None, terms_of_service: typing.Optional[str]=None) -> None:
         self.privacy_policy = privacy_policy
         self.terms_of_service = terms_of_service
 
-    def to_dict(self) -> dict:
-        return {'privacyPolicy': self.privacy_policy, 'termsOfService': self.terms_of_service, '$type': 'app.bsky.feed.describeFeedGenerator#links'}
+    def to_dict(self) -> dict[str, typing.Any]:
+        return {'privacyPolicy': self.privacy_policy, 'termsOfService': self.terms_of_service, '$type': 'com.atproto.server.describeServer#links'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/feed/generator.py` & `chitose-0.0.9/chitose/app/bsky/feed/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,9 +12,9 @@
         self.did = did
         self.display_name = display_name
         self.created_at = created_at
         self.description = description
         self.description_facets = description_facets
         self.avatar = avatar
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'did': self.did, 'displayName': self.display_name, 'createdAt': self.created_at, 'description': self.description, 'descriptionFacets': self.description_facets, 'avatar': self.avatar, '$type': 'app.bsky.feed.generator'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/feed/get_likes.py` & `chitose-0.0.9/chitose/app/bsky/feed/get_likes.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,9 +13,9 @@
     """"""
 
     def __init__(self, indexed_at: str, created_at: str, actor: chitose.app.bsky.actor.defs.ProfileView) -> None:
         self.indexed_at = indexed_at
         self.created_at = created_at
         self.actor = actor
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'indexedAt': self.indexed_at, 'createdAt': self.created_at, 'actor': self.actor, '$type': 'app.bsky.feed.getLikes#like'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/feed/post.py` & `chitose-0.0.9/chitose/app/bsky/feed/post.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,44 +22,44 @@
         self.text = text
         self.created_at = created_at
         self.entities = entities
         self.facets = facets
         self.reply = reply
         self.embed = embed
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'text': self.text, 'createdAt': self.created_at, 'entities': self.entities, 'facets': self.facets, 'reply': self.reply, 'embed': self.embed, '$type': 'app.bsky.feed.post'}
 
 class ReplyRef(chitose.Object):
     """"""
 
     def __init__(self, root: chitose.com.atproto.repo.strong_ref.StrongRef, parent: chitose.com.atproto.repo.strong_ref.StrongRef) -> None:
         self.root = root
         self.parent = parent
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'root': self.root, 'parent': self.parent, '$type': 'app.bsky.feed.post#replyRef'}
 
 class Entity(chitose.Object):
     """
 
 
     :param type: Expected values are 'mention' and 'link'.
     """
 
     def __init__(self, index: chitose.app.bsky.feed.post.TextSlice, type: str, value: str) -> None:
         self.index = index
         self.type = type
         self.value = value
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'index': self.index, 'type': self.type, 'value': self.value, '$type': 'app.bsky.feed.post#entity'}
 
 class TextSlice(chitose.Object):
     """"""
 
     def __init__(self, start: int, end: int) -> None:
         self.start = start
         self.end = end
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'start': self.start, 'end': self.end, '$type': 'app.bsky.feed.post#textSlice'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/graph/__init__.py` & `chitose-0.0.9/chitose/app/bsky/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/app/bsky/graph/defs.py` & `chitose-0.0.9/chitose/app/bsky/graph/defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.uri = uri
         self.name = name
         self.purpose = purpose
         self.avatar = avatar
         self.viewer = viewer
         self.indexed_at = indexed_at
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, 'name': self.name, 'purpose': self.purpose, 'avatar': self.avatar, 'viewer': self.viewer, 'indexedAt': self.indexed_at, '$type': 'app.bsky.graph.defs#listViewBasic'}
 
 class ListView(chitose.Object):
     """"""
 
     def __init__(self, uri: str, creator: chitose.app.bsky.actor.defs.ProfileView, name: str, purpose: chitose.app.bsky.graph.defs.ListPurpose, indexed_at: str, description: typing.Optional[str]=None, description_facets: typing.Optional[list[chitose.app.bsky.richtext.facet.Facet]]=None, avatar: typing.Optional[str]=None, viewer: typing.Optional[chitose.app.bsky.graph.defs.ListViewerState]=None) -> None:
         self.uri = uri
@@ -31,29 +31,29 @@
         self.purpose = purpose
         self.indexed_at = indexed_at
         self.description = description
         self.description_facets = description_facets
         self.avatar = avatar
         self.viewer = viewer
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, 'creator': self.creator, 'name': self.name, 'purpose': self.purpose, 'indexedAt': self.indexed_at, 'description': self.description, 'descriptionFacets': self.description_facets, 'avatar': self.avatar, 'viewer': self.viewer, '$type': 'app.bsky.graph.defs#listView'}
 
 class ListItemView(chitose.Object):
     """"""
 
     def __init__(self, subject: chitose.app.bsky.actor.defs.ProfileView) -> None:
         self.subject = subject
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'subject': self.subject, '$type': 'app.bsky.graph.defs#listItemView'}
 ListPurpose = typing.Literal['app.bsky.graph.defs#modlist',]
 MODLIST = 'app.bsky.graph.defs#modlist'
 
 class ListViewerState(chitose.Object):
     """"""
 
     def __init__(self, muted: typing.Optional[bool]=None) -> None:
         self.muted = muted
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'muted': self.muted, '$type': 'app.bsky.graph.defs#listViewerState'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/graph/list.py` & `chitose-0.0.9/chitose/app/bsky/graph/list.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,9 +13,9 @@
         self.purpose = purpose
         self.name = name
         self.created_at = created_at
         self.description = description
         self.description_facets = description_facets
         self.avatar = avatar
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'purpose': self.purpose, 'name': self.name, 'createdAt': self.created_at, 'description': self.description, 'descriptionFacets': self.description_facets, 'avatar': self.avatar, '$type': 'app.bsky.graph.list'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/notification/__init__.py` & `chitose-0.0.9/chitose/app/bsky/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/app/bsky/notification/list_notifications.py` & `chitose-0.0.9/chitose/app/bsky/notification/list_notifications.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,9 +24,9 @@
         self.reason = reason
         self.record = record
         self.is_read = is_read
         self.indexed_at = indexed_at
         self.reason_subject = reason_subject
         self.labels = labels
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, 'cid': self.cid, 'author': self.author, 'reason': self.reason, 'record': self.record, 'isRead': self.is_read, 'indexedAt': self.indexed_at, 'reasonSubject': self.reason_subject, 'labels': self.labels, '$type': 'app.bsky.notification.listNotifications#notification'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/richtext/facet.py` & `chitose-0.0.9/chitose/app/bsky/richtext/facet.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 class Facet(chitose.Object):
     """"""
 
     def __init__(self, index: chitose.app.bsky.richtext.facet.ByteSlice, features: list[typing.Union[chitose.app.bsky.richtext.facet.Mention, chitose.app.bsky.richtext.facet.Link]]) -> None:
         self.index = index
         self.features = features
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'index': self.index, 'features': self.features, '$type': 'app.bsky.richtext.facet'}
 
 class Mention(chitose.Object):
     """"""
 
     def __init__(self, did: str) -> None:
         self.did = did
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'did': self.did, '$type': 'app.bsky.richtext.facet#mention'}
 
 class Link(chitose.Object):
     """"""
 
     def __init__(self, uri: str) -> None:
         self.uri = uri
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, '$type': 'app.bsky.richtext.facet#link'}
 
 class ByteSlice(chitose.Object):
     """"""
 
     def __init__(self, byte_start: int, byte_end: int) -> None:
         self.byte_start = byte_start
         self.byte_end = byte_end
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'byteStart': self.byte_start, 'byteEnd': self.byte_end, '$type': 'app.bsky.richtext.facet#byteSlice'}
```

### Comparing `chitose-0.0.8/chitose/app/bsky/unspecced/__init__.py` & `chitose-0.0.9/chitose/app/bsky/unspecced/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/__init__.py` & `chitose-0.0.9/chitose/com/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,9 +8,9 @@
     """We recommend calling methods in this class via the :doc:`chitose.BskyAgent <chitose>` class instead of creating instances of this class directly."""
 
     def __init__(self, call: XrpcCall, subscribe: XrpcSubscribe) -> None:
         self.call = call
         self.subscribe = subscribe
 
     @property
-    def atproto(self):
+    def atproto(self) -> Atproto_:
         return Atproto_(self.call, self.subscribe)
```

### Comparing `chitose-0.0.8/chitose/com/atproto/admin/__init__.py` & `chitose-0.0.9/chitose/com/atproto/admin/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,21 +30,23 @@
         self.call = call
         self.subscribe = subscribe
 
     def get_repo(self, did: str) -> bytes:
         """View details about a repository."""
         return _get_repo(self.call, did)
 
-    def get_moderation_reports(self, subject: typing.Optional[str]=None, ignore_subjects: typing.Optional[list[str]]=None, resolved: typing.Optional[bool]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, reverse: typing.Optional[bool]=None) -> bytes:
+    def get_moderation_reports(self, subject: typing.Optional[str]=None, ignore_subjects: typing.Optional[list[str]]=None, reporters: typing.Optional[list[str]]=None, resolved: typing.Optional[bool]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, reverse: typing.Optional[bool]=None) -> bytes:
         """List moderation reports related to a subject.
 
 
+        :param reporters: Filter reports made by one or more DIDs
+
         :param reverse: Reverse the order of the returned records? when true, returns reports in chronological order
         """
-        return _get_moderation_reports(self.call, subject, ignore_subjects, resolved, action_type, limit, cursor, reverse)
+        return _get_moderation_reports(self.call, subject, ignore_subjects, reporters, resolved, action_type, limit, cursor, reverse)
 
     def take_moderation_action(self, action: typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge'], subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reason: str, created_by: str, subject_blob_cids: typing.Optional[list[str]]=None, create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None) -> bytes:
         """Take a moderation action on a repo."""
         return _take_moderation_action(self.call, action, subject, reason, created_by, subject_blob_cids, create_label_vals, negate_label_vals)
 
     def update_account_email(self, account: str, email: str) -> bytes:
         """Administrative action to update an account's email
```

### Comparing `chitose-0.0.8/chitose/com/atproto/admin/defs.py` & `chitose-0.0.9/chitose/com/atproto/admin/defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.created_by = created_by
         self.created_at = created_at
         self.resolved_report_ids = resolved_report_ids
         self.create_label_vals = create_label_vals
         self.negate_label_vals = negate_label_vals
         self.reversal = reversal
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'id': self.id, 'action': self.action, 'subject': self.subject, 'subjectBlobCids': self.subject_blob_cids, 'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at, 'resolvedReportIds': self.resolved_report_ids, 'createLabelVals': self.create_label_vals, 'negateLabelVals': self.negate_label_vals, 'reversal': self.reversal, '$type': 'com.atproto.admin.defs#actionView'}
 
 class ActionViewDetail(chitose.Object):
     """"""
 
     def __init__(self, id: int, action: chitose.com.atproto.admin.defs.ActionType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoView, chitose.com.atproto.admin.defs.RepoViewNotFound, chitose.com.atproto.admin.defs.RecordView, chitose.com.atproto.admin.defs.RecordViewNotFound], subject_blobs: list[chitose.com.atproto.admin.defs.BlobView], reason: str, created_by: str, created_at: str, resolved_reports: list[chitose.com.atproto.admin.defs.ReportView], create_label_vals: typing.Optional[list[str]]=None, negate_label_vals: typing.Optional[list[str]]=None, reversal: typing.Optional[chitose.com.atproto.admin.defs.ActionReversal]=None) -> None:
         self.id = id
@@ -40,71 +40,72 @@
         self.created_by = created_by
         self.created_at = created_at
         self.resolved_reports = resolved_reports
         self.create_label_vals = create_label_vals
         self.negate_label_vals = negate_label_vals
         self.reversal = reversal
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'id': self.id, 'action': self.action, 'subject': self.subject, 'subjectBlobs': self.subject_blobs, 'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at, 'resolvedReports': self.resolved_reports, 'createLabelVals': self.create_label_vals, 'negateLabelVals': self.negate_label_vals, 'reversal': self.reversal, '$type': 'com.atproto.admin.defs#actionViewDetail'}
 
 class ActionViewCurrent(chitose.Object):
     """"""
 
     def __init__(self, id: int, action: chitose.com.atproto.admin.defs.ActionType) -> None:
         self.id = id
         self.action = action
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'id': self.id, 'action': self.action, '$type': 'com.atproto.admin.defs#actionViewCurrent'}
 
 class ActionReversal(chitose.Object):
     """"""
 
     def __init__(self, reason: str, created_by: str, created_at: str) -> None:
         self.reason = reason
         self.created_by = created_by
         self.created_at = created_at
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'reason': self.reason, 'createdBy': self.created_by, 'createdAt': self.created_at, '$type': 'com.atproto.admin.defs#actionReversal'}
 ActionType = typing.Literal['#takedown', '#flag', '#acknowledge', '#escalate']
 TAKEDOWN = 'com.atproto.admin.defs#takedown'
 FLAG = 'com.atproto.admin.defs#flag'
 ACKNOWLEDGE = 'com.atproto.admin.defs#acknowledge'
 ESCALATE = 'com.atproto.admin.defs#escalate'
 
 class ReportView(chitose.Object):
     """"""
 
-    def __init__(self, id: int, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reported_by: str, created_at: str, resolved_by_action_ids: list[int], reason: typing.Optional[str]=None) -> None:
+    def __init__(self, id: int, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoRef, chitose.com.atproto.repo.strong_ref.StrongRef], reported_by: str, created_at: str, resolved_by_action_ids: list[int], reason: typing.Optional[str]=None, subject_repo_handle: typing.Optional[str]=None) -> None:
         self.id = id
         self.reason_type = reason_type
         self.subject = subject
         self.reported_by = reported_by
         self.created_at = created_at
         self.resolved_by_action_ids = resolved_by_action_ids
         self.reason = reason
+        self.subject_repo_handle = subject_repo_handle
 
-    def to_dict(self) -> dict:
-        return {'id': self.id, 'reasonType': self.reason_type, 'subject': self.subject, 'reportedBy': self.reported_by, 'createdAt': self.created_at, 'resolvedByActionIds': self.resolved_by_action_ids, 'reason': self.reason, '$type': 'com.atproto.admin.defs#reportView'}
+    def to_dict(self) -> dict[str, typing.Any]:
+        return {'id': self.id, 'reasonType': self.reason_type, 'subject': self.subject, 'reportedBy': self.reported_by, 'createdAt': self.created_at, 'resolvedByActionIds': self.resolved_by_action_ids, 'reason': self.reason, 'subjectRepoHandle': self.subject_repo_handle, '$type': 'com.atproto.admin.defs#reportView'}
 
 class ReportViewDetail(chitose.Object):
     """"""
 
     def __init__(self, id: int, reason_type: chitose.com.atproto.moderation.defs.ReasonType, subject: typing.Union[chitose.com.atproto.admin.defs.RepoView, chitose.com.atproto.admin.defs.RepoViewNotFound, chitose.com.atproto.admin.defs.RecordView, chitose.com.atproto.admin.defs.RecordViewNotFound], reported_by: str, created_at: str, resolved_by_actions: list[chitose.com.atproto.admin.defs.ActionView], reason: typing.Optional[str]=None) -> None:
         self.id = id
         self.reason_type = reason_type
         self.subject = subject
         self.reported_by = reported_by
         self.created_at = created_at
         self.resolved_by_actions = resolved_by_actions
         self.reason = reason
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'id': self.id, 'reasonType': self.reason_type, 'subject': self.subject, 'reportedBy': self.reported_by, 'createdAt': self.created_at, 'resolvedByActions': self.resolved_by_actions, 'reason': self.reason, '$type': 'com.atproto.admin.defs#reportViewDetail'}
 
 class RepoView(chitose.Object):
     """"""
 
     def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.Moderation, email: typing.Optional[str]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None, invites_disabled: typing.Optional[bool]=None) -> None:
         self.did = did
@@ -112,15 +113,15 @@
         self.related_records = related_records
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.email = email
         self.invited_by = invited_by
         self.invites_disabled = invites_disabled
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'did': self.did, 'handle': self.handle, 'relatedRecords': self.related_records, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'email': self.email, 'invitedBy': self.invited_by, 'invitesDisabled': self.invites_disabled, '$type': 'com.atproto.admin.defs#repoView'}
 
 class RepoViewDetail(chitose.Object):
     """"""
 
     def __init__(self, did: str, handle: str, related_records: list[typing.Any], indexed_at: str, moderation: chitose.com.atproto.admin.defs.ModerationDetail, email: typing.Optional[str]=None, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None, invited_by: typing.Optional[chitose.com.atproto.server.defs.InviteCode]=None, invites: typing.Optional[list[chitose.com.atproto.server.defs.InviteCode]]=None, invites_disabled: typing.Optional[bool]=None) -> None:
         self.did = did
@@ -130,48 +131,48 @@
         self.moderation = moderation
         self.email = email
         self.labels = labels
         self.invited_by = invited_by
         self.invites = invites
         self.invites_disabled = invites_disabled
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'did': self.did, 'handle': self.handle, 'relatedRecords': self.related_records, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'email': self.email, 'labels': self.labels, 'invitedBy': self.invited_by, 'invites': self.invites, 'invitesDisabled': self.invites_disabled, '$type': 'com.atproto.admin.defs#repoViewDetail'}
 
 class RepoViewNotFound(chitose.Object):
     """"""
 
     def __init__(self, did: str) -> None:
         self.did = did
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'did': self.did, '$type': 'com.atproto.admin.defs#repoViewNotFound'}
 
 class RepoRef(chitose.Object):
     """"""
 
     def __init__(self, did: str) -> None:
         self.did = did
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'did': self.did, '$type': 'com.atproto.admin.defs#repoRef'}
 
 class RecordView(chitose.Object):
     """"""
 
     def __init__(self, uri: str, cid: str, value: typing.Any, blob_cids: list[str], indexed_at: str, moderation: chitose.com.atproto.admin.defs.Moderation, repo: chitose.com.atproto.admin.defs.RepoView) -> None:
         self.uri = uri
         self.cid = cid
         self.value = value
         self.blob_cids = blob_cids
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.repo = repo
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, 'cid': self.cid, 'value': self.value, 'blobCids': self.blob_cids, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'repo': self.repo, '$type': 'com.atproto.admin.defs#recordView'}
 
 class RecordViewDetail(chitose.Object):
     """"""
 
     def __init__(self, uri: str, cid: str, value: typing.Any, blobs: list[chitose.com.atproto.admin.defs.BlobView], indexed_at: str, moderation: chitose.com.atproto.admin.defs.ModerationDetail, repo: chitose.com.atproto.admin.defs.RepoView, labels: typing.Optional[list[chitose.com.atproto.label.defs.Label]]=None) -> None:
         self.uri = uri
@@ -179,73 +180,73 @@
         self.value = value
         self.blobs = blobs
         self.indexed_at = indexed_at
         self.moderation = moderation
         self.repo = repo
         self.labels = labels
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, 'cid': self.cid, 'value': self.value, 'blobs': self.blobs, 'indexedAt': self.indexed_at, 'moderation': self.moderation, 'repo': self.repo, 'labels': self.labels, '$type': 'com.atproto.admin.defs#recordViewDetail'}
 
 class RecordViewNotFound(chitose.Object):
     """"""
 
     def __init__(self, uri: str) -> None:
         self.uri = uri
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, '$type': 'com.atproto.admin.defs#recordViewNotFound'}
 
 class Moderation(chitose.Object):
     """"""
 
     def __init__(self, current_action: typing.Optional[chitose.com.atproto.admin.defs.ActionViewCurrent]=None) -> None:
         self.current_action = current_action
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'currentAction': self.current_action, '$type': 'com.atproto.admin.defs#moderation'}
 
 class ModerationDetail(chitose.Object):
     """"""
 
     def __init__(self, actions: list[chitose.com.atproto.admin.defs.ActionView], reports: list[chitose.com.atproto.admin.defs.ReportView], current_action: typing.Optional[chitose.com.atproto.admin.defs.ActionViewCurrent]=None) -> None:
         self.actions = actions
         self.reports = reports
         self.current_action = current_action
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'actions': self.actions, 'reports': self.reports, 'currentAction': self.current_action, '$type': 'com.atproto.admin.defs#moderationDetail'}
 
 class BlobView(chitose.Object):
     """"""
 
     def __init__(self, cid: str, mime_type: str, size: int, created_at: str, details: typing.Optional[typing.Union[chitose.com.atproto.admin.defs.ImageDetails, chitose.com.atproto.admin.defs.VideoDetails]]=None, moderation: typing.Optional[chitose.com.atproto.admin.defs.Moderation]=None) -> None:
         self.cid = cid
         self.mime_type = mime_type
         self.size = size
         self.created_at = created_at
         self.details = details
         self.moderation = moderation
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'cid': self.cid, 'mimeType': self.mime_type, 'size': self.size, 'createdAt': self.created_at, 'details': self.details, 'moderation': self.moderation, '$type': 'com.atproto.admin.defs#blobView'}
 
 class ImageDetails(chitose.Object):
     """"""
 
     def __init__(self, width: int, height: int) -> None:
         self.width = width
         self.height = height
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'width': self.width, 'height': self.height, '$type': 'com.atproto.admin.defs#imageDetails'}
 
 class VideoDetails(chitose.Object):
     """"""
 
     def __init__(self, width: int, height: int, length: int) -> None:
         self.width = width
         self.height = height
         self.length = length
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'width': self.width, 'height': self.height, 'length': self.length, '$type': 'com.atproto.admin.defs#videoDetails'}
```

### Comparing `chitose-0.0.8/chitose/com/atproto/admin/get_moderation_reports.py` & `chitose-0.0.9/chitose/com/atproto/admin/get_moderation_reports.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import typing
 
-def _get_moderation_reports(call: chitose.xrpc.XrpcCall, subject: typing.Optional[str]=None, ignore_subjects: typing.Optional[list[str]]=None, resolved: typing.Optional[bool]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, reverse: typing.Optional[bool]=None) -> bytes:
+def _get_moderation_reports(call: chitose.xrpc.XrpcCall, subject: typing.Optional[str]=None, ignore_subjects: typing.Optional[list[str]]=None, reporters: typing.Optional[list[str]]=None, resolved: typing.Optional[bool]=None, action_type: typing.Optional[typing.Literal['com.atproto.admin.defs#takedown', 'com.atproto.admin.defs#flag', 'com.atproto.admin.defs#acknowledge', 'com.atproto.admin.defs#escalate']]=None, limit: typing.Optional[int]=None, cursor: typing.Optional[str]=None, reverse: typing.Optional[bool]=None) -> bytes:
     """List moderation reports related to a subject.
 
 
+    :param reporters: Filter reports made by one or more DIDs
+
     :param reverse: Reverse the order of the returned records? when true, returns reports in chronological order
     """
-    return call('com.atproto.admin.getModerationReports', [('subject', subject), ('ignoreSubjects', ignore_subjects), ('resolved', resolved), ('actionType', action_type), ('limit', limit), ('cursor', cursor), ('reverse', reverse)], None, {})
+    return call('com.atproto.admin.getModerationReports', [('subject', subject), ('ignoreSubjects', ignore_subjects), ('reporters', reporters), ('resolved', resolved), ('actionType', action_type), ('limit', limit), ('cursor', cursor), ('reverse', reverse)], None, {})
```

### Comparing `chitose-0.0.8/chitose/com/atproto/admin/rebase_repo.py` & `chitose-0.0.9/chitose/com/atproto/admin/rebase_repo.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/admin/take_moderation_action.py` & `chitose-0.0.9/chitose/com/atproto/admin/take_moderation_action.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/identity/__init__.py` & `chitose-0.0.9/chitose/com/atproto/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/label/__init__.py` & `chitose-0.0.9/chitose/com/atproto/label/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/label/defs.py` & `chitose-0.0.9/chitose/com/atproto/label/defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,9 +25,9 @@
         self.src = src
         self.uri = uri
         self.val = val
         self.cts = cts
         self.cid = cid
         self.neg = neg
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'src': self.src, 'uri': self.uri, 'val': self.val, 'cts': self.cts, 'cid': self.cid, 'neg': self.neg, '$type': 'com.atproto.label.defs#label'}
```

### Comparing `chitose-0.0.8/chitose/com/atproto/label/query_labels.py` & `chitose-0.0.9/chitose/com/atproto/label/query_labels.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/label/subscribe_labels.py` & `chitose-0.0.9/chitose/com/atproto/label/subscribe_labels.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 class Labels(chitose.Object):
     """"""
 
     def __init__(self, seq: int, labels: list[chitose.com.atproto.label.defs.Label]) -> None:
         self.seq = seq
         self.labels = labels
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'seq': self.seq, 'labels': self.labels, '$type': 'com.atproto.label.subscribeLabels#labels'}
 
 class Info(chitose.Object):
     """"""
 
     def __init__(self, name: typing.Literal['OutdatedCursor',], message: typing.Optional[str]=None) -> None:
         self.name = name
         self.message = message
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'name': self.name, 'message': self.message, '$type': 'com.atproto.label.subscribeLabels#info'}
```

### Comparing `chitose-0.0.8/chitose/com/atproto/moderation/__init__.py` & `chitose-0.0.9/chitose/com/atproto/moderation/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/moderation/create_report.py` & `chitose-0.0.9/chitose/com/atproto/moderation/create_report.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/moderation/defs.py` & `chitose-0.0.9/chitose/com/atproto/moderation/defs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/repo/__init__.py` & `chitose-0.0.9/chitose/com/atproto/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/repo/apply_writes.py` & `chitose-0.0.9/chitose/com/atproto/repo/apply_writes.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,30 +19,30 @@
     """"""
 
     def __init__(self, collection: str, value: typing.Any, rkey: typing.Optional[str]=None) -> None:
         self.collection = collection
         self.value = value
         self.rkey = rkey
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'collection': self.collection, 'value': self.value, 'rkey': self.rkey, '$type': 'com.atproto.repo.applyWrites#create'}
 
 class Update(chitose.Object):
     """"""
 
     def __init__(self, collection: str, rkey: str, value: typing.Any) -> None:
         self.collection = collection
         self.rkey = rkey
         self.value = value
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'collection': self.collection, 'rkey': self.rkey, 'value': self.value, '$type': 'com.atproto.repo.applyWrites#update'}
 
 class Delete(chitose.Object):
     """"""
 
     def __init__(self, collection: str, rkey: str) -> None:
         self.collection = collection
         self.rkey = rkey
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'collection': self.collection, 'rkey': self.rkey, '$type': 'com.atproto.repo.applyWrites#delete'}
```

### Comparing `chitose-0.0.8/chitose/com/atproto/repo/create_record.py` & `chitose-0.0.9/chitose/com/atproto/repo/create_record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/repo/delete_record.py` & `chitose-0.0.9/chitose/com/atproto/repo/delete_record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/repo/get_record.py` & `chitose-0.0.9/chitose/com/atproto/repo/get_record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/repo/list_records.py` & `chitose-0.0.9/chitose/com/atproto/repo/list_records.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,9 +26,9 @@
     """"""
 
     def __init__(self, uri: str, cid: str, value: typing.Any) -> None:
         self.uri = uri
         self.cid = cid
         self.value = value
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'uri': self.uri, 'cid': self.cid, 'value': self.value, '$type': 'com.atproto.repo.listRecords#record'}
```

### Comparing `chitose-0.0.8/chitose/com/atproto/repo/put_record.py` & `chitose-0.0.9/chitose/com/atproto/repo/put_record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/repo/rebase_repo.py` & `chitose-0.0.9/chitose/com/atproto/repo/rebase_repo.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/server/__init__.py` & `chitose-0.0.9/chitose/com/atproto/server/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/server/create_account.py` & `chitose-0.0.9/chitose/com/atproto/server/create_account.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/server/create_app_password.py` & `chitose-0.0.9/chitose/com/atproto/server/create_app_password.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
+import typing
 
 def _create_app_password(call: chitose.xrpc.XrpcCall, name: str) -> bytes:
     """Create an app-specific password."""
     return call('com.atproto.server.createAppPassword', [], {'name': name}, {'Content-Type': 'application/json'})
 
 class AppPassword(chitose.Object):
     """"""
 
     def __init__(self, name: str, password: str, created_at: str) -> None:
         self.name = name
         self.password = password
         self.created_at = created_at
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'name': self.name, 'password': self.password, 'createdAt': self.created_at, '$type': 'com.atproto.server.createAppPassword#appPassword'}
```

### Comparing `chitose-0.0.8/chitose/com/atproto/server/create_invite_codes.py` & `chitose-0.0.9/chitose/com/atproto/server/create_invite_codes.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 class AccountCodes(chitose.Object):
     """"""
 
     def __init__(self, account: str, codes: list[str]) -> None:
         self.account = account
         self.codes = codes
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'account': self.account, 'codes': self.codes, '$type': 'com.atproto.server.createInviteCodes#accountCodes'}
```

### Comparing `chitose-0.0.8/chitose/com/atproto/server/defs.py` & `chitose-0.0.9/chitose/com/atproto/server/defs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
 import chitose.com.atproto.server.defs
+import typing
 
 class InviteCode(chitose.Object):
     """"""
 
     def __init__(self, code: str, available: int, disabled: bool, for_account: str, created_by: str, created_at: str, uses: list[chitose.com.atproto.server.defs.InviteCodeUse]) -> None:
         self.code = code
         self.available = available
         self.disabled = disabled
         self.for_account = for_account
         self.created_by = created_by
         self.created_at = created_at
         self.uses = uses
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'code': self.code, 'available': self.available, 'disabled': self.disabled, 'forAccount': self.for_account, 'createdBy': self.created_by, 'createdAt': self.created_at, 'uses': self.uses, '$type': 'com.atproto.server.defs#inviteCode'}
 
 class InviteCodeUse(chitose.Object):
     """"""
 
     def __init__(self, used_by: str, used_at: str) -> None:
         self.used_by = used_by
         self.used_at = used_at
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'usedBy': self.used_by, 'usedAt': self.used_at, '$type': 'com.atproto.server.defs#inviteCodeUse'}
```

### Comparing `chitose-0.0.8/chitose/com/atproto/server/list_app_passwords.py` & `chitose-0.0.9/chitose/com/atproto/server/list_app_passwords.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # GENERATED CODE - DO NOT MODIFY
 """"""
 from __future__ import annotations
 import chitose
+import typing
 
 def _list_app_passwords(call: chitose.xrpc.XrpcCall) -> bytes:
     """List all app-specific passwords."""
     return call('com.atproto.server.listAppPasswords', [], None, {})
 
 class AppPassword(chitose.Object):
     """"""
 
     def __init__(self, name: str, created_at: str) -> None:
         self.name = name
         self.created_at = created_at
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'name': self.name, 'createdAt': self.created_at, '$type': 'com.atproto.server.listAppPasswords#appPassword'}
```

### Comparing `chitose-0.0.8/chitose/com/atproto/sync/__init__.py` & `chitose-0.0.9/chitose/com/atproto/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/sync/get_commit_path.py` & `chitose-0.0.9/chitose/com/atproto/sync/get_commit_path.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/sync/get_record.py` & `chitose-0.0.9/chitose/com/atproto/sync/get_record.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/sync/get_repo.py` & `chitose-0.0.9/chitose/com/atproto/sync/get_repo.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/sync/list_blobs.py` & `chitose-0.0.9/chitose/com/atproto/sync/list_blobs.py`

 * *Files identical despite different names*

### Comparing `chitose-0.0.8/chitose/com/atproto/sync/list_repos.py` & `chitose-0.0.9/chitose/com/atproto/sync/list_repos.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 class Repo(chitose.Object):
     """"""
 
     def __init__(self, did: str, head: str) -> None:
         self.did = did
         self.head = head
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'did': self.did, 'head': self.head, '$type': 'com.atproto.sync.listRepos#repo'}
```

### Comparing `chitose-0.0.8/chitose/com/atproto/sync/subscribe_repos.py` & `chitose-0.0.9/chitose/com/atproto/sync/subscribe_repos.py`

 * *Files 27% similar despite different names*

```diff
@@ -28,65 +28,65 @@
         self.commit = commit
         self.prev = prev
         self.blocks = blocks
         self.ops = ops
         self.blobs = blobs
         self.time = time
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'seq': self.seq, 'rebase': self.rebase, 'tooBig': self.too_big, 'repo': self.repo, 'commit': self.commit, 'prev': self.prev, 'blocks': self.blocks, 'ops': self.ops, 'blobs': self.blobs, 'time': self.time, '$type': 'com.atproto.sync.subscribeRepos#commit'}
 
 class Handle(chitose.Object):
     """"""
 
     def __init__(self, seq: int, did: str, handle: str, time: str) -> None:
         self.seq = seq
         self.did = did
         self.handle = handle
         self.time = time
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'seq': self.seq, 'did': self.did, 'handle': self.handle, 'time': self.time, '$type': 'com.atproto.sync.subscribeRepos#handle'}
 
 class Migrate(chitose.Object):
     """"""
 
     def __init__(self, seq: int, did: str, migrate_to: str, time: str) -> None:
         self.seq = seq
         self.did = did
         self.migrate_to = migrate_to
         self.time = time
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'seq': self.seq, 'did': self.did, 'migrateTo': self.migrate_to, 'time': self.time, '$type': 'com.atproto.sync.subscribeRepos#migrate'}
 
 class Tombstone(chitose.Object):
     """"""
 
     def __init__(self, seq: int, did: str, time: str) -> None:
         self.seq = seq
         self.did = did
         self.time = time
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'seq': self.seq, 'did': self.did, 'time': self.time, '$type': 'com.atproto.sync.subscribeRepos#tombstone'}
 
 class Info(chitose.Object):
     """"""
 
     def __init__(self, name: typing.Literal['OutdatedCursor',], message: typing.Optional[str]=None) -> None:
         self.name = name
         self.message = message
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'name': self.name, 'message': self.message, '$type': 'com.atproto.sync.subscribeRepos#info'}
 
 class RepoOp(chitose.Object):
     """"""
 
     def __init__(self, action: typing.Literal['create', 'update', 'delete'], path: str, cid: typing.Any) -> None:
         self.action = action
         self.path = path
         self.cid = cid
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, typing.Any]:
         return {'action': self.action, 'path': self.path, 'cid': self.cid, '$type': 'com.atproto.sync.subscribeRepos#repoOp'}
```

### Comparing `chitose-0.0.8/chitose/xrpc.py` & `chitose-0.0.9/chitose/xrpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         data = None
     else:
         # for POST requests
         # d = {} => data = b''
         data = b''
 
     r = urllib.request.urlopen(req, data)
-    return r.read()
+    return r.read()  # type: ignore[no-any-return]
 
 
 def subscribe(method: str, params: XrpcParams, service: str,
               handler: XrpcHandler) -> None:
     with connect(_url(method, params, service)) as websocket:
         for message in websocket:
             handler(message)
```

### Comparing `chitose-0.0.8/pyproject.toml` & `chitose-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chitose"
-version = "0.0.8"
+version = "0.0.9"
 description = "A client library for the AT Protocol (Bluesky) "
 license = "MIT"
 authors = [
     "Muneyuki Noguchi <nogu.dev@gmail.com>",
 ]
 readme = "README.md"
 homepage = "https://github.com/mnogu/chitose"
```

### Comparing `chitose-0.0.8/PKG-INFO` & `chitose-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chitose
-Version: 0.0.8
+Version: 0.0.9
 Summary: A client library for the AT Protocol (Bluesky) 
 Home-page: https://github.com/mnogu/chitose
 License: MIT
 Author: Muneyuki Noguchi
 Author-email: nogu.dev@gmail.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
```

