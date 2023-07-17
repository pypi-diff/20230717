# Comparing `tmp/mysam_tagmanager-0.3.3-py3-none-any.whl.zip` & `tmp/mysam_tagmanager-0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,15 @@
-Zip file size: 30641 bytes, number of entries: 11
+Zip file size: 37553 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx        3 b- defN 18-Mar-12 21:11 mysam/__init__.py
--rw-rw-r--  2.0 unx     9027 b- defN 20-Apr-29 19:53 mysam/tag_const.py
--rw-r--r--  2.0 unx     3820 b- defN 21-Feb-10 18:20 mysam/tagcoder.py
--rw-rw-r--  2.0 unx     9532 b- defN 20-Apr-29 19:53 mysam/tagconfig.py
--rw-r--r--  2.0 unx    20619 b- defN 21-Feb-10 18:14 mysam/tagmaker.py
--rw-rw-r--  2.0 unx     6475 b- defN 20-Sep-03 07:48 mysam/config/tag.config
--rw-rw-r--  2.0 unx    35147 b- defN 21-Jul-03 11:02 mysam_tagmanager-0.3.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    10726 b- defN 21-Jul-03 11:02 mysam_tagmanager-0.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jul-03 11:02 mysam_tagmanager-0.3.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 21-Jul-03 11:02 mysam_tagmanager-0.3.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      882 b- defN 21-Jul-03 11:02 mysam_tagmanager-0.3.3.dist-info/RECORD
-11 files, 96329 bytes uncompressed, 29155 bytes compressed:  69.7%
+-rw-r--r--  2.0 unx     8764 b- defN 23-Jul-14 20:40 mysam/tag_const.py
+-rw-r--r--  2.0 unx    87483 b- defN 23-Jul-14 20:50 mysam/tag_const_inflect.py
+-rw-r--r--  2.0 unx     4945 b- defN 23-Jul-17 06:23 mysam/tagcoder.py
+-rw-r--r--  2.0 unx     9424 b- defN 23-Jul-13 19:20 mysam/tagconfig.py
+-rw-r--r--  2.0 unx    12941 b- defN 23-Jul-14 20:55 mysam/taginflector.py
+-rw-r--r--  2.0 unx    20971 b- defN 23-Jul-14 09:28 mysam/tagmaker.py
+-rw-rw-r--  2.0 unx     6500 b- defN 23-Jul-13 20:08 mysam/config/tag.config
+-rw-rw-r--  2.0 unx    35147 b- defN 23-Jul-17 06:36 mysam_tagmanager-0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10941 b- defN 23-Jul-17 06:36 mysam_tagmanager-0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 06:36 mysam_tagmanager-0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jul-17 06:36 mysam_tagmanager-0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1035 b- defN 23-Jul-17 06:36 mysam_tagmanager-0.4.dist-info/RECORD
+13 files, 198252 bytes uncompressed, 35841 bytes compressed:  81.9%
```

## zipnote {}

```diff
@@ -1,34 +1,40 @@
 Filename: mysam/__init__.py
 Comment: 
 
 Filename: mysam/tag_const.py
 Comment: 
 
+Filename: mysam/tag_const_inflect.py
+Comment: 
+
 Filename: mysam/tagcoder.py
 Comment: 
 
 Filename: mysam/tagconfig.py
 Comment: 
 
+Filename: mysam/taginflector.py
+Comment: 
+
 Filename: mysam/tagmaker.py
 Comment: 
 
 Filename: mysam/config/tag.config
 Comment: 
 
-Filename: mysam_tagmanager-0.3.3.dist-info/LICENSE
+Filename: mysam_tagmanager-0.4.dist-info/LICENSE
 Comment: 
 
-Filename: mysam_tagmanager-0.3.3.dist-info/METADATA
+Filename: mysam_tagmanager-0.4.dist-info/METADATA
 Comment: 
 
-Filename: mysam_tagmanager-0.3.3.dist-info/WHEEL
+Filename: mysam_tagmanager-0.4.dist-info/WHEEL
 Comment: 
 
-Filename: mysam_tagmanager-0.3.3.dist-info/top_level.txt
+Filename: mysam_tagmanager-0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mysam_tagmanager-0.3.3.dist-info/RECORD
+Filename: mysam_tagmanager-0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mysam/tag_const.py

```diff
@@ -17,20 +17,14 @@
 #  
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #  
 #  
-from __future__ import (
-    absolute_import,
-    print_function,
-    unicode_literals,
-    division,
-    )
 import os
 CONFIG_FILE = os.path.join( os.path.dirname(__file__), "config/tag.config")
 # stucture
 TAGS_CONFIG=u"""#Part;Pos;Attribute;خاصية;code;Value;قيمة;inflection;
 # Word Type نوع الكلمة
 1;1;word_type;نوع الكلمة;n;Noun;اسم;اسم;
 1;1;word_type;نوع الكلمة;V;Verb;فعل;فعل;
@@ -191,37 +185,31 @@
 , u"هما مؤ" : [u'غائب', u'مؤنث',  u'مثنى'] 
 , u"نحن" : [u'متكلم',   u'جمع']
 , u"أنتم" : [u'مخاطب', u'مذكر',  u'جمع']
 , u"أنتن" : [u'مخاطب', u'مؤنث',  u'جمع']
 , u"هم" : [u'غائب', u'مذكر',  u'جمع']
 , u"هن" : [u'غائب', u'مؤنث',  u'جمع'],
 #TENSE_FEATURES = [
-TensePast : [ u'ماضي', u'معلوم',  ],
+TensePast : [ u'ماضي', u'معلوم',  u"مبني"],
 TenseFuture : [ u'مضارع', u'معلوم', u'مرفوع',  ],
 TenseImperative : [ u'أمر', ],
 TenseConfirmedImperative : [ u'أمر',  u'مؤكذ', ],
 TenseJussiveFuture : [ u'مضارع', u'معلوم', u'مجزوم',  ],
 TenseSubjunctiveFuture : [ u'مضارع', u'معلوم', u'منصوب',  ],
 TenseConfirmedFuture : [ u'مضارع', u'معلوم',  u'مؤكد', ],
 
 
-TensePassivePast :  [ u'ماضي', u'مجهول', ],
+TensePassivePast :  [ u'ماضي', u'مجهول', u"مبني"],
 TensePassiveFuture : [ u'مضارع', u'مجهول', u'مرفوع',  ],
 TensePassiveJussiveFuture : [ u'مضارع', u'مجهول', u'مجزوم',  ],
 TensePassiveSubjunctiveFuture : [ u'مضارع', u'مجهول', u'منصوب',  ], 
 TensePassiveConfirmedFuture : [ u'مضارع', u'مجهول',  u'مؤكد', ],
 
 "Verb": [u'فعل'],
 "Noun": [u'اسم'],
 u"مفعول به": [u'ضمير متصل'],
 u"تعريف": [u'معرفة'],
 u"n": [u'لازم'],
 u"y": [u'متعدي'],
 u"مضاف": [u'ضمير متصل'],
 
 }
-
-# you must call tag_config class to load tags indexes 
-if __name__ == "__main__":
-    print("""Test ir from tag_config to load configuration
-    Call it from tagmaker
-    """)
```

## mysam/tagcoder.py

```diff
@@ -17,23 +17,17 @@
 #  
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #  
 #  
-from __future__ import (
-    absolute_import,
-    print_function,
-    unicode_literals,
-    division,
-    )
+
 import os
-# ~ if __name__ == "__main__":
-    
+   
 try:
     import tag_const 
     import tagconfig
     import tagmaker    
 except:
     from . import tag_const 
     from . import tagconfig
@@ -50,68 +44,117 @@
         tagmaker.tagMaker.__init__(self, configfile)
         self.reset()
 
     def encode(self, taglist = []):
         """Encode  a tag list into string tag.
         
         Example:
-            >>> import mysam.tagmaker as tagmaker
-            >>> tag_maker = tagmaker.tagMaker()
-            >>> taglist = [u'اسم', u'مضير متصل', u'مجرور']
-            >>> tag_maker.encode(taglist)
-            >>> tagstr = str(tag_maker)
+            >>> import mysam.tagcoder
+            >>> tag_coder = mysam.tagcoder.tagCoder()
+            >>> taglist = [u'اسم', u'ضمير متصل', u'مجرور']
+            >>> tagstr = tag_coder.encode(taglist)
             >>> print(tagstr)
-            N--;--I-;----;----
+            N--;------I;--H
         
         @param taglist: an given tag list to be coded
         @type taglist: string list
         @return: a string
         @rtype: string
         """
 
         if not taglist:
             return u""
         self.reset()            
         for tag in taglist:
             self.add(tag)
         
         return self.__str__()
+        
     def decode(self, tagstring):
         """Decode a string tag to get all tags
         Example:
-            >>> import mysam.tagcoder as tagcoder
-            >>> tag_coder = tagcoder.tagCoder()
-            >>> tagcode = 'N--;--I-;----;---'
+            >>> import mysam.tagcoder
+            >>> tag_coder = mysam.tagcoder.tagCoder()
+            >>> tagcode = 'N--;--I-;----;--H'
             >>> print(tag_coder.decode(tagcode)))
-            [(u'نوع الكلمة', u'اسم'), (u'جنس', u'لاشيء'), (u'عدد', u'لاشيء'), (u'إعراب', u'مجرور'), (u'علامة', u'لاشيء'), (u'عطف', u'لاشيء'), (u'جر', u'لاشيء'), (u'تعريف', u'نكرة'), (u'ضمير متصل', u'لاشيء'), (u'استقبال', u'لاشيء'), (u'بناء', u'لاشيء'), (u'زمن', u'لاشي
-        
+            [('نوع الكلمة', 'اسم'), ('خاصية', 'لاشيء'), ('جنس', 'لاشيء'), ('عدد', 'لاشيء'), ('شخص', 'متكلم'), ('علامة', 'لاشيء'), ('عطف', 'لاشيء'), ('استقبال', 'لاشيء'), ('ضمير متصل', 'لاشيء')]
+
         @param tagstring: a string tag to be decoded, if not given, return null
         @type tagstring: string
         @return: tag list
         @rtype: stringlist
         """
         if not tagstring:
             return ""
         else:
             return self._decode(tagstring)
         return tags
 
-            
+    def add_tag(self, tag, tagstring):
+        """ Add new tag to th tagstring code
+        Example:
+            >>> import mysam.tagcoder
+            >>> tag_coder = mysam.tagcoder.tagCoder()
+            >>> tagcode = 'V-0;M1H-faU;W--'
+            >>> tag = "ضمير متصل"
+            >>> print(tag_coder.add_tag(tag, tagcode))
+            V-0;M1H-faU;W-H
+
+
+        @param tagstring: a string tag to be decoded, if not given, return null
+        @type tagstring: string
+        @return: tag list
+        @rtype: stringlist
+        """
+        if not tagstring:
+            return ""
+        else:
+            # decode the string
+            decoded_taglist = self._decode(tagstring)
+            # extract values
+            tag_values = [v for (k,v) in decoded_taglist]
+            # add tag to tag_values
+            if tag in tag_values:
+                return tagstring
+            else:
+                tag_values.append(tag)
+                # encode
+                return self.encode(tag_values)
+
+    def remove_tag(self, tag, tagstring):
+        """ remove a tag from tagstring code
+        Example:
+            >>> import mysam.tagcoder
+            >>> tag_coder = mysam.tagcoder.tagCoder()
+            >>> tagcode = 'V-0;M1H-faU;W-H'
+            >>> tag = "ضمير متصل"
+            >>> print(tag_coder.remove_tag(tag, tagcode))
+            V-0;M1H-faU;W--
+
+
+        @param tagstring: a string tag to be decoded, if not given, return null
+        @type tagstring: string
+        @return: tag list
+        @rtype: stringlist
+        """
+        if not tagstring:
+            return ""
+        else:
+            # decode the string
+            decoded_taglist = self._decode(tagstring)
+            # extract values
+            tag_values = [v for (k,v) in decoded_taglist]
+            # add tag to tag_values
+            if not tag in tag_values:
+                return tagstring
+            else:
+                tag_values.remove(tag)
+                # encode
+                return self.encode(tag_values)
+
+
+
 if __name__ == "__main__":
-    taglists = [[u'اسم', u'هاء', u'مجرور',"مصدر"],
-                u'تعريف::مرفوع:متحرك:ينون:::'.split(":"),
-                u'المضارع المعلوم:هو:::n:'.split(":"),
-                u':مضاف:مجرور:متحرك:ينون:::'.split(':'),
-                ]
-    tag_maker = tagMaker("config/tag.config")
-
-    for taglist in taglists:
-        tag_maker.reset()
-        tag_maker.encode(taglist)
-        print(u"+".join(taglist))
-        tagstr = str(tag_maker)
-        print(tagstr)
-        # decode a unifed tag string
-        print(tag_maker.repr(tag_maker.decode()))
+    pass
```

## mysam/tagconfig.py

```diff
@@ -17,20 +17,14 @@
 #  
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #  
 #  
-from __future__ import (
-    absolute_import,
-    print_function,
-    unicode_literals,
-    division,
-    )
 try:
     from . import tag_const 
 except:
     import tag_const
     
 import re
 import codecs
```

## mysam/tagmaker.py

```diff
@@ -17,23 +17,17 @@
 #  
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, write to the Free Software
 #  Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,
 #  MA 02110-1301, USA.
 #  
 #  
-from __future__ import (
-    absolute_import,
-    print_function,
-    unicode_literals,
-    division,
-    )
 import os
 # ~ if __name__ == "__main__":
-    
+
 try:
     import tag_const 
     import tagconfig
 except:
     from . import tag_const 
     from . import tagconfig
 
@@ -77,14 +71,20 @@
             self.inverse_tagsdict  = tag_const.INVERSE_TAGSDICT 
             self.attr_tagsdict = tag_const.ATTR_TAGSDICT 
             # if structure not defined, the default structure is used.
             self.tag_parts_sizes = tag_const.TAG_PARTS_SIZES
             self.tag_parts_sep = tag_const.TAG_PARTS_SEP
             self.tagsmap = tag_const.TAGSMAP
         # prepare the tag maker
+        # inverse tag map
+        self.inverse_tagsmap = {}
+        for key in self.tagsmap:
+            newkey = "-".join(self.tagsmap[key])
+            newvalue = key
+            self.inverse_tagsmap[newkey]= newvalue
         self.reset()
 
     
     def set_config(self,configfile):
         """ set a config to encode tags"""
         configueur = tagconfig.tagConfig()
         configueur.load_config(configfile)
@@ -284,14 +284,15 @@
                     add_part = u"وهو مضاف، %s في محل جر مضاف إليه"%add_p
                     inflct.append(add_part)
             else: # no case
                 word_type = self.get_value(u'نوع الكلمة', tagstring)
                 if word_type:
                     inflct.append(word_type)  
         return u" ".join(inflct)
+        
     def inflect_verb(self, tagstring):
         """
         get inflection for a noun
         @param tagstring: a string tag to be decoded, if not given the internal tag string is decoded.
         @type tagstring: string
         @return: string
         @rtype: string
@@ -300,19 +301,25 @@
             tagstring = self.__str__()
         inflct = []
         if self.has_tag(u"فعل", tagstring):
              # inflect = Syntaxtic classe
              # مفعول به منصوب وعلامة نصبه الفتحة
              #نعت منصوب وعلامةنصبه الياء لأنه مثنى
              #مبتدأ مرفوع وعلامة رفعه الواو لأنه جمع مذكر سالم
+            # tense:
+            tense = self.get_inflect(u'زمن', tagstring)
+            voice = self.get_inflect(u'بناء', tagstring)
+            inflct.append(u"فعل") 
+            inflct.append(tense) 
+            inflct.append(voice) 
             # case
             case = self.get_inflect(u'إعراب', tagstring)
             #~ print((u"###%s####"%case), tagstring)
             if case:
-                case_part = u"فعل %s"%case
+                case_part = case
                 inflct.append(case_part)
 
                 # inflect Mark
                 mark =self.get_inflect(u'علامة', tagstring)
                 mark_value =self.get_value(u'علامة', tagstring)
                 if mark:
                     #علامة الإعراب
@@ -359,14 +366,15 @@
                 if word_type:
                     inflct.append(word_type)  
         return u" ".join(inflct)
     def inflect_tool(self, tagstring = False):
         """
         """
         return u""
+
     def inflect(self, tagstring = False):
         """
         Display inlfection in traditional way
         عرض إعراب الكلمة حسب التقاليد
         
         Example:
             >>> tag_maker = tagmaker.tagMaker()
```

## mysam/config/tag.config

```diff
@@ -69,21 +69,21 @@
 2;4;mark;علامة;I;kasratan;تنوين الكسرة;;
 2;4;mark;علامة;A;alef;الألف;الألف;
 2;4;mark;علامة;W;waw;الواو;الواو;
 2;4;mark;علامة;Y;yeh;الياء;الياء;
 2;4;mark;علامة;N;noon;ثبوت النون;ثبوت النون;
 2;4;mark;علامة;-;undef;لاشيء;;
 ## tense الزمن
-2;5;tense;زمن;p;past;ماضي;ماضي;
+2;5;tense;زمن;p;past;ماضي;ماضٍ;
 2;5;tense;زمن;f;present;مضارع;مضارع;
 2;5;tense;زمن;i;imperative;أمر;أمر;
 2;5;tense;زمن;-;undef;لاشيء;;
 
 ## Voice البناء
-2;6;voice;بناء;a;acive voice;معلوم;مبني للمعلوم;
+2;6;voice;بناء;a;acive voice;معلوم;;
 2;6;voice;بناء;p;acive voice;مجهول;مبني للمجهول;
 2;6;voice;بناء;-;undef;لاشيء;;
 
 
 
 ## Inlfection case الحالة الإعرابية
 2;7;case;إعراب;U;marfou3;مرفوع;مرفوع;
@@ -92,16 +92,16 @@
 2;7;case;إعراب;A;mansoub;منصوب;منصوب;
 2;7;case;إعراب;B;mabni;مبني;مبني;
 2;7;case;إعراب;-;undef;لاشيء;;
 2;7;case;إعراب;M;confirmed;مؤكد;مؤكد;
 
 # Procletics and prefixes
 ## Conjuction
-3;1;conjonction;عطف;W;WAW;معطوف بالواو;;
-3;1;conjonction;عطف;F;FEH;معطوف بالفاء;;
+3;1;conjonction;عطف;W;WAW;معطوف بالواو;الواو حرف عطف;
+3;1;conjonction;عطف;F;FEH;معطوف بالفاء;الفاء حرف عطف;
 3;1;conjonction;عطف;-;undef;لاشيء;;
 ## preposition
 3;2;preposition;جر;B;Beh;مجرور بالباء;باء;
 3;2;preposition;جر;K;Kaf;مجرور بالكاف;كاف;
 3;2;preposition;جر;L;Lam;مجرور باللام;لام;
 3;2;preposition;جر;-;undef;لاشيء;;
```

## Comparing `mysam_tagmanager-0.3.3.dist-info/LICENSE` & `mysam_tagmanager-0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mysam_tagmanager-0.3.3.dist-info/RECORD` & `mysam_tagmanager-0.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 mysam/__init__.py,sha256=8ZRc1sGeVrPBx4lD717BgRaQekyh78QKV9SKsdt638U,3
-mysam/tag_const.py,sha256=JRP_xxeDSo2ppFERgNKm_KlYD7vz05cmqG1EmUytQyE,9027
-mysam/tagcoder.py,sha256=h1Twbs9spw1e_5dk-itB9hDyYgKVO0Hf6MGi77mDgfg,3820
-mysam/tagconfig.py,sha256=wIG1iGjAarMspDQfhsZcazoJp2SrP5CTxq-Qt8bdYjc,9532
-mysam/tagmaker.py,sha256=q4LyUDEiQdFm_sA-V3jkNz8A9SyC3SjFQ9yXpAcdlqo,20619
-mysam/config/tag.config,sha256=iaw9Uos5N9K4Gp6EykbMVVCmwdsjGzg33zuKiRbFKnY,6475
-mysam_tagmanager-0.3.3.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
-mysam_tagmanager-0.3.3.dist-info/METADATA,sha256=r55fLP9ZbWPTsfv7whrmrQMp6Cm3TUTA--vfV5vNbow,10726
-mysam_tagmanager-0.3.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mysam_tagmanager-0.3.3.dist-info/top_level.txt,sha256=WHDShpxMJtIKPUZbG07an3-GW97GICht_6u6nvS1sso,6
-mysam_tagmanager-0.3.3.dist-info/RECORD,,
+mysam/tag_const.py,sha256=-J59SnSLPz266iI6p3OGL1gTPpax1vDZrCUhu0SE9BI,8764
+mysam/tag_const_inflect.py,sha256=fOi8Xc7PdkisrW0M4iWjXggmGEEdOwJ24NklMa7ASJ8,87483
+mysam/tagcoder.py,sha256=taqwWFRd8IV68kelCjXnNWkJdFW2wpYPF3dPUV89VLE,4945
+mysam/tagconfig.py,sha256=aDQTG1-ybXqWTYP8nze64nFs-I9TqZGgWCfT1HKowMw,9424
+mysam/taginflector.py,sha256=5X_yi45oq-7wes_GKUpkSDndZaO4KFKV9qfm3PynM_M,12941
+mysam/tagmaker.py,sha256=sFt9ns1UeaO0rs4MXxQFqz3xa2a44FqoRSdoDbKQvtI,20971
+mysam/config/tag.config,sha256=vAw-GIGy_m7QD7VyvNMM4ydDrJd1rJx3n0a_YVol6yc,6500
+mysam_tagmanager-0.4.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
+mysam_tagmanager-0.4.dist-info/METADATA,sha256=dMtOavElZru-P7aG2_7a6OzuIk-G0ud0kedCe6Sc8Fc,10941
+mysam_tagmanager-0.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mysam_tagmanager-0.4.dist-info/top_level.txt,sha256=WHDShpxMJtIKPUZbG07an3-GW97GICht_6u6nvS1sso,6
+mysam_tagmanager-0.4.dist-info/RECORD,,
```

