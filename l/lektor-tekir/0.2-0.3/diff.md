# Comparing `tmp/lektor-tekir-0.2.tar.gz` & `tmp/lektor-tekir-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektor-tekir-0.2.tar", last modified: Wed Jul 12 20:08:25 2023, max compression
+gzip compressed data, was "lektor-tekir-0.3.tar", last modified: Mon Jul 17 12:00:19 2023, max compression
```

## Comparing `lektor-tekir-0.2.tar` & `lektor-tekir-0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.521859 lektor-tekir-0.2/
--rw-------   0 uyar      (1000) uyar      (1000)      179 2023-06-29 15:50:02.000000 lektor-tekir-0.2/.gitignore
--rw-------   0 uyar      (1000) uyar      (1000)      332 2023-07-12 20:07:14.000000 lektor-tekir-0.2/CHANGES.rst
--rw-------   0 uyar      (1000) uyar      (1000)     1491 2023-06-29 15:50:02.000000 lektor-tekir-0.2/LICENSE.txt
--rw-------   0 uyar      (1000) uyar      (1000)     3974 2023-07-12 20:08:25.521859 lektor-tekir-0.2/PKG-INFO
--rw-------   0 uyar      (1000) uyar      (1000)     1171 2023-07-12 17:56:26.000000 lektor-tekir-0.2/README.rst
--rw-------   0 uyar      (1000) uyar      (1000)       48 2023-06-29 15:50:02.000000 lektor-tekir-0.2/babel.cfg
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.521859 lektor-tekir-0.2/lektor_tekir/
--rw-------   0 uyar      (1000) uyar      (1000)     6612 2023-07-12 18:06:32.000000 lektor-tekir-0.2/lektor_tekir/api.py
--rw-------   0 uyar      (1000) uyar      (1000)      981 2023-07-07 10:58:40.000000 lektor-tekir-0.2/lektor_tekir/cli.py
--rw-------   0 uyar      (1000) uyar      (1000)     1374 2023-07-12 18:56:35.000000 lektor-tekir-0.2/lektor_tekir/dash.py
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.521859 lektor-tekir-0.2/lektor_tekir/static/
--rw-------   0 uyar      (1000) uyar      (1000)    42819 2023-06-29 15:51:05.000000 lektor-tekir-0.2/lektor_tekir/static/htmx.min.js
--rw-------   0 uyar      (1000) uyar      (1000)     5060 2023-07-12 18:20:59.000000 lektor-tekir-0.2/lektor_tekir/static/tekir-admin.css
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.521859 lektor-tekir-0.2/lektor_tekir/templates/
--rw-------   0 uyar      (1000) uyar      (1000)     1893 2023-07-11 09:09:41.000000 lektor-tekir-0.2/lektor_tekir/templates/tekir_base.html
--rw-------   0 uyar      (1000) uyar      (1000)      988 2023-07-11 12:27:43.000000 lektor-tekir-0.2/lektor_tekir/templates/tekir_content_edit.html
--rw-------   0 uyar      (1000) uyar      (1000)     2903 2023-07-12 18:59:22.000000 lektor-tekir-0.2/lektor_tekir/templates/tekir_contents.html
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.517859 lektor-tekir-0.2/lektor_tekir/translations/
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.517859 lektor-tekir-0.2/lektor_tekir/translations/tr/
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.521859 lektor-tekir-0.2/lektor_tekir/translations/tr/LC_MESSAGES/
--rw-------   0 uyar      (1000) uyar      (1000)     1909 2023-07-12 20:08:21.000000 lektor-tekir-0.2/lektor_tekir/translations/tr/LC_MESSAGES/messages.mo
--rw-------   0 uyar      (1000) uyar      (1000)     3936 2023-07-12 20:06:22.000000 lektor-tekir-0.2/lektor_tekir/translations/tr/LC_MESSAGES/messages.po
-drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-12 20:08:25.521859 lektor-tekir-0.2/lektor_tekir.egg-info/
--rw-------   0 uyar      (1000) uyar      (1000)     3974 2023-07-12 20:08:25.000000 lektor-tekir-0.2/lektor_tekir.egg-info/PKG-INFO
--rw-------   0 uyar      (1000) uyar      (1000)      675 2023-07-12 20:08:25.000000 lektor-tekir-0.2/lektor_tekir.egg-info/SOURCES.txt
--rw-------   0 uyar      (1000) uyar      (1000)        1 2023-07-12 20:08:25.000000 lektor-tekir-0.2/lektor_tekir.egg-info/dependency_links.txt
--rw-------   0 uyar      (1000) uyar      (1000)       55 2023-07-12 20:08:25.000000 lektor-tekir-0.2/lektor_tekir.egg-info/entry_points.txt
--rw-------   0 uyar      (1000) uyar      (1000)       82 2023-07-12 20:08:25.000000 lektor-tekir-0.2/lektor_tekir.egg-info/requires.txt
--rw-------   0 uyar      (1000) uyar      (1000)       13 2023-07-12 20:08:25.000000 lektor-tekir-0.2/lektor_tekir.egg-info/top_level.txt
--rw-------   0 uyar      (1000) uyar      (1000)     3445 2023-07-12 20:06:12.000000 lektor-tekir-0.2/messages.pot
--rw-------   0 uyar      (1000) uyar      (1000)     2047 2023-07-12 20:08:16.000000 lektor-tekir-0.2/pyproject.toml
--rw-------   0 uyar      (1000) uyar      (1000)       93 2023-07-12 20:08:25.521859 lektor-tekir-0.2/setup.cfg
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-17 12:00:19.428551 lektor-tekir-0.3/
+-rw-------   0 uyar      (1000) uyar      (1000)      179 2023-06-29 15:50:02.000000 lektor-tekir-0.3/.gitignore
+-rw-------   0 uyar      (1000) uyar      (1000)      454 2023-07-17 11:59:47.000000 lektor-tekir-0.3/CHANGES.rst
+-rw-------   0 uyar      (1000) uyar      (1000)     1491 2023-06-29 15:50:02.000000 lektor-tekir-0.3/LICENSE.txt
+-rw-------   0 uyar      (1000) uyar      (1000)     3974 2023-07-17 12:00:19.428551 lektor-tekir-0.3/PKG-INFO
+-rw-------   0 uyar      (1000) uyar      (1000)     1171 2023-07-12 22:12:48.000000 lektor-tekir-0.3/README.rst
+-rw-------   0 uyar      (1000) uyar      (1000)       48 2023-06-29 15:50:02.000000 lektor-tekir-0.3/babel.cfg
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-17 12:00:19.424551 lektor-tekir-0.3/lektor_tekir/
+-rw-------   0 uyar      (1000) uyar      (1000)     9233 2023-07-17 11:46:12.000000 lektor-tekir-0.3/lektor_tekir/api.py
+-rw-------   0 uyar      (1000) uyar      (1000)      981 2023-07-07 10:58:40.000000 lektor-tekir-0.3/lektor_tekir/cli.py
+-rw-------   0 uyar      (1000) uyar      (1000)     1859 2023-07-17 11:45:31.000000 lektor-tekir-0.3/lektor_tekir/dash.py
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-17 12:00:19.424551 lektor-tekir-0.3/lektor_tekir/static/
+-rw-------   0 uyar      (1000) uyar      (1000)    42819 2023-06-29 15:51:05.000000 lektor-tekir-0.3/lektor_tekir/static/htmx.min.js
+-rw-------   0 uyar      (1000) uyar      (1000)     5100 2023-07-17 11:40:00.000000 lektor-tekir-0.3/lektor_tekir/static/tekir-admin.css
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-17 12:00:19.424551 lektor-tekir-0.3/lektor_tekir/templates/
+-rw-------   0 uyar      (1000) uyar      (1000)     1893 2023-07-11 09:09:41.000000 lektor-tekir-0.3/lektor_tekir/templates/tekir_base.html
+-rw-------   0 uyar      (1000) uyar      (1000)     1311 2023-07-14 20:08:39.000000 lektor-tekir-0.3/lektor_tekir/templates/tekir_content_edit.html
+-rw-------   0 uyar      (1000) uyar      (1000)     4818 2023-07-17 09:54:30.000000 lektor-tekir-0.3/lektor_tekir/templates/tekir_contents.html
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-17 12:00:19.420551 lektor-tekir-0.3/lektor_tekir/translations/
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-17 12:00:19.420551 lektor-tekir-0.3/lektor_tekir/translations/tr/
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-17 12:00:19.424551 lektor-tekir-0.3/lektor_tekir/translations/tr/LC_MESSAGES/
+-rw-------   0 uyar      (1000) uyar      (1000)     2252 2023-07-17 12:00:14.000000 lektor-tekir-0.3/lektor_tekir/translations/tr/LC_MESSAGES/messages.mo
+-rw-------   0 uyar      (1000) uyar      (1000)     5221 2023-07-17 11:47:14.000000 lektor-tekir-0.3/lektor_tekir/translations/tr/LC_MESSAGES/messages.po
+drwx------   0 uyar      (1000) uyar      (1000)        0 2023-07-17 12:00:19.424551 lektor-tekir-0.3/lektor_tekir.egg-info/
+-rw-------   0 uyar      (1000) uyar      (1000)     3974 2023-07-17 12:00:19.000000 lektor-tekir-0.3/lektor_tekir.egg-info/PKG-INFO
+-rw-------   0 uyar      (1000) uyar      (1000)      675 2023-07-17 12:00:19.000000 lektor-tekir-0.3/lektor_tekir.egg-info/SOURCES.txt
+-rw-------   0 uyar      (1000) uyar      (1000)        1 2023-07-17 12:00:19.000000 lektor-tekir-0.3/lektor_tekir.egg-info/dependency_links.txt
+-rw-------   0 uyar      (1000) uyar      (1000)       55 2023-07-17 12:00:19.000000 lektor-tekir-0.3/lektor_tekir.egg-info/entry_points.txt
+-rw-------   0 uyar      (1000) uyar      (1000)       97 2023-07-17 12:00:19.000000 lektor-tekir-0.3/lektor_tekir.egg-info/requires.txt
+-rw-------   0 uyar      (1000) uyar      (1000)       13 2023-07-17 12:00:19.000000 lektor-tekir-0.3/lektor_tekir.egg-info/top_level.txt
+-rw-------   0 uyar      (1000) uyar      (1000)     4562 2023-07-17 11:47:13.000000 lektor-tekir-0.3/messages.pot
+-rw-------   0 uyar      (1000) uyar      (1000)     2065 2023-07-17 11:59:57.000000 lektor-tekir-0.3/pyproject.toml
+-rw-------   0 uyar      (1000) uyar      (1000)       93 2023-07-17 12:00:19.428551 lektor-tekir-0.3/setup.cfg
```

### Comparing `lektor-tekir-0.2/LICENSE.txt` & `lektor-tekir-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lektor-tekir-0.2/PKG-INFO` & `lektor-tekir-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lektor-tekir
-Version: 0.2
+Version: 0.3
 Summary: An alternative admin panel for Lektor.
 Author-email: "H. Turgut Uyar" <uyar@tekir.org>
 License: Copyright 2023 H. Turgut Uyar <uyar@tekir.org>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -61,22 +61,22 @@
 It doesn't modify existing behavior, but only adds new routes
 for the new panel.
 
 What -sort of- works, hopefully:
 
 - Navigating existing content.
 - Editing existing content.
+- Adding new content.
 - Deleting content.
 - Deleting attachments.
 - Multiple language support in the UI (English and Turkish at the moment).
 - Light/dark mode toggle.
 
 What's planned in the short term:
 
-- Adding new content.
 - Adding attachments.
 - Editing system fields.
 - Dividing edit form fields into tabs.
 - Deploying the site.
 - Supporting Git.
 - Managing content translations.
 - TinyMCE, Quill or some other editor integration.
```

### Comparing `lektor-tekir-0.2/README.rst` & `lektor-tekir-0.3/README.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 It doesn't modify existing behavior, but only adds new routes
 for the new panel.
 
 What -sort of- works, hopefully:
 
 - Navigating existing content.
 - Editing existing content.
+- Adding new content.
 - Deleting content.
 - Deleting attachments.
 - Multiple language support in the UI (English and Turkish at the moment).
 - Light/dark mode toggle.
 
 What's planned in the short term:
 
-- Adding new content.
 - Adding attachments.
 - Editing system fields.
 - Dividing edit form fields into tabs.
 - Deploying the site.
 - Supporting Git.
 - Managing content translations.
 - TinyMCE, Quill or some other editor integration.
```

### Comparing `lektor-tekir-0.2/lektor_tekir/cli.py` & `lektor-tekir-0.3/lektor_tekir/cli.py`

 * *Files identical despite different names*

### Comparing `lektor-tekir-0.2/lektor_tekir/static/htmx.min.js` & `lektor-tekir-0.3/lektor_tekir/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `lektor-tekir-0.2/lektor_tekir/static/tekir-admin.css` & `lektor-tekir-0.3/lektor_tekir/static/tekir-admin.css`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 body {
   display: grid;
   grid-template-areas:
     ".         main-header"
     "main-tabs main-content";
   grid-template-columns: 10em 1fr;
   grid-template-rows: auto 1fr;
-  min-height: 100vh;
+  height: 100dvh;
 }
 
 #main-header {
   grid-area: main-header;
 }
 
 #main-tabs {
@@ -223,22 +223,22 @@
 
 details {
   margin: 1em 0;
 }
 
 /* CUSTOM */
 
-#tekir-page-count {
-  max-width: min(20em, 50%);
-  border-bottom: 1px solid;
+button img {
+  display: inline;
+  height: 1em;
+  margin-inline-start: 1em;
 }
 
-#tekir-page-count h2 {
-  margin-block-end: 0.25rem;
-  font-size: 1.2em;
+#tekir-page-count {
+  max-width: min(20em, 50%);
 }
 
 #tekir-page-count p {
   font-size: 2.5em;
 }
 
 #tekir-breadcrumbs {
@@ -264,25 +264,30 @@
 
 #tekir-breadcrumbs li:not(:first-child)::before {
   content: "» ";
 }
 
 #tekir-contents {
   display: grid;
-  gap: 3rem 2rem;
+  gap: 1rem 3rem;
   grid-template-areas:
     "contents-summary  contents-summary"
     "contents-subpages contents-attachments";
-  grid-template-columns: 1fr 1fr;
+  grid-template-columns: 2fr 1fr;
 }
 
 #tekir-summary {
   grid-area: contents-summary;
 }
 
+.content-listing {
+  height: 15em;
+  overflow-y: auto;
+}
+
 #tekir-subpages {
   grid-area: contents-subpages;
 }
 
 #tekir-attachments {
   grid-area: contents-attachments;
 }
@@ -356,14 +361,15 @@
 @media (prefers-color-scheme: dark) {
   :root {
     --color-bg: var(--color-bg-dark);
     --color-text: var(--color-text-dark);
     --color-link: var(--color-link-dark);
   }
 
+  dialog,
   input {
     color-scheme: dark;
   }
 
   select option {
     background-color: var(--color-bg);
   }
```

### Comparing `lektor-tekir-0.2/lektor_tekir/templates/tekir_base.html` & `lektor-tekir-0.3/lektor_tekir/templates/tekir_base.html`

 * *Files identical despite different names*

### Comparing `lektor-tekir-0.2/lektor_tekir/templates/tekir_content_edit.html` & `lektor-tekir-0.3/lektor_tekir/templates/tekir_content_edit.html`

 * *Files 11% similar despite different names*

```diff
@@ -20,8 +20,16 @@
   </dialog>
 
   <dialog id="changes-dialog">
     <p id="changes-result"></p>
     <button id="changes-continue">{{ _('Continue') }}</button>
     <button id="changes-cancel">{{ _('Cancel') }}</button>
   </dialog>
+
+  <dialog id="navigate-dialog">
+    <div class="field">
+      <select id="navigables" name="path" hx-get="{{ url_for('tekir_admin_api.navigables', lang=g.lang_code) }}"></select>
+    </div>
+    <button id="navigate-select">{{ _('Select') }}</button>
+    <button id="navigate-cancel">{{ _('Cancel') }}</button>
+  </dialog>
 {% endblock %}
```

### Comparing `lektor-tekir-0.2/lektor_tekir/translations/tr/LC_MESSAGES/messages.mo` & `lektor-tekir-0.3/lektor_tekir/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-07-12 23:06+0300\n"
+"POT-Creation-Date: 2023-07-17 14:47+0300\n"
 "PO-Revision-Date: 2023-06-25 21:11+0300\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: tr\n"
 "Language-Team: tr <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -18,23 +18,32 @@
 
 msgid "Admin Panel"
 msgstr "Yönetim Paneli"
 
 msgid "Attachments"
 msgstr "Ekler"
 
+msgid "Build"
+msgstr "Üret"
+
 msgid "Cancel"
 msgstr "Vazgeç"
 
+msgid "Clean"
+msgstr "Temizle"
+
 msgid "Close"
 msgstr "Kapat"
 
 msgid "Content"
 msgstr "İçerik"
 
+msgid "Content Type"
+msgstr "İçerik Tipi"
+
 msgid "Content saved."
 msgstr "İçerik kaydedildi."
 
 msgid "Continue"
 msgstr "Devam et"
 
 msgid "Delete"
@@ -54,29 +63,47 @@
 
 msgid "Edit"
 msgstr "Düzenle"
 
 msgid "File name"
 msgstr "Dosya adı"
 
+msgid "Folder:"
+msgstr "Klasör:"
+
+msgid "ID"
+msgstr "Kimlik"
+
 msgid "Move down"
 msgstr "Aşağı"
 
 msgid "Move up"
 msgstr "Yukarı"
 
+msgid "No attachments."
+msgstr "Ek yok."
+
 msgid "No changes."
 msgstr "Değişiklik yok."
 
+msgid "No output"
+msgstr "Çıktı yok"
+
+msgid "No subpages."
+msgstr "Altsayfa yok."
+
 msgid "No, cancel"
 msgstr "Hayır, vazgeç"
 
 msgid "Number of Pages"
 msgstr "Sayfa Sayısı"
 
+msgid "Output"
+msgstr "Çıktı"
+
 msgid "Save"
 msgstr "Kaydet"
 
 msgid "Select"
 msgstr "Seç"
 
 msgid "Subpages"
@@ -87,14 +114,17 @@
 
 msgid "There are unsaved changes. Do you want to continue?"
 msgstr "Kaydedilmemiş değişiklikler var. Devam etmek istiyor musunuz?"
 
 msgid "This operation will delete the following content items:"
 msgstr "Bu işlem aşağıdaki içerik unsurlarını silecek:"
 
+msgid "Time:"
+msgstr "Zaman:"
+
 msgid "Title"
 msgstr "Başlık"
 
 msgid "Toggle dark mode"
 msgstr "Karanlık moda geç"
 
 msgid "Toggle light mode"
```

### Comparing `lektor-tekir-0.2/lektor_tekir/translations/tr/LC_MESSAGES/messages.po` & `lektor-tekir-0.3/lektor_tekir/translations/tr/LC_MESSAGES/messages.po`

 * *Files 22% similar despite different names*

```diff
@@ -3,38 +3,47 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-07-12 23:06+0300\n"
+"POT-Creation-Date: 2023-07-17 14:47+0300\n"
 "PO-Revision-Date: 2023-06-25 21:11+0300\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: tr\n"
 "Language-Team: tr <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: lektor_tekir/api.py:117
+#: lektor_tekir/api.py:37 lektor_tekir/api.py:52 lektor_tekir/dash.py:37
+msgid "No output"
+msgstr "Çıktı yok"
+
+#: lektor_tekir/api.py:62 lektor_tekir/templates/tekir_contents.html:8
+#: lektor_tekir/templates/tekir_contents.html:10
+msgid "home"
+msgstr "ana sayfa"
+
+#: lektor_tekir/api.py:159
 msgid "No changes."
 msgstr "Değişiklik yok."
 
-#: lektor_tekir/api.py:120
+#: lektor_tekir/api.py:162
 msgid "Content saved."
 msgstr "İçerik kaydedildi."
 
-#: lektor_tekir/api.py:137
+#: lektor_tekir/api.py:178
 msgid "There are unsaved changes. Do you want to continue?"
 msgstr "Kaydedilmemiş değişiklikler var. Devam etmek istiyor musunuz?"
 
-#: lektor_tekir/api.py:175
+#: lektor_tekir/api.py:216
 msgid "Deleted."
 msgstr "Silindi."
 
 #: lektor_tekir/templates/tekir_base.html:6
 #: lektor_tekir/templates/tekir_base.html:14
 msgid "Admin Panel"
 msgstr "Yönetim Paneli"
@@ -72,89 +81,132 @@
 msgstr "Kapat"
 
 #: lektor_tekir/templates/tekir_content_edit.html:24
 msgid "Continue"
 msgstr "Devam et"
 
 #: lektor_tekir/templates/tekir_content_edit.html:25
+#: lektor_tekir/templates/tekir_content_edit.html:33
+#: lektor_tekir/templates/tekir_contents.html:133
 msgid "Cancel"
 msgstr "Vazgeç"
 
+#: lektor_tekir/templates/tekir_content_edit.html:32
+#: lektor_tekir/templates/tekir_contents.html:28
+#: lektor_tekir/templates/tekir_contents.html:65
+msgid "Select"
+msgstr "Seç"
+
 #: lektor_tekir/templates/tekir_contents.html:5
 msgid "You are here:"
 msgstr "Buradasınız:"
 
-#: lektor_tekir/templates/tekir_contents.html:8
-#: lektor_tekir/templates/tekir_contents.html:10
-msgid "home"
-msgstr "ana sayfa"
-
 #: lektor_tekir/templates/tekir_contents.html:17
 msgid "Edit"
 msgstr "Düzenle"
 
 #: lektor_tekir/templates/tekir_contents.html:21
 msgid "Subpages"
 msgstr "Altsayfalar"
 
-#: lektor_tekir/templates/tekir_contents.html:27
-#: lektor_tekir/templates/tekir_contents.html:55
-msgid "Select"
-msgstr "Seç"
-
-#: lektor_tekir/templates/tekir_contents.html:28
-msgid "Title"
-msgstr "Başlık"
-
 #: lektor_tekir/templates/tekir_contents.html:29
+#: lektor_tekir/templates/tekir_contents.html:128
+msgid "ID"
+msgstr "Kimlik"
+
+#: lektor_tekir/templates/tekir_contents.html:30
 msgid "Type"
 msgstr "Tip"
 
-#: lektor_tekir/templates/tekir_contents.html:43
-#: lektor_tekir/templates/tekir_contents.html:69
+#: lektor_tekir/templates/tekir_contents.html:46
+#: lektor_tekir/templates/tekir_contents.html:80
 msgid "Delete selected items"
 msgstr "Seçilenleri sil"
 
 #: lektor_tekir/templates/tekir_contents.html:49
+msgid "No subpages."
+msgstr "Altsayfa yok."
+
+#: lektor_tekir/templates/tekir_contents.html:53
+#: lektor_tekir/templates/tekir_contents.html:132
+#: lektor_tekir/templates/tekir_fields.html:56
+msgid "Add"
+msgstr "Ekle"
+
+#: lektor_tekir/templates/tekir_contents.html:58
 msgid "Attachments"
 msgstr "Ekler"
 
-#: lektor_tekir/templates/tekir_contents.html:56
+#: lektor_tekir/templates/tekir_contents.html:66
 msgid "File name"
 msgstr "Dosya adı"
 
-#: lektor_tekir/templates/tekir_contents.html:76
+#: lektor_tekir/templates/tekir_contents.html:83
+msgid "No attachments."
+msgstr "Ek yok."
+
+#: lektor_tekir/templates/tekir_contents.html:91
 msgid "This operation will delete the following content items:"
 msgstr "Bu işlem aşağıdaki içerik unsurlarını silecek:"
 
-#: lektor_tekir/templates/tekir_contents.html:78
+#: lektor_tekir/templates/tekir_contents.html:93
 msgid "Do you want to continue?"
 msgstr "Devam etmek istiyor musunuz?"
 
-#: lektor_tekir/templates/tekir_contents.html:79
+#: lektor_tekir/templates/tekir_contents.html:94
 msgid "Yes, delete"
 msgstr "Evet, sil"
 
-#: lektor_tekir/templates/tekir_contents.html:80
+#: lektor_tekir/templates/tekir_contents.html:95
 msgid "No, cancel"
 msgstr "Hayır, vazgeç"
 
-#: lektor_tekir/templates/tekir_fields.html:47
-msgid "Add"
-msgstr "Ekle"
+#: lektor_tekir/templates/tekir_contents.html:101
+msgid "Content Type"
+msgstr "İçerik Tipi"
 
-#: lektor_tekir/templates/tekir_fields.html:64
+#: lektor_tekir/templates/tekir_contents.html:120
+msgid "Title"
+msgstr "Başlık"
+
+#: lektor_tekir/templates/tekir_fields.html:73
 msgid "Delete"
 msgstr "Sil"
 
-#: lektor_tekir/templates/tekir_fields.html:65
+#: lektor_tekir/templates/tekir_fields.html:74
 msgid "Move up"
 msgstr "Yukarı"
 
-#: lektor_tekir/templates/tekir_fields.html:66
+#: lektor_tekir/templates/tekir_fields.html:75
 msgid "Move down"
 msgstr "Aşağı"
 
-#: lektor_tekir/templates/tekir_summary.html:4
+#: lektor_tekir/templates/tekir_summary.html:5
 msgid "Number of Pages"
 msgstr "Sayfa Sayısı"
 
+#: lektor_tekir/templates/tekir_summary.html:10
+msgid "Output"
+msgstr "Çıktı"
+
+#: lektor_tekir/templates/tekir_summary.html:12
+msgid "Folder:"
+msgstr "Klasör:"
+
+#: lektor_tekir/templates/tekir_summary.html:13
+msgid "Time:"
+msgstr "Zaman:"
+
+#: lektor_tekir/templates/tekir_summary.html:17
+msgid "Clean"
+msgstr "Temizle"
+
+#: lektor_tekir/templates/tekir_summary.html:22
+msgid "Build"
+msgstr "Üret"
+
+#~ msgid "Cleaned"
+#~ msgstr "Temizlendi"
+
+#~ msgid "Built"
+#~ msgstr "Üretildi"
+
```

### Comparing `lektor-tekir-0.2/lektor_tekir.egg-info/PKG-INFO` & `lektor-tekir-0.3/lektor_tekir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lektor-tekir
-Version: 0.2
+Version: 0.3
 Summary: An alternative admin panel for Lektor.
 Author-email: "H. Turgut Uyar" <uyar@tekir.org>
 License: Copyright 2023 H. Turgut Uyar <uyar@tekir.org>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -61,22 +61,22 @@
 It doesn't modify existing behavior, but only adds new routes
 for the new panel.
 
 What -sort of- works, hopefully:
 
 - Navigating existing content.
 - Editing existing content.
+- Adding new content.
 - Deleting content.
 - Deleting attachments.
 - Multiple language support in the UI (English and Turkish at the moment).
 - Light/dark mode toggle.
 
 What's planned in the short term:
 
-- Adding new content.
 - Adding attachments.
 - Editing system fields.
 - Dividing edit form fields into tabs.
 - Deploying the site.
 - Supporting Git.
 - Managing content translations.
 - TinyMCE, Quill or some other editor integration.
```

### Comparing `lektor-tekir-0.2/lektor_tekir.egg-info/SOURCES.txt` & `lektor-tekir-0.3/lektor_tekir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lektor-tekir-0.2/messages.pot` & `lektor-tekir-0.3/messages.pot`

 * *Files 17% similar despite different names*

```diff
@@ -4,36 +4,45 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-07-12 23:06+0300\n"
+"POT-Creation-Date: 2023-07-17 14:47+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: lektor_tekir/api.py:117
+#: lektor_tekir/api.py:37 lektor_tekir/api.py:52 lektor_tekir/dash.py:37
+msgid "No output"
+msgstr ""
+
+#: lektor_tekir/api.py:62 lektor_tekir/templates/tekir_contents.html:8
+#: lektor_tekir/templates/tekir_contents.html:10
+msgid "home"
+msgstr ""
+
+#: lektor_tekir/api.py:159
 msgid "No changes."
 msgstr ""
 
-#: lektor_tekir/api.py:120
+#: lektor_tekir/api.py:162
 msgid "Content saved."
 msgstr ""
 
-#: lektor_tekir/api.py:137
+#: lektor_tekir/api.py:178
 msgid "There are unsaved changes. Do you want to continue?"
 msgstr ""
 
-#: lektor_tekir/api.py:175
+#: lektor_tekir/api.py:216
 msgid "Deleted."
 msgstr ""
 
 #: lektor_tekir/templates/tekir_base.html:6
 #: lektor_tekir/templates/tekir_base.html:14
 msgid "Admin Panel"
 msgstr ""
@@ -71,89 +80,126 @@
 msgstr ""
 
 #: lektor_tekir/templates/tekir_content_edit.html:24
 msgid "Continue"
 msgstr ""
 
 #: lektor_tekir/templates/tekir_content_edit.html:25
+#: lektor_tekir/templates/tekir_content_edit.html:33
+#: lektor_tekir/templates/tekir_contents.html:133
 msgid "Cancel"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:5
-msgid "You are here:"
+#: lektor_tekir/templates/tekir_content_edit.html:32
+#: lektor_tekir/templates/tekir_contents.html:28
+#: lektor_tekir/templates/tekir_contents.html:65
+msgid "Select"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:8
-#: lektor_tekir/templates/tekir_contents.html:10
-msgid "home"
+#: lektor_tekir/templates/tekir_contents.html:5
+msgid "You are here:"
 msgstr ""
 
 #: lektor_tekir/templates/tekir_contents.html:17
 msgid "Edit"
 msgstr ""
 
 #: lektor_tekir/templates/tekir_contents.html:21
 msgid "Subpages"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:27
-#: lektor_tekir/templates/tekir_contents.html:55
-msgid "Select"
-msgstr ""
-
-#: lektor_tekir/templates/tekir_contents.html:28
-msgid "Title"
+#: lektor_tekir/templates/tekir_contents.html:29
+#: lektor_tekir/templates/tekir_contents.html:128
+msgid "ID"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:29
+#: lektor_tekir/templates/tekir_contents.html:30
 msgid "Type"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:43
-#: lektor_tekir/templates/tekir_contents.html:69
+#: lektor_tekir/templates/tekir_contents.html:46
+#: lektor_tekir/templates/tekir_contents.html:80
 msgid "Delete selected items"
 msgstr ""
 
 #: lektor_tekir/templates/tekir_contents.html:49
+msgid "No subpages."
+msgstr ""
+
+#: lektor_tekir/templates/tekir_contents.html:53
+#: lektor_tekir/templates/tekir_contents.html:132
+#: lektor_tekir/templates/tekir_fields.html:56
+msgid "Add"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_contents.html:58
 msgid "Attachments"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:56
+#: lektor_tekir/templates/tekir_contents.html:66
 msgid "File name"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:76
+#: lektor_tekir/templates/tekir_contents.html:83
+msgid "No attachments."
+msgstr ""
+
+#: lektor_tekir/templates/tekir_contents.html:91
 msgid "This operation will delete the following content items:"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:78
+#: lektor_tekir/templates/tekir_contents.html:93
 msgid "Do you want to continue?"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:79
+#: lektor_tekir/templates/tekir_contents.html:94
 msgid "Yes, delete"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_contents.html:80
+#: lektor_tekir/templates/tekir_contents.html:95
 msgid "No, cancel"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_fields.html:47
-msgid "Add"
+#: lektor_tekir/templates/tekir_contents.html:101
+msgid "Content Type"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_contents.html:120
+msgid "Title"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_fields.html:64
+#: lektor_tekir/templates/tekir_fields.html:73
 msgid "Delete"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_fields.html:65
+#: lektor_tekir/templates/tekir_fields.html:74
 msgid "Move up"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_fields.html:66
+#: lektor_tekir/templates/tekir_fields.html:75
 msgid "Move down"
 msgstr ""
 
-#: lektor_tekir/templates/tekir_summary.html:4
+#: lektor_tekir/templates/tekir_summary.html:5
 msgid "Number of Pages"
 msgstr ""
 
+#: lektor_tekir/templates/tekir_summary.html:10
+msgid "Output"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_summary.html:12
+msgid "Folder:"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_summary.html:13
+msgid "Time:"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_summary.html:17
+msgid "Clean"
+msgstr ""
+
+#: lektor_tekir/templates/tekir_summary.html:22
+msgid "Build"
+msgstr ""
+
```

### Comparing `lektor-tekir-0.2/pyproject.toml` & `lektor-tekir-0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lektor-tekir"
-version = "0.2"
+version = "0.3"
 description = "An alternative admin panel for Lektor."
 readme = "README.rst"
 
 authors = [{name = "H. Turgut Uyar", email = "uyar@tekir.org"}]
 license = {file = "LICENSE.txt"}
 
 keywords = ["lektor", "cms"]
@@ -24,15 +24,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet",
     "Topic :: Internet :: WWW/HTTP :: Site Management",
 ]
 
 requires-python = "~=3.8"
-dependencies = ["lektor", "flask-babel"]
+dependencies = ["lektor", "python-slugify", "flask-babel"]
 
 [project.optional-dependencies]
 style = ["ruff"]
 dev = [
     "lektor-tekir[style]",
     "babel",
     "build",
```

