# Comparing `tmp/arthub_login_widgets-0.3.3.tar.gz` & `tmp/arthub_login_widgets-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_login_widgets-0.3.3.tar", last modified: Tue Jun 27 13:54:03 2023, max compression
+gzip compressed data, was "arthub_login_widgets-0.4.0.tar", last modified: Mon Jul 17 06:09:57 2023, max compression
```

## Comparing `arthub_login_widgets-0.3.3.tar` & `arthub_login_widgets-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 13:54:03.065169 arthub_login_widgets-0.3.3/
--rw-rw-rw-   0        0        0      375 2023-06-27 13:54:03.065169 arthub_login_widgets-0.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 13:54:03.023552 arthub_login_widgets-0.3.3/arthub_login_widgets/
--rw-rw-rw-   0        0        0      435 2023-03-23 06:34:09.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/__init__.py
--rw-rw-rw-   0        0        0       23 2023-06-27 13:45:55.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/__version__.py
--rw-rw-rw-   0        0        0      502 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/constants.py
--rw-rw-rw-   0        0        0     7756 2023-03-23 06:37:43.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/core.py
--rw-rw-rw-   0        0        0     1182 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/filesystem.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:54:03.047218 arthub_login_widgets-0.3.3/arthub_login_widgets/resources/
--rw-rw-rw-   0        0        0        0 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/resources/__init__.py
--rw-rw-rw-   0        0        0    12338 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/resources/arthub_white.png
--rw-rw-rw-   0        0        0      721 2023-03-23 03:49:40.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/resources/style.qss
-drwxrwxrwx   0        0        0        0 2023-06-27 13:54:03.054201 arthub_login_widgets-0.3.3/arthub_login_widgets/test/
--rw-rw-rw-   0        0        0      173 2023-01-31 11:18:49.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/test/__init__.py
--rw-rw-rw-   0        0        0     1628 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/test/test_core.py
--rw-rw-rw-   0        0        0      766 2023-02-08 03:29:52.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/test/test_filesystem.py
--rw-rw-rw-   0        0        0      699 2023-02-07 12:54:18.000000 arthub_login_widgets-0.3.3/arthub_login_widgets/test/test_imports.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:54:03.063176 arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/
--rw-rw-rw-   0        0        0      375 2023-06-27 13:54:02.000000 arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      714 2023-06-27 13:54:02.000000 arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 13:54:02.000000 arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-27 13:54:02.000000 arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-27 13:54:02.000000 arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 13:54:03.066168 arthub_login_widgets-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-06-27 13:46:39.000000 arthub_login_widgets-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:09:57.600177 arthub_login_widgets-0.4.0/
+-rw-rw-rw-   0        0        0      375 2023-07-17 06:09:57.600177 arthub_login_widgets-0.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 06:09:57.570186 arthub_login_widgets-0.4.0/arthub_login_widgets/
+-rw-rw-rw-   0        0        0      435 2023-03-23 06:34:09.000000 arthub_login_widgets-0.4.0/arthub_login_widgets/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-17 05:59:48.000000 arthub_login_widgets-0.4.0/arthub_login_widgets/__version__.py
+-rw-rw-rw-   0        0        0      590 2023-07-17 06:03:02.000000 arthub_login_widgets-0.4.0/arthub_login_widgets/constants.py
+-rw-rw-rw-   0        0        0     9782 2023-07-17 06:07:05.000000 arthub_login_widgets-0.4.0/arthub_login_widgets/core.py
+-rw-rw-rw-   0        0        0     1182 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.0/arthub_login_widgets/filesystem.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:09:57.575120 arthub_login_widgets-0.4.0/arthub_login_widgets/resources/
+-rw-rw-rw-   0        0        0        0 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.0/arthub_login_widgets/resources/__init__.py
+-rw-rw-rw-   0        0        0    12338 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.0/arthub_login_widgets/resources/arthub_white.png
+-rw-rw-rw-   0        0        0      965 2023-07-17 06:00:27.000000 arthub_login_widgets-0.4.0/arthub_login_widgets/resources/style.qss
+drwxrwxrwx   0        0        0        0 2023-07-17 06:09:57.582036 arthub_login_widgets-0.4.0/arthub_login_widgets/test/
+-rw-rw-rw-   0        0        0      173 2023-01-31 11:18:49.000000 arthub_login_widgets-0.4.0/arthub_login_widgets/test/__init__.py
+-rw-rw-rw-   0        0        0     1628 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.0/arthub_login_widgets/test/test_core.py
+-rw-rw-rw-   0        0        0      766 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.0/arthub_login_widgets/test/test_filesystem.py
+-rw-rw-rw-   0        0        0      699 2023-02-07 12:54:18.000000 arthub_login_widgets-0.4.0/arthub_login_widgets/test/test_imports.py
+drwxrwxrwx   0        0        0        0 2023-07-17 06:09:57.593135 arthub_login_widgets-0.4.0/arthub_login_widgets.egg-info/
+-rw-rw-rw-   0        0        0      375 2023-07-17 06:09:57.000000 arthub_login_widgets-0.4.0/arthub_login_widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1177 2023-07-17 06:09:57.000000 arthub_login_widgets-0.4.0/arthub_login_widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 06:09:57.000000 arthub_login_widgets-0.4.0/arthub_login_widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-17 06:09:57.000000 arthub_login_widgets-0.4.0/arthub_login_widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-17 06:09:57.000000 arthub_login_widgets-0.4.0/arthub_login_widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 06:09:57.602156 arthub_login_widgets-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-06-27 13:46:39.000000 arthub_login_widgets-0.4.0/setup.py
```

### Comparing `arthub_login_widgets-0.3.3/arthub_login_widgets/core.py` & `arthub_login_widgets-0.4.0/arthub_login_widgets/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,38 +14,40 @@
 # Import third-party modules
 from qtpy import QtCore
 from qtpy import QtGui
 from qtpy import QtWidgets
 
 # Import local modules
 from arthub_login_widgets.constants import ARTHUB_RESET_PASSWORD_WEB_URL
+from arthub_login_widgets.constants import ARTHUB_SET_ACCOUNT_INFO_WEB_URL
 from arthub_login_widgets.constants import UI_TEXT_MAP
 from arthub_login_widgets.filesystem import get_login_account
 from arthub_login_widgets.filesystem import get_resource_file
 from arthub_login_widgets.filesystem import save_login_account
 
 
-def _load_style_sheet(style_file):
+def load_style_sheet(style_file):
     try:
-        from lightbox_ui.style import load_style_sheet
-        return load_style_sheet(style_file)
+        from lightbox_ui.style import load_style_sheet as style_sheet
+        return style_sheet(style_file)
     except ImportError:
         with open(style_file, "r") as css_file:
             css_string = css_file.read().strip("\n")
             data = os.path.expandvars(css_string)
             return data
 
 
-class LoginWindow(QtWidgets.QDialog):
+class LoginWindow(QtWidgets.QMainWindow):
     def __init__(
             self,
             api,
             api_callback=None,
             parent_window=None,
             language_cn=True,
+            save_login_state=True
     ):
         """Initialize an instance.
 
         Args:
             api(arthub_api.OpenAPI): The instance of the arthub_api.OpenAPI.
             api_callback (Function, optional): Called when the login is successful, the login status will be saved
                                                      in arthub_open_api.
@@ -54,36 +56,37 @@
 
         """
         super(LoginWindow, self).__init__(parent=parent_window)
         self.language_cn = language_cn
         self.arthub_open_api = api
         self._api_callback = api_callback
         self.logged = False
+        self.login_account_info = None
+        self.save_login_state = save_login_state
 
         # init ui
-        self.setFixedSize(280, 290)
-        # self.central_widget = QtWidgets.QWidget(self)
-        # self.central_widget.setObjectName("central_widget")
-        # self.setCentralWidget(self.central_widget)
-        self.central_widget = self
+        self.setFixedSize(300, 300)
+        self.central_widget = QtWidgets.QWidget(self)
+        self.central_widget.setObjectName("central_widget")
+        self.setCentralWidget(self.central_widget)
 
         # icon
         self.icon_label = QtWidgets.QLabel(self)
         self.icon_label.setFixedSize(QtCore.QSize(167, 40))
         self.icon_label.setPixmap(QtGui.QPixmap(get_resource_file("arthub_white.png")))
         self.icon_label.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.icon_label.setScaledContents(True)
 
         # line edit
         def _create_line_edit():
             _line_edit_font = QtGui.QFont()
             _line_edit_font.setPixelSize(13)
             _line_edit = QtWidgets.QLineEdit(self)
             _line_edit.setFont(_line_edit_font)
-            _line_edit.setFixedSize(228, 31)
+            _line_edit.setFixedSize(238, 31)
             _line_edit.setTextMargins(5, 0, 5, 0)
             return _line_edit
 
         self.line_edit_account = _create_line_edit()
         self.line_edit_password = _create_line_edit()
         self.line_edit_password.setEchoMode(QtWidgets.QLineEdit.EchoMode.Password)
 
@@ -91,42 +94,57 @@
         _label_prompt_font = QtGui.QFont()
         _label_prompt_font.setPixelSize(11)
         self.label_prompt = QtWidgets.QLabel("", self)
         self.label_prompt.setObjectName("label_prompt")
         self.label_prompt.setFont(_label_prompt_font)
         self.label_prompt.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
 
+        # set account info button
+        _label_button_font = QtGui.QFont()
+        _label_button_font.setPixelSize(11)
+        self.label_set_account_info = QtWidgets.QPushButton("", self)
+        self.label_set_account_info.setText("Please complete personal information")
+        self.label_set_account_info.setObjectName("label_set_account_info")
+        self.label_set_account_info.setFont(_label_button_font)
+        self.label_set_account_info.setCursor(QtCore.Qt.CursorShape.PointingHandCursor)
+        self.label_set_account_info.clicked.connect(self.on_set_account_info)
+
         # login button
         self.pushButton_login = QtWidgets.QPushButton(self.central_widget)
         self.pushButton_login.setObjectName("pushButton_login")
         self.pushButton_login.setText("")
-        self.pushButton_login.setFixedSize(228, 34)
+        self.pushButton_login.setFixedSize(238, 34)
         self.pushButton_login.setCursor(QtCore.Qt.CursorShape.PointingHandCursor)
         self.pushButton_login.clicked.connect(self.on_login)
 
         # reset password button
-        _label_forgot_password_font = QtGui.QFont()
-        _label_forgot_password_font.setPixelSize(11)
         self.label_forgot_password = QtWidgets.QPushButton("", self)
         self.label_forgot_password.setObjectName("label_forgot_password")
-        self.label_forgot_password.setFont(_label_forgot_password_font)
+        self.label_forgot_password.setFont(_label_button_font)
         self.label_forgot_password.setCursor(QtCore.Qt.CursorShape.PointingHandCursor)
         self.label_forgot_password.clicked.connect(self.on_forgot_password)
 
+        prompt_area = QtWidgets.QWidget(self)
+        prompt_area.setObjectName("prompt_area")
+        prompt_area.setFixedHeight(27)
+        prompt_area_layout = QtWidgets.QHBoxLayout(prompt_area)
+        prompt_area_layout.addWidget(self.label_prompt)
+        prompt_area_layout.addWidget(self.label_set_account_info)
+
         main_layout = QtWidgets.QVBoxLayout(self.central_widget)
         main_layout.addSpacing(31)
         main_layout.setSpacing(5)
         main_layout.addWidget(self.icon_label)
         main_layout.addSpacing(15)
         main_layout.setAlignment(self.icon_label, QtCore.Qt.AlignmentFlag.AlignCenter)
         main_layout.addWidget(self.line_edit_account)
         main_layout.setAlignment(self.line_edit_account, QtCore.Qt.AlignmentFlag.AlignCenter)
         main_layout.addWidget(self.line_edit_password)
         main_layout.setAlignment(self.line_edit_password, QtCore.Qt.AlignmentFlag.AlignCenter)
-        main_layout.addWidget(self.label_prompt)
+        main_layout.addWidget(prompt_area)
         main_layout.setAlignment(self.label_prompt, QtCore.Qt.AlignmentFlag.AlignCenter)
         main_layout.addWidget(self.pushButton_login)
         main_layout.setAlignment(self.pushButton_login, QtCore.Qt.AlignmentFlag.AlignCenter)
         main_layout.addSpacing(1)
         main_layout.addWidget(self.label_forgot_password)
         main_layout.setAlignment(self.label_forgot_password, QtCore.Qt.AlignmentFlag.AlignCenter)
         main_layout.addSpacing(23)
@@ -136,17 +154,20 @@
         # init model
         last_account = get_login_account()
         if last_account is not None:
             self.line_edit_account.setText(last_account)
 
         # set style
         qss_file = get_resource_file("style.qss")
-        style_sheet = _load_style_sheet(qss_file)
+        style_sheet = load_style_sheet(qss_file)
         self.setStyleSheet(style_sheet)
 
+        # init status
+        self.show_prompt("")
+
     def set_callback(self, callback):
         self._api_callback = callback
 
     def _get_ui_text_by_language(self, key):
         v = UI_TEXT_MAP.get(key)
         if v is None:
             return ""
@@ -155,44 +176,67 @@
     def translate_ui(self):
         self.setWindowTitle(self._get_ui_text_by_language("window_title"))
         self.line_edit_account.setPlaceholderText(self._get_ui_text_by_language("account_placeholder"))
         self.line_edit_password.setPlaceholderText(self._get_ui_text_by_language("password_placeholder"))
         self.pushButton_login.setText(self._get_ui_text_by_language("login_button"))
         self.label_forgot_password.setText(self._get_ui_text_by_language("forgot_password_button"))
 
-    def set_prompt(self, text):
+    def show_prompt(self, text):
+        self.label_set_account_info.setVisible(False)
+        self.label_prompt.setVisible(True)
         self.label_prompt.setText(text)
 
+    def show_set_account_info(self):
+        self.label_set_account_info.setVisible(True)
+        self.label_prompt.setVisible(False)
+
     def _on_login_succeeded(self, account):
         save_login_account(account)
         if self._api_callback:
             self._api_callback(self)
+        if self.save_login_state:
+            self.arthub_open_api.save_token_to_cache()
         self.logged = True
         self.close()
 
+    def check_account_info(self):
+        res = self.arthub_open_api.get_account_detail()
+        if not res.is_succeeded():
+            self.show_prompt("Account information not found")
+            return False
+        self.login_account_info = res.first_result()
+        company = self.login_account_info.get("company")
+        if not company:
+            self.show_set_account_info()
+            return False
+        return True
+
     def login(self):
-        self.set_prompt("")
+        self.show_prompt("")
         account = self.line_edit_account.text()
         password = self.line_edit_password.text()
         if account == "":
-            self.set_prompt("Email/Phone cannot be empty")
+            self.show_prompt("Email/Phone cannot be empty")
             return
         if password == "":
-            self.set_prompt("Password cannot be empty")
+            self.show_prompt("Password cannot be empty")
             return
-
-        res = self.arthub_open_api.login(account, password)
+        res = self.arthub_open_api.login(account, password, save_token_to_cache=False)
         if not res.is_succeeded():
             error_msg = res.error_message()
             logging.warning("Log in ArtHub failed: %s", error_msg)
-            self.set_prompt(error_msg)
+            self.show_prompt(error_msg)
             return
-
-        self._on_login_succeeded(account)
-        self.accept()
+        if self.check_account_info():
+            self._on_login_succeeded(account)
 
     def on_login(self):
         self.login()
 
     @staticmethod
     def on_forgot_password():
         webbrowser.open(ARTHUB_RESET_PASSWORD_WEB_URL)
+
+    def on_set_account_info(self):
+        if self.login_account_info:
+            account_name = self.login_account_info.get("account_name")
+            webbrowser.open(ARTHUB_SET_ACCOUNT_INFO_WEB_URL + account_name)
```

### Comparing `arthub_login_widgets-0.3.3/arthub_login_widgets/filesystem.py` & `arthub_login_widgets-0.4.0/arthub_login_widgets/filesystem.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.3.3/arthub_login_widgets/resources/arthub_white.png` & `arthub_login_widgets-0.4.0/arthub_login_widgets/resources/arthub_white.png`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.3.3/arthub_login_widgets/resources/style.qss` & `arthub_login_widgets-0.4.0/arthub_login_widgets/resources/style.qss`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-QDialog{
+#central_widget{
     background-color:rgb(68,68,68)
 }
 QLineEdit{
     color:rgb(185,185,185);
     border-radius:2px;
     border:1px solid rgb(110,110,110);
     background-color:rgb(56,56,56)
 }
 #label_prompt{
     border:0;
-    color:rgb(145,145,145);
+    color:rgb(165,165,165);
 }
 #pushButton_login{
     color:rgb(210,210,210);
     border-radius:17px;
     border:0;
     background-color:rgba(2,120,255,0.9)
 }
@@ -27,7 +27,17 @@
     background-color:transparent
 }
 #label_forgot_password:hover{
     color:rgb(137,202,255);
     background-color:transparent;
     text-decoration: underline
 }
+#label_set_account_info{
+    color:rgb(109,188,255);
+    border:0;
+    background-color:transparent
+}
+#label_set_account_info:hover{
+    color:rgb(137,202,255);
+    background-color:transparent;
+    text-decoration: underline
+}
```

### Comparing `arthub_login_widgets-0.3.3/arthub_login_widgets/test/test_core.py` & `arthub_login_widgets-0.4.0/arthub_login_widgets/test/test_core.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.3.3/arthub_login_widgets/test/test_filesystem.py` & `arthub_login_widgets-0.4.0/arthub_login_widgets/test/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.3.3/arthub_login_widgets/test/test_imports.py` & `arthub_login_widgets-0.4.0/arthub_login_widgets/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.3.3/arthub_login_widgets.egg-info/SOURCES.txt` & `arthub_login_widgets-0.4.0/arthub_login_widgets.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,12 +7,24 @@
 ./arthub_login_widgets/resources/__init__.py
 ./arthub_login_widgets/resources/arthub_white.png
 ./arthub_login_widgets/resources/style.qss
 ./arthub_login_widgets/test/__init__.py
 ./arthub_login_widgets/test/test_core.py
 ./arthub_login_widgets/test/test_filesystem.py
 ./arthub_login_widgets/test/test_imports.py
+arthub_login_widgets/__init__.py
+arthub_login_widgets/__version__.py
+arthub_login_widgets/constants.py
+arthub_login_widgets/core.py
+arthub_login_widgets/filesystem.py
 arthub_login_widgets.egg-info/PKG-INFO
 arthub_login_widgets.egg-info/SOURCES.txt
 arthub_login_widgets.egg-info/dependency_links.txt
 arthub_login_widgets.egg-info/requires.txt
-arthub_login_widgets.egg-info/top_level.txt
+arthub_login_widgets.egg-info/top_level.txt
+arthub_login_widgets/resources/__init__.py
+arthub_login_widgets/resources/arthub_white.png
+arthub_login_widgets/resources/style.qss
+arthub_login_widgets/test/__init__.py
+arthub_login_widgets/test/test_core.py
+arthub_login_widgets/test/test_filesystem.py
+arthub_login_widgets/test/test_imports.py
```

### Comparing `arthub_login_widgets-0.3.3/setup.py` & `arthub_login_widgets-0.4.0/setup.py`

 * *Files identical despite different names*

