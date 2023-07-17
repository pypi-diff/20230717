# Comparing `tmp/fastapi_amis_admin_nav-0.0.4a1.tar.gz` & `tmp/fastapi_amis_admin_nav-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_amis_admin_nav-0.0.4a1.tar", last modified: Sat Apr 15 09:28:24 2023, max compression
+gzip compressed data, was "fastapi_amis_admin_nav-0.1.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fastapi_amis_admin_nav-0.0.4a1.tar` & `fastapi_amis_admin_nav-0.1.0a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3037 2023-02-19 04:26:35.599654 fastapi_amis_admin_nav-0.0.4a1/README.md
--rw-r--r--   0        0        0      382 2023-04-15 09:28:19.081403 fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/__init__.py
--rw-r--r--   0        0        0     5168 2023-03-23 08:41:54.647360 fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/admin.py
--rw-r--r--   0        0        0     4715 2023-04-15 09:15:19.759421 fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/models.py
--rw-r--r--   0        0        0     8437 2023-03-23 11:45:23.744360 fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/utils.py
--rw-r--r--   0        0        0     1645 2023-03-22 07:48:40.603529 fastapi_amis_admin_nav-0.0.4a1/pyproject.toml
--rw-r--r--   0        0        0     4110 1970-01-01 00:00:00.000000 fastapi_amis_admin_nav-0.0.4a1/PKG-INFO
+-rw-r--r--   0        0        0     3037 2023-02-19 04:26:35.599654 fastapi_amis_admin_nav-0.1.0a1/README.md
+-rw-r--r--   0        0        0      382 2023-07-17 10:51:32.245636 fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/__init__.py
+-rw-r--r--   0        0        0     5445 2023-07-17 03:22:25.604890 fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/admin.py
+-rw-r--r--   0        0        0     5694 2023-07-17 03:36:39.135513 fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/models.py
+-rw-r--r--   0        0        0     8701 2023-07-17 02:27:22.952772 fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/utils.py
+-rw-r--r--   0        0        0     1645 2023-03-22 07:48:40.603529 fastapi_amis_admin_nav-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4110 1970-01-01 00:00:00.000000 fastapi_amis_admin_nav-0.1.0a1/PKG-INFO
```

### Comparing `fastapi_amis_admin_nav-0.0.4a1/README.md` & `fastapi_amis_admin_nav-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/admin.py` & `fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,51 +19,60 @@
     page_parser_mode = "html"  # 页面显示为iframe
     model = NavPage
     list_per_page = 100
     list_display = [
         NavPage.id,
         NavPage.label,
         NavPage.icon,
+        amis.TableColumn(
+            type="tpl",
+            label="图标预览",
+            tpl="<i class=\"cxd-Button-icon fa-2x ${icon}\"></i>",
+        ),
         NavPage.url,
         NavPage.desc,
         NavPage.visible,
         NavPage.unique_id,
+        NavPage.is_locked,
         NavPage.is_active,
         NavPage.update_time,
     ]
 
     ordering = [NavPage.parent_id, NavPage.sort.desc()]
 
     list_filter = [
         NavPage.visible,
         NavPage.is_custom,
         NavPage.is_group,
         NavPage.is_active,
+        NavPage.is_locked,
         NavPage.parent_id,
     ]
 
     create_fields = [
         NavPage.type,
         NavPage.label,
         NavPage.icon,
         NavPage.url,
         NavPage.desc,
         NavPage.visible,
-        NavPage.tabs_mode,
+        NavPage.tabsMode,
+        NavPage.is_locked,
         NavPage.page_schema,
     ]
 
     update_fields = [
         NavPage.type,
         NavPage.label,
         NavPage.icon,
         NavPage.url,
         NavPage.desc,
         NavPage.visible,
-        NavPage.tabs_mode,
+        NavPage.tabsMode,
+        NavPage.is_locked,
         NavPage.page_schema,
     ]
 
     def __init__(self, app: "AdminApp"):
         super().__init__(app)
 
         @self.site.fastapi.on_event("startup")
```

### Comparing `fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/models.py` & `fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,15 +43,33 @@
         "",
         title="页面路径",
         amis_form_item={  # 非自定义页面, 都是只读
             "disabledOn": "!this.is_custom",
         },
     )
     label: str = Field(..., title="页面名称", max_length=20)
-    icon: str = Field(default="fa fa-flash", title="页面图标", max_length=50)
+    icon: str = Field(
+        default="fa fa-flash",
+        max_length=50,
+        title="页面图标",
+        description="参考: https://fontawesome.com/",
+        amis_form_item=amis.Group(
+            name="icon",
+            body=[
+                amis.InputText(
+                    name="icon",
+                    required=True
+                ),
+                amis.Tpl(
+                    label="图标预览",
+                    tpl="<i class=\"cxd-Button-icon fa-2x ${icon}\"></i>",
+                ),
+            ],
+        )
+    )
     sort: int = Field(0, title="排序")
     desc: str = Field(default="", title="页面描述", max_length=400, amis_form_item="textarea")
     page_schema: str = Field(
         "{}",
         title="页面配置",
         sa_column=Column(Text, nullable=False),
         amis_form_item=amis.Editor(language="json"),
@@ -60,51 +78,61 @@
     parent_id: Optional[int] = Field(None, title="上级菜单", foreign_key="system_page.id")
     unique_id: str = Field(
         default_factory=lambda: str(uuid.uuid4()).replace("-", "")[:16],
         title="标识",
         max_length=40,
         unique=True,
     )
-    tabs_mode: Optional[amis.TabsModeEnum] = Field(
+    tabsMode: Optional[amis.TabsModeEnum] = Field(
         None,
         title="分组展示模式",
         description="默认为空,展示为导航菜单."
-        "其他模式参考: https://aisuda.bce.baidu.com/amis/zh-CN/components/tabs#%E5%B1%95%E7%A4%BA%E6%A8%A1%E5%BC%8F",
+                    "其他模式参考: https://aisuda.bce.baidu.com/amis/zh-CN/components/tabs#%E5%B1%95%E7%A4%BA%E6%A8%A1%E5%BC%8F",
         amis_form_item={
             "visibleOn": f"(this.is_group || this.type === {NavPageType.Group.value}) && this.type !== {NavPageType.Custom.value}"
         },
     )
     visible: bool = Field(True, title="是否可见")
     is_group: bool = Field(False, title="是否为分组")
     is_custom: bool = Field(False, title="是否自定义")
     is_active: bool = Field(True, title="是否激活")
+    is_locked: bool = Field(False, title="是否锁定", description="不锁定,则自动同步系统页面默认配置")
 
     def as_page_schema(self) -> PageSchema:
         page = PageSchema.parse_raw(self.page_schema)
         page.label = self.label or page.label
         page.icon = self.icon or page.icon
         page.url = self.url or page.url or f"/{self.unique_id}"
         page.sort = self.sort
         if self.is_group:  # 如果是分组,则同步tabsMode
-            page.tabsMode = self.tabs_mode
+            page.tabsMode = self.tabsMode
         page.visible = self.visible
         return page
 
     @classmethod
     def parse_page_schema(cls, obj: PageSchema, **kwargs):
-        data = obj.dict(include={"label", "url", "icon", "sort", "visible"})
-        data.update(
-            {
-                "page_schema": obj.amis_json(),
-                "type": parse_page_schema_type(obj),
-                "tabs_mode": obj.tabsMode,
-            }
-        )
+        data = obj.dict(include={"label", "sort"})
         data.update(kwargs)
-        return cls(**data)
+        return cls(**data).update_from_page_schema(obj)
+
+    def update_from_page_schema(self, obj: PageSchema):
+        """从PageSchema更新数据"""
+        update = False
+        for key in ("label", "icon", "url", "visible", "tabsMode"):
+            value = getattr(obj, key)
+            if value is None and key in ("visible",):
+                continue
+            if getattr(self, key) == value:
+                continue
+            setattr(self, key, value)
+            update = True
+        if update:
+            self.page_schema = obj.amis_json()
+            self.type = parse_page_schema_type(obj)
+        return self
 
     def as_nav_link(self) -> amis.Nav.Link:
         link = amis.Nav.Link(
             label=self.label,
             icon=self.icon,
             to=f"?parent_id={self.parent_id or ''}",
             children=[],
```

### Comparing `fastapi_amis_admin_nav-0.0.4a1/fastapi_amis_admin_nav/utils.py` & `fastapi_amis_admin_nav-0.1.0a1/fastapi_amis_admin_nav/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from sqlalchemy.future import select
 from sqlalchemy.orm import Session
 
 from fastapi_amis_admin_nav.models import NavPage
 
 
 class AmisPageManager:
+
     def __init__(self, session: Session):
         self.session = session
 
     @cached_property
     def db_pages(self) -> List[NavPage]:
         return self.session.scalars(select(NavPage)).all()
 
@@ -43,23 +44,27 @@
             if not admin_.page_schema:  # 如果不存在page_schema,则不保存到数据库
                 return None
             unique_id = str(admin_.unique_id)
             page = self.db_pages_uid_map.get(unique_id)
             # print('unique_id', unique_id, page)
             if page:  # 如果存在数据库中,则读取数据库中设置,并且更新到admin
                 page.is_active = True  # 设置为激活
+                if not page.is_locked:  # 判断是否锁定,如果锁定,则不更新.
+                    page.update_from_page_schema(admin_.page_schema)
                 return page.id
             # 保存到数据库
             kwargs = {
+                "label": admin_.page_schema.label,
+                "sort": admin_.page_schema.sort,
                 "parent_id": parent_id,
                 "unique_id": unique_id,
             }
             if isinstance(admin_, AdminGroup):
                 kwargs["is_group"] = True
-            new_page = NavPage.parse_page_schema(admin_.page_schema, **kwargs)
+            new_page = NavPage(**kwargs).update_from_page_schema(admin_.page_schema)
             self.session.add(new_page)
             self.session.flush()  # 刷新,获取page_id
             return new_page.id
 
         if not parent_id:  # 如果没有parent_id,则作为根节点添加到数据库中,并且获取parent_id
             if not self.site_page:
                 parent_id = append_page_to_db(admin_group)
```

### Comparing `fastapi_amis_admin_nav-0.0.4a1/pyproject.toml` & `fastapi_amis_admin_nav-0.1.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_amis_admin_nav-0.0.4a1/PKG-INFO` & `fastapi_amis_admin_nav-0.1.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_amis_admin_nav
-Version: 0.0.4a1
+Version: 0.1.0a1
 Summary: FastAPI-Amis-Admin-Nav是一个基于FastAPI-Amis-Admin并且为FastAPI-Amis-Admin提供可视化导航页面管理的拓展库.
 Keywords: fastapi,fastapi-user-auth,fastapi-amis-admin,fastapi-amis-admin-nav
 Author-email: Atomi <1456417373@qq.com>
 Maintainer-email: Atomi <1456417373@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Framework :: FastAPI
```

