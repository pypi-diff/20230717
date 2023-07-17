# Comparing `tmp/arkprts-0.2.4.tar.gz` & `tmp/arkprts-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkprts-0.2.4.tar", last modified: Sat Jul  8 21:45:22 2023, max compression
+gzip compressed data, was "arkprts-0.2.5.tar", last modified: Mon Jul 17 20:52:07 2023, max compression
```

## Comparing `arkprts-0.2.4.tar` & `arkprts-0.2.5.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:45:22.763181 arkprts-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-08 21:45:13.000000 arkprts-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-08 21:45:22.763181 arkprts-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-08 21:45:13.000000 arkprts-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:45:22.759181 arkprts-0.2.4/arkprts/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-08 21:45:13.000000 arkprts-0.2.4/arkprts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-08 21:45:13.000000 arkprts-0.2.4/arkprts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39810 2023-07-08 21:45:13.000000 arkprts-0.2.4/arkprts/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-07-08 21:45:13.000000 arkprts-0.2.4/arkprts/automation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-07-08 21:45:13.000000 arkprts-0.2.4/arkprts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-08 21:45:13.000000 arkprts-0.2.4/arkprts/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-07-08 21:45:13.000000 arkprts-0.2.4/arkprts/gamedata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:45:22.759181 arkprts-0.2.4/arkprts/models/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-08 21:45:13.000000 arkprts-0.2.4/arkprts/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-08 21:45:13.000000 arkprts-0.2.4/arkprts/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-07-08 21:45:13.000000 arkprts-0.2.4/arkprts/models/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-07-08 21:45:13.000000 arkprts-0.2.4/arkprts/models/social.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:45:13.000000 arkprts-0.2.4/arkprts/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:45:22.759181 arkprts-0.2.4/arkprts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-08 21:45:22.000000 arkprts-0.2.4/arkprts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-08 21:45:22.000000 arkprts-0.2.4/arkprts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:45:22.000000 arkprts-0.2.4/arkprts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-08 21:45:22.000000 arkprts-0.2.4/arkprts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 21:45:22.000000 arkprts-0.2.4/arkprts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-08 21:45:13.000000 arkprts-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:45:22.763181 arkprts-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-08 21:45:13.000000 arkprts-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:45:22.763181 arkprts-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-08 21:45:13.000000 arkprts-0.2.4/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-08 21:45:13.000000 arkprts-0.2.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-08 21:45:13.000000 arkprts-0.2.4/tests/test_gamedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:07.467250 arkprts-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 20:51:54.000000 arkprts-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-17 20:52:07.467250 arkprts-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-17 20:51:54.000000 arkprts-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:07.463250 arkprts-0.2.5/arkprts/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-17 20:51:54.000000 arkprts-0.2.5/arkprts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-17 20:51:54.000000 arkprts-0.2.5/arkprts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39820 2023-07-17 20:51:54.000000 arkprts-0.2.5/arkprts/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-07-17 20:51:54.000000 arkprts-0.2.5/arkprts/automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9498 2023-07-17 20:51:54.000000 arkprts-0.2.5/arkprts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-17 20:51:54.000000 arkprts-0.2.5/arkprts/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-17 20:51:54.000000 arkprts-0.2.5/arkprts/gamedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:07.467250 arkprts-0.2.5/arkprts/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 20:51:54.000000 arkprts-0.2.5/arkprts/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-17 20:51:54.000000 arkprts-0.2.5/arkprts/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-17 20:51:54.000000 arkprts-0.2.5/arkprts/models/battle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-17 20:51:54.000000 arkprts-0.2.5/arkprts/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-07-17 20:51:54.000000 arkprts-0.2.5/arkprts/models/social.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:51:54.000000 arkprts-0.2.5/arkprts/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:07.463250 arkprts-0.2.5/arkprts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-17 20:52:07.000000 arkprts-0.2.5/arkprts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-17 20:52:07.000000 arkprts-0.2.5/arkprts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:52:07.000000 arkprts-0.2.5/arkprts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 20:52:07.000000 arkprts-0.2.5/arkprts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 20:52:07.000000 arkprts-0.2.5/arkprts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-17 20:51:54.000000 arkprts-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:52:07.467250 arkprts-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-17 20:51:54.000000 arkprts-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:07.467250 arkprts-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-17 20:51:54.000000 arkprts-0.2.5/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-17 20:51:54.000000 arkprts-0.2.5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-17 20:51:54.000000 arkprts-0.2.5/tests/test_gamedata.py
```

### Comparing `arkprts-0.2.4/LICENSE` & `arkprts-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.4/PKG-INFO` & `arkprts-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.2.4
+Version: 0.2.5
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: rsa
@@ -13,15 +13,15 @@
 
 # ArkPRTS
 
 Arknights python wrapper.
 
 Interacts directly with the game servers, no delays.
 
-支持**中文和 B 站**账户!
+支持**中文和B站**账户!
 
 <!-- Supports Chinese and BiliBili accounts -->
 
 ---
 
 Source Code: <https://github.com/thesadru/arkprts>
```

### Comparing `arkprts-0.2.4/README.md` & `arkprts-0.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ArkPRTS
 
 Arknights python wrapper.
 
 Interacts directly with the game servers, no delays.
 
-支持**中文和 B 站**账户!
+支持**中文和B站**账户!
 
 <!-- Supports Chinese and BiliBili accounts -->
 
 ---
 
 Source Code: <https://github.com/thesadru/arkprts>
```

### Comparing `arkprts-0.2.4/arkprts/__main__.py` & `arkprts-0.2.5/arkprts/__main__.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.4/arkprts/auth.py` & `arkprts-0.2.5/arkprts/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
 RawAuthMapping = typing.TypedDict("RawAuthMapping", {"server": ArknightsServer, "channel_uid": str, "token": str})
 
 
 def parse_server(identifier: ArknightsIdentifier) -> tuple[ArknightsDistributor, ArknightsServer, ArknightsLanguage]:
     """Parse a server, distributor, or language into a distributor, server, and language."""
     if identifier not in REGION_IDENTIFIER_MAPPING:
-        raise ValueError(f"Invalid region, server, or language {identifier!r}")
+        raise ValueError(f"Invalid distributor, server, or language {identifier!r}")
 
     result = REGION_IDENTIFIER_MAPPING[identifier]
     if result is None:
         raise ValueError(f"{identifier} is not supported")
 
     return result
 
@@ -371,27 +371,27 @@
     network: NetworkSession
     """Network session."""
 
     async def auth_request(
         self,
         endpoint: str,
         *,
-        region: ArknightsServer | None = None,
+        server: ArknightsServer | None = None,
         **kwargs: typing.Any,
     ) -> typing.Any:
         """Send an authenticated request to the arkights game server."""
 
 
 class Auth(abc.ABC, CoreAuth):
     """Authentication client for single sessions."""
 
     server: ArknightsServer
-    """Arknights region."""
-    distributor: ArknightsDistributor
     """Arknights server."""
+    distributor: ArknightsDistributor
+    """Arknights distributor."""
     network: NetworkSession
     """Network session."""
     device_ids: tuple[str, str, str]
     """Device ids."""
     session: AuthSession
     """Authentication session."""
 
@@ -438,15 +438,15 @@
         endpoint: str,
         *,
         server: ArknightsServer | None = None,
         **kwargs: typing.Any,
     ) -> typing.Any:
         """Send an authenticated request to the arknights game server."""
         if server and server != self.server:
-            raise ValueError(f"Single-session client is bound to {self.server!r} region.")
+            raise ValueError(f"Single-session client is bound to {self.server!r} server.")
 
         if not self.session.uid:
             raise errors.NotLoggedInError("Not logged in.")
 
         async with self.session as headers:
             logger.debug("[UID: %s] Sending request #%s to %s.", self.uid, headers["seqnum"], endpoint)
             return await self.request("gs", endpoint, headers=headers, server=self.server, **kwargs)
@@ -517,35 +517,35 @@
         self.session.secret = secret
         logger.info("Logged in with UID %s", uid)
         return secret
 
     @classmethod
     async def from_token(
         cls,
-        region: ArknightsServer,
+        server: ArknightsServer,
         channel_uid: str,
         token: str,
         *,
         network: NetworkSession | None = None,
     ) -> Auth:
         """Create a client from a token."""
-        if region in ("en", "jp", "kr"):
-            auth = YostarAuth(region, network=network)
+        if server in ("en", "jp", "kr"):
+            auth = YostarAuth(server, network=network)
             await auth.login_with_token(channel_uid, token)
-        elif region == "cn":
-            auth = HypergryphAuth(region, network=network)
+        elif server == "cn":
+            auth = HypergryphAuth(server, network=network)
             await auth.login_with_token(channel_uid, token)
-        elif region == "bili":
-            auth = BilibiliAuth(region, network=network)
+        elif server == "bili":
+            auth = BilibiliAuth(server, network=network)
             await auth.login_with_token(channel_uid, token)
-        elif region == "tw":
-            auth = LongchengAuth(region, network=network)
+        elif server == "tw":
+            auth = LongchengAuth(server, network=network)
             await auth.login_with_token(channel_uid, token)
         else:
-            raise ValueError(f"Cannot create a generic auth client for region {region!r}")
+            raise ValueError(f"Cannot create a generic auth client for server {server!r}")
 
         return auth
 
 
 class YostarAuth(Auth):
     """Authentication client for global accounts."""
 
@@ -889,15 +889,15 @@
     """Authentication client for multiple sessions."""
 
     network: NetworkSession
     """Network session."""
 
     # may be exceeded if multiple sessions are created at once
     max_sessions: int
-    """Maximum number of concurrent sessions per region."""
+    """Maximum number of concurrent sessions per server."""
     sessions: list[AuthSession]
     """Authentication sessions."""
 
     def __init__(
         self,
         max_sessions: int = 6,
         *,
```

### Comparing `arkprts-0.2.4/arkprts/automation.py` & `arkprts-0.2.5/arkprts/automation.py`

 * *Files 3% similar despite different names*

```diff
@@ -284,14 +284,21 @@
         APP behavior: Called when claiming all trading post products.
         """
         data = {
             "slotList": slot_list,
         }
         return await self.request("building/deliveryBatchOrder", json=data)
 
+    async def building_gain_all_intimacy(self) -> typing.Any:
+        """Claim trust increase of all operators stationed in the base.
+
+        APP behavior: Called when claiming trust of all operators in the base every 12h.
+        """
+        return await self.request("building/gainAllIntimacy")
+
     async def building_accelerate_solution(self, slot_id: str, cost: int) -> typing.Any:
         """Accelerate a room with drones.
 
         slot_id: Room slot ID to accelerate.
         cost: Amount of drones to use.
 
         APP behavior: Called when using drones.
@@ -388,14 +395,26 @@
     async def building_start_info_share(self) -> typing.Any:
         """Start a clue exchange.
 
         APP behavior: Called when starting a clue exchange in the meeting room after gathering all clues.
         """
         return await self.request("building/startInfoShare")
 
+    async def building_get_meetingroom_reward(self, type: typing.Sequence[int]) -> typing.Any:
+        """Get rewards from a clue exchange and such.
+
+        type: Array of booleans. No idea what they correspond to. I got [0, 1]
+
+        APP behavior: Called when entering the base.
+        """
+        data = {
+            "type": type,
+        }
+        return await self.request("building/getMeetingroomReward", json=data)
+
     async def social_get_friend_list(self, id_list: typing.Sequence[str]) -> typing.Any:
         """Get a list of friends by ID.
 
         APP behavior: Called after any request for friend IDs.
         """
         data = {
             "idList": id_list,
@@ -481,17 +500,19 @@
         APP behavior: Called when finishing a recruitment.
         """
         data = {
             "slotId": slot_id,
         }
         return await self.request("gacha/finishNormalGacha", json=data)
 
-    async def get_battle_replay(self, battle_type: str, stage_id: str) -> typing.Any:
+    async def battle_get_battle_replay(self, battle_type: str, stage_id: str) -> typing.Any:
         """Get a replay of a stage.
 
+        Needs to be decrypted with decrypt_battle_replay.
+
         stage_id: Stage ID.
 
         APP behavior: Called when entering the squad selection screen with auto-deploy enabled.
         """
         data = {
             "stageId": stage_id,
         }
```

### Comparing `arkprts-0.2.4/arkprts/client.py` & `arkprts-0.2.5/arkprts/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,21 +13,24 @@
 >>> await client.get_data()
 User(...)
 
 >>> # Client for read & write (usage is potentially bannable)
 >>> auth = arkprts.YostarAuth("en")
 >>> await auth.login_with_email_code("doctor@gmail.com")
 >>> client = arkprts.AutomationClient(auth=auth)
->>> await client.login_with_token("...", "...")
 >>> await client.account_sync_data()
 """
 from __future__ import annotations
 
+import base64
+import io
+import json
 import typing
 import warnings
+import zipfile
 
 from . import auth as authn
 from . import gamedata as gd
 from . import models
 
 if typing.TYPE_CHECKING:
     from typing_extensions import Self
@@ -205,14 +208,24 @@
         return await self._get_social_sort_list(
             0,
             ["level"],
             {"nickName": nickname, "nickNumber": nicknumber},
             server=server,
         )
 
+    async def get_raw_battle_replay(self, battle_type: str, stage_id: str) -> typing.Any:
+        """Get a battle replay."""
+        self._assert_private()
+
+        data = await self.request(f"{battle_type}/getBattleReplay", json={"stageId": stage_id})
+
+        replay_data = base64.b64decode(data["battleReplay"])
+        with zipfile.ZipFile(io.BytesIO(replay_data), "r") as z, z.open("default_entry") as f:
+            return json.load(f)
+
     async def search_players(
         self,
         nickname: str,
         nicknumber: str = "",
         *,
         server: authn.ArknightsServer | None = None,
         limit: int | None = None,
@@ -246,7 +259,12 @@
         data = await self.get_raw_friend_info([uid["uid"] for uid in uid_data["result"][:limit]], server=server)
         return [models.Player(client=self, **i) for i in data["friends"]]
 
     async def get_data(self) -> models.User:
         """Get user sync data and return a model. Use raw data for more info."""
         data = await self.get_raw_data()
         return models.User(client=self, **data["user"])
+
+    async def get_battle_replay(self, battle_type: str, stage_id: str) -> models.BattleReplay:
+        """Get a battle replay and return a model."""
+        data = await self.get_raw_battle_replay(battle_type, stage_id)
+        return models.BattleReplay(client=self, **data)
```

### Comparing `arkprts-0.2.4/arkprts/errors.py` & `arkprts-0.2.5/arkprts/errors.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.4/arkprts/gamedata.py` & `arkprts-0.2.5/arkprts/gamedata.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 from arkprts.auth import ArknightsLanguage
 from arkprts.models import base as models
 
 __all__ = ("GameData",)
 
 PathLike = typing.Union[pathlib.Path, str]
 
-GITHUB_REPOSITORY = "aelurum/ArknightsGameData"  # zh-tw fork
-FALLBACK_GITHUB_REPOSITORY = "Kengxxiao/ArknightsGameData"
+GITHUB_REPOSITORY = "Kengxxiao/ArknightsGameData"
+TW_GITHUB_REPOSITORY = "aelurum/ArknightsGameData"  # zh-tw fork
 RELEVANT_FILES = r"excel"
 
 logger: logging.Logger = logging.getLogger("arkprts.gamedata")
 
 
 class GameData:
     """Game data client."""
@@ -159,35 +159,35 @@
             if (await proc.wait()) == 0:
                 await self.update_git_gamedata()
             else:
                 await self.download_tarball_gamedata(allow=allow, force=force)
 
             self.loaded = True
 
-    def _get_data(self, filename: str, *, language: str | None = None) -> models.DDict:
+    def _get_data(self, filename: str, *, language: str | None = None) -> typing.Any:
         """Get a file."""
         language = language or self.language
 
         if self._cache.get(language, {}).get(filename):
-            return models.DDict(self._cache[language][filename])
+            return self._cache[language][filename]
 
         path = self.directory / language / "gamedata" / filename
         if not path.exists():
             raise FileNotFoundError("Static gamedata has not been loaded.")
 
         with path.open(encoding="utf-8") as file:
             data = json.load(file)
 
         self._cache.setdefault(language, {})[filename] = data
 
-        return models.DDict(data)
+        return data
 
     def get_excel(self, name: str, *, language: str | None = None) -> models.DDict:
         """Get an excel table file."""
-        return self._get_data(f"excel/{name}.json", language=language)
+        return models.DDict(self._get_data(f"excel/{name}.json", language=language))
 
     def __getitem__(self, name: str) -> models.DDict:
         """Get an excel table file."""
         return self.get_excel(name)
 
     def __getattr__(self, name: str) -> models.DDict:
         """Get an excel table file."""
```

### Comparing `arkprts-0.2.4/arkprts/models/base.py` & `arkprts-0.2.5/arkprts/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     """Parse an arknights timestamp and use the local timezone.
 
     Arknights provides timestamps not with UTC but with the client's timezone.
     """
     if timestamp in (0, -1):
         return None
 
-    return datetime.datetime.fromtimestamp(timestamp).astimezone()  # noqa: DTZ006
+    return datetime.datetime.fromtimestamp(int(timestamp)).astimezone()
 
 
 class BaseModel(pydantic.BaseModel, arbitrary_types_allowed=True):
     """Client-aware pydantic base model."""
 
     client: CoreClient = pydantic.Field(repr=False)
     """Client instance."""
@@ -61,15 +61,17 @@
         if client:
             _set_recursively(self, "client", client)
 
     @pydantic.model_validator(mode="before")
     def _fix_amiya(cls, value: typing.Any, info: pydantic.ValidationInfo) -> typing.Any:
         """Flatten Amiya to only keep her selected form if applicable."""
         if value and value.get("tmpl"):
-            current = value["tmpl"][value["currentTmpl"]]
+            # tmplId present in battle replays
+            current_tmpl = value["currentTmpl"] if "currentTmpl" in value else value["tmplId"]
+            current = value["tmpl"][current_tmpl]
             value.update(current)
 
         return value
 
 
 class DList(collections.UserList[typing.Any]):
     """Dot-accessed list."""
```

### Comparing `arkprts-0.2.4/arkprts/models/data.py` & `arkprts-0.2.5/arkprts/models/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Arknights API data models.
 
 Any field description prefixed with IDK means it's just a guess.
 """
+import datetime
 import typing
 
 import pydantic
 
 from . import base
 
 
@@ -40,51 +41,51 @@
     hgg_shard: int = pydantic.Field(alias="hggShard")
     """Amount of yellow distinction certificates."""
     lgg_shard: int = pydantic.Field(alias="lggShard")
     """Amount of green commendation certificates.."""
     recruit_license: int = pydantic.Field(alias="recruitLicense")
     """Amount of recruitment permit."""
     progress: int = pydantic.Field(repr=False)
-    """IDK."""
+    """IDK. Seems to always be 3000."""
     buy_ap_remain_times: int = pydantic.Field(alias="buyApRemainTimes", repr=False)
-    """IDK. Ap refers to sanity."""
+    """How many more times you can refresh sanity with originite prime."""
     ap_limit_up_flag: bool = pydantic.Field(alias="apLimitUpFlag", repr=False)
-    """IDK. Ap refers to sanity."""
+    """IDK. Ap refers to sanity. Always zero."""
     uid: str
     """User ID."""
     flags: typing.Mapping[str, bool] = pydantic.Field(repr=False)
     """Completed stories."""
     ap: int
-    """Current sanity. Actually not a true value."""
+    """Sanity value when last incrememnted. See current_sanity for true value."""
     max_ap: int = pydantic.Field(alias="maxAp")
     """Max sanity."""
     pay_diamond: int = pydantic.Field(alias="payDiamond")
     """Bough originium prime."""
     free_diamond: int = pydantic.Field(alias="freeDiamond")
     """Earned originium prime."""
     diamond_shard: int = pydantic.Field(alias="diamondShard")
     """Amount of orundum."""
     gold: int
     """Amount of LMD."""
     practice_ticket: int = pydantic.Field(alias="practiceTicket")
     """Amount of training permits."""
     last_refresh_ts: base.ArknightsTimestamp = pydantic.Field(alias="lastRefreshTs")
-    """IDK. When sanity was last incremented."""
+    """Last time a sanity refresh was used. IDK the influence on ap calculation."""
     last_ap_add_time: base.ArknightsTimestamp = pydantic.Field(alias="lastApAddTime")
-    """IDK."""
+    """Last time AP was incremented/calculated."""
     last_online_ts: base.ArknightsTimestamp = pydantic.Field(alias="lastOnlineTs")
-    """IDK. When the player was last online."""
+    """When the player was last online."""
     main_stage_progress: typing.Optional[str] = pydantic.Field(alias="mainStageProgress")
     """Current main story stage ID. None if completed."""
     register_ts: base.ArknightsTimestamp = pydantic.Field(alias="registerTs")
     """Account creation time."""
     server_name: str = pydantic.Field(alias="serverName")
     """Server name. Should always be Terra."""
     avatar_id: str = pydantic.Field(alias="avatarId", repr=False)
-    """IDK. Always 0."""
+    """IDK. Always "0"."""
     resume: str
     """Player display bio."""
     friend_num_limit: int = pydantic.Field(alias="friendNumLimit")
     """How many friend slots are open."""
     secretary: str
     """ID of the secretary operator."""
     secretary_skin_id: str = pydantic.Field(alias="secretarySkinId")
@@ -97,18 +98,26 @@
     # fmt: off
     # optional:
     monthly_subscription_start_time: typing.Optional[base.ArknightsTimestamp] = pydantic.Field(None, alias="monthlySubscriptionStartTime")
     """When the monthly subscription started."""
     monthly_subscription_end_time: typing.Optional[base.ArknightsTimestamp] = pydantic.Field(None, alias="monthlySubscriptionEndTime")
     """When the monthly subscription is ending."""
     tip_monthly_card_expire: typing.Optional[base.ArknightsTimestamp] = pydantic.Field(None, alias="tipMonthlyCardExpire")
-    """IDK."""
+    """IDK. Seems to be close to register time, so likely the first the monthly card was used?"""
     # fmt: on
 
     @property
+    def current_ap(self) -> int:
+        """Current sanity."""
+        last_calculation = max(self.last_refresh_ts, self.last_ap_add_time)
+        since_calculation = last_calculation - datetime.datetime.now(tz=datetime.timezone.utc)
+        ap_add_amount = since_calculation // datetime.timedelta(minutes=6)
+        return self.ap + ap_add_amount
+
+    @property
     def basic_item_inventory(self) -> typing.Mapping[str, int]:
         """Basic item inventory. These are not shown in the inventory object."""
         return {
             "SOCIAL_PT": self.social_point,
             "AP_GAMEPLAY": self.ap,
             "4001": self.gold,
             "4002": self.pay_diamond + self.free_diamond,
@@ -156,15 +165,15 @@
     unlock: bool
     """Whether the skill is unlocked."""
     state: bool = pydantic.Field(repr=False)
     """IDK. Always false."""
     specialize_level: int = pydantic.Field(alias="specializeLevel")
     """Skill mastery level."""
     complete_upgrade_time: typing.Optional[base.ArknightsTimestamp] = pydantic.Field(alias="completeUpgradeTime")
-    """IDK. Time left until skill upgrade is complete. Is raw -1 if not upgrading."""
+    """IDK. Time of mastery upgrade completion. Is raw -1 if not upgrading."""
 
     @property
     def static(self) -> base.DDict:
         """Static data for this skill."""
         return self.client.gamedata.skill_table[self.skill_id]
 
 
@@ -248,17 +257,17 @@
     squads: typing.Mapping[int, Squads]
     """Squad data."""
     chars: typing.Mapping[int, Character]
     """Operator data."""
     char_group: typing.Mapping[str, CharGroup] = pydantic.Field(alias="charGroup")
     """Additional operator data."""
     char_mission: typing.Mapping[str, typing.Mapping[str, int]] = pydantic.Field(alias="charMission", repr=False)
-    """IDK. Special operation missions."""
+    """IDK. Special operation missions. See GameData char_meta_table."""
     addon: base.DDict = pydantic.Field(default_factory=base.DDict, repr=False)
-    """IDK."""
+    """IDK. Unlockable character story and stage."""
 
 
 class Skins(base.BaseModel):
     """Operator skin data."""
 
     character_skins: typing.Mapping[str, bool] = pydantic.Field(alias="characterSkins")
     """Owned skins."""
@@ -283,15 +292,15 @@
     """Social data."""
 
     assist_char_list: typing.Sequence[typing.Optional[AssistChar]] = pydantic.Field(alias="assistCharList")
     """Support operators."""
     yesterday_reward: base.DDict = pydantic.Field(alias="yesterdayReward")
     """IDK. Clue exchange data."""
     y_crisis_ss: typing.Union[str, typing.Any] = pydantic.Field(alias="yCrisisSs", repr=False)
-    """IDK."""
+    """IDK. Crisis refers to contingency contract. Always empty string."""
     medal_board: base.DDict = pydantic.Field(default_factory=base.DDict, alias="medalBoard")
     """Medal board."""
 
 
 class ConsumableExpire(base.BaseModel):
     """Consumable expiration data."""
```

### Comparing `arkprts-0.2.4/arkprts/models/social.py` & `arkprts-0.2.5/arkprts/models/social.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         return self.client.gamedata.skill_table[self.skill_id]
 
 
 class UniEquip(base.BaseModel):
     """Equipped modules."""
 
     hide: bool
-    """IDK. Whether the module is publicly hidden."""
+    """Whether the player may see the modules. For operators below E2."""
     locked: bool
     """Whether module access is locked."""
     level: int
     """Module level."""
 
 
 class AssistChar(base.BaseModel):
@@ -182,12 +182,12 @@
     resume: str
     """Player display bio."""
     team_v2: typing.Mapping[str, int] = pydantic.Field(alias="teamV2")
     """Amount of characters owned in each faction."""
     board: typing.Sequence[str]
     """Owned clues in the meeting room."""
     info_share: typing.Optional[base.ArknightsTimestamp] = pydantic.Field(alias="infoShare")
-    """IDK."""
+    """Last time clue exchange was activated."""
     recent_visited: bool = pydantic.Field(alias="recentVisited")
-    """IDK."""
+    """IDK. Whether the player base has recently been visited."""
     info_share_visited: typing.Optional[int] = pydantic.Field(None, alias="infoShareVisited")
-    """IDK."""
+    """IDK. Whether the last player base visit yielded any credit shop credits."""
```

### Comparing `arkprts-0.2.4/arkprts.egg-info/PKG-INFO` & `arkprts-0.2.5/arkprts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.2.4
+Version: 0.2.5
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: rsa
@@ -13,15 +13,15 @@
 
 # ArkPRTS
 
 Arknights python wrapper.
 
 Interacts directly with the game servers, no delays.
 
-支持**中文和 B 站**账户!
+支持**中文和B站**账户!
 
 <!-- Supports Chinese and BiliBili accounts -->
 
 ---
 
 Source Code: <https://github.com/thesadru/arkprts>
```

### Comparing `arkprts-0.2.4/pyproject.toml` & `arkprts-0.2.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "arkprts"
 requires-python = ">=3.9"
-version = "0.2.4"
+version = "0.2.5"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
@@ -48,14 +48,15 @@
 # ANN401: Use of typing.Any (complicates)
 # B008: Do not perform function calls in argument defaults (pydantic)
 # B027: Empty method in ABC (optional rewrite)
 # B028: No stacklevel in warnings
 # B905: zip without strict= (ugly)
 # C408: Unnecessary dict call (ugly)
 # D105: Missing docstring in magic method (useless)
+# FA100: Missing future annotations.
 # E501: Line too long (black already manages this)
 # N805: First argument is not self (pydantic)
 # PGH003: Specific rules when ignoring type issues
 # PLR0913: Too many arguments
 # PLR2004: constant value in comparison (asserts)
 # PLW2901: Redefining for-loop variable
 # RET504: Unnecessary variable before return (ugly)
@@ -78,14 +79,15 @@
     "ANN401",
     "B008",
     "B027",
     "B028",
     "B905",
     "C408",
     "D105",
+    "FA100",
     "E501",
     "N805",
     "PGH003",
     "PLR0913",
     "PLR2004",
     "PLW2901",
     "RET504",
```

### Comparing `arkprts-0.2.4/setup.py` & `arkprts-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Run setuptools."""
 import pathlib
 
 from setuptools import find_packages, setup
 
 setup(
     name="arkprts",
-    version="0.2.4",
+    version="0.2.5",
     description="Arknights python wrapper.",
     url="https://github.com/thesadru/arkprts",
     packages=find_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     package_data={"arkprts": ["py.typed"]},
     install_requires=["aiohttp", "pydantic==2.*"],
     extras_require={"all": ["rsa", "pycryptodome"], "rsa": ["rsa"], "aes": ["pycryptodome"]},
```

### Comparing `arkprts-0.2.4/tests/test_auth.py` & `arkprts-0.2.5/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.2.4/tests/test_client.py` & `arkprts-0.2.5/tests/test_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Test arkprts client."""
+import typing
+
 import arkprts
 
 
-def _force_forbid(cls: type[arkprts.models.BaseModel]) -> None:
+def _force_forbid(cls: typing.Type[arkprts.models.BaseModel]) -> None:
     """Force forbid extra."""
     cls.model_config["extra"] = "forbid"
     for subclass in cls.__subclasses__():
         _force_forbid(subclass)
 
 
 _force_forbid(arkprts.models.BaseModel)
```

