# Comparing `tmp/quick_menu-0.5.0.tar.gz` & `tmp/quick_menu-0.6.0.tar.gz`

## Comparing `quick_menu-0.5.0.tar` & `quick_menu-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 quick_menu-0.5.0/mkdocs.yml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 quick_menu-0.5.0/.vscode/settings.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 quick_menu-0.5.0/docs/index.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 quick_menu-0.5.0/src/quick_menu/__about__.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 quick_menu-0.5.0/src/quick_menu/__init__.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 quick_menu-0.5.0/src/quick_menu/menu.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 quick_menu-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 quick_menu-0.5.0/tests/test_menu.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 quick_menu-0.5.0/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 quick_menu-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 quick_menu-0.5.0/README.md
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 quick_menu-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 quick_menu-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 quick_menu-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 quick_menu-0.6.0/mkdocs.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 quick_menu-0.6.0/.vscode/settings.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 quick_menu-0.6.0/docs/index.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 quick_menu-0.6.0/src/quick_menu/__about__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 quick_menu-0.6.0/src/quick_menu/__init__.py
+-rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 quick_menu-0.6.0/src/quick_menu/menu.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 quick_menu-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 quick_menu-0.6.0/tests/test_menu.py
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 quick_menu-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 quick_menu-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 quick_menu-0.6.0/README.md
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 quick_menu-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 quick_menu-0.6.0/PKG-INFO
```

### Comparing `quick_menu-0.5.0/mkdocs.yml` & `quick_menu-0.6.0/mkdocs.yml`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-site_name: quick-menu
-theme:
-  name: material
-  features:
-    - navigation.tabs
-    - toc.integrate
-    - navigation.top
-    - navigation.footer
-    - content.code.copy
-  language: en
-  palette:
-    - scheme: default
-      toggle:
-        icon: material/toggle-switch-off-outline
-        name: Switch to dark mode
-    - scheme: slate
-      toggle:
-        icon: material/toggle-switch
-        name: Switch to light mode
-watch:
-  - src/quick_menu
-
-plugins:
-  - search:
-      lang: en
-  - mkdocstrings:
-      handlers:
-        python:
-          paths: [src]
-  - offline
-markdown_extensions:
-  - pymdownx.highlight:
-      anchor_linenums: true
-      line_spans: __span
-      pygments_lang_class: true
-  - pymdownx.inlinehilite
-  - pymdownx.snippets
-  - pymdownx.superfences
-  - pymdownx.details
-  - pymdownx.mark
-  - pymdownx.tabbed:
-      alternate_style: true
-  - pymdownx.tasklist:
-      custom_checkbox: true
-  - pymdownx.arithmatex:
-      generic: true
-  - pymdownx.emoji:
-      emoji_index: !!python/name:materialx.emoji.twemoji
-      emoji_generator: !!python/name:materialx.emoji.to_svg
-  - admonition
-  - attr_list
-  - md_in_html
-  - abbr
-  - footnotes
-copyright: |
-  &copy; 2023, Stephan Poole
+site_name: quick-menu
+theme:
+  name: material
+  features:
+    - navigation.tabs
+    - toc.integrate
+    - navigation.top
+    - navigation.footer
+    - content.code.copy
+  language: en
+  palette:
+    - scheme: default
+      toggle:
+        icon: material/toggle-switch-off-outline
+        name: Switch to dark mode
+    - scheme: slate
+      toggle:
+        icon: material/toggle-switch
+        name: Switch to light mode
+watch:
+  - src/quick_menu
+
+plugins:
+  - search:
+      lang: en
+  - mkdocstrings:
+      handlers:
+        python:
+          paths: [src]
+  - offline
+markdown_extensions:
+  - pymdownx.highlight:
+      anchor_linenums: true
+      line_spans: __span
+      pygments_lang_class: true
+  - pymdownx.inlinehilite
+  - pymdownx.snippets
+  - pymdownx.superfences
+  - pymdownx.details
+  - pymdownx.mark
+  - pymdownx.tabbed:
+      alternate_style: true
+  - pymdownx.tasklist:
+      custom_checkbox: true
+  - pymdownx.arithmatex:
+      generic: true
+  - pymdownx.emoji:
+      emoji_index: !!python/name:materialx.emoji.twemoji
+      emoji_generator: !!python/name:materialx.emoji.to_svg
+  - admonition
+  - attr_list
+  - md_in_html
+  - abbr
+  - footnotes
+copyright: |
+  &copy; 2023, Stephan Poole
```

### Comparing `quick_menu-0.5.0/src/quick_menu/menu.py` & `quick_menu-0.6.0/src/quick_menu/menu.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,140 +1,186 @@
-"""Provide a simple means to create text menus for a console application.
-
-Example:
-
-    This example shows two ways to create a menu, one for the submenu and the other
-    for the main menu.
-
-        from quick_menu.menu import Menu, MenuItem
-
-        def func1(val=1):
-            print("func1: val =", val)
-            input("\\nPress [Enter] to continue")
-
-        submenu = Menu("Submenu", menu_items=[
-            MenuItem("1", "Do func1", action=func1),
-            MenuItem("X", "Go back", is_exit=True),
-        ])
-        menu = (
-            Menu("Some Title")
-            .add(MenuItem("1", "Func1 default", action=func1))
-            .add(MenuItem("2", "Func1 with val", action=func1, kwargs={"val": 4}))
-            .add(MenuItem("S", "Submenu", action=submenu.run))
-            .add(MenuItem("X", "Exit", is_exit=True))
-        )
-
-        menu.run()
-"""
-import os
-from dataclasses import dataclass, field
-from typing import Callable, Dict, List, Optional
-
-from typing_extensions import Self
-
-
-@dataclass
-class MenuItem:
-    """A menu item to add to a menu.
-
-    The menu item can optionally call a function or start a submenu. A menu item can
-    also be an exit item which exits the curren menu.
-
-    Parameters:
-        choice:  The string used to select the menu item.
-        label:   The text label displayed for the menu item.
-        action:  An optional function to be called when the menu item is selected.
-        kwargs:  Arguments to pass to a menu item action.
-        is_exit: Whether or not this menu item exits the current menu
-    """
-
-    choice: str
-    label: str
-    action: Optional[Callable[..., None]] = None
-    kwargs: dict = field(default_factory=dict)
-    is_exit: bool = False
-
-    def select(self):
-        """Select the menu item.
-
-        This selects the `MenuItem` which runs any associated action with kwargs and
-        then returns whether or not selecting this item should tell the current menu to
-        exit.
-        """
-        if self.action:
-            self.action(**self.kwargs)
-        return not self.is_exit
-
-
-class Menu:
-    """A menu that can be displayed and accepts user selections."""
-
-    BANNER_WIDTH: int = 40
-
-    def __init__(
-        self,
-        title: str,
-        menu_items: Optional[List[MenuItem]] = None,
-        prompt: Optional[str] = None,
-        auto_clear: Optional[bool] = None,
-    ):
-        """Create a new menu.
-
-        Parameters:
-            title: The title to display at the top of the menu.
-            menu_items: An optional list of `MenuItem` to add to the menu.
-            prompt:     An optional custom prompt for input.
-            auto_clear:  Whether or not to clear the screen before running.
-        """
-        self.title = title
-        self.menu_items: Dict[str, MenuItem] = {}
-        if menu_items:
-            for menu_item in menu_items:
-                self.add(menu_item)
-        self.prompt = prompt if prompt else ">> "
-        self.auto_clear = auto_clear if auto_clear else True
-
-    def add(self, menu_item: MenuItem) -> Self:
-        """Add a new MenuItemq.
-
-        Parameters:
-            menu_item: A `MenuItem` instance.
-
-        Returns:
-            The `Menu` instance. This allows chaining of the `add` calls. For example:
-
-                    menu.add("1", "First").add("2", "Second")
-        """
-        self.menu_items[menu_item.choice.lower()] = menu_item
-        return self
-
-    def display(self) -> str:
-        """Return the Menu display as a string."""
-        title_length = len(self.title) + 2
-        right_length = (Menu.BANNER_WIDTH - title_length) // 2
-        left_length = Menu.BANNER_WIDTH - title_length - right_length
-        out = [" ".join(["=" * left_length, self.title, "=" * right_length])]
-        for key in sorted(self.menu_items):
-            menu_item = self.menu_items[key]
-            out.append(f"{menu_item.choice}: {menu_item.label}")
-        out.append("=" * Menu.BANNER_WIDTH)
-        return "\n".join(out)
-
-    def run(self) -> None:
-        """Display the `Menu` and start a loop to process selections."""
-        running = True
-        while running:
-            if self.auto_clear:
-                Menu.clear()
-            print(self.display())
-            choice = input(self.prompt)
-            key = choice.lower()
-            if key in self.menu_items:
-                running = self.menu_items[key].select()
-            else:
-                print(f"Invalid choice: {choice}")
-                input("\nPress [Enter] to continue")
-
-    @staticmethod
-    def clear() -> None:
-        """Calls a system method to clear the console."""
-        os.system("clear" if os.name == "posix" else "cls")
+"""Provide a simple means to create text menus for a console application.
+
+Example:
+
+    This example shows two ways to create a menu, one for the submenu and the other
+    for the main menu.
+
+        from quick_menu.menu import Menu, MenuItem
+
+        def func1(val=1):
+            print("func1: val =", val)
+            input("Press [Enter] to continue")
+
+        submenu = Menu(
+            "Submenu",
+            menu_items=[
+                MenuItem("1", "Do func1", action=func1),
+                MenuItem("X", "Go back", is_exit=True),
+            ]
+        )
+        menu = (
+            Menu("Some Title")
+            .add(MenuItem("1", "Func1 default", action=func1))
+            .add(MenuItem("2", "Func1 with val", action=func1, action_args={"val": 4}))
+            .add(MenuItem("S", "Submenu", action=submenu.run))
+            .add(MenuItem("X", "Exit", is_exit=True))
+        )
+
+        menu.run()
+"""
+import os
+from dataclasses import dataclass, field
+from typing import Any, Callable, ClassVar, Dict, List, Optional, Tuple
+
+from typing_extensions import Self
+
+
+@dataclass
+class MenuItem:
+    """A menu item to add to a menu.
+
+    The menu item can optionally call a function or start a submenu. A menu item can
+    also be an exit item which exits the curren menu.
+
+    Parameters:
+        choice:       The string used to select the menu item.
+        label:        The text label displayed for the menu item.
+        action:       An optional function to be called when the menu item is selected.
+        action_args:  Arguments to pass to a menu item action.
+        is_exit:      Whether or not this menu item exits the current menu
+    """
+
+    VALID_UPDATE_FIELDS: ClassVar[Tuple[str, ...]] = ("label", "action", "action_args")
+
+    choice: str
+    label: str
+    action: Optional[Callable[..., None]] = None
+    action_args: dict = field(default_factory=dict)
+    is_exit: bool = False
+
+    def select(self) -> bool:
+        """Select the menu item.
+
+        This selects the `MenuItem` which runs any associated action with kwargs and
+        then returns whether or not selecting this item should tell the current menu to
+        exit.
+
+        Returns:
+            True if the item is an exit item; False otherwise
+        """
+        if self.action:
+            self.action(**self.action_args)
+        return not self.is_exit
+
+    def update(self, **kwargs: Dict[str, Any]) -> None:
+        """Update menu item fields.
+
+        Any key matching a field to be updated is replaced with the new vlaue. Any
+        remaining key/value pairs are used to update the `action_args`.
+
+        Paramaters:
+            kwargs: A dict with fields to be updated.
+        """
+        for name in MenuItem.VALID_UPDATE_FIELDS:
+            val = kwargs.pop(name, None)
+            if val:
+                setattr(self, name, val)
+        # Anything else is used to update kwargs
+        self.action_args.update(kwargs)
+
+
+class Menu:
+    """A menu that can be displayed and accepts user selections."""
+
+    BANNER_WIDTH: int = 40
+
+    def __init__(
+        self,
+        title: str,
+        menu_items: Optional[List[MenuItem]] = None,
+        prompt: Optional[str] = None,
+        auto_clear: Optional[bool] = None,
+    ):
+        """Create a new menu.
+
+        Parameters:
+            title: The title to display at the top of the menu.
+            menu_items: An optional list of `MenuItem` to add to the menu.
+            prompt:     An optional custom prompt for input.
+            auto_clear:  Whether or not to clear the screen before running.
+        """
+        self.title = title
+        self.menu_items: Dict[str, MenuItem] = {}
+        if menu_items:
+            for menu_item in menu_items:
+                self.add(menu_item)
+        self.prompt = prompt if prompt else ">> "
+        self.auto_clear = auto_clear if auto_clear else True
+
+    def add(self, menu_item: MenuItem) -> Self:
+        """Add a new MenuItemq.
+
+        Parameters:
+            menu_item: A `MenuItem` instance.
+
+        Returns:
+            The `Menu` instance. This allows chaining of the `add` calls. For example:
+
+                    menu.add("1", "First").add("2", "Second")
+        """
+        if menu_item.is_exit is True:
+            # Check if there is an existing exit since there can be only one
+            exit_key = self._exit_choice()
+            if exit_key:
+                del self.menu_items[exit_key]
+        self.menu_items[menu_item.choice.lower()] = menu_item
+        self._ensure_one_exit_exists()
+        return self
+
+    def display(self) -> str:
+        """Return the Menu display as a string."""
+        title_length = len(self.title) + 2
+        right_length = (Menu.BANNER_WIDTH - title_length) // 2
+        left_length = Menu.BANNER_WIDTH - title_length - right_length
+        out = [" ".join(["=" * left_length, self.title, "=" * right_length])]
+        for key in sorted(self.menu_items):
+            menu_item = self.menu_items[key]
+            out.append(f"{menu_item.choice}: {menu_item.label}")
+        out.append("=" * Menu.BANNER_WIDTH)
+        return "\n".join(out)
+
+    def run(self) -> None:
+        """Display the `Menu` and start a loop to process selections."""
+        running = True
+        while running:
+            if self.auto_clear:
+                Menu.clear()
+            print(self.display())
+            choice = input(self.prompt)
+            key = choice.lower()
+            if key in self.menu_items:
+                running = self.menu_items[key].select()
+            else:
+                print(f"Invalid choice: {choice}")
+                input("\nPress [Enter] to continue")
+
+    def update(self, choice: str, **kwargs: Dict[str, Any]) -> None:
+        menu_item = self.menu_items.get(choice.lower())
+        if menu_item:
+            menu_item.update(**kwargs)
+
+    def _exit_choice(self) -> Optional[str]:
+        exit_keys = [k for k, v in self.menu_items.items() if v.is_exit is True]
+        if exit_keys:
+            return exit_keys[0]
+        return None
+
+    def _ensure_one_exit_exists(self) -> None:
+        exit_key = self._exit_choice()
+        if not exit_key:
+            self.menu_items["x"] = MenuItem("X", "Exit", is_exit=True)
+
+    @staticmethod
+    def clear() -> None:
+        """Calls a system method to clear the console."""
+        os.system("clear" if os.name == "posix" else "cls")
```

### Comparing `quick_menu-0.5.0/LICENSE.txt` & `quick_menu-0.6.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-MIT License
-
-Copyright (c) 2023-present Stephan Poole <yqbear@gmail.com>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+MIT License
+
+Copyright (c) 2023-present Stephan Poole <yqbear@gmail.com>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `quick_menu-0.5.0/pyproject.toml` & `quick_menu-0.6.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,174 +1,176 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "quick-menu"
-dynamic = ["version"]
-description = ''
-readme = "README.md"
-requires-python = ">=3.7"
-license = "MIT"
-keywords = []
-authors = [
-  { name = "Stephan Poole", email = "yqbear@gmail.com" },
-]
-classifiers = [
-  "Development Status :: 4 - Beta",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
-]
-dependencies = ["typing_extensions"]
-
-[project.urls]
-Documentation = "https://yqbear.github.io/quick-menu"
-Issues = "https://github.com/yqbear/quick-menu/issues"
-Source = "https://github.com/yqbear/quick-menu"
-
-[tool.hatch.version]
-path = "src/quick_menu/__about__.py"
-
-[tool.hatch.envs.default]
-dependencies = [
-  "coverage[toml]>=6.5",
-  "pytest",
-  "pytest-mock",
-]
-[tool.hatch.envs.default.scripts]
-test = "pytest {args:tests}"
-test-cov = "coverage run -m pytest {args:tests}"
-cov-report = [
-  "- coverage combine",
-  "coverage report",
-]
-cov = [
-  "test-cov",
-  "cov-report",
-]
-
-[[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
-
-[tool.hatch.envs.lint]
-detached = true
-dependencies = [
-  "black>=23.1.0",
-  "mypy>=1.0.0",
-  "ruff>=0.0.243",
-]
-[tool.hatch.envs.lint.scripts]
-typing = "mypy --install-types --non-interactive {args:src/quick_menu tests}"
-style = [
-  "ruff {args:.}",
-  "black --check --diff {args:.}",
-]
-fmt = [
-  "black {args:.}",
-  "ruff --fix {args:.}",
-  "style",
-]
-all = [
-  "style",
-  "typing",
-]
-
-[tool.hatch.envs.doc]
-detached = true
-dependencies = [
-  "mkdocs",
-  "mkdocstrings[python]",
-  "mkdocs-material",
-]
-
-[tool.hatch.envs.doc.scripts]
-serve = "mkdocs serve"
-build = "mkdocs build"
-
-[tool.black]
-target-version = ["py37"]
-line-length = 120
-skip-string-normalization = true
-
-[tool.ruff]
-target-version = "py37"
-line-length = 120
-select = [
-  "A",
-  "ARG",
-  "B",
-  "C",
-  "DTZ",
-  "E",
-  "EM",
-  "F",
-  "FBT",
-  "I",
-  "ICN",
-  "ISC",
-  "N",
-  "PLC",
-  "PLE",
-  "PLR",
-  "PLW",
-  "Q",
-  "RUF",
-  "S",
-  "T",
-  "TID",
-  "UP",
-  "W",
-  "YTT",
-]
-ignore = [
-  # Allow non-abstract empty methods in abstract base classes
-  "B027",
-  # Allow boolean positional values in function calls, like `dict.get(... True)`
-  "FBT003",
-  # Ignore checks for possible passwords
-  "S105", "S106", "S107",
-  # Ignore complexity
-  "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
-  # Ignore print check
-  "T201",
-  # Ignore process with a shell
-  "S605",
-]
-unfixable = [
-  # Don't touch unused imports
-  "F401",
-]
-
-[tool.ruff.isort]
-known-first-party = ["quick_menu"]
-
-[tool.ruff.flake8-tidy-imports]
-ban-relative-imports = "all"
-
-[tool.ruff.per-file-ignores]
-# Tests can use magic values, assertions, and relative imports
-"tests/**/*" = ["PLR2004", "S101", "TID252"]
-
-[tool.coverage.run]
-source_pkgs = ["quick_menu", "tests"]
-branch = true
-parallel = true
-omit = [
-  "src/quick_menu/__about__.py",
-]
-
-[tool.coverage.paths]
-quick_menu = ["src/quick_menu", "*/quick-menu/src/quick_menu"]
-tests = ["tests", "*/quick-menu/tests"]
-
-[tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-]
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "quick-menu"
+dynamic = ["version"]
+description = "A simple package to create text menus for use in console applications"
+readme = "README.md"
+requires-python = ">=3.7"
+license = "MIT"
+keywords = []
+authors = [
+  { name = "Stephan Poole", email = "yqbear@gmail.com" },
+]
+classifiers = [
+  "Development Status :: 4 - Beta",
+  "Environment :: Console",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
+]
+dependencies = ["typing_extensions"]
+
+[project.urls]
+Documentation = "https://yqbear.github.io/quick-menu"
+Issues = "https://github.com/yqbear/quick-menu/issues"
+Source = "https://github.com/yqbear/quick-menu"
+
+[tool.hatch.version]
+path = "src/quick_menu/__about__.py"
+
+[tool.hatch.envs.default]
+dependencies = [
+  "coverage[toml]>=6.5",
+  "pytest",
+  "pytest-mock",
+]
+[tool.hatch.envs.default.scripts]
+test = "pytest {args:tests}"
+test-cov = "coverage run -m pytest {args:tests}"
+cov-report = [
+  "- coverage combine",
+  "coverage report",
+]
+cov = [
+  "test-cov",
+  "cov-report",
+]
+
+[[tool.hatch.envs.all.matrix]]
+python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+
+[tool.hatch.envs.lint]
+detached = true
+dependencies = [
+  "black>=23.1.0",
+  "mypy>=1.0.0",
+  "ruff>=0.0.243",
+]
+[tool.hatch.envs.lint.scripts]
+typing = "mypy --install-types --non-interactive {args:src/quick_menu tests}"
+style = [
+  "ruff {args:.}",
+  "black --check --diff {args:.}",
+]
+fmt = [
+  "black {args:.}",
+  "ruff --fix {args:.}",
+  "style",
+]
+all = [
+  "style",
+  "typing",
+]
+
+[tool.hatch.envs.doc]
+detached = true
+dependencies = [
+  "mkdocs",
+  "mkdocstrings[python]",
+  "mkdocs-material",
+]
+
+[tool.hatch.envs.doc.scripts]
+serve = "mkdocs serve"
+build = "mkdocs build"
+deploy = "mkdocs gh-deploy"
+
+[tool.black]
+target-version = ["py37"]
+line-length = 120
+skip-string-normalization = true
+
+[tool.ruff]
+target-version = "py37"
+line-length = 120
+select = [
+  "A",
+  "ARG",
+  "B",
+  "C",
+  "DTZ",
+  "E",
+  "EM",
+  "F",
+  "FBT",
+  "I",
+  "ICN",
+  "ISC",
+  "N",
+  "PLC",
+  "PLE",
+  "PLR",
+  "PLW",
+  "Q",
+  "RUF",
+  "S",
+  "T",
+  "TID",
+  "UP",
+  "W",
+  "YTT",
+]
+ignore = [
+  # Allow non-abstract empty methods in abstract base classes
+  "B027",
+  # Allow boolean positional values in function calls, like `dict.get(... True)`
+  "FBT003",
+  # Ignore checks for possible passwords
+  "S105", "S106", "S107",
+  # Ignore complexity
+  "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
+  # Ignore print check
+  "T201",
+  # Ignore process with a shell
+  "S605",
+]
+unfixable = [
+  # Don't touch unused imports
+  "F401",
+]
+
+[tool.ruff.isort]
+known-first-party = ["quick_menu"]
+
+[tool.ruff.flake8-tidy-imports]
+ban-relative-imports = "all"
+
+[tool.ruff.per-file-ignores]
+# Tests can use magic values, assertions, and relative imports
+"tests/**/*" = ["PLR2004", "S101", "TID252"]
+
+[tool.coverage.run]
+source_pkgs = ["quick_menu", "tests"]
+branch = true
+parallel = true
+omit = [
+  "src/quick_menu/__about__.py",
+]
+
+[tool.coverage.paths]
+quick_menu = ["src/quick_menu", "*/quick-menu/src/quick_menu"]
+tests = ["tests", "*/quick-menu/tests"]
+
+[tool.coverage.report]
+exclude_lines = [
+  "no cov",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+]
```

