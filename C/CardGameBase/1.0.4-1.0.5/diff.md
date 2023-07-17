# Comparing `tmp/CardGameBase-1.0.4.tar.gz` & `tmp/CardGameBase-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CardGameBase-1.0.4.tar", last modified: Tue May 23 13:11:41 2023, max compression
+gzip compressed data, was "CardGameBase-1.0.5.tar", last modified: Mon Jul 17 11:33:06 2023, max compression
```

## Comparing `CardGameBase-1.0.4.tar` & `CardGameBase-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 13:11:41.434572 CardGameBase-1.0.4/
-drwxrwxrwx   0        0        0        0 2023-05-23 13:11:41.418939 CardGameBase-1.0.4/CardGameBase/
--rw-rw-rw-   0        0        0     3156 2023-05-23 12:58:36.000000 CardGameBase-1.0.4/CardGameBase/Card.py
--rw-rw-rw-   0        0        0     6293 2023-05-23 13:02:38.000000 CardGameBase-1.0.4/CardGameBase/Deck.py
--rw-rw-rw-   0        0        0       39 2023-04-13 10:08:54.000000 CardGameBase-1.0.4/CardGameBase/Exceptions.py
--rw-rw-rw-   0        0        0     7899 2023-05-23 12:57:36.000000 CardGameBase-1.0.4/CardGameBase/Hand.py
--rw-rw-rw-   0        0        0      972 2023-05-23 12:54:04.000000 CardGameBase-1.0.4/CardGameBase/Utility.py
--rw-rw-rw-   0        0        0      119 2023-04-13 10:09:58.000000 CardGameBase-1.0.4/CardGameBase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:11:41.418939 CardGameBase-1.0.4/CardGameBase.egg-info/
--rw-rw-rw-   0        0        0     1500 2023-05-23 13:11:41.000000 CardGameBase-1.0.4/CardGameBase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-05-23 13:11:41.000000 CardGameBase-1.0.4/CardGameBase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 13:11:41.000000 CardGameBase-1.0.4/CardGameBase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-23 13:11:41.000000 CardGameBase-1.0.4/CardGameBase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1235 2023-05-16 07:57:54.000000 CardGameBase-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1500 2023-05-23 13:11:41.434572 CardGameBase-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      889 2023-05-16 11:03:15.000000 CardGameBase-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 13:11:41.434572 CardGameBase-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1172 2023-05-23 13:11:23.000000 CardGameBase-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:33:06.446100 CardGameBase-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-17 11:33:06.446100 CardGameBase-1.0.5/CardGameBase/
+-rw-rw-rw-   0        0        0     3422 2023-07-17 11:19:04.000000 CardGameBase-1.0.5/CardGameBase/Card.py
+-rw-rw-rw-   0        0        0     6160 2023-07-17 11:19:04.000000 CardGameBase-1.0.5/CardGameBase/Deck.py
+-rw-rw-rw-   0        0        0      317 2023-07-17 09:40:35.000000 CardGameBase-1.0.5/CardGameBase/Exceptions.py
+-rw-rw-rw-   0        0        0     8472 2023-07-17 11:19:04.000000 CardGameBase-1.0.5/CardGameBase/Hand.py
+-rw-rw-rw-   0        0        0      972 2023-07-17 09:40:35.000000 CardGameBase-1.0.5/CardGameBase/Utility.py
+-rw-rw-rw-   0        0        0      119 2023-07-17 09:40:35.000000 CardGameBase-1.0.5/CardGameBase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 11:33:06.446100 CardGameBase-1.0.5/CardGameBase.egg-info/
+-rw-rw-rw-   0        0        0     1500 2023-07-17 11:33:06.000000 CardGameBase-1.0.5/CardGameBase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-07-17 11:33:06.000000 CardGameBase-1.0.5/CardGameBase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 11:33:06.000000 CardGameBase-1.0.5/CardGameBase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-17 11:33:06.000000 CardGameBase-1.0.5/CardGameBase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1235 2023-07-17 09:40:35.000000 CardGameBase-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1500 2023-07-17 11:33:06.446100 CardGameBase-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-07-17 09:40:35.000000 CardGameBase-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 11:33:06.446100 CardGameBase-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1172 2023-07-17 11:32:52.000000 CardGameBase-1.0.5/setup.py
```

### Comparing `CardGameBase-1.0.4/CardGameBase/Card.py` & `CardGameBase-1.0.5/CardGameBase/Card.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,86 +3,97 @@
     Card Base Type with comparison features
     """
 
     def __init__(self,
                  symbol: str,
                  symbol_rank: int,
                  value: int,
-                 _format: str = "{v}{s}",
-                 special_value_format: str = None
+                 card_format: str = "{v}{s}",
+                 special_value_format: str = None,
+                 calculate_with_rank: bool = False,
                  ):
         """
         Card Base Type with comparison features
 
         :param symbol: card symbol (like: spades, diamond, etc.)
         :param symbol_rank: symbol rank is required for comparing 2 cards
         :param value: card value
-        :param _format: print format; {v} = value, {s} = symbol
+        :param card_format: print format; {v} = value, {s} = symbol
         :param special_value_format: if set will be printed instead of value
         """
 
         self.symbol = symbol
         self.symbol_rank = symbol_rank
         self.value = value
-        self._format = _format
+        self.card_format = card_format
         self.special_value_format = special_value_format
+        self.calculate_with_rank = calculate_with_rank
+
+    def _check_type(self, other):
+        exceptions = ["int"]
+        if not isinstance(other, self.__class__) and not type(other).__name__ in exceptions:
+            raise NotImplementedError(f"Cannot perform operation between '{type(self).__name__}' and '{type(other).__name__}'")
 
     def __add__(self, other) -> int:
+        self._check_type(other)
+
         if isinstance(other, int):
+            return self.value + other
+        if self.calculate_with_rank:
             return self.value * self.symbol_rank + other
 
-        if not type(self) == type(other):
-            raise TypeError(f"Cannot add type '{type(self)}' and '{type(other)}'")
-
         return self.value + other.value
 
     def __radd__(self, other):
+        self._check_type(other)
+
         if isinstance(other, int):
             return self.value + other
-
-        if not type(self) == type(other):
-            raise TypeError(f"Cannot add type '{type(self)}' and '{type(other)}'")
-
+        if self.calculate_with_rank:
+            return self.value * self.symbol_rank + other
         return self.value + other.value
 
     def __eq__(self, other) -> bool:
-        if not type(self) == type(other):
-            raise TypeError(f"Cannot compare type '{type(self)}' against '{type(other)}'")
+        self._check_type(other)
 
-        return self.value == self.value and self.symbol_rank == other.symbol_rank
+        if isinstance(other, int):
+            return self.value == other
+        if self.calculate_with_rank:
+            return self.value == other.value and self.symbol_rank == other.symbol_rank
+        return self.value == other.value
 
     def __gt__(self, other) -> bool:
-        if not type(self) == type(other):
-            raise TypeError(f"Cannot compare type '{type(self)}' against '{type(other)}'")
+        self._check_type(other)
 
-        if self.value == other.value:
+        if isinstance(other, int):
+            return self.value > other
+        if self.value == other.value and self.calculate_with_rank:
             return self.symbol_rank > other.symbol_rank
         return self.value > other.value
 
     def __lt__(self, other) -> bool:
-        if not type(self) == type(other):
-            raise TypeError(f"Cannot compare type '{type(self)}' against '{type(other)}'")
+        self._check_type(other)
 
-        if self.value == other.value:
+        if isinstance(other, int):
+            return self.value < other
+        if self.value == other.value and self.calculate_with_rank:
             return self.symbol_rank < other.symbol_rank
         return self.value < other.value
 
     def __ge__(self, other) -> bool:
-        if not type(self) == type(other):
-            raise TypeError(f"Cannot compare type '{type(self)}' against '{type(other)}'")
+        self._check_type(other)
 
         return self.__gt__(other) or self.__eq__(other)
 
     def __le__(self, other) -> bool:
-        if not type(self) == type(other):
-            raise TypeError(f"Cannot compare type '{type(self)}' against '{type(other)}'")
+        self._check_type(other)
 
         return self.__lt__(other) or self.__eq__(other)
 
     def __str__(self) -> str:
-        return self._format.format(
+        return self.card_format.format(
             v=self.value if not self.special_value_format else self.special_value_format,
             s=self.symbol
         )
 
     def __repr__(self) -> str:
-        return f"Card('{self.symbol}', '{self.symbol_rank}', '{self._format}')"
+        return f"Card('{self.symbol}', '{self.symbol_rank}', '{self.card_format}')"
```

### Comparing `CardGameBase-1.0.4/CardGameBase/Deck.py` & `CardGameBase-1.0.5/CardGameBase/Deck.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Iterable, List, Set
+from typing import Iterable, List, Set, Union
 from . import Card, EmptyDeck
 from random import shuffle
 import pickle
 
 
 class DeckConfig:
     """
@@ -34,16 +34,14 @@
         :param special_value_format: is displayed instead of the card value when set
         :return:
         """
         key = (symbol, symbol_rank)
         if not self.__deck_config.get(key):
             self.__deck_config[key] = [[value, special_value_format]]
         else:
-            # if [value, special_value_format] in self.__deck[key]:
-            #    raise KeyError(f"a card with '{symbol=}', '{symbol_rank=}', '{value=}'; already exists!")
             self.__deck_config[key].append([value, special_value_format])
 
     def get(self) -> dict[tuple: List[List[int, str]]]:
         """
         :return: gives back a deck config copy
         """
         return self.__deck_config.copy()
@@ -59,15 +57,15 @@
         """
         save deck config to file
         """
         with open(file, "wb") as f:
             pickle.dump(self.__deck_config, f)
 
     def __add__(self, other):
-        if not type(self) == type(other):  # hasattr(other, "_DeckConfig__deck_config"):
+        if not type(self) == type(other):
             raise TypeError(f"Cannot add type '{type(self)}' and '{type(other)}'")
 
         new_deck = self.__deck_config.copy()
         for symbol, symbol_rank in other.get().keys():
             if new_deck.get((symbol, symbol_rank)):
                 new_deck[(symbol, symbol_rank)].append(other.get()[(symbol, symbol_rank)])
             else:
@@ -90,15 +88,14 @@
 
     def __create(self, deck_config: DeckConfig) -> None:
         """
         Creates cards with the deck configuration
         """
         deck = deck_config.get()
         for card_symbol, card_symbol_rank in deck:
-            # print(deck[(card_symbol, card_symbol_rank)])
             for card_value, special_value_format in deck[(card_symbol, card_symbol_rank)]:
                 self.cards.append(Card(
                     card_symbol,
                     card_symbol_rank,
                     card_value,
                     special_value_format=special_value_format
                 ))
@@ -111,15 +108,15 @@
         # Since random can also create the same deck as before
         # would be extremely rare, but it could happen.
         # And if the deck is smaller than or equal to 1 this would
         # create a infinite loop
         while self.cards == cards_before and len(self.cards) > 1:
             shuffle(self.cards)
 
-    def get_card(self, amount: int = 1, put_to_bottom: bool = False) -> Card | List[Card]:
+    def get_card(self, amount: int = 1, put_to_bottom: bool = False) -> Union[Card, List[Card]]:
         """
         Returns the top card of the deck and removes the card from the deck
 
         :param amount: Amount of cards to draw
         :param put_to_bottom: Don't remove card when taking one from top and put it at the bottom
         :return: {amount} amount of cards
         """
@@ -130,15 +127,15 @@
         for i in range(amount):
             cards.append(self.cards.pop(0))
             if put_to_bottom:
                 self.cards.append(cards[-1])
 
         return cards[0] if len(cards) == 1 else cards
 
-    def add_card(self, cards: Card | List[Card] | DeckConfig) -> None:
+    def add_card(self, cards: Union[Card, List[Card], DeckConfig]) -> None:
         """
         Adds card(s) to bottom of the deck
 
         :param cards: The card(s) to add
         """
         if isinstance(cards, list):
             self.cards.extend(cards)
@@ -159,24 +156,29 @@
         """
         Returns a set of card symbols
         :return: a set of all card symbols
         """
         symbols = set()
         for card in self.cards:
             symbols.add(card.symbol)
-        # return {card.symbol for card in self.cards}
         return symbols
 
     def __contains__(self, card: Card) -> bool:
         return card in self.cards
 
     def __iter__(self) -> Iterable[Card]:
         return self.cards.__iter__()
 
     def __next__(self) -> Card:
+        if self.__iterator >= len(self.cards):
+            raise StopIteration
         self.__iterator += 1
-        if self.__iterator > len(self.cards):
-            return self.cards[self.__iterator]
-        raise StopIteration
+        return self.cards[self.__iterator - 1]
 
     def __str__(self) -> str:
-        return ', '.join(map(lambda _: str(_), self.cards))
+        return ', '.join([str(card) for card in self.cards])
+
+    def __len__(self) -> int:
+        return len(self.cards)
+
+    def __getitem__(self, index: Union[int, slice]) -> Union[Card, List[Card]]:
+        return self.cards[index]
```

### Comparing `CardGameBase-1.0.4/CardGameBase/Hand.py` & `CardGameBase-1.0.5/CardGameBase/Hand.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,25 +20,36 @@
         """
         Draw {amount} amount of card(s)
 
         :param amount: amount of cards to be drawn
         :param dont_take_away: Don't take the cards away from deck and put to the bottom of the deck
         """
         if amount > 1:
-            self.hand.extend(self.deck.get_card(amount, dont_take_away))
+            extend_hand = self.deck.get_card(amount, dont_take_away)
+            if self.check_with_rank:
+                for card in extend_hand:
+                    card.calculate_with_rank = True
+            self.hand.extend(extend_hand)
         else:
-            self.hand.append(self.deck.get_card(amount, dont_take_away))
+            append_hand = self.deck.get_card(amount, dont_take_away)
+            if self.check_with_rank:
+                for card in append_hand:
+                    card.calculate_with_rank = True
+            self.hand.append(append_hand)
 
     def empty(self, put_back: bool = True) -> None:
         """
         Removes cards from hand
 
         :param put_back: when true puts cards back to the deck
         """
         if put_back:
+            if self.check_with_rank:
+                for card in self.hand:
+                    card.calculate_with_rank = False
             self.deck.add_card(self.hand)
         self.hand = []
 
     def check_rules(self, on_invalid: callable = None) -> None | str:
         """
         Check if the hand is valid
 
@@ -78,40 +89,41 @@
                     return self.rules
 
                 fixed_hand = on_invalid(self.hand, self.rules)
                 if fixed_hand is not None:
                     self.hand = fixed_hand
                 return self.rules
 
-    def get_total_value(self, symbol: str = None, with_rank: bool = False) -> int:
+    def get_total_value(self, symbol: str = None, with_rank: bool = None) -> int:
         """
         Get the value of all cards in hand
         :param symbol: if set only cards with the given symbol are counted
         :param with_rank: when set the value of the card is multiplied by the cards symbol_rank
         :return: The sum
         """
         _sum = 0
         if symbol:
-            if with_rank:
+            if with_rank or (self.check_with_rank and with_rank is None):
                 for card in self.hand:
                     if card.symbol == symbol:
                         _sum += card.value * card.symbol_rank
                     elif symbol is None:
                         _sum += card.value * card.symbol_rank
                 return _sum
 
             for card in self.hand:
                 if card.symbol == symbol:
                     _sum += card.value
             return _sum
 
-        if with_rank:
+        if with_rank or (self.check_with_rank and with_rank is None):
             for card in self.hand:
                 _sum += card.value * card.symbol_rank
             return _sum
+
         return sum(self.hand)
 
     @property
     def check_with_rank(self) -> bool:
         return self.__check_with_rank
 
     @check_with_rank.setter
```

### Comparing `CardGameBase-1.0.4/CardGameBase/Utility.py` & `CardGameBase-1.0.5/CardGameBase/Utility.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def create_classic_deck() -> Deck:
     """
     Creates a classic deck with 52 cards of clubs, spades, diamonds and hearts (2 - Ace)
 
     :return: The Deck
     """
-    symbols = [['c', 1], ['d', 2], ['h', 3], ['s', 4]]
+    symbols = [('c', 1), ('d', 2), ('h', 3), ('s', 4)]
     deck_config = DeckConfig()
 
     for symbol, symbol_rank in symbols:
         for card_value in range(2, 14 + 1):
             # 10 = 10, 11 = j, 12 = d, 13 = j, 14 = k
             if card_value == 11:
                 deck_config.add_card(symbol, symbol_rank, 10, "J")
```

### Comparing `CardGameBase-1.0.4/CardGameBase.egg-info/PKG-INFO` & `CardGameBase-1.0.5/CardGameBase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CardGameBase
-Version: 1.0.4
+Version: 1.0.5
 Summary: Card Game Base with basic deck and card class
 Home-page: https://github.com/DerSchinken/CardGameBase/
 Author: DerSchinken
 Maintainer: DerSchinken
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `CardGameBase-1.0.4/LICENSE` & `CardGameBase-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.4/PKG-INFO` & `CardGameBase-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CardGameBase
-Version: 1.0.4
+Version: 1.0.5
 Summary: Card Game Base with basic deck and card class
 Home-page: https://github.com/DerSchinken/CardGameBase/
 Author: DerSchinken
 Maintainer: DerSchinken
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `CardGameBase-1.0.4/README.md` & `CardGameBase-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.4/setup.py` & `CardGameBase-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 # Get requirements
 with open("requirements.txt", "r") as reqs:
     requirements = reqs.read().splitlines()
 
 setup(
     name="CardGameBase",
-    version="1.0.4",
+    version="1.0.5",
     # Major version 1
     # Minor version 0
-    # Maintenance version 0
+    # Maintenance version 5
 
     author="DerSchinken",
     maintainer="DerSchinken",
     description="Card Game Base with basic deck and card class",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

