# Comparing `tmp/nonebot_plugin_groupmate_waifu-1.2.6.tar.gz` & `tmp/nonebot_plugin_groupmate_waifu-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.2.6.tar", last modified: Wed May  3 13:12:14 2023, max compression
+gzip compressed data, was "nonebot_plugin_groupmate_waifu-1.2.7.tar", last modified: Mon Jul 17 15:14:55 2023, max compression
```

## Comparing `nonebot_plugin_groupmate_waifu-1.2.6.tar` & `nonebot_plugin_groupmate_waifu-1.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 13:12:14.630504 nonebot_plugin_groupmate_waifu-1.2.6/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.2.6/LICENSE
--rw-rw-rw-   0        0        0      279 2023-05-03 13:12:14.630004 nonebot_plugin_groupmate_waifu-1.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 13:12:14.618494 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu/
--rw-rw-rw-   0        0        0    20160 2023-05-03 13:08:54.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu/__init__.py
--rw-rw-rw-   0        0        0      305 2023-02-04 06:03:38.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu/config.py
--rw-rw-rw-   0        0        0     2261 2023-02-04 04:51:53.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:12:14.628503 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu.egg-info/
--rw-rw-rw-   0        0        0      279 2023-05-03 13:12:14.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-05-03 13:12:14.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 13:12:14.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-05-03 13:12:14.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-05-03 13:12:14.000000 nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 13:12:14.631005 nonebot_plugin_groupmate_waifu-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      583 2023-05-03 13:12:06.000000 nonebot_plugin_groupmate_waifu-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:14:55.474599 nonebot_plugin_groupmate_waifu-1.2.7/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_groupmate_waifu-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0      279 2023-07-17 15:14:55.474099 nonebot_plugin_groupmate_waifu-1.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 15:14:55.461087 nonebot_plugin_groupmate_waifu-1.2.7/nonebot_plugin_groupmate_waifu/
+-rw-rw-rw-   0        0        0    21635 2023-07-17 14:59:30.000000 nonebot_plugin_groupmate_waifu-1.2.7/nonebot_plugin_groupmate_waifu/__init__.py
+-rw-rw-rw-   0        0        0      354 2023-07-17 15:11:43.000000 nonebot_plugin_groupmate_waifu-1.2.7/nonebot_plugin_groupmate_waifu/config.py
+-rw-rw-rw-   0        0        0     2090 2023-07-17 13:11:31.000000 nonebot_plugin_groupmate_waifu-1.2.7/nonebot_plugin_groupmate_waifu/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:14:55.471595 nonebot_plugin_groupmate_waifu-1.2.7/nonebot_plugin_groupmate_waifu.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-17 15:14:55.000000 nonebot_plugin_groupmate_waifu-1.2.7/nonebot_plugin_groupmate_waifu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-17 15:14:55.000000 nonebot_plugin_groupmate_waifu-1.2.7/nonebot_plugin_groupmate_waifu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 15:14:55.000000 nonebot_plugin_groupmate_waifu-1.2.7/nonebot_plugin_groupmate_waifu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-07-17 15:14:55.000000 nonebot_plugin_groupmate_waifu-1.2.7/nonebot_plugin_groupmate_waifu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-17 15:14:55.000000 nonebot_plugin_groupmate_waifu-1.2.7/nonebot_plugin_groupmate_waifu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 15:14:55.475100 nonebot_plugin_groupmate_waifu-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      583 2023-07-17 15:14:42.000000 nonebot_plugin_groupmate_waifu-1.2.7/setup.py
```

### Comparing `nonebot_plugin_groupmate_waifu-1.2.6/LICENSE` & `nonebot_plugin_groupmate_waifu-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu/__init__.py` & `nonebot_plugin_groupmate_waifu-1.2.7/nonebot_plugin_groupmate_waifu/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,556 +1,560 @@
-from nonebot import require
-from nonebot.plugin.on import on_command
-from nonebot.adapters.onebot.v11 import (
-    GROUP,
-    Bot,
-    GroupMessageEvent,
-    Message,
-    MessageSegment,
-    )
-
-import nonebot
-import os
-import random
-import asyncio
-import time
-
-from pathlib import Path
-
-try:
-    import ujson as json
-except ModuleNotFoundError:
-    import json
-
-from .utils import *
-from .config import Config
-
-# 加载全局配置
-global_config = nonebot.get_driver().config
-waifu_config = Config.parse_obj(global_config.dict())
-
-waifu_cd_bye = waifu_config.waifu_cd_bye
-
-waifu_save = waifu_config.waifu_save
-
-waifu_reset = waifu_config.waifu_reset
-
-HE = waifu_config.waifu_he
-BE = HE + waifu_config.waifu_be
-NTR = waifu_config.waifu_ntr
-
-yinpa_HE = waifu_config.yinpa_he
-yinpa_BE = yinpa_HE + waifu_config.yinpa_be
-yinpa_CP = waifu_config.yinpa_cp
-yinpa_CP = yinpa_HE if yinpa_CP == 0 else yinpa_CP
-
-
-waifu_file = Path() / "data" / "waifu"
-
-if not waifu_file.exists():
-    os.makedirs(waifu_file)
-
-record_waifu_file = waifu_file / "record_waifu"
-record_yinpa1_file = waifu_file / "record_yinpa1"
-record_yinpa2_file = waifu_file / "record_yinpa2"
-
-if waifu_save:
-    def save(file, data):
-        with open(file, "w", encoding="utf8") as f:
-            f.write(str(data))
-else:
-    def save(file, data):
-        pass
-
-scheduler = require("nonebot_plugin_apscheduler").scheduler
-
-if waifu_reset:
-
-    # 判断文件时效
-    timestr = time.strftime('%Y-%m-%d',time.localtime(time.time()))
-    timeArray = time.strptime(timestr,'%Y-%m-%d')
-    Zero_today = time.mktime(timeArray)
-
-    if record_waifu_file.exists() and os.path.getmtime(record_waifu_file) > Zero_today:
-        with open(record_waifu_file,'r') as f:
-            line = f.read()
-            record_waifu = eval(line)
-    else:
-        record_waifu = {}
-
-    if record_yinpa1_file.exists() and os.path.getmtime(record_yinpa1_file) > Zero_today:
-        with open(record_yinpa1_file,'r') as f:
-            line = f.read()
-            record_yinpa1 = eval(line)
-    else:
-        record_yinpa1 = {}
-
-    if record_yinpa2_file.exists() and os.path.getmtime(record_yinpa2_file) > Zero_today:
-        with open(record_yinpa2_file,'r') as f:
-            line = f.read()
-            record_yinpa2 = eval(line)
-    else:
-        record_yinpa2 = {}
-
-    # 重置记录
-
-    @scheduler.scheduled_job("cron",hour = 0)
-    def _():
-        global record_waifu,record_yinpa1,record_yinpa2
-        record_waifu = {}
-        record_yinpa1 = {}
-        record_yinpa2 = {}
-else:
-
-    if record_waifu_file.exists():
-        with open(record_waifu_file,'r') as f:
-            line = f.read()
-            record_waifu = eval(line)
-    else:
-        record_waifu = {}
-
-    if record_yinpa1_file.exists():
-        with open(record_yinpa1_file,'r') as f:
-            line = f.read()
-            record_yinpa1 = eval(line)
-    else:
-        record_yinpa1 = {}
-
-    if record_yinpa2_file.exists():
-        with open(record_yinpa2_file,'r') as f:
-            line = f.read()
-            record_yinpa2 = eval(line)
-    else:
-        record_yinpa2 = {}
-
-    # 重置记录
-    @scheduler.scheduled_job("cron",hour = 0)
-    def _():
-        global record_waifu,record_yinpa1,record_yinpa2
-        for group_id in record_waifu:
-            for user_id in record_waifu[group_id]:
-                if record_waifu[group_id][user_id] == user_id:
-                    record_waifu[group_id][user_id] = 0
-        record_yinpa1 = {}
-        record_yinpa2 = {}
-
-
-
-# 娶群友
-
-waifu = on_command("娶群友", permission=GROUP, priority = 90, block = True)
-
-no_waifu = [
-    "你没有娶到群友，强者注定孤独，加油！",
-    "找不到对象.jpg",
-    "恭喜你没有娶到老婆~",
-    "さんが群友で結婚するであろうヒロインは、\n『自分の左手』です！"
-    ]
-happy_end= [
-    "好耶~",
-    "需要咱主持婚礼吗qwq",
-    "不许秀恩爱！",
-    "(响起婚礼进行曲♪)",
-    "祝你们生八个。"
-    ]
-
-@waifu.handle()
-async def _(bot:Bot, event: GroupMessageEvent):
-    group_id = event.group_id
-    user_id = event.user_id
-    global record_waifu_file, record_waifu
-    record_waifu.setdefault(group_id,{})
-    at = get_message_at(event.json())
-    if at and at[0] != user_id:
-        at = at[0]
-        if record_waifu[group_id].get(user_id,0) == 0:
-            if record_waifu[group_id].get(at,0) in (0, at):
-                X = random.randint(1,100)
-                if 0 < X <= HE:
-                    record_waifu[group_id].update(
-                        {
-                            user_id: at,
-                            at: user_id
-                            }
-                        )
-                    await waifu.send("恭喜你娶到了群友" + MessageSegment.at(at), at_sender=True)
-                    await asyncio.sleep(1)
-                elif HE < X <= BE:
-                    record_waifu[group_id][user_id] = user_id
-                else:
-                    pass
-            else:
-                try:
-                    member = await bot.get_group_member_info(group_id = group_id, user_id = record_waifu[group_id][at])
-                except:
-                    member = None
-                if random.randint(1,100) <= NTR: # 彩蛋
-                    record_waifu[group_id].pop(record_waifu[group_id][at])
-                    record_waifu[group_id].update(
-                        {
-                            user_id: at,
-                            at: user_id
-                            }
-                        )
-                    await waifu.send(
-                        "人家已经名花有主了~" + 
-                        MessageSegment.image(file = await user_img(record_waifu[group_id][at])) +
-                        "ta的CP：" + ( member['card'] or member['nickname'] ) + '\n'
-                        "但是...",
-                        at_sender=True
-                        )
-                else:
-                    await waifu.send(
-                        "人家已经名花有主啦！" + 
-                        MessageSegment.image(file = await user_img(record_waifu[group_id][at])) +
-                        "ta的CP：" + ( member['card'] or member['nickname'] ),
-                        at_sender=True
-                        )
-                await asyncio.sleep(1)
-        elif record_waifu[group_id][user_id] == at:
-            await waifu.finish(
-                "这是你的CP！"+ MessageSegment.at(record_waifu[group_id][user_id]) + '\n' +
-                random.choice(happy_end) +
-                MessageSegment.image(file = await user_img(record_waifu[group_id][user_id])),
-                at_sender=True
-                )
-        elif record_waifu[group_id][user_id] == user_id:
-            pass
-        else:
-            try:
-                member = await bot.get_group_member_info(group_id = group_id, user_id = record_waifu[group_id][user_id])
-            except:
-                member = None
-            if member:
-                await waifu.finish(
-                    "你已经有CP了，不许花心哦~" +
-                    MessageSegment.image(file = await user_img(record_waifu[group_id][user_id])) +
-                    "你的CP：" + ( member['card'] or member['nickname'] ),
-                    at_sender=True
-                    )
-            else:
-                record_waifu[group_id][user_id] = user_id
-
-    if record_waifu[group_id].get(user_id,0) == 0:
-        member_list = await bot.get_group_member_list(group_id = event.group_id)
-        i = 0
-        while i < len(member_list):
-            if member_list[i]['user_id'] in record_waifu[group_id].keys():
-                del member_list[i]
-            else:
-                i += 1
-        else:
-            if member_list:
-                member_list.sort(key = lambda x:x["last_sent_time"] ,reverse = True)
-                member = random.choice(member_list[:80])
-                record_waifu[group_id].update(
-                    {
-                        user_id: member['user_id'],
-                        member['user_id']: user_id
-                        }
-                    )
-                nickname = member['card'] or member['nickname']
-                if record_waifu[group_id][user_id] == user_id:
-                    msg = random.choice(no_waifu)
-                else:
-                    msg = (
-                        "的群友結婚对象是、\n",
-                        MessageSegment.image(file = await user_img(record_waifu[group_id][user_id])),
-                        f"『{nickname}』！"
-                        )
-            else:
-                record_waifu[group_id][user_id] = 1
-                msg = "群友已经被娶光了、\n" + random.choice(no_waifu)
-    else:
-        if record_waifu[group_id][user_id] == event.user_id:
-            msg = random.choice(no_waifu)
-        elif record_waifu[group_id][user_id] == 1:
-            msg = "群友已经被娶光了、\n" + random.choice(no_waifu)
-        else:
-            try:
-                member = await bot.get_group_member_info(group_id = group_id, user_id = record_waifu[group_id][user_id])
-            except:
-                member = None
-            if member:
-                nickname = member['card'] or member['nickname']
-                msg = (
-                    "的群友結婚对象是、\n",
-                    MessageSegment.image(file = await user_img(record_waifu[group_id][user_id])),
-                    f"『{nickname}』！"
-                    )
-            else:
-                msg = random.choice(no_waifu)
-
-    save(record_waifu_file,record_waifu)
-    await waifu.finish(msg, at_sender=True)
-
-# 分手
-
-async def FACTOR(bot: Bot, event: GroupMessageEvent) -> bool:
-    global record_waifu
-    record_waifu.setdefault(event.group_id,{})
-    return record_waifu[event.group_id].get(event.user_id,0) not in (0, 1, event.user_id) and waifu_cd_bye != -1
-
-global cd_bye
-cd_bye = {}
-
-bye = on_command("离婚", aliases = {"分手"}, permission = FACTOR, priority = 90, block = True)
-
-@bye.handle()
-async def _(bot:Bot, event: GroupMessageEvent):
-    global record_waifu_file, record_waifu, cd_bye
-    cd_bye.setdefault(event.group_id,{})
-    flag = cd_bye[event.group_id].setdefault(event.user_id,[0,0])
-    Now = time.time()
-    cd = flag[0] - Now
-    if cd <= 0:
-        cd_bye[event.group_id][event.user_id][0] = Now + waifu_cd_bye
-        A = event.user_id
-        B = int(record_waifu[event.group_id][event.user_id])
-        del record_waifu[event.group_id][A]
-        del record_waifu[event.group_id][B]
-        save(record_waifu_file,record_waifu)
-        if random.randint(1,2) == 1:
-            await bye.finish(random.choice(("嗯。","...","好。")))
-        else:
-            await bye.finish(Message(f'[CQ:poke,qq={event.user_id}]'))
-    else:
-        flag[1] += 1
-        if flag[1] == 1:
-            await bye.finish(f"你的cd还有{round(cd/60,1)}分钟。", at_sender=True)
-        elif flag[1] <= 3:
-            await bye.finish(f"你已经问过了哦~ 你的cd还有{round(cd/60,1)}分钟。", at_sender=True)
-        elif flag[1] <= 10:
-            t = random.randint(flag[1], 3 * flag[1])
-            flag[0] += t * 60
-            await bye.finish(f"还问！罚时！你的cd还有{round(cd/60,1)}+{t}分钟。", at_sender=True)
-        else:
-            if random.randint(1,6) == 6:
-                await bye.finish("哼！")
-
-# 查看娶群友卡池
-
-waifu_list = on_command("查看群友卡池", aliases = {"群友卡池"}, permission = GROUP, priority = 90, block = True)
-
-@waifu_list.handle()
-async def _(bot:Bot, event: GroupMessageEvent):
-    member_list = await bot.get_group_member_list(group_id = event.group_id)
-    i = 0
-    while i < len(member_list):
-        if member_list[i]['user_id'] in record_waifu.setdefault(event.group_id,{}).keys():
-            del member_list[i]
-        else:
-            i += 1
-    else:
-        if member_list:
-            member_list.sort(key = lambda x:x["last_sent_time"] ,reverse = True)
-            msg ="卡池：\n——————————————\n"
-            for member in member_list[:80]:
-                nickname = member['card'] or member['nickname']
-                msg += f"{nickname}\n"
-            else:
-                output = text_to_png(msg[:-1])
-                await waifu_list.finish(MessageSegment.image(output))
-        else:
-            await waifu_list.finish("群友已经被娶光了。")
-
-# 查看本群CP
-
-cp_list = on_command("本群CP", aliases = {"本群cp"}, permission=GROUP, priority = 90, block = True)
-
-@cp_list.handle()
-async def _(bot:Bot, event: GroupMessageEvent):
-    group_id = event.group_id
-    global record_waifu
-    record_waifu.setdefault(group_id,{})
-    lst = record_waifu[group_id].keys()
-    if lst:
-        listA = []
-        listB = []
-        for A in lst:
-            listA.append(A)
-            B = record_waifu[group_id][A]
-            if B not in listA and B != A:
-                listB.append(B)
-
-        msg = ""
-        for user_id in listB:
-            try:
-                member = await bot.get_group_member_info(group_id = group_id, user_id = record_waifu[group_id][user_id])
-                niknameA = member['card'] or member['nickname']
-            except:
-                niknameA = ""
-            try:
-                member = await bot.get_group_member_info(group_id = group_id, user_id = user_id)
-                niknameB = member['card'] or member['nickname']
-            except:
-                niknameB = ""
-            msg += f"♥ {niknameA} | {niknameB}\n"
-        if msg:
-            output = text_to_png("本群CP：\n——————————————\n" + msg[:-1])
-            await cp_list.finish(MessageSegment.image(output))
-
-    await cp_list.finish("本群暂无cp哦~")
-
-
-# 透群友
-
-yinpa = on_command("透群友", permission=GROUP, priority = 90, block = True)
-
-@yinpa.handle()
-async def _(bot:Bot, event: GroupMessageEvent):
-    group_id = event.group_id
-    user_id = event.user_id
-    global record_yinpa1,record_yinpa2
-    at = get_message_at(event.json())
-    msg = ""
-    if at:
-        if at[0] == user_id:
-            pass
-        elif at[0] == record_waifu[group_id].get(user_id,0):
-            X = random.randint(1,100)
-            if 0 < X <= yinpa_CP:
-                member = await bot.get_group_member_info(group_id = group_id, user_id = at[0])
-                nickname = member['card'] or member['nickname']
-                record_yinpa1.setdefault(user_id,0)
-                record_yinpa1[user_id] += 1
-                record_yinpa2.setdefault(member['user_id'],0)
-                record_yinpa2[member['user_id']] += 1
-                msg = (
-                    f"恭喜你涩到了你的老婆\n",
-                    MessageSegment.image(file = await user_img(member["user_id"])),
-                    f"『{nickname}』！"
-                    )
-            else:
-                msg = "你的老婆拒绝和你涩涩！"
-        else:
-            X = random.randint(1,100)
-            if 0 < X <= yinpa_HE:
-                member = await bot.get_group_member_info(group_id = group_id, user_id = at[0])
-                nickname = member['card'] or member['nickname']
-                record_yinpa1.setdefault(user_id,0)
-                record_yinpa1[user_id] += 1
-                record_yinpa2.setdefault(member['user_id'],0)
-                record_yinpa2[member['user_id']] += 1
-                msg = (
-                    f"恭喜你涩到了群友\n",
-                    MessageSegment.image(file = await user_img(member["user_id"])),
-                    f"『{nickname}』！"
-                    )
-            elif yinpa_HE < X < yinpa_BE:
-                msg = "不可以涩涩！"
-            else:
-                pass
-    if not msg:
-        member_list = await bot.get_group_member_list(group_id = event.group_id)
-        member_list.sort(key = lambda x:x["last_sent_time"] ,reverse = True)
-        member = random.choice(member_list[:80])
-        if member["user_id"] == event.user_id:
-            msg = "不可以涩涩！"
-        else:
-            nickname = member['card'] or member['nickname']
-            record_yinpa1.setdefault(user_id,0)
-            record_yinpa1[user_id] += 1
-            record_yinpa2.setdefault(member['user_id'],0)
-            record_yinpa2[member['user_id']] += 1
-            msg = (
-                "的涩涩对象是、\n",
-                MessageSegment.image(file = await user_img(member["user_id"])),
-                f"『{nickname}』！"
-                )
-
-    save(record_yinpa1_file,record_yinpa1)
-    save(record_yinpa2_file,record_yinpa2)
-    await yinpa.finish(msg, at_sender=True)
-
-# 查看涩涩记录
-
-yinpa_list = on_command("涩涩记录",aliases = {"色色记录"}, permission=GROUP, priority = 90, block = True)
-
-@yinpa_list.handle()
-async def _(bot:Bot, event: GroupMessageEvent):
-    global record_yinpa1,record_yinpa2
-
-    msg_list =[]
-
-    # 输出卡池
-    member_list = await bot.get_group_member_list(group_id = event.group_id)
-    member_list.sort(key = lambda x:x["last_sent_time"] ,reverse = True)
-
-    msg ="卡池：\n——————————————\n"
-    for member in member_list[:80]:
-        nickname = member['card'] or member['nickname']
-        msg += f"{nickname}\n"
-
-    output = text_to_png(msg[:-1])
-    msg_list.append(
-        {
-            "type": "node",
-            "data": {
-                "name": "卡池",
-                "uin": event.self_id,
-                "content": MessageSegment.image(output)
-                }
-            }
-        )
-
-    # 输出透群友记录
-
-    record = []
-    for member in member_list:
-        nickname = member['card'] or member['nickname']
-        times = record_yinpa1.get(member['user_id'],0)
-        if times:
-            record.append([nickname,times])
-
-    record.sort(key = lambda x:x[1],reverse = True)
-
-    msg = "涩涩记录①：\n——————————————\n"
-    for info in record:
-        msg += f"[align=left]{info[0]}[/align][align=right]今日透群友 {info[1]} 次[/align]\n"
-    else:
-        if msg:
-            output = bbcode_to_png(msg[:-1])
-            msg_list.append(
-                {
-                    "type": "node",
-                    "data": {
-                        "name": "记录①",
-                        "uin": event.self_id,
-                        "content": MessageSegment.image(output)
-                        }
-                    }
-                )
-        else:
-            pass
-
-    # 输出被透记录
-
-    record = []
-    for member in member_list:
-        nickname = member['card'] or member['nickname']
-        times = record_yinpa2.get(member['user_id'],0)
-        if times:
-            record.append([nickname,times])
-
-    record.sort(key = lambda x:x[1],reverse = True)
-
-    msg = "涩涩记录②：\n——————————————\n"
-    for info in record:
-        msg += f"[align=left]{info[0]}[/align][align=right]今日被透 {info[1]} 次[/align]\n"
-    else:
-        if msg:
-            output = bbcode_to_png(msg[:-1])
-            msg_list.append(
-                {
-                    "type": "node",
-                    "data": {
-                        "name": "记录②",
-                        "uin": event.self_id,
-                        "content": MessageSegment.image(output)
-                        }
-                    }
-                )
-        else:
-            pass
-    await bot.send_group_forward_msg(group_id = event.group_id, messages = msg_list)
+from nonebot import require
+from nonebot.plugin.on import on_command,on_message
+from nonebot.permission import SUPERUSER
+from nonebot.typing import T_State
+from nonebot.adapters.onebot.v11 import (
+    GROUP,
+    GROUP_ADMIN,
+    GROUP_OWNER,
+    Bot,
+    GroupMessageEvent,
+    Message,
+    MessageSegment,
+    )
+
+import nonebot
+import os
+import random
+import asyncio
+import time
+
+from pathlib import Path
+
+try:
+    import ujson as json
+except ModuleNotFoundError:
+    import json
+
+from .utils import *
+from .config import Config
+
+from nonebot.plugin import PluginMetadata
+
+__plugin_meta__ = PluginMetadata(
+    name = "娶群友",
+    description = "娶群友",
+    usage = "娶群友",
+    config = Config,
+    extra = {}
+    )
+
+# 加载全局配置
+global_config = nonebot.get_driver().config
+waifu_config = Config.parse_obj(global_config.dict())
+waifu_cd_bye = waifu_config.waifu_cd_bye
+waifu_save = waifu_config.waifu_save
+waifu_reset = waifu_config.waifu_reset
+last_sent_time_filter = waifu_config.waifu_last_sent_time_filter
+HE = waifu_config.waifu_he
+BE = HE + waifu_config.waifu_be
+NTR = waifu_config.waifu_ntr
+yinpa_HE = waifu_config.yinpa_he
+yinpa_BE = yinpa_HE + waifu_config.yinpa_be
+yinpa_CP = waifu_config.yinpa_cp
+yinpa_CP = yinpa_HE if yinpa_CP == 0 else yinpa_CP
+
+waifu_file = Path() / "data" / "waifu"
+
+if not waifu_file.exists():
+    os.makedirs(waifu_file)
+
+record_CP_file = waifu_file / "record_CP"
+
+if record_CP_file.exists():
+    with open(record_CP_file,'r') as f:
+        line = f.read()
+        record_CP = eval(line)
+else:
+    record_CP = {}
+
+record_waifu_file = waifu_file / "record_waifu"
+if record_waifu_file.exists():
+    with open(record_waifu_file,'r') as f:
+        line = f.read()
+        record_waifu = eval(line)
+else:
+    record_waifu = {}
+
+record_lock_file = waifu_file / "record_lock"
+if record_lock_file.exists():
+    with open(record_lock_file,'r') as f:
+        line = f.read()
+        record_lock = eval(line)
+else:
+    record_lock = {}
+
+record_yinpa1_file = waifu_file / "record_yinpa1"
+if record_yinpa1_file.exists():
+    with open(record_yinpa1_file,'r') as f:
+        line = f.read()
+        record_yinpa1 = eval(line)
+else:
+    record_yinpa1 = {}
+record_yinpa2_file = waifu_file / "record_yinpa2"
+if record_yinpa2_file.exists():
+    with open(record_yinpa2_file,'r') as f:
+        line = f.read()
+        record_yinpa2 = eval(line)
+else:
+    record_yinpa2 = {}
+
+
+if waifu_save:
+    def save(file, data):
+        with open(file, "w", encoding="utf8") as f:
+            f.write(str(data))
+else:
+    def save(file, data):
+        pass
+
+require("nonebot_plugin_apscheduler")
+from nonebot_plugin_apscheduler import scheduler
+
+if waifu_reset:
+
+    # 判断文件时效
+    timestr = time.strftime('%Y-%m-%d',time.localtime(time.time()))
+    timeArray = time.strptime(timestr,'%Y-%m-%d')
+    Zero_today = time.mktime(timeArray)
+
+    if record_CP_file.exists() and os.path.getmtime(record_CP_file) < Zero_today:
+        record_CP = {}
+    if record_waifu_file.exists() and os.path.getmtime(record_waifu_file) > Zero_today:
+        record_waifu = {}
+    if record_lock_file.exists() and os.path.getmtime(record_lock_file) > Zero_today:
+        record_lock = {}
+    if record_yinpa1_file.exists() and os.path.getmtime(record_yinpa1_file) > Zero_today:
+        record_yinpa1 = {}
+    if record_yinpa2_file.exists() and os.path.getmtime(record_yinpa2_file) > Zero_today:
+        record_yinpa2 = {}
+
+    # 重置记录
+    @scheduler.scheduled_job("cron",hour = 0, misfire_grace_time = 120)
+    def _():
+        global record_CP,record_yinpa1,record_yinpa2
+        record_CP = {}
+        record_yinpa1 = {}
+        record_yinpa2 = {}
+else:
+    # 重置记录
+    @scheduler.scheduled_job("cron",hour = 0, misfire_grace_time = 120)
+    def _():
+        global record_CP,record_yinpa1,record_yinpa2
+        for group_id in record_CP:
+            for user_id in record_CP[group_id]:
+                if record_CP[group_id][user_id] == user_id:
+                    record_CP[group_id][user_id] = 0
+        record_yinpa1 = {}
+        record_yinpa2 = {}
+
+protect_list_file = waifu_file / "list_protect"
+if protect_list_file.exists():
+    with open(protect_list_file,'r') as f:
+        line = f.read()
+        protect_list = eval(line)
+else:
+    protect_list = {}
+
+#设置保护名单
+
+protect = on_command("娶群友保护", priority = 80, block = True)
+
+@protect.handle()
+async def _(bot:Bot, event: GroupMessageEvent, permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER):
+    group_id = event.group_id
+    protect_set = protect_list.setdefault(group_id,set())
+    at = get_message_at(event.message)
+    if not at:
+        protect_set.add(event.user_id)
+        save(protect_list_file,protect_list)
+        await protect.finish("保护成功！", at_sender =True)
+    elif await permission(bot,event):
+        protect_set.update(set(at))
+        namelist = '\n'.join([(member['card'] or member['nickname']) for user_id in at if (member := await bot.get_group_member_info(group_id = group_id,user_id = user_id))])
+        save(protect_list_file,protect_list)
+        await protect.finish(f"保护成功！\n保护名单为：\n{namelist}",at_sender =True)
+    else:
+        await protect.finish("保护失败。你无法为其他人设置保护。", at_sender =True)
+
+#移出保护名单
+
+unprotect = on_command("解除娶群友保护", priority = 80,block = True)
+
+@unprotect.handle()
+async def _(bot:Bot, event: GroupMessageEvent, permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER):
+    group_id = event.group_id
+    protect_set = protect_list.setdefault(group_id,set())
+    at = get_message_at(event.message)
+    if not at:
+        user_id = event.user_id
+        if user_id in protect_set:
+            protect_set.discard(user_id)
+            save(protect_list_file,protect_list)
+            await unprotect.finish("解除保护成功！", at_sender =True)
+        else:
+            await unprotect.finish("你不在保护名单内。", at_sender =True)
+    elif await permission(bot,event):
+        valid_at = protect_set & set(at)
+        if not valid_at:
+            await unprotect.finish("保护名单内不存在指定成员。",at_sender =True)
+        protect_set -= valid_at
+        save(protect_list_file,protect_list)
+        namelist = '\n'.join([(member['card'] or member['nickname']) for user_id in valid_at if (member := await bot.get_group_member_info(group_id = group_id,user_id = user_id))])
+        await unprotect.finish(f"解除保护成功！\n解除保护名单为：\n{namelist}",at_sender =True)
+    else:
+        await unprotect.finish("解除保护失败。你无法为其他人解除保护。", at_sender =True)
+
+# 查看保护名单
+show_protect = on_command("查看保护名单", priority = 90,block = True)
+
+@show_protect.handle()
+async def _(bot:Bot, event: GroupMessageEvent):
+    group_id = event.group_id
+    protect_set = protect_list.get(group_id)
+    if not protect_set:
+        await show_protect.finish("保护名单为空")
+    namelist = '\n'.join([(member['card'] or member['nickname']) for user_id in protect_set if (member := await bot.get_group_member_info(group_id = group_id,user_id = user_id))])
+    await show_protect.finish(MessageSegment.image(text_to_png(f"保护名单为：\n{namelist}")))
+     
+# 娶群友
+
+no_waifu = [
+    "你没有娶到群友，强者注定孤独，加油！",
+    "找不到对象.jpg",
+    "恭喜你没有娶到老婆~",
+    "さんが群友で結婚するであろうヒロインは、\n『自分の左手』です！"
+    ]
+
+happy_end= [
+    "好耶~",
+    "需要咱主持婚礼吗qwq",
+    "不许秀恩爱！",
+    "(响起婚礼进行曲♪)",
+    "祝你们生八个。"
+    ]
+
+async def waifu_rule(bot:Bot, event:GroupMessageEvent, state:T_State)-> bool:
+    """
+    规则：娶群友
+    """
+    msg = event.message.extract_plain_text()
+    if not msg.startswith("娶群友"):
+        return False
+    group_id = event.group_id
+    user_id = event.user_id
+    protect_set = protect_list.get(group_id,set())
+    if user_id in protect_set:
+        return False
+    at = get_message_at(event.message)
+    at = at[0] if at else None
+    if at in protect_set:
+        return False
+    tips = "你的群友結婚对象是、"
+    rec = record_CP.setdefault(group_id,{})
+    if (waifu_id := rec.get(user_id)) and waifu_id != user_id:
+        try:
+            member = await bot.get_group_member_info(group_id = group_id, user_id = waifu_id)
+        except:
+            member = None
+            waifu_id = user_id
+        if member:
+            if at:
+                if waifu_id == at:
+                    msg = "这是你的CP！" + random.choice(happy_end) + MessageSegment.image(file = await user_img(waifu_id))
+                    if user_id in record_waifu.get(group_id,set()):
+                        record_lock.setdefault(group_id,{})
+                        record_lock[group_id][waifu_id] = user_id
+                        record_lock[group_id][user_id] = waifu_id
+                        save(record_lock_file,record_lock)
+                        msg += "\ncp已锁！"
+                else:
+                    msg = "你已经有CP了，不许花心哦~" + MessageSegment.image(file = await user_img(waifu_id)) + f"你的CP：{member['card'] or member['nickname']}"
+            else:
+                msg = tips + MessageSegment.image(file = await user_img(waifu_id)) + f"『{member['card'] or member['nickname']}』！"
+            await bot.send(event,msg,at_sender = True)
+            return False
+
+    if at:
+        X = random.randint(1,100)
+        if 0 < X <= HE:
+            waifu_id = at
+            tips = "恭喜你娶到了群友\n" + tips
+        elif HE < X <= BE:
+            waifu_id = user_id
+    if not waifu_id:
+        group_id = event.group_id
+        member_list = await bot.get_group_member_list(group_id = group_id)
+        lastmonth = event.time - last_sent_time_filter
+        id_list = {member['user_id'] for member in member_list if member["last_sent_time"] > lastmonth}
+        waifu_ids = id_list - set(rec.keys())
+        waifu_ids -= protect_set
+        if waifu_ids:
+            waifu_id = random.choice(list(waifu_ids))
+        else:
+            msg = "群友已经被娶光了、\n" + random.choice(no_waifu)
+            await bot.send(event,msg,at_sender = True)
+            return False
+    state["waifu"] = waifu_id,tips
+    return True
+
+waifu = on_message(rule = waifu_rule, priority = 90, block = True)
+
+@waifu.handle()
+async def _(bot:Bot, event: GroupMessageEvent, state:T_State):
+    group_id = event.group_id
+    user_id = event.user_id
+    waifu_id,tips = state["waifu"]
+    if waifu_id == user_id:
+        record_CP[group_id][user_id] = user_id
+        save(record_CP_file,record_CP)
+        await waifu.finish(random.choice(no_waifu),at_sender = True)
+    rec = record_CP.setdefault(group_id,{})
+    waifu_set = record_waifu.setdefault(group_id,set())
+    if waifu_id in rec:
+        waifu_cp = rec[waifu_id]
+        member = await bot.get_group_member_info(group_id = group_id, user_id = waifu_cp)
+        msg = "人家已经名花有主了~" + MessageSegment.image(file = await user_img(waifu_cp)) + "ta的cp：" + (member['card'] or member['nickname'])
+        if waifu_id in record_lock.get(group_id,{}).keys():
+            record_CP[group_id][user_id] = user_id
+            await waifu.finish(msg + "\n本对cp已锁！",at_sender = True)
+        elif random.randint(1,100) <= NTR: # 彩蛋
+            rec.pop(waifu_cp)
+            waifu_set.discard(waifu_cp)
+            await waifu.send(msg + "\n但是...",at_sender = True)
+        else:
+            record_CP[group_id][user_id] = user_id
+            await waifu.finish(msg,at_sender = True)
+        await asyncio.sleep(1)
+    record_CP[group_id][user_id] = waifu_id
+    record_CP[group_id][waifu_id] = user_id
+    waifu_set.add(waifu_id)
+    member = await bot.get_group_member_info(group_id = group_id, user_id = waifu_id)
+    msg = tips + MessageSegment.image(file = await user_img(waifu_id)) + f"『{(member['card'] or member['nickname'])}』！"
+    save(record_waifu_file,record_waifu)
+    save(record_CP_file,record_CP)
+    await waifu.finish(msg, at_sender=True)
+
+# 分手
+if waifu_cd_bye > -1:
+    global cd_bye
+    cd_bye = {}
+
+    bye = on_command(
+        "离婚",
+        aliases = {"分手"},
+        rule = lambda event:event.group_id in record_CP and record_CP[event.group_id].get(event.user_id,event.user_id) != event.user_id,
+        priority = 90,
+        block = True
+        )
+    @bye.handle()
+    async def _(event: GroupMessageEvent):
+        group_id = event.group_id
+        user_id = event.user_id
+        cd_bye.setdefault(group_id,{})
+        T,N,A = cd_bye[group_id].setdefault(user_id,[0,0,0])
+        Now = event.time
+        cd = T - Now
+        if Now > T:
+            cd_bye[group_id][user_id] = [Now + waifu_cd_bye, 0,0]
+            rec = record_CP[group_id]
+            waifu_set = record_waifu.setdefault(group_id,set())
+            waifu_id = rec[user_id]
+            del rec[user_id]
+            del rec[waifu_id]
+            waifu_set.discard(user_id)
+            waifu_set.discard(waifu_id)
+            if group_id in record_lock:
+                if waifu_id in record_lock[group_id]:
+                    del record_lock[group_id][waifu_id]
+                if user_id in record_lock[group_id]: 
+                    del record_lock[group_id][user_id]
+                save(record_lock_file,record_lock)
+            save(record_waifu_file,record_waifu)
+            save(record_CP_file,record_CP)
+            if random.randint(1,2) == 1:
+                await bye.finish(random.choice(("嗯。","...","好。")))
+            else:
+                await bye.finish(Message(f'[CQ:poke,qq={event.user_id}]'))
+        else:
+            if A > Now:
+                A = Now
+                N = 0
+            else:
+                N += 1
+            if N == 1:
+                msg = f"你的cd还有{round(cd/60,1)}分钟。"
+            elif N == 2:
+                msg = f"你已经问过了哦~ 你的cd还有{round(cd/60,1)}分钟。"
+            elif N < 6:
+                T += 10
+                msg = f"还问！罚时！你的cd还有{round(cd/60,1)}+10分钟。"
+            elif random.randint(0,2) == 0:
+                await bye.finish("哼！")
+            else:
+                await bye.finish()
+            cd_bye[group_id][user_id] = [T,N,A]
+            await bye.finish(msg, at_sender = True)
+
+# 查看娶群友卡池
+
+waifu_list = on_command("查看群友卡池", aliases = {"群友卡池"}, priority = 90, block = True)
+
+@waifu_list.handle()
+async def _(bot:Bot, event: GroupMessageEvent):
+    group_id = event.group_id
+    member_list = await bot.get_group_member_list(group_id = group_id)
+    lastmonth = event.time - last_sent_time_filter
+    waifu_ids = protect_list.get(group_id,set()) | set(record_CP.get(group_id).keys())
+    member_list = [member for member in member_list if member['user_id'] not in waifu_ids and member["last_sent_time"] > lastmonth]
+    member_list.sort(key = lambda x:x["last_sent_time"] ,reverse = True)
+    if member_list:
+        msg ="卡池：\n——————————————\n"
+        for member in member_list[:80]:
+            msg += f"{member['card'] or member['nickname']}\n"
+        await waifu_list.finish(MessageSegment.image(text_to_png(msg[:-1])))
+    else:
+        await waifu_list.finish("群友已经被娶光了。")
+
+# 查看本群CP
+
+cp_list = on_command("本群CP", aliases = {"本群cp"}, priority = 90, block = True)
+
+@cp_list.handle()
+async def _(bot:Bot, event: GroupMessageEvent):
+    group_id = event.group_id
+    waifu_set = record_waifu.get(group_id)
+    if not waifu_set:
+        await cp_list.finish("本群暂无cp哦~")
+    rec = record_CP.get(group_id)
+    msg = ""
+    for waifu_id in waifu_set:
+        user_id = rec[waifu_id]
+        try:
+            member = await bot.get_group_member_info(group_id = group_id, user_id = user_id)
+            niknameA = member['card'] or member['nickname']
+        except:
+            niknameA = ""
+        try:
+            member = await bot.get_group_member_info(group_id = group_id, user_id = waifu_id)
+            niknameB = member['card'] or member['nickname']
+        except:
+            niknameB = ""
+
+        msg += f"♥ {niknameA} | {niknameB}\n"
+    await cp_list.finish(MessageSegment.image(text_to_png("本群CP：\n——————————————\n" + msg[:-1])))
+
+
+# 透群友
+async def yinpa_rule(bot:Bot, event:GroupMessageEvent, state:T_State)-> bool:
+    """
+    规则：透群友
+    """
+    msg = event.message.extract_plain_text()
+    if not msg.startswith("透群友"):
+        return False
+    group_id = event.group_id
+    user_id = event.user_id
+    protect_set = protect_list.get(group_id,set())
+    if user_id in protect_set:
+        return False
+    at = get_message_at(event.message)
+    at = at[0] if at else None
+    if at in protect_set:
+        return False
+    yinpa_id = None
+    tips = "你的涩涩对象是、"
+    protect_set = protect_list.get(group_id,set())
+    if at:
+        if at == user_id:
+            msg = f"恭喜你涩到了你自己！" + MessageSegment.image(file = await user_img(user_id))
+            await bot.send(event,msg,at_sender = True)
+            return False
+        elif at == record_CP[group_id].get(user_id,0):
+            if 0 < random.randint(1,100) <= yinpa_CP:
+                tips = "恭喜你涩到了你的老婆！"
+            else:
+                await bot.send(event,"你的老婆拒绝和你涩涩！",at_sender = True)
+                return False
+        X = random.randint(1,100)
+        if 0 < X <= yinpa_HE:
+            yinpa_id = at
+            tips = "恭喜你涩到了群友！" + tips
+        elif yinpa_HE < X <= yinpa_BE:
+            yinpa_id = user_id
+    if not yinpa_id:
+
+        member_list = await bot.get_group_member_list(group_id = group_id)
+        lastmonth = event.time - last_sent_time_filter
+        yinpa_ids = {member['user_id'] for member in member_list if member["last_sent_time"] > lastmonth} - protect_set
+        if not yinpa_ids:
+            return False
+        else:
+            yinpa_id = random.choice(list(yinpa_ids))
+    state["yinpa"] = yinpa_id,tips
+    return True
+
+yinpa = on_message(rule = yinpa_rule, priority = 90, block = True)
+
+@yinpa.handle()
+async def _(bot:Bot, event: GroupMessageEvent, state:T_State):
+    group_id = event.group_id
+    user_id = event.user_id
+    yinpa_id,tips = state["yinpa"]
+    member = await bot.get_group_member_info(group_id = group_id, user_id = yinpa_id)
+    msg = tips + MessageSegment.image(file = await user_img(yinpa_id)) + f"『{(member['card'] or member['nickname'])}』！"
+    record_yinpa1[user_id] = record_yinpa1.get(user_id,0) + 1
+    save(record_yinpa1_file,record_yinpa1)
+    record_yinpa2[user_id] = record_yinpa2.get(yinpa_id,0) + 1
+    save(record_yinpa2_file,record_yinpa2)
+    await yinpa.finish(msg, at_sender=True)
+
+# 查看涩涩记录
+
+yinpa_list = on_command("涩涩记录",aliases = {"色色记录"}, priority = 90, block = True)
+
+@yinpa_list.handle()
+async def _(bot:Bot, event: GroupMessageEvent):
+    group_id = event.group_id
+    msg_list =[]
+    # 输出卡池
+    member_list = await bot.get_group_member_list(group_id = event.group_id)
+    lastmonth = event.time - last_sent_time_filter
+    protect_set = protect_list.get(group_id,set())
+    member_list = [member for member in member_list if member['user_id'] not in protect_set and member["last_sent_time"] > lastmonth]
+    member_list.sort(key = lambda x:x["last_sent_time"] ,reverse = True)
+    msg = "卡池：\n——————————————\n"
+    msg += "\n".join([(member['card'] or member['nickname']) for member in member_list[:80]])
+    msg_list.append({"type": "node",
+                     "data": {
+                         "name": "卡池",
+                         "uin": event.self_id,
+                         "content": MessageSegment.image(text_to_png(msg))}})
+
+    # 输出透群友记录
+
+    record = [((member['card'] or member['nickname']),times) for member in member_list if (times := record_yinpa1.get(member['user_id']))]
+    record.sort(key = lambda x:x[1], reverse = True)
+    msg = "\n".join([f"[align=left]{nickname}[/align][align=right]今日透群友 {times} 次[/align]" for nickname,times in record])
+    if msg:
+        msg_list.append({"type": "node",
+                         "data": {
+                             "name": "记录①",
+                             "uin": event.self_id,
+                             "content": MessageSegment.image(bbcode_to_png("涩涩记录①：\n——————————————\n" + msg))}})
+
+    # 输出被透记录
+
+    record = [((member['card'] or member['nickname']),times) for member in member_list if (times := record_yinpa2.get(member['user_id']))]
+    record.sort(key = lambda x:x[1],reverse = True)
+
+    msg = "涩涩记录②：\n——————————————\n"
+    msg = "\n".join([f"[align=left]{nickname}[/align][align=right]今日被透 {times} 次[/align]"for nickname,times in record])
+    if msg:
+        msg_list.append({"type": "node",
+                         "data": {
+                             "name": "记录②",
+                             "uin": event.self_id,
+                             "content": MessageSegment.image(bbcode_to_png("涩涩记录②：\n——————————————\n" + msg))}})
+
+    await bot.send_group_forward_msg(group_id = event.group_id, messages = msg_list)
     await yinpa_list.finish()
```

### Comparing `nonebot_plugin_groupmate_waifu-1.2.6/nonebot_plugin_groupmate_waifu/utils.py` & `nonebot_plugin_groupmate_waifu-1.2.7/nonebot_plugin_groupmate_waifu/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,72 @@
-import io
-import httpx
-import hashlib
-import asyncio
-
-from nonebot_plugin_imageutils import BuildImage,Text2Image
-
-try:
-    import ujson as json
-except ModuleNotFoundError:
-    import json
-
-async def download_avatar(user_id: int) -> bytes:
-    url = f"http://q1.qlogo.cn/g?b=qq&nk={user_id}&s=640"
-    data = await download_url(url)
-    if hashlib.md5(data).hexdigest() == "acef72340ac0e914090bd35799f5594e":
-        url = f"http://q1.qlogo.cn/g?b=qq&nk={user_id}&s=100"
-        data = await download_url(url)
-    return data
-
-async def download_url(url: str) -> bytes:
-    async with httpx.AsyncClient() as client:
-        for i in range(3):
-            try:
-                resp = await client.get(url, timeout=20)
-                resp.raise_for_status()
-                return resp.content
-            except Exception:
-                await asyncio.sleep(3)
-    raise Exception(f"{url} 下载失败！")
-
-async def download_user_img(user_id: int):
-    data = await download_avatar(user_id)
-    img = BuildImage.open(io.BytesIO(data))
-    return img.save_png()
-
-async def user_img(user_id: int) -> bytes:
-    '''
-    获取用户头像url
-    '''
-    url = f"http://q1.qlogo.cn/g?b=qq&nk={user_id}&s=640"
-    data = await download_url(url)
-    if hashlib.md5(data).hexdigest() == "acef72340ac0e914090bd35799f5594e":
-        url = f"http://q1.qlogo.cn/g?b=qq&nk={user_id}&s=100"
-    return url
-
-def text_to_png(msg):
-    '''
-    文字转png
-    '''
-    output = io.BytesIO()
-    Text2Image.from_text(msg,50,spacing = 10).to_image("white",(20,20)).save(output, format="png")
-    return output
-
-def bbcode_to_png(msg, spacing: int = 10):
-    '''
-    bbcode文字转png
-    '''
-    output = io.BytesIO()
-    Text2Image.from_bbcode_text(msg, 50, spacing = spacing).to_image("white", (20,20)).save(output, format="png")
-    return output
-
-def get_message_at(data: str) -> list:
-    '''
-    获取at列表
-    :param data: event.json()
-    '''
-    qq_list = []
-    data = json.loads(data)
-    try:
-        for msg in data['message']:
-            if msg['type'] == 'at':
-                qq_list.append(int(msg['data']['qq']))
-        return qq_list
-    except Exception:
-        return []
+import io
+import httpx
+import hashlib
+import asyncio
+
+from pil_utils import BuildImage,Text2Image
+from nonebot.adapters.onebot.v11 import Message
+
+try:
+    import ujson as json
+except ModuleNotFoundError:
+    import json
+
+async def download_avatar(user_id: int) -> bytes:
+    url = f"https://q1.qlogo.cn/g?b=qq&nk={user_id}&s=640"
+    data = await download_url(url)
+    if hashlib.md5(data).hexdigest() == "acef72340ac0e914090bd35799f5594e":
+        url = f"https://q1.qlogo.cn/g?b=qq&nk={user_id}&s=100"
+        data = await download_url(url)
+    return data
+
+async def download_url(url: str) -> bytes:
+    async with httpx.AsyncClient() as client:
+        for i in range(3):
+            try:
+                resp = await client.get(url, timeout=20)
+                resp.raise_for_status()
+                return resp.content
+            except Exception:
+                await asyncio.sleep(3)
+    raise Exception(f"{url} 下载失败！")
+
+async def download_user_img(user_id: int):
+    data = await download_avatar(user_id)
+    img = BuildImage.open(io.BytesIO(data))
+    return img.save_png()
+
+async def user_img(user_id: int) -> bytes:
+    '''
+    获取用户头像url
+    '''
+    url = f"https://q1.qlogo.cn/g?b=qq&nk={user_id}&s=640"
+    data = await download_url(url)
+    if hashlib.md5(data).hexdigest() == "acef72340ac0e914090bd35799f5594e":
+        url = f"https://q1.qlogo.cn/g?b=qq&nk={user_id}&s=100"
+    return url
+
+def text_to_png(msg):
+    '''
+    文字转png
+    '''
+    output = io.BytesIO()
+    Text2Image.from_text(msg,50,spacing = 10).to_image("white",(20,20)).save(output, format="png")
+    return output
+
+def bbcode_to_png(msg, spacing: int = 10):
+    '''
+    bbcode文字转png
+    '''
+    output = io.BytesIO()
+    Text2Image.from_bbcode_text(msg, 50, spacing = spacing).to_image("white", (20,20)).save(output, format="png")
+    return output
+
+def get_message_at(message:Message) -> list:
+    '''
+    获取at列表
+    '''
+    qq_list = []
+    for msg in message:
+        if msg.type == "at":
+            qq_list.append(int(msg.data["qq"]))
+    return qq_list
```

### Comparing `nonebot_plugin_groupmate_waifu-1.2.6/setup.py` & `nonebot_plugin_groupmate_waifu-1.2.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_groupmate_waifu',
-version='1.2.6',
+version='1.2.7',
 description='娶群友',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_groupmate_waifu"]),
```

