# Comparing `tmp/highrise_bot_sdk-23.2.0.tar.gz` & `tmp/highrise_bot_sdk-23.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highrise_bot_sdk-23.2.0.tar", max compression
+gzip compressed data, was "highrise_bot_sdk-23.3.0.tar", max compression
```

## Comparing `highrise_bot_sdk-23.2.0.tar` & `highrise_bot_sdk-23.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     8050 2023-07-05 14:35:02.697133 highrise_bot_sdk-23.2.0/README.md
--rw-r--r--   0        0        0     1037 2023-07-05 13:51:49.568149 highrise_bot_sdk-23.2.0/pyproject.toml
--rw-r--r--   0        0        0    14031 2023-07-05 13:51:49.569748 highrise_bot_sdk-23.2.0/src/highrise/__init__.py
--rw-r--r--   0        0        0    15583 2023-06-30 08:26:21.404700 highrise_bot_sdk-23.2.0/src/highrise/__main__.py
--rw-r--r--   0        0        0     3064 2023-03-31 11:07:05.693250 highrise_bot_sdk-23.2.0/src/highrise/_unions.py
--rw-r--r--   0        0        0    16035 2023-07-05 13:51:49.569715 highrise_bot_sdk-23.2.0/src/highrise/models.py
--rw-r--r--   0        0        0      621 2023-06-30 16:42:03.849460 highrise_bot_sdk-23.2.0/src/highrise/models_control.py
--rw-r--r--   0        0        0     3171 2023-07-04 12:50:01.833389 highrise_bot_sdk-23.2.0/src/highrise/models_webapi.py
--rw-r--r--   0        0        0        0 2023-03-30 13:16:17.585454 highrise_bot_sdk-23.2.0/src/highrise/py.typed
--rw-r--r--   0        0        0     5431 2023-06-30 08:26:21.404899 highrise_bot_sdk-23.2.0/src/highrise/webapi.py
--rw-r--r--   0        0        0     9149 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.2.0/setup.py
--rw-r--r--   0        0        0     8755 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.2.0/PKG-INFO
+-rw-r--r--   0        0        0     9172 2023-07-17 10:55:12.430027 highrise_bot_sdk-23.3.0/README.md
+-rw-r--r--   0        0        0     1037 2023-07-06 12:07:34.332326 highrise_bot_sdk-23.3.0/pyproject.toml
+-rw-r--r--   0        0        0    15262 2023-07-17 10:54:35.897911 highrise_bot_sdk-23.3.0/src/highrise/__init__.py
+-rw-r--r--   0        0        0    15627 2023-07-17 10:54:35.897984 highrise_bot_sdk-23.3.0/src/highrise/__main__.py
+-rw-r--r--   0        0        0     3064 2023-03-31 11:07:05.693250 highrise_bot_sdk-23.3.0/src/highrise/_unions.py
+-rw-r--r--   0        0        0    16975 2023-07-17 10:54:35.897940 highrise_bot_sdk-23.3.0/src/highrise/models.py
+-rw-r--r--   0        0        0      621 2023-06-30 16:42:03.849460 highrise_bot_sdk-23.3.0/src/highrise/models_control.py
+-rw-r--r--   0        0        0     9557 2023-07-12 14:49:51.270902 highrise_bot_sdk-23.3.0/src/highrise/models_webapi.py
+-rw-r--r--   0        0        0        0 2023-03-30 13:16:17.585454 highrise_bot_sdk-23.3.0/src/highrise/py.typed
+-rw-r--r--   0        0        0     8842 2023-07-17 10:55:23.462681 highrise_bot_sdk-23.3.0/src/highrise/webapi.py
+-rw-r--r--   0        0        0    10282 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.3.0/setup.py
+-rw-r--r--   0        0        0     9877 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.3.0/PKG-INFO
```

### Comparing `highrise_bot_sdk-23.2.0/README.md` & `highrise_bot_sdk-23.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ---
 
 The Highrise Python Bot SDK is a python library for writing and running Highrise bots.
 
 First, install the library (preferably in a virtual environment):
 
 ```shell
-$ pip install highrise-bot-sdk==23.2.0
+$ pip install highrise-bot-sdk==23.3.0
 ```
 
 In the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.
 You will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.
 
 Open a new file, and paste the following to get started (into `mybot.py` for example):
 
@@ -28,14 +28,25 @@
 
 ```
 $ highrise mybot:Bot <room ID> <API token>
 ```
 
 ## Changelog
 
+### 23.3.0 (2023-07-17)
+- Add support for bot to get its inventory(`self.highrise.get_inventory()`). It returns list of items that bot has in its inventory.
+- Add support for bot to get its own outfit(`self.highrise.get_outfit()`). It returns list of items that bot has equipped.
+- Add support for bot to change his outfit(`self.highrise.set_outfit(outfit)`). It takes list of items that bot should equip. Bot can equip free items or items in his own inventory.
+- Add support for buying items as a bot(`self.highrise.buy_item(item_id)`). It takes item id and attempts to buy this item from highrise. Note bot can only use his own wallet to buy items. Some items are not available for purchase. Take note that bots can only equip those items and not trade them, there is no use in buying items more than one time.
+- Added items and grabs helper methods for Highrise Web API: 
+    - `self.webapi.get_item()`: Fetches a specific item by id.
+    - `self.webapi.get_items()`: Retrieves a list of items.
+    - `self.webapi.get_grab()`: Fetches a specific grab by id.
+    - `self.webapi.get_grabs()`: Retrieves a list of rooms.
+
 ### 23.2.0 (2023-07-5)
 - Add support to tip users in the room (`self.highrise.tip_user(user_id, amount)`). Amount needs to be expressed in gold bars. Possible values are:
   "gold_bar_1",
   "gold_bar_5",
   "gold_bar_10",
   "gold_bar_50",
   "gold_bar_100",
```

### Comparing `highrise_bot_sdk-23.2.0/pyproject.toml` & `highrise_bot_sdk-23.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highrise-bot-sdk"
-version = "23.2.0"
+version = "23.3.0"
 description = "The Highrise Bot SDK, for running Highrise bots written in Python."
 authors = ["Pocket Worlds Inc <server@high.rs>"]
 license = "proprietary"
 readme = "README.md"
 packages = [{include = "highrise", from = "src"}]
```

### Comparing `highrise_bot_sdk-23.2.0/src/highrise/__init__.py` & `highrise_bot_sdk-23.3.0/src/highrise/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from cattrs.preconf.json import make_converter
 from quattro import TaskGroup
 
 from ._unions import configure_tagged_union
 from .models import (
     AnchorHitRequest,
     AnchorPosition,
+    BuyItemRequest,
     BuyRoomBoostRequest,
     BuyVoiceTimeRequest,
     ChangeBackpackRequest,
     ChangeRoomPrivilegeRequest,
     ChannelEvent,
     ChannelRequest,
     ChatEvent,
@@ -26,14 +27,15 @@
     CurrencyItem,
     EmoteEvent,
     EmoteRequest,
     Error,
     FloorHitRequest,
     GetBackpackRequest,
     GetConversationsRequest,
+    GetInventoryRequest,
     GetMessagesRequest,
     GetRoomPrivilegeRequest,
     GetRoomUsersRequest,
     GetUserOutfitRequest,
     GetWalletRequest,
     IndicatorRequest,
     InviteSpeakerRequest,
@@ -47,14 +49,15 @@
     Reaction,
     ReactionEvent,
     ReactionRequest,
     RemoveSpeakerRequest,
     RoomPermissions,
     SendMessageRequest,
     SessionMetadata,
+    SetOutfitRequest,
     TeleportRequest,
     TipReactionEvent,
     TipUserRequest,
     User,
     UserJoinedEvent,
     UserLeftEvent,
     UserMovedEvent,
@@ -157,14 +160,15 @@
         self, user_id: str, conversation_id: str, is_new_conversation: bool
     ) -> None:
         """On a inbox message received from a user."""
         pass
 
 
 class Highrise:
+    my_id: str
     ws: ClientWebSocketResponse
     tg: TaskGroup
     _req_id = count()
     _req_id_registry: dict[str, Queue[Any]] = {}
 
     async def chat(self, message: str) -> None:
         """Broadcast a room-wide chat message."""
@@ -357,14 +361,44 @@
     ) -> Literal["success", "insufficient_funds"] | Error:
         """Tip a user."""
         res = await do_req_resp(self, TipUserRequest(user_id, tip))
         if isinstance(res, Error):
             return res
         return res.result
 
+    async def get_my_outfit(self) -> GetUserOutfitRequest.GetUserOutfitResponse | Error:
+        """Get the bot's outfit."""
+        res = await do_req_resp(self, GetUserOutfitRequest(self.my_id))
+        if isinstance(res, Error):
+            return res
+        return res
+
+    async def get_inventory(self) -> GetInventoryRequest.GetInventoryResponse | Error:
+        """Get the bot's inventory."""
+        res = await do_req_resp(self, GetInventoryRequest())
+        if isinstance(res, Error):
+            return res
+        return res
+
+    async def set_outfit(self, outfit: list[Item]) -> None | Error:
+        """Set the bot's outfit."""
+        resp = await do_req_resp(self, SetOutfitRequest(outfit))
+        if isinstance(resp, Error):
+            return resp
+        return None
+
+    async def buy_item(
+        self, item_id: str
+    ) -> Literal["success", "insufficient_funds"] | Error:
+        """Buy an item."""
+        resp = await do_req_resp(self, BuyItemRequest(item_id))
+        if isinstance(resp, Error):
+            return resp
+        return resp.result
+
     def call_in(self, callback: Callable, delay: float) -> None:
         self.tg.create_task(_delayed_callback(callback, delay))
 
 
 class ResponseError(Exception):
     """An API response error."""
 
@@ -434,14 +468,17 @@
     | GetConversationsRequest
     | SendMessageRequest
     | GetMessagesRequest
     | LeaveConversationRequest
     | BuyVoiceTimeRequest
     | BuyRoomBoostRequest
     | TipUserRequest
+    | SetOutfitRequest
+    | GetInventoryRequest
+    | BuyItemRequest
 )
 IncomingEvents = (
     Error
     | ChatEvent
     | EmoteEvent
     | ReactionEvent
     | UserJoinedEvent
```

### Comparing `highrise_bot_sdk-23.2.0/src/highrise/__main__.py` & `highrise_bot_sdk-23.3.0/src/highrise/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,15 @@
                         if isinstance(session_metadata, Error):
                             print(f"ERROR: {session_metadata}")
                             ka_task.cancel()
                             return
                         bot_id = str(session_metadata.user_id)
                         webapi = WebAPI()
                         chat = Highrise()
+                        chat.my_id = bot_id
                         chat.ws = ws
                         chat.tg = tg
 
                         if (
                             session_metadata.sdk_version is not None
                             and session_metadata.sdk_version != VERSION
                         ):
```

### Comparing `highrise_bot_sdk-23.2.0/src/highrise/_unions.py` & `highrise_bot_sdk-23.3.0/src/highrise/_unions.py`

 * *Files identical despite different names*

### Comparing `highrise_bot_sdk-23.2.0/src/highrise/models.py` & `highrise_bot_sdk-23.3.0/src/highrise/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 @define
 class Item:
     """A Highrise item."""
 
     type: Literal["clothing"]
     amount: int
     id: str
+    account_bound: bool = False
+    active_palette: int | None = None
 
 
 @define
 class Message:
     """
     A Highrise conversation message.
     """
@@ -811,7 +813,56 @@
     class TipUserResponse:
         """Tip a user."""
 
         result: Literal["success", "insufficient_funds"]
         rid: str | None = None
 
     Response: ClassVar = TipUserResponse
+
+
+@define
+class GetInventoryRequest:
+    """Get the inventory of a bot."""
+
+    rid: str | None = None
+
+    @define
+    class GetInventoryResponse:
+        """Get the inventory of a bot."""
+
+        items: list[Item]
+        rid: str | None = None
+
+    Response: ClassVar = GetInventoryResponse
+
+
+@define
+class SetOutfitRequest:
+    """Set the outfit of a bot."""
+
+    outfit: list[Item]
+    rid: str | None = None
+
+    @define
+    class SetOutfitResponse:
+        """Set the outfit of a bot."""
+
+        rid: str | None = None
+
+    Response: ClassVar = SetOutfitResponse
+
+
+@define
+class BuyItemRequest:
+    """Buy an item."""
+
+    item_id: str
+    rid: str | None = None
+
+    @define
+    class BuyItemResponse:
+        """Buy an item."""
+
+        result: Literal["success", "insufficient_funds"]
+        rid: str | None = None
+
+    Response: ClassVar = BuyItemResponse
```

### Comparing `highrise_bot_sdk-23.2.0/src/highrise/models_control.py` & `highrise_bot_sdk-23.3.0/src/highrise/models_control.py`

 * *Files identical despite different names*

### Comparing `highrise_bot_sdk-23.2.0/setup.py` & `highrise_bot_sdk-23.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,17 +19,17 @@
  'typing_extensions<4.0.0']
 
 entry_points = \
 {'console_scripts': ['highrise = highrise.__main__:run']}
 
 setup_kwargs = {
     'name': 'highrise-bot-sdk',
-    'version': '23.2.0',
+    'version': '23.3.0',
     'description': 'The Highrise Bot SDK, for running Highrise bots written in Python.',
-    'long_description': '# The Highrise Python Bot SDK\n\n---\n\nThe Highrise Python Bot SDK is a python library for writing and running Highrise bots.\n\nFirst, install the library (preferably in a virtual environment):\n\n```shell\n$ pip install highrise-bot-sdk==23.2.0\n```\n\nIn the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You\'ll need the token to start your bot later.\nYou will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.\n\nOpen a new file, and paste the following to get started (into `mybot.py` for example):\n\n```python\nfrom highrise import BaseBot\n\nclass Bot(BaseBot):\n    pass\n```\n\nOverride methods from `BaseBot` as needed.\n\nWhen you\'re ready, run the bot from the terminal using the SDK, giving it the Python path to the Bot class:\n\n```\n$ highrise mybot:Bot <room ID> <API token>\n```\n\n## Changelog\n\n### 23.2.0 (2023-07-5)\n- Add support to tip users in the room (`self.highrise.tip_user(user_id, amount)`). Amount needs to be expressed in gold bars. Possible values are:\n  "gold_bar_1",\n  "gold_bar_5",\n  "gold_bar_10",\n  "gold_bar_50",\n  "gold_bar_100",\n  "gold_bar_500",\n  "gold_bar_1k",\n  "gold_bar_5000",\n  "gold_bar_10k",\n\n### 23.1.0b16 (2023-07-03)\n- Hotfix web-api models issue.\n\n### 23.1.0b15 (2023-06-30)\n- Hotfix dependency issue with cattrs.\n\n### 23.1.0b14 (2023-06-30)\n- Added Highrise Web API Support: Introduced helper methods within the BaseBot class accessible through `self.webapi`. This enables easy communication with the Highrise Web API to gain access to public information about the game. Included are the following methods:\n    - `self.webapi.get_user()`: Fetches a specific user by id.\n    - `self.webapi.get_users()`: Retrieves a list of users.\n    - `self.webapi.get_room()`: Fetches a specific room by id.\n    - `self.webapi.get_rooms()`: Retrieves a list of rooms.\n    - `self.webapi.get_post()`: Fetches a specific post by id.\n    - `self.webapi.get_posts()`: Retrieves a list of posts.\n- Add a method to buy room boost for a room (`self.highrise.buy_room_boost(payment_type, amount)`).\n- Add a method to buy voice time for a room (`self.highrise.buy_voice_time(payment_type)`).\n- Both methods support several payment options `bot_wallet_only`, `bot_wallet_priority`, `user_wallet_only` allowing bot to use its own wallet or user\'s wallet to pay for the purchase. Or to try to prioritize bot\'s wallet over user\'s wallet.\n- Get wallet method will now return room_boost_tokens and voice_tokens if bot has any.\n\n### 23.1.0b13 (2023-06-19)\n\n- Add optional hook that is triggered on bot startup (`async def before_start(self) -> None:`). All bot initialization should be done here, and most things like reading from files, setting up database connections can be done here instead of on_connect.\n- Enable support for bot to get access to inbox features, direct conversation and ability to respond to messages if messaged by user.\n- Add handler that is triggered when bot received message from user (`async def on_message(user_id, conversation_id, is_new_conversation)`). It is triggered when user sends in game message to bot, using either new conversation or existing conversation. If this is new conversation `is_new_conversation` will be set to True, otherwise it will be set to False.\n- Add support for bot to send message to user (`self.highrise.send_message(conversation_id, message, type, room_id)`). This can be only used on existing conversation, and will fail if conversation is not found. Bot can only send two types of messages, `text` and `invite`. Text is the normal message in which bot can send text to user, and invite is used to invite user to room. If type is invite then room_id must be provided in order to generate room invite for users.\n- Add support for bot to list conversations (`self.highrise.get_conversations(not_joined, last_id)`). This will return list of conversations opened with bot, there are two types of conversations, the ones bot has joined and unjoined. If `not_joined` is set to True then only unjoined conversations will be returned, otherwise only joined conversations will be returned. Response will also return number of unjoined conversations that bot has. This method will return at most 20 conversations ordered from newest to the oldest,  If `last_id` is provided then only conversations that are older than specified id will be returned.\n- Add support for bot to list messages in conversation (`self.highrise.get_messages(conversation_id, last_id)`). This will return list of messages in conversation, at most 20 messages will be returned ordered from newest to the oldest. If `last_id` is provided then only messages that are older than specified id will be returned. conversation_id must be from conversation that is available to bot.\n- Add support for bot to leave conversation (`self.highrise.leave_conversation(conversation_id)`). This will leave conversation, and bot will no longer receive messages from user in that conversation or have that conversation in his list. \n\n### 23.1.0b12 (2023-06-06)\n\n- Add support for getting information about user outfit if user is in the room (`self.highrise.get_user_outfit(user_id)`).\n- Enable automatic filtering of events based on bot usage.\n\n### 23.1.0b11 (2023-05-29)\n\n- Add support for running multiple bots in the same process.\n- Add additional room information such as owner\'s id and room name to session metadata on connection\n- Add support for voice chat management and info, bots can now get information about voice chat in the room if bot owner has privileges to get info or manage bots in the room (`self.highrise.get_voice_status()`)\n- Add support for bots to invite users to voice chat (`self.highrise.add_user_to_voice(user_id)`\n- Add support for bots to remove users from voice chat (`self.highrise.remove_user_from_voice(user_id)`\n- Add handler that is triggered when state of voice in the room changed(`self.on_voice_change(users, seconds_left)`\n\n\n### 23.1.0b10 (2023-05-12)\n\n- Fix bug with handling of error responses.\n\n### 23.1.0b9 (2023-05-11)\n\n- Add support for moving bot to an anchor in walk_to command (`self.highrise.walk_to(AnchorPosition)`).\n- Change the way client ws messages are parsed, return error if message is not valid json.\n\n### 23.1.0b8 (2023-04-25)\n\n- Add support for moving users to another room (`self.highrise.move_user_to_room(user_id, room_id)`).\n- Add handler that is triggered when user moves inside a room  (`self.on_user_move(user_id, position)`).) \n- Expand session_metadata information with information about client rates\n- Expand session_metadata with information about sdk versions if client uses skd\n\n### 23.1.0b6 (2023-04-17)\n\n- Add Python 3.10 support\n\n### 23.1.0b5 (2023-04-11)\n\n- Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).\n- Add support changing room permissions for users (`self.highrise.set_room_privilege(user_id, privilege)`).\n- Add support for moderating rooms (`self.highrise.moderate_room(user_id, moderate_action, action_length)`). \n- Rework how keepalive is handled\n\n### 23.1.0b4 (2023-04-05)\n\n- Methods mapping to requests with empty responses (`chat`, `send_whisper`, `send_emote`, `react`, `set_indicator`, `send_channel`, `walk_to`, `teleport`) now return `None`, and raise a `highrise.ResponseError` on an error response.\n- Fix the emote API.\n- Internally rework request handling to improve robustness.\n\n### 23.1.0b3 (2023-04-03)\n\n- Fix the chatting API.\n\n### 23.1.0b2 (2023-04-03)\n\n- Add support for receiving and sending reactions.\n- Fix support for hidden channels.\n- Migrate to the new message for avatars leaving.\n- Improve concurrency when awaiting bot methods.\n- Fix issues with teleporting users.\n- Fix issues with user coordinates.\n- Add support for fetching the bot wallet (`self.highrise.get_wallet()`).\n\n### 23.1.0b1 (2023-03-28)\n\n- Add support for emotes and hidden channel messages.\n\n### 23.1.0b0 (2023-03-10)\n\n- Initial beta release.\n',
+    'long_description': '# The Highrise Python Bot SDK\n\n---\n\nThe Highrise Python Bot SDK is a python library for writing and running Highrise bots.\n\nFirst, install the library (preferably in a virtual environment):\n\n```shell\n$ pip install highrise-bot-sdk==23.3.0\n```\n\nIn the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You\'ll need the token to start your bot later.\nYou will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.\n\nOpen a new file, and paste the following to get started (into `mybot.py` for example):\n\n```python\nfrom highrise import BaseBot\n\nclass Bot(BaseBot):\n    pass\n```\n\nOverride methods from `BaseBot` as needed.\n\nWhen you\'re ready, run the bot from the terminal using the SDK, giving it the Python path to the Bot class:\n\n```\n$ highrise mybot:Bot <room ID> <API token>\n```\n\n## Changelog\n\n### 23.3.0 (2023-07-17)\n- Add support for bot to get its inventory(`self.highrise.get_inventory()`). It returns list of items that bot has in its inventory.\n- Add support for bot to get its own outfit(`self.highrise.get_outfit()`). It returns list of items that bot has equipped.\n- Add support for bot to change his outfit(`self.highrise.set_outfit(outfit)`). It takes list of items that bot should equip. Bot can equip free items or items in his own inventory.\n- Add support for buying items as a bot(`self.highrise.buy_item(item_id)`). It takes item id and attempts to buy this item from highrise. Note bot can only use his own wallet to buy items. Some items are not available for purchase. Take note that bots can only equip those items and not trade them, there is no use in buying items more than one time.\n- Added items and grabs helper methods for Highrise Web API: \n    - `self.webapi.get_item()`: Fetches a specific item by id.\n    - `self.webapi.get_items()`: Retrieves a list of items.\n    - `self.webapi.get_grab()`: Fetches a specific grab by id.\n    - `self.webapi.get_grabs()`: Retrieves a list of rooms.\n\n### 23.2.0 (2023-07-5)\n- Add support to tip users in the room (`self.highrise.tip_user(user_id, amount)`). Amount needs to be expressed in gold bars. Possible values are:\n  "gold_bar_1",\n  "gold_bar_5",\n  "gold_bar_10",\n  "gold_bar_50",\n  "gold_bar_100",\n  "gold_bar_500",\n  "gold_bar_1k",\n  "gold_bar_5000",\n  "gold_bar_10k",\n\n### 23.1.0b16 (2023-07-03)\n- Hotfix web-api models issue.\n\n### 23.1.0b15 (2023-06-30)\n- Hotfix dependency issue with cattrs.\n\n### 23.1.0b14 (2023-06-30)\n- Added Highrise Web API Support: Introduced helper methods within the BaseBot class accessible through `self.webapi`. This enables easy communication with the Highrise Web API to gain access to public information about the game. Included are the following methods:\n    - `self.webapi.get_user()`: Fetches a specific user by id.\n    - `self.webapi.get_users()`: Retrieves a list of users.\n    - `self.webapi.get_room()`: Fetches a specific room by id.\n    - `self.webapi.get_rooms()`: Retrieves a list of rooms.\n    - `self.webapi.get_post()`: Fetches a specific post by id.\n    - `self.webapi.get_posts()`: Retrieves a list of posts.\n- Add a method to buy room boost for a room (`self.highrise.buy_room_boost(payment_type, amount)`).\n- Add a method to buy voice time for a room (`self.highrise.buy_voice_time(payment_type)`).\n- Both methods support several payment options `bot_wallet_only`, `bot_wallet_priority`, `user_wallet_only` allowing bot to use its own wallet or user\'s wallet to pay for the purchase. Or to try to prioritize bot\'s wallet over user\'s wallet.\n- Get wallet method will now return room_boost_tokens and voice_tokens if bot has any.\n\n### 23.1.0b13 (2023-06-19)\n\n- Add optional hook that is triggered on bot startup (`async def before_start(self) -> None:`). All bot initialization should be done here, and most things like reading from files, setting up database connections can be done here instead of on_connect.\n- Enable support for bot to get access to inbox features, direct conversation and ability to respond to messages if messaged by user.\n- Add handler that is triggered when bot received message from user (`async def on_message(user_id, conversation_id, is_new_conversation)`). It is triggered when user sends in game message to bot, using either new conversation or existing conversation. If this is new conversation `is_new_conversation` will be set to True, otherwise it will be set to False.\n- Add support for bot to send message to user (`self.highrise.send_message(conversation_id, message, type, room_id)`). This can be only used on existing conversation, and will fail if conversation is not found. Bot can only send two types of messages, `text` and `invite`. Text is the normal message in which bot can send text to user, and invite is used to invite user to room. If type is invite then room_id must be provided in order to generate room invite for users.\n- Add support for bot to list conversations (`self.highrise.get_conversations(not_joined, last_id)`). This will return list of conversations opened with bot, there are two types of conversations, the ones bot has joined and unjoined. If `not_joined` is set to True then only unjoined conversations will be returned, otherwise only joined conversations will be returned. Response will also return number of unjoined conversations that bot has. This method will return at most 20 conversations ordered from newest to the oldest,  If `last_id` is provided then only conversations that are older than specified id will be returned.\n- Add support for bot to list messages in conversation (`self.highrise.get_messages(conversation_id, last_id)`). This will return list of messages in conversation, at most 20 messages will be returned ordered from newest to the oldest. If `last_id` is provided then only messages that are older than specified id will be returned. conversation_id must be from conversation that is available to bot.\n- Add support for bot to leave conversation (`self.highrise.leave_conversation(conversation_id)`). This will leave conversation, and bot will no longer receive messages from user in that conversation or have that conversation in his list. \n\n### 23.1.0b12 (2023-06-06)\n\n- Add support for getting information about user outfit if user is in the room (`self.highrise.get_user_outfit(user_id)`).\n- Enable automatic filtering of events based on bot usage.\n\n### 23.1.0b11 (2023-05-29)\n\n- Add support for running multiple bots in the same process.\n- Add additional room information such as owner\'s id and room name to session metadata on connection\n- Add support for voice chat management and info, bots can now get information about voice chat in the room if bot owner has privileges to get info or manage bots in the room (`self.highrise.get_voice_status()`)\n- Add support for bots to invite users to voice chat (`self.highrise.add_user_to_voice(user_id)`\n- Add support for bots to remove users from voice chat (`self.highrise.remove_user_from_voice(user_id)`\n- Add handler that is triggered when state of voice in the room changed(`self.on_voice_change(users, seconds_left)`\n\n\n### 23.1.0b10 (2023-05-12)\n\n- Fix bug with handling of error responses.\n\n### 23.1.0b9 (2023-05-11)\n\n- Add support for moving bot to an anchor in walk_to command (`self.highrise.walk_to(AnchorPosition)`).\n- Change the way client ws messages are parsed, return error if message is not valid json.\n\n### 23.1.0b8 (2023-04-25)\n\n- Add support for moving users to another room (`self.highrise.move_user_to_room(user_id, room_id)`).\n- Add handler that is triggered when user moves inside a room  (`self.on_user_move(user_id, position)`).) \n- Expand session_metadata information with information about client rates\n- Expand session_metadata with information about sdk versions if client uses skd\n\n### 23.1.0b6 (2023-04-17)\n\n- Add Python 3.10 support\n\n### 23.1.0b5 (2023-04-11)\n\n- Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).\n- Add support changing room permissions for users (`self.highrise.set_room_privilege(user_id, privilege)`).\n- Add support for moderating rooms (`self.highrise.moderate_room(user_id, moderate_action, action_length)`). \n- Rework how keepalive is handled\n\n### 23.1.0b4 (2023-04-05)\n\n- Methods mapping to requests with empty responses (`chat`, `send_whisper`, `send_emote`, `react`, `set_indicator`, `send_channel`, `walk_to`, `teleport`) now return `None`, and raise a `highrise.ResponseError` on an error response.\n- Fix the emote API.\n- Internally rework request handling to improve robustness.\n\n### 23.1.0b3 (2023-04-03)\n\n- Fix the chatting API.\n\n### 23.1.0b2 (2023-04-03)\n\n- Add support for receiving and sending reactions.\n- Fix support for hidden channels.\n- Migrate to the new message for avatars leaving.\n- Improve concurrency when awaiting bot methods.\n- Fix issues with teleporting users.\n- Fix issues with user coordinates.\n- Add support for fetching the bot wallet (`self.highrise.get_wallet()`).\n\n### 23.1.0b1 (2023-03-28)\n\n- Add support for emotes and hidden channel messages.\n\n### 23.1.0b0 (2023-03-10)\n\n- Initial beta release.\n',
     'author': 'Pocket Worlds Inc',
     'author_email': 'server@high.rs',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `highrise_bot_sdk-23.2.0/PKG-INFO` & `highrise_bot_sdk-23.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highrise-bot-sdk
-Version: 23.2.0
+Version: 23.3.0
 Summary: The Highrise Bot SDK, for running Highrise bots written in Python.
 License: Proprietary
 Author: Pocket Worlds Inc
 Author-email: server@high.rs
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
 ---
 
 The Highrise Python Bot SDK is a python library for writing and running Highrise bots.
 
 First, install the library (preferably in a virtual environment):
 
 ```shell
-$ pip install highrise-bot-sdk==23.2.0
+$ pip install highrise-bot-sdk==23.3.0
 ```
 
 In the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.
 You will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.
 
 Open a new file, and paste the following to get started (into `mybot.py` for example):
 
@@ -48,14 +48,25 @@
 
 ```
 $ highrise mybot:Bot <room ID> <API token>
 ```
 
 ## Changelog
 
+### 23.3.0 (2023-07-17)
+- Add support for bot to get its inventory(`self.highrise.get_inventory()`). It returns list of items that bot has in its inventory.
+- Add support for bot to get its own outfit(`self.highrise.get_outfit()`). It returns list of items that bot has equipped.
+- Add support for bot to change his outfit(`self.highrise.set_outfit(outfit)`). It takes list of items that bot should equip. Bot can equip free items or items in his own inventory.
+- Add support for buying items as a bot(`self.highrise.buy_item(item_id)`). It takes item id and attempts to buy this item from highrise. Note bot can only use his own wallet to buy items. Some items are not available for purchase. Take note that bots can only equip those items and not trade them, there is no use in buying items more than one time.
+- Added items and grabs helper methods for Highrise Web API: 
+    - `self.webapi.get_item()`: Fetches a specific item by id.
+    - `self.webapi.get_items()`: Retrieves a list of items.
+    - `self.webapi.get_grab()`: Fetches a specific grab by id.
+    - `self.webapi.get_grabs()`: Retrieves a list of rooms.
+
 ### 23.2.0 (2023-07-5)
 - Add support to tip users in the room (`self.highrise.tip_user(user_id, amount)`). Amount needs to be expressed in gold bars. Possible values are:
   "gold_bar_1",
   "gold_bar_5",
   "gold_bar_10",
   "gold_bar_50",
   "gold_bar_100",
```

