# Comparing `tmp/discordtool-0.0.2.tar.gz` & `tmp/discordtool-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordtool-0.0.2.tar", last modified: Mon Jul 17 16:19:11 2023, max compression
+gzip compressed data, was "discordtool-0.1.tar", last modified: Mon Jul 17 16:10:02 2023, max compression
```

## Comparing `discordtool-0.0.2.tar` & `discordtool-0.1.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.309970 discordtool-0.0.2/
--rw-rw-rw-   0        0        0       13 2023-07-17 14:30:37.000000 discordtool-0.0.2/.gitattributes
--rw-rw-rw-   0        0        0     4191 2023-07-17 14:30:37.000000 discordtool-0.0.2/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1146 2023-07-17 14:30:37.000000 discordtool-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      405 2023-07-17 14:33:32.000000 discordtool-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5519 2023-07-17 16:19:11.309467 discordtool-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4542 2023-07-17 14:30:37.000000 discordtool-0.0.2/README.rst
--rw-rw-rw-   0        0        0      361 2023-07-17 14:33:36.000000 discordtool-0.0.2/codecov.yml
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.024940 discordtool-0.0.2/discordtool/
--rw-rw-rw-   0        0        0     1825 2023-07-17 16:16:46.000000 discordtool-0.0.2/discordtool/__init__.py
--rw-rw-rw-   0        0        0    11000 2023-07-17 16:18:18.000000 discordtool-0.0.2/discordtool/__main__.py
--rw-rw-rw-   0        0        0     1540 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/_typed_dict.py
--rw-rw-rw-   0        0        0     4914 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/_version.py
--rw-rw-rw-   0        0        0    67010 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/abc.py
--rw-rw-rw-   0        0        0    27697 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/activity.py
--rw-rw-rw-   0        0        0     9033 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/appinfo.py
--rw-rw-rw-   0        0        0     5016 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/application_role_connection.py
--rw-rw-rw-   0        0        0    13736 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/asset.py
--rw-rw-rw-   0        0        0    25325 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/audit_logs.py
--rw-rw-rw-   0        0        0    19206 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/automod.py
--rw-rw-rw-   0        0        0     3861 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/backoff.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.038433 discordtool-0.0.2/discordtool/bin/
--rw-rw-rw-   0        0        0   441856 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/bin/libopus-0.x64.dll
--rw-rw-rw-   0        0        0   366080 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/bin/libopus-0.x86.dll
--rw-rw-rw-   0        0        0    59251 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/bot.py
--rw-rw-rw-   0        0        0   109671 2023-07-17 14:32:49.000000 discordtool-0.0.2/discordtool/channel.py
--rw-rw-rw-   0        0        0    67317 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/client.py
--rw-rw-rw-   0        0        0    42792 2023-07-17 14:32:49.000000 discordtool-0.0.2/discordtool/cog.py
--rw-rw-rw-   0        0        0    11524 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/colour.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.052786 discordtool-0.0.2/discordtool/commands/
--rw-rw-rw-   0        0        0     1255 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/commands/__init__.py
--rw-rw-rw-   0        0        0    13934 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/commands/context.py
--rw-rw-rw-   0        0        0    73220 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/commands/core.py
--rw-rw-rw-   0        0        0    17719 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/commands/options.py
--rw-rw-rw-   0        0        0     4532 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/commands/permissions.py
--rw-rw-rw-   0        0        0    16676 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/components.py
--rw-rw-rw-   0        0        0     3029 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/context_managers.py
--rw-rw-rw-   0        0        0    30203 2023-07-17 14:32:49.000000 discordtool-0.0.2/discordtool/embeds.py
--rw-rw-rw-   0        0        0     8647 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/emoji.py
--rw-rw-rw-   0        0        0    27022 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/enums.py
--rw-rw-rw-   0        0        0    13270 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:10.823078 discordtool-0.0.2/discordtool/ext/
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.065923 discordtool-0.0.2/discordtool/ext/bridge/
--rw-rw-rw-   0        0        0     1223 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/ext/bridge/__init__.py
--rw-rw-rw-   0        0        0     8152 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/bridge/bot.py
--rw-rw-rw-   0        0        0     8324 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/bridge/context.py
--rw-rw-rw-   0        0        0    22226 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/bridge/core.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.104677 discordtool-0.0.2/discordtool/ext/commands/
--rw-rw-rw-   0        0        0      443 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/ext/commands/__init__.py
--rw-rw-rw-   0        0        0     1857 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/ext/commands/_types.py
--rw-rw-rw-   0        0        0    16658 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/commands/bot.py
--rw-rw-rw-   0        0        0     3157 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/commands/cog.py
--rw-rw-rw-   0        0        0    14998 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/commands/context.py
--rw-rw-rw-   0        0        0    41773 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/commands/converter.py
--rw-rw-rw-   0        0        0    13215 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/commands/cooldowns.py
--rw-rw-rw-   0        0        0    84640 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/commands/core.py
--rw-rw-rw-   0        0        0    30406 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/commands/errors.py
--rw-rw-rw-   0        0        0    22704 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/commands/flags.py
--rw-rw-rw-   0        0        0    50176 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/commands/help.py
--rw-rw-rw-   0        0        0     6282 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/ext/commands/view.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.112425 discordtool-0.0.2/discordtool/ext/pages/
--rw-rw-rw-   0        0        0      227 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/ext/pages/__init__.py
--rw-rw-rw-   0        0        0    54728 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/pages/pagination.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.119911 discordtool-0.0.2/discordtool/ext/tasks/
--rw-rw-rw-   0        0        0    27594 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/ext/tasks/__init__.py
--rw-rw-rw-   0        0        0     4963 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/file.py
--rw-rw-rw-   0        0        0    48205 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/flags.py
--rw-rw-rw-   0        0        0    33282 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/gateway.py
--rw-rw-rw-   0        0        0   131873 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/guild.py
--rw-rw-rw-   0        0        0    94274 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/http.py
--rw-rw-rw-   0        0        0    12173 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/integrations.py
--rw-rw-rw-   0        0        0    47877 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/interactions.py
--rw-rw-rw-   0        0        0    19718 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/invite.py
--rw-rw-rw-   0        0        0    31379 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/iterators.py
--rw-rw-rw-   0        0        0    39125 2023-07-17 14:32:49.000000 discordtool-0.0.2/discordtool/member.py
--rw-rw-rw-   0        0        0     5907 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/mentions.py
--rw-rw-rw-   0        0        0    74885 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/message.py
--rw-rw-rw-   0        0        0     1687 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/mixins.py
--rw-rw-rw-   0        0        0     3496 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/object.py
--rw-rw-rw-   0        0        0     3893 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/oggparse.py
--rw-rw-rw-   0        0        0    17472 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/opus.py
--rw-rw-rw-   0        0        0     7662 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/partial_emoji.py
--rw-rw-rw-   0        0        0    28130 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/permissions.py
--rw-rw-rw-   0        0        0    27838 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/player.py
--rw-rw-rw-   0        0        0        0 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/py.typed
--rw-rw-rw-   0        0        0    26527 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/raw_models.py
--rw-rw-rw-   0        0        0     7286 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/reaction.py
--rw-rw-rw-   0        0        0    16751 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/role.py
--rw-rw-rw-   0        0        0    19152 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/scheduled_events.py
--rw-rw-rw-   0        0        0    20306 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/shard.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.161097 discordtool-0.0.2/discordtool/sinks/
--rw-rw-rw-   0        0        0      392 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/sinks/__init__.py
--rw-rw-rw-   0        0        0     6483 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/sinks/core.py
--rw-rw-rw-   0        0        0     2543 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/sinks/errors.py
--rw-rw-rw-   0        0        0     3317 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/sinks/m4a.py
--rw-rw-rw-   0        0        0     3084 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/sinks/mka.py
--rw-rw-rw-   0        0        0     3052 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/sinks/mkv.py
--rw-rw-rw-   0        0        0     3079 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/sinks/mp3.py
--rw-rw-rw-   0        0        0     3316 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/sinks/mp4.py
--rw-rw-rw-   0        0        0     3079 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/sinks/ogg.py
--rw-rw-rw-   0        0        0     1610 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/sinks/pcm.py
--rw-rw-rw-   0        0        0     2385 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/sinks/wave.py
--rw-rw-rw-   0        0        0     6523 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/stage_instance.py
--rw-rw-rw-   0        0        0    75970 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/state.py
--rw-rw-rw-   0        0        0    16774 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/sticker.py
--rw-rw-rw-   0        0        0     5563 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/team.py
--rw-rw-rw-   0        0        0     9590 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/template.py
--rw-rw-rw-   0        0        0    31430 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/threads.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.260650 discordtool-0.0.2/discordtool/types/
--rw-rw-rw-   0        0        0      192 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/__init__.py
--rw-rw-rw-   0        0        0     2864 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/activity.py
--rw-rw-rw-   0        0        0     2053 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/appinfo.py
--rw-rw-rw-   0        0        0     1589 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/application_role_connection.py
--rw-rw-rw-   0        0        0     6992 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/audit_log.py
--rw-rw-rw-   0        0        0     2881 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/automod.py
--rw-rw-rw-   0        0        0     4835 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/channel.py
--rw-rw-rw-   0        0        0     2630 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/components.py
--rw-rw-rw-   0        0        0     2486 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/embed.py
--rw-rw-rw-   0        0        0     1637 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/emoji.py
--rw-rw-rw-   0        0        0     1451 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/gateway.py
--rw-rw-rw-   0        0        0     5555 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/guild.py
--rw-rw-rw-   0        0        0     2341 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/integration.py
--rw-rw-rw-   0        0        0     7121 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/interactions.py
--rw-rw-rw-   0        0        0     2853 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/invite.py
--rw-rw-rw-   0        0        0     1925 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/member.py
--rw-rw-rw-   0        0        0     4083 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/message.py
--rw-rw-rw-   0        0        0     4011 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/raw_models.py
--rw-rw-rw-   0        0        0     1620 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/role.py
--rw-rw-rw-   0        0        0     2141 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/scheduled_events.py
--rw-rw-rw-   0        0        0     1254 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/snowflake.py
--rw-rw-rw-   0        0        0     2449 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/sticker.py
--rw-rw-rw-   0        0        0     1569 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/team.py
--rw-rw-rw-   0        0        0     1685 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/template.py
--rw-rw-rw-   0        0        0     2387 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/threads.py
--rw-rw-rw-   0        0        0     1686 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/user.py
--rw-rw-rw-   0        0        0     2412 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/voice.py
--rw-rw-rw-   0        0        0     2046 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/webhook.py
--rw-rw-rw-   0        0        0     1524 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/welcome_screen.py
--rw-rw-rw-   0        0        0     1947 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/types/widget.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.284536 discordtool-0.0.2/discordtool/ui/
--rw-rw-rw-   0        0        0      330 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/ui/__init__.py
--rw-rw-rw-   0        0        0    11075 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/ui/button.py
--rw-rw-rw-   0        0        0     8368 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/ui/input_text.py
--rw-rw-rw-   0        0        0     4334 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/ui/item.py
--rw-rw-rw-   0        0        0    11652 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/ui/modal.py
--rw-rw-rw-   0        0        0    25702 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/ui/select.py
--rw-rw-rw-   0        0        0    22215 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/ui/view.py
--rw-rw-rw-   0        0        0    18378 2023-07-17 14:32:48.000000 discordtool-0.0.2/discordtool/user.py
--rw-rw-rw-   0        0        0    43234 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/utils.py
--rw-rw-rw-   0        0        0    33725 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/voice_client.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.293994 discordtool-0.0.2/discordtool/webhook/
--rw-rw-rw-   0        0        0      249 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/webhook/__init__.py
--rw-rw-rw-   0        0        0    66249 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/webhook/async_.py
--rw-rw-rw-   0        0        0    42193 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/webhook/sync.py
--rw-rw-rw-   0        0        0     8034 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/welcome_screen.py
--rw-rw-rw-   0        0        0    10838 2023-07-17 14:30:37.000000 discordtool-0.0.2/discordtool/widget.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.034443 discordtool-0.0.2/discordtool.egg-info/
--rw-rw-rw-   0        0        0     5519 2023-07-17 16:19:10.000000 discordtool-0.0.2/discordtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4146 2023-07-17 16:19:10.000000 discordtool-0.0.2/discordtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 16:19:10.000000 discordtool-0.0.2/discordtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      379 2023-07-17 16:19:10.000000 discordtool-0.0.2/discordtool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-17 16:19:10.000000 discordtool-0.0.2/discordtool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-07-17 14:30:37.000000 discordtool-0.0.2/install
--rw-rw-rw-   0        0        0     2290 2023-07-17 16:09:54.000000 discordtool-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-17 16:19:11.307475 discordtool-0.0.2/requirements/
--rw-rw-rw-   0        0        0       73 2023-07-17 14:30:37.000000 discordtool-0.0.2/requirements/_.txt
--rw-rw-rw-   0        0        0       53 2023-07-17 14:30:37.000000 discordtool-0.0.2/requirements/all.txt
--rw-rw-rw-   0        0        0      183 2023-07-17 14:30:37.000000 discordtool-0.0.2/requirements/dev.txt
--rw-rw-rw-   0        0        0      236 2023-07-17 14:30:37.000000 discordtool-0.0.2/requirements/docs.txt
--rw-rw-rw-   0        0        0       34 2023-07-17 14:30:37.000000 discordtool-0.0.2/requirements/speed.txt
--rw-rw-rw-   0        0        0       20 2023-07-17 14:30:37.000000 discordtool-0.0.2/requirements/voice.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 16:19:11.309970 discordtool-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       88 2023-07-17 16:19:07.000000 discordtool-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.695372 discordtool-0.1/
+-rw-rw-rw-   0        0        0       13 2023-07-17 14:30:37.000000 discordtool-0.1/.gitattributes
+-rw-rw-rw-   0        0        0     4191 2023-07-17 14:30:37.000000 discordtool-0.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1146 2023-07-17 14:30:37.000000 discordtool-0.1/LICENSE
+-rw-rw-rw-   0        0        0      405 2023-07-17 14:33:32.000000 discordtool-0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5517 2023-07-17 16:10:02.694374 discordtool-0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4542 2023-07-17 14:30:37.000000 discordtool-0.1/README.rst
+-rw-rw-rw-   0        0        0      361 2023-07-17 14:33:36.000000 discordtool-0.1/codecov.yml
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.419235 discordtool-0.1/discordtool/
+-rw-rw-rw-   0        0        0     1827 2023-07-17 15:50:22.000000 discordtool-0.1/discordtool/__init__.py
+-rw-rw-rw-   0        0        0    11023 2023-07-17 15:50:04.000000 discordtool-0.1/discordtool/__main__.py
+-rw-rw-rw-   0        0        0     1540 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/_typed_dict.py
+-rw-rw-rw-   0        0        0     4914 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/_version.py
+-rw-rw-rw-   0        0        0    67010 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/abc.py
+-rw-rw-rw-   0        0        0    27697 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/activity.py
+-rw-rw-rw-   0        0        0     9033 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/appinfo.py
+-rw-rw-rw-   0        0        0     5016 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/application_role_connection.py
+-rw-rw-rw-   0        0        0    13736 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/asset.py
+-rw-rw-rw-   0        0        0    25325 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/audit_logs.py
+-rw-rw-rw-   0        0        0    19206 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/automod.py
+-rw-rw-rw-   0        0        0     3861 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/backoff.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.433554 discordtool-0.1/discordtool/bin/
+-rw-rw-rw-   0        0        0   441856 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/bin/libopus-0.x64.dll
+-rw-rw-rw-   0        0        0   366080 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/bin/libopus-0.x86.dll
+-rw-rw-rw-   0        0        0    59251 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/bot.py
+-rw-rw-rw-   0        0        0   109671 2023-07-17 14:32:49.000000 discordtool-0.1/discordtool/channel.py
+-rw-rw-rw-   0        0        0    67317 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/client.py
+-rw-rw-rw-   0        0        0    42792 2023-07-17 14:32:49.000000 discordtool-0.1/discordtool/cog.py
+-rw-rw-rw-   0        0        0    11524 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/colour.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.449110 discordtool-0.1/discordtool/commands/
+-rw-rw-rw-   0        0        0     1255 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/commands/__init__.py
+-rw-rw-rw-   0        0        0    13934 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/commands/context.py
+-rw-rw-rw-   0        0        0    73220 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/commands/core.py
+-rw-rw-rw-   0        0        0    17719 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/commands/options.py
+-rw-rw-rw-   0        0        0     4532 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/commands/permissions.py
+-rw-rw-rw-   0        0        0    16676 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/components.py
+-rw-rw-rw-   0        0        0     3029 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/context_managers.py
+-rw-rw-rw-   0        0        0    30203 2023-07-17 14:32:49.000000 discordtool-0.1/discordtool/embeds.py
+-rw-rw-rw-   0        0        0     8647 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/emoji.py
+-rw-rw-rw-   0        0        0    27022 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/enums.py
+-rw-rw-rw-   0        0        0    13270 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.217429 discordtool-0.1/discordtool/ext/
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.461240 discordtool-0.1/discordtool/ext/bridge/
+-rw-rw-rw-   0        0        0     1223 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/ext/bridge/__init__.py
+-rw-rw-rw-   0        0        0     8152 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/bridge/bot.py
+-rw-rw-rw-   0        0        0     8324 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/bridge/context.py
+-rw-rw-rw-   0        0        0    22226 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/bridge/core.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.503814 discordtool-0.1/discordtool/ext/commands/
+-rw-rw-rw-   0        0        0      443 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     1857 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    16658 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/commands/bot.py
+-rw-rw-rw-   0        0        0     3157 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/commands/cog.py
+-rw-rw-rw-   0        0        0    14998 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/commands/context.py
+-rw-rw-rw-   0        0        0    41773 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/commands/converter.py
+-rw-rw-rw-   0        0        0    13215 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    84640 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/commands/core.py
+-rw-rw-rw-   0        0        0    30406 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    22704 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/commands/flags.py
+-rw-rw-rw-   0        0        0    50176 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/commands/help.py
+-rw-rw-rw-   0        0        0     6282 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.511794 discordtool-0.1/discordtool/ext/pages/
+-rw-rw-rw-   0        0        0      227 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/ext/pages/__init__.py
+-rw-rw-rw-   0        0        0    54728 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/pages/pagination.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.515300 discordtool-0.1/discordtool/ext/tasks/
+-rw-rw-rw-   0        0        0    27594 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0     4963 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/file.py
+-rw-rw-rw-   0        0        0    48205 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/flags.py
+-rw-rw-rw-   0        0        0    33282 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/gateway.py
+-rw-rw-rw-   0        0        0   131873 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/guild.py
+-rw-rw-rw-   0        0        0    94274 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/http.py
+-rw-rw-rw-   0        0        0    12173 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/integrations.py
+-rw-rw-rw-   0        0        0    47877 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/interactions.py
+-rw-rw-rw-   0        0        0    19718 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/invite.py
+-rw-rw-rw-   0        0        0    31379 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/iterators.py
+-rw-rw-rw-   0        0        0    39125 2023-07-17 14:32:49.000000 discordtool-0.1/discordtool/member.py
+-rw-rw-rw-   0        0        0     5907 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/mentions.py
+-rw-rw-rw-   0        0        0    74885 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/message.py
+-rw-rw-rw-   0        0        0     1687 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/mixins.py
+-rw-rw-rw-   0        0        0     3496 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/object.py
+-rw-rw-rw-   0        0        0     3893 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/oggparse.py
+-rw-rw-rw-   0        0        0    17472 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/opus.py
+-rw-rw-rw-   0        0        0     7662 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/partial_emoji.py
+-rw-rw-rw-   0        0        0    28130 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/permissions.py
+-rw-rw-rw-   0        0        0    27838 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/player.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/py.typed
+-rw-rw-rw-   0        0        0    26527 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/raw_models.py
+-rw-rw-rw-   0        0        0     7286 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/reaction.py
+-rw-rw-rw-   0        0        0    16751 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/role.py
+-rw-rw-rw-   0        0        0    19152 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/scheduled_events.py
+-rw-rw-rw-   0        0        0    20306 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/shard.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.553068 discordtool-0.1/discordtool/sinks/
+-rw-rw-rw-   0        0        0      392 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/sinks/__init__.py
+-rw-rw-rw-   0        0        0     6483 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/sinks/core.py
+-rw-rw-rw-   0        0        0     2543 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/sinks/errors.py
+-rw-rw-rw-   0        0        0     3317 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/sinks/m4a.py
+-rw-rw-rw-   0        0        0     3084 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/sinks/mka.py
+-rw-rw-rw-   0        0        0     3052 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/sinks/mkv.py
+-rw-rw-rw-   0        0        0     3079 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/sinks/mp3.py
+-rw-rw-rw-   0        0        0     3316 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/sinks/mp4.py
+-rw-rw-rw-   0        0        0     3079 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/sinks/ogg.py
+-rw-rw-rw-   0        0        0     1610 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/sinks/pcm.py
+-rw-rw-rw-   0        0        0     2385 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/sinks/wave.py
+-rw-rw-rw-   0        0        0     6523 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/stage_instance.py
+-rw-rw-rw-   0        0        0    75970 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/state.py
+-rw-rw-rw-   0        0        0    16774 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/sticker.py
+-rw-rw-rw-   0        0        0     5563 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/team.py
+-rw-rw-rw-   0        0        0     9590 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/template.py
+-rw-rw-rw-   0        0        0    31430 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/threads.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.649480 discordtool-0.1/discordtool/types/
+-rw-rw-rw-   0        0        0      192 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/__init__.py
+-rw-rw-rw-   0        0        0     2864 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/activity.py
+-rw-rw-rw-   0        0        0     2053 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/appinfo.py
+-rw-rw-rw-   0        0        0     1589 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/application_role_connection.py
+-rw-rw-rw-   0        0        0     6992 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/audit_log.py
+-rw-rw-rw-   0        0        0     2881 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/automod.py
+-rw-rw-rw-   0        0        0     4835 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/channel.py
+-rw-rw-rw-   0        0        0     2630 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/components.py
+-rw-rw-rw-   0        0        0     2486 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/embed.py
+-rw-rw-rw-   0        0        0     1637 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/emoji.py
+-rw-rw-rw-   0        0        0     1451 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/gateway.py
+-rw-rw-rw-   0        0        0     5555 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/guild.py
+-rw-rw-rw-   0        0        0     2341 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/integration.py
+-rw-rw-rw-   0        0        0     7121 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/interactions.py
+-rw-rw-rw-   0        0        0     2853 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/invite.py
+-rw-rw-rw-   0        0        0     1925 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/member.py
+-rw-rw-rw-   0        0        0     4083 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/message.py
+-rw-rw-rw-   0        0        0     4011 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/raw_models.py
+-rw-rw-rw-   0        0        0     1620 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/role.py
+-rw-rw-rw-   0        0        0     2141 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/scheduled_events.py
+-rw-rw-rw-   0        0        0     1254 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/snowflake.py
+-rw-rw-rw-   0        0        0     2449 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/sticker.py
+-rw-rw-rw-   0        0        0     1569 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/team.py
+-rw-rw-rw-   0        0        0     1685 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/template.py
+-rw-rw-rw-   0        0        0     2387 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/threads.py
+-rw-rw-rw-   0        0        0     1686 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/user.py
+-rw-rw-rw-   0        0        0     2412 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/voice.py
+-rw-rw-rw-   0        0        0     2046 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/webhook.py
+-rw-rw-rw-   0        0        0     1524 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1947 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/types/widget.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.671487 discordtool-0.1/discordtool/ui/
+-rw-rw-rw-   0        0        0      330 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/ui/__init__.py
+-rw-rw-rw-   0        0        0    11075 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/ui/button.py
+-rw-rw-rw-   0        0        0     8368 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/ui/input_text.py
+-rw-rw-rw-   0        0        0     4334 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/ui/item.py
+-rw-rw-rw-   0        0        0    11652 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/ui/modal.py
+-rw-rw-rw-   0        0        0    25702 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/ui/select.py
+-rw-rw-rw-   0        0        0    22215 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/ui/view.py
+-rw-rw-rw-   0        0        0    18378 2023-07-17 14:32:48.000000 discordtool-0.1/discordtool/user.py
+-rw-rw-rw-   0        0        0    43234 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/utils.py
+-rw-rw-rw-   0        0        0    33725 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.680749 discordtool-0.1/discordtool/webhook/
+-rw-rw-rw-   0        0        0      249 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/webhook/__init__.py
+-rw-rw-rw-   0        0        0    66249 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/webhook/async_.py
+-rw-rw-rw-   0        0        0    42193 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/webhook/sync.py
+-rw-rw-rw-   0        0        0     8034 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/welcome_screen.py
+-rw-rw-rw-   0        0        0    10838 2023-07-17 14:30:37.000000 discordtool-0.1/discordtool/widget.py
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.429272 discordtool-0.1/discordtool.egg-info/
+-rw-rw-rw-   0        0        0     5517 2023-07-17 16:10:01.000000 discordtool-0.1/discordtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4146 2023-07-17 16:10:02.000000 discordtool-0.1/discordtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 16:10:01.000000 discordtool-0.1/discordtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      379 2023-07-17 16:10:01.000000 discordtool-0.1/discordtool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-17 16:10:01.000000 discordtool-0.1/discordtool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-07-17 14:30:37.000000 discordtool-0.1/install
+-rw-rw-rw-   0        0        0     2290 2023-07-17 16:09:54.000000 discordtool-0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-17 16:10:02.692380 discordtool-0.1/requirements/
+-rw-rw-rw-   0        0        0       73 2023-07-17 14:30:37.000000 discordtool-0.1/requirements/_.txt
+-rw-rw-rw-   0        0        0       53 2023-07-17 14:30:37.000000 discordtool-0.1/requirements/all.txt
+-rw-rw-rw-   0        0        0      183 2023-07-17 14:30:37.000000 discordtool-0.1/requirements/dev.txt
+-rw-rw-rw-   0        0        0      236 2023-07-17 14:30:37.000000 discordtool-0.1/requirements/docs.txt
+-rw-rw-rw-   0        0        0       34 2023-07-17 14:30:37.000000 discordtool-0.1/requirements/speed.txt
+-rw-rw-rw-   0        0        0       20 2023-07-17 14:30:37.000000 discordtool-0.1/requirements/voice.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 16:10:02.696373 discordtool-0.1/setup.cfg
+-rw-rw-rw-   0        0        0       87 2023-07-17 16:09:58.000000 discordtool-0.1/setup.py
```

### Comparing `discordtool-0.0.2/CONTRIBUTING.md` & `discordtool-0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/LICENSE` & `discordtool-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/PKG-INFO` & `discordtool-0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordtool
-Version: 0.0.2
+Version: 0.1
 Summary: A Python wrapper for the discordtool API
 Author: Pycord Development
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `discordtool-0.0.2/README.rst` & `discordtool-0.1/README.rst`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/__init__.py` & `discordtool-0.1/discordtool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 __path__ = __import__("pkgutil").extend_path(__path__, __name__)
 
 import logging
 
 # We need __version__ to be imported first
 # isort: off
 from ._version import *
+
 # isort: on
 
 
 from . import abc, opus, sinks, ui, utils
 from .activity import *
 from .appinfo import *
 from .application_role_connection import *
```

### Comparing `discordtool-0.0.2/discordtool/__main__.py` & `discordtool-0.1/discordtool/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 def show_version() -> None:
     entries = [
         "- Python v{0.major}.{0.minor}.{0.micro}-{0.releaselevel}".format(
             sys.version_info
         )
     ]
 
-    version_info = 0
+    version_info = discordtool.version_info
     entries.append(
         "- discordtool v{0.major}.{0.minor}.{0.micro}-{0.releaselevel}".format(version_info)
     )
     if version_info.releaselevel != "final":
         pkg = pkg_resources.get_distribution("discordtool")
         if pkg:
             entries.append(f"    - discordtool pkg_resources: v{pkg.version}")
```

### Comparing `discordtool-0.0.2/discordtool/_typed_dict.py` & `discordtool-0.1/discordtool/_typed_dict.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/_version.py` & `discordtool-0.1/discordtool/_version.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/abc.py` & `discordtool-0.1/discordtool/abc.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/activity.py` & `discordtool-0.1/discordtool/activity.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/appinfo.py` & `discordtool-0.1/discordtool/appinfo.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/application_role_connection.py` & `discordtool-0.1/discordtool/application_role_connection.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/asset.py` & `discordtool-0.1/discordtool/asset.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/audit_logs.py` & `discordtool-0.1/discordtool/audit_logs.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/automod.py` & `discordtool-0.1/discordtool/automod.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/backoff.py` & `discordtool-0.1/discordtool/backoff.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/bin/libopus-0.x64.dll` & `discordtool-0.1/discordtool/bin/libopus-0.x64.dll`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/bin/libopus-0.x86.dll` & `discordtool-0.1/discordtool/bin/libopus-0.x86.dll`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/bot.py` & `discordtool-0.1/discordtool/bot.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/channel.py` & `discordtool-0.1/discordtool/channel.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/client.py` & `discordtool-0.1/discordtool/client.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/cog.py` & `discordtool-0.1/discordtool/cog.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/colour.py` & `discordtool-0.1/discordtool/colour.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/commands/__init__.py` & `discordtool-0.1/discordtool/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/commands/context.py` & `discordtool-0.1/discordtool/commands/context.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/commands/core.py` & `discordtool-0.1/discordtool/commands/core.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/commands/options.py` & `discordtool-0.1/discordtool/commands/options.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/commands/permissions.py` & `discordtool-0.1/discordtool/commands/permissions.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/components.py` & `discordtool-0.1/discordtool/components.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/context_managers.py` & `discordtool-0.1/discordtool/context_managers.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/embeds.py` & `discordtool-0.1/discordtool/embeds.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/emoji.py` & `discordtool-0.1/discordtool/emoji.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/enums.py` & `discordtool-0.1/discordtool/enums.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/errors.py` & `discordtool-0.1/discordtool/errors.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/bridge/__init__.py` & `discordtool-0.1/discordtool/ext/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/bridge/bot.py` & `discordtool-0.1/discordtool/ext/bridge/bot.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/bridge/context.py` & `discordtool-0.1/discordtool/ext/bridge/context.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/bridge/core.py` & `discordtool-0.1/discordtool/ext/bridge/core.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/commands/_types.py` & `discordtool-0.1/discordtool/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/commands/bot.py` & `discordtool-0.1/discordtool/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/commands/cog.py` & `discordtool-0.1/discordtool/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/commands/context.py` & `discordtool-0.1/discordtool/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/commands/converter.py` & `discordtool-0.1/discordtool/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/commands/cooldowns.py` & `discordtool-0.1/discordtool/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/commands/core.py` & `discordtool-0.1/discordtool/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/commands/errors.py` & `discordtool-0.1/discordtool/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/commands/flags.py` & `discordtool-0.1/discordtool/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/commands/help.py` & `discordtool-0.1/discordtool/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/commands/view.py` & `discordtool-0.1/discordtool/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/pages/pagination.py` & `discordtool-0.1/discordtool/ext/pages/pagination.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ext/tasks/__init__.py` & `discordtool-0.1/discordtool/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/file.py` & `discordtool-0.1/discordtool/file.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/flags.py` & `discordtool-0.1/discordtool/flags.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/gateway.py` & `discordtool-0.1/discordtool/gateway.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/guild.py` & `discordtool-0.1/discordtool/guild.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/http.py` & `discordtool-0.1/discordtool/http.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/integrations.py` & `discordtool-0.1/discordtool/integrations.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/interactions.py` & `discordtool-0.1/discordtool/interactions.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/invite.py` & `discordtool-0.1/discordtool/invite.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/iterators.py` & `discordtool-0.1/discordtool/iterators.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/member.py` & `discordtool-0.1/discordtool/member.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/mentions.py` & `discordtool-0.1/discordtool/mentions.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/message.py` & `discordtool-0.1/discordtool/message.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/mixins.py` & `discordtool-0.1/discordtool/mixins.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/object.py` & `discordtool-0.1/discordtool/object.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/oggparse.py` & `discordtool-0.1/discordtool/oggparse.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/opus.py` & `discordtool-0.1/discordtool/opus.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/partial_emoji.py` & `discordtool-0.1/discordtool/partial_emoji.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/permissions.py` & `discordtool-0.1/discordtool/permissions.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/player.py` & `discordtool-0.1/discordtool/player.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/raw_models.py` & `discordtool-0.1/discordtool/raw_models.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/reaction.py` & `discordtool-0.1/discordtool/reaction.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/role.py` & `discordtool-0.1/discordtool/role.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/scheduled_events.py` & `discordtool-0.1/discordtool/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/shard.py` & `discordtool-0.1/discordtool/shard.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/sinks/core.py` & `discordtool-0.1/discordtool/sinks/core.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/sinks/errors.py` & `discordtool-0.1/discordtool/sinks/errors.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/sinks/m4a.py` & `discordtool-0.1/discordtool/sinks/m4a.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/sinks/mka.py` & `discordtool-0.1/discordtool/sinks/mka.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/sinks/mkv.py` & `discordtool-0.1/discordtool/sinks/mkv.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/sinks/mp3.py` & `discordtool-0.1/discordtool/sinks/mp3.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/sinks/mp4.py` & `discordtool-0.1/discordtool/sinks/mp4.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/sinks/ogg.py` & `discordtool-0.1/discordtool/sinks/ogg.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/sinks/pcm.py` & `discordtool-0.1/discordtool/sinks/pcm.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/sinks/wave.py` & `discordtool-0.1/discordtool/sinks/wave.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/stage_instance.py` & `discordtool-0.1/discordtool/stage_instance.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/state.py` & `discordtool-0.1/discordtool/state.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/sticker.py` & `discordtool-0.1/discordtool/sticker.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/team.py` & `discordtool-0.1/discordtool/team.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/template.py` & `discordtool-0.1/discordtool/template.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/threads.py` & `discordtool-0.1/discordtool/threads.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/activity.py` & `discordtool-0.1/discordtool/types/activity.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/appinfo.py` & `discordtool-0.1/discordtool/types/appinfo.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/application_role_connection.py` & `discordtool-0.1/discordtool/types/application_role_connection.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/audit_log.py` & `discordtool-0.1/discordtool/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/automod.py` & `discordtool-0.1/discordtool/types/automod.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/channel.py` & `discordtool-0.1/discordtool/types/channel.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/components.py` & `discordtool-0.1/discordtool/types/components.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/embed.py` & `discordtool-0.1/discordtool/types/embed.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/emoji.py` & `discordtool-0.1/discordtool/types/emoji.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/gateway.py` & `discordtool-0.1/discordtool/types/gateway.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/guild.py` & `discordtool-0.1/discordtool/types/guild.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/integration.py` & `discordtool-0.1/discordtool/types/integration.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/interactions.py` & `discordtool-0.1/discordtool/types/interactions.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/invite.py` & `discordtool-0.1/discordtool/types/invite.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/member.py` & `discordtool-0.1/discordtool/types/member.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/message.py` & `discordtool-0.1/discordtool/types/message.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/raw_models.py` & `discordtool-0.1/discordtool/types/raw_models.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/role.py` & `discordtool-0.1/discordtool/types/role.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/scheduled_events.py` & `discordtool-0.1/discordtool/types/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/snowflake.py` & `discordtool-0.1/discordtool/types/snowflake.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/sticker.py` & `discordtool-0.1/discordtool/types/sticker.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/team.py` & `discordtool-0.1/discordtool/types/team.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/template.py` & `discordtool-0.1/discordtool/types/template.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/threads.py` & `discordtool-0.1/discordtool/types/threads.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/user.py` & `discordtool-0.1/discordtool/types/user.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/voice.py` & `discordtool-0.1/discordtool/types/voice.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/webhook.py` & `discordtool-0.1/discordtool/types/webhook.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/welcome_screen.py` & `discordtool-0.1/discordtool/types/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/types/widget.py` & `discordtool-0.1/discordtool/types/widget.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ui/button.py` & `discordtool-0.1/discordtool/ui/button.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ui/input_text.py` & `discordtool-0.1/discordtool/ui/input_text.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ui/item.py` & `discordtool-0.1/discordtool/ui/item.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ui/modal.py` & `discordtool-0.1/discordtool/ui/modal.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ui/select.py` & `discordtool-0.1/discordtool/ui/select.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/ui/view.py` & `discordtool-0.1/discordtool/ui/view.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/user.py` & `discordtool-0.1/discordtool/user.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/utils.py` & `discordtool-0.1/discordtool/utils.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/voice_client.py` & `discordtool-0.1/discordtool/voice_client.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/webhook/async_.py` & `discordtool-0.1/discordtool/webhook/async_.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/webhook/sync.py` & `discordtool-0.1/discordtool/webhook/sync.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/welcome_screen.py` & `discordtool-0.1/discordtool/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool/widget.py` & `discordtool-0.1/discordtool/widget.py`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/discordtool.egg-info/PKG-INFO` & `discordtool-0.1/discordtool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordtool
-Version: 0.0.2
+Version: 0.1
 Summary: A Python wrapper for the discordtool API
 Author: Pycord Development
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `discordtool-0.0.2/discordtool.egg-info/SOURCES.txt` & `discordtool-0.1/discordtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discordtool-0.0.2/pyproject.toml` & `discordtool-0.1/pyproject.toml`

 * *Files identical despite different names*

