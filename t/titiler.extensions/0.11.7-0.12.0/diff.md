# Comparing `tmp/titiler.extensions-0.11.7.tar.gz` & `tmp/titiler.extensions-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler.extensions-0.11.7.tar", last modified: Thu May 18 16:08:14 2023, max compression
+gzip compressed data, was "titiler.extensions-0.12.0.tar", last modified: Mon Jul 17 16:06:33 2023, max compression
```

## Comparing `titiler.extensions-0.11.7.tar` & `titiler.extensions-0.12.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4700 2023-05-18 16:07:25.370668 titiler.extensions-0.11.7/README.md
--rw-r--r--   0        0        0     1656 2023-05-18 16:07:25.370668 titiler.extensions-0.11.7/pyproject.toml
--rw-r--r--   0        0        0      244 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/__init__.py
--rw-r--r--   0        0        0     1011 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/cogeo.py
--rw-r--r--   0        0        0     5274 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/stac.py
--rw-r--r--   0        0        0    30665 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/templates/cog_viewer.html
--rw-r--r--   0        0        0    35135 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/templates/stac_viewer.html
--rw-r--r--   0        0        0     2231 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/templates/wms_1.0.0.xml
--rw-r--r--   0        0        0     2715 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/templates/wms_1.1.1.xml
--rw-r--r--   0        0        0     3452 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/templates/wms_1.3.0.xml
--rw-r--r--   0        0        0     2194 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/viewer.py
--rw-r--r--   0        0        0    20787 2023-05-18 16:07:25.386668 titiler.extensions-0.11.7/titiler/extensions/wms.py
--rw-r--r--   0        0        0     5828 1970-01-01 00:00:00.000000 titiler.extensions-0.11.7/PKG-INFO
+-rw-r--r--   0        0        0     4666 2023-07-17 16:05:41.729037 titiler.extensions-0.12.0/README.md
+-rw-r--r--   0        0        0     1664 2023-07-17 16:05:41.729037 titiler.extensions-0.12.0/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-07-17 16:05:41.745038 titiler.extensions-0.12.0/titiler/extensions/__init__.py
+-rw-r--r--   0        0        0     1359 2023-07-17 16:05:41.745038 titiler.extensions-0.12.0/titiler/extensions/cogeo.py
+-rw-r--r--   0        0        0     6606 2023-07-17 16:05:41.745038 titiler.extensions-0.12.0/titiler/extensions/stac.py
+-rw-r--r--   0        0        0    30665 2023-07-17 16:05:41.745038 titiler.extensions-0.12.0/titiler/extensions/templates/cog_viewer.html
+-rw-r--r--   0        0        0    35135 2023-07-17 16:05:41.745038 titiler.extensions-0.12.0/titiler/extensions/templates/stac_viewer.html
+-rw-r--r--   0        0        0     2231 2023-07-17 16:05:41.745038 titiler.extensions-0.12.0/titiler/extensions/templates/wms_1.0.0.xml
+-rw-r--r--   0        0        0     2715 2023-07-17 16:05:41.745038 titiler.extensions-0.12.0/titiler/extensions/templates/wms_1.1.1.xml
+-rw-r--r--   0        0        0     3452 2023-07-17 16:05:41.745038 titiler.extensions-0.12.0/titiler/extensions/templates/wms_1.3.0.xml
+-rw-r--r--   0        0        0     2194 2023-07-17 16:05:41.745038 titiler.extensions-0.12.0/titiler/extensions/viewer.py
+-rw-r--r--   0        0        0    21121 2023-07-17 16:05:41.745038 titiler.extensions-0.12.0/titiler/extensions/wms.py
+-rw-r--r--   0        0        0     5794 1970-01-01 00:00:00.000000 titiler.extensions-0.12.0/PKG-INFO
```

### Comparing `titiler.extensions-0.11.7/README.md` & `titiler.extensions-0.12.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -114,35 +114,35 @@
             ),
             colormap=Depends(factory.colormap_dependency),
             render_params=Depends(factory.render_dependency),
             reader_params=Depends(factory.reader_dependency),
             env=Depends(factory.environment_dependency),
         ):
             with rasterio.Env(**env):
-                with self.reader(src_path, **reader_params) as src_dst:
-                        im = src.preview(
-                            max_size=self.max_size,
-                            **layer_params,
-                            **dataset_params,
-                        )
+                with factory.reader(src_path, **reader_params) as src:
+                    image = src.preview(
+                        max_size=self.max_size,
+                        **layer_params,
+                        **dataset_params,
+                    )
 
             if post_process:
                 image = post_process(image)
 
             if rescale:
                 image.rescale(rescale)
 
             if color_formula:
                 image.apply_color_formula(color_formula)
 
             format = ImageType.jpeg if image.mask.all() else ImageType.png
 
             content = image.render(
                 img_format=format.driver,
-                colormap=colormap or dst_colormap,
+                colormap=colormap,
                 **format.profile,
                 **render_params,
             )
 
             return Response(content, media_type=format.mediatype)
 
 # Use it
```

### Comparing `titiler.extensions-0.11.7/pyproject.toml` & `titiler.extensions-0.12.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -24,34 +24,34 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = []
 dependencies = [
-    "titiler.core==0.11.7",
+    "titiler.core==0.12.0",
 ]
-version = "0.11.7"
+version = "0.12.0"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
     "pytest-asyncio",
     "httpx",
-    "jsonschema>=3.0",
+    "jsonschema>=3.0,<4.18.0",
 ]
 cogeo = [
-    "rio-cogeo>=3.1,<4.0",
+    "rio-cogeo>=4.0,<5.0",
 ]
 stac = [
-    "rio-stac>=0.6,<0.7",
+    "rio-stac>=0.8,<0.9",
 ]
 
 [project.urls]
 Homepage = "https://developmentseed.org/titiler/"
 Documentation = "https://developmentseed.org/titiler/"
 Issues = "https://github.com/developmentseed/titiler/issues"
 Source = "https://github.com/developmentseed/titiler"
```

### Comparing `titiler.extensions-0.11.7/titiler/extensions/cogeo.py` & `titiler.extensions-0.12.0/titiler/extensions/cogeo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 """rio-cogeo Extension."""
 
+import sys
 from dataclasses import dataclass
 
 from fastapi import Depends, Query
 
 from titiler.core.factory import BaseTilerFactory, FactoryExtension
+from titiler.core.resources.responses import JSONResponse
+
+if sys.version_info >= (3, 9):
+    from typing import Annotated  # pylint: disable=no-name-in-module
+else:
+    from typing_extensions import Annotated
 
 try:
     from rio_cogeo.cogeo import cog_info
     from rio_cogeo.models import Info
 except ImportError:  # pragma: nocover
     cog_info = None  # type: ignore
     Info = None
@@ -19,16 +26,23 @@
     """Add /validate endpoint to a COG TilerFactory."""
 
     def register(self, factory: BaseTilerFactory):
         """Register endpoint to the tiler factory."""
 
         assert (
             cog_info is not None
-        ), "'rio_cogeo' must be installed to use CogValidateExtension"
+        ), "'rio-cogeo' must be installed to use CogValidateExtension"
 
-        @factory.router.get("/validate", response_model=Info)
+        @factory.router.get(
+            "/validate",
+            response_model=Info,
+            response_class=JSONResponse,
+        )
         def validate(
-            src_path: str = Depends(factory.path_dependency),
-            strict: bool = Query(False, description="Treat warnings as errors"),
+            src_path=Depends(factory.path_dependency),
+            strict: Annotated[
+                bool,
+                Query(description="Treat warnings as errors"),
+            ] = False,
         ):
             """Validate a COG"""
             return cog_info(src_path, strict=strict)
```

### Comparing `titiler.extensions-0.11.7/titiler/extensions/stac.py` & `titiler.extensions-0.12.0/titiler/extensions/stac.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 # Without it, there is no way to differentiate required and optional fields when subclassed.
 # Ref: https://github.com/pydantic/pydantic/pull/3374
 if sys.version_info < (3, 9, 2):
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
+if sys.version_info >= (3, 9):
+    from typing import Annotated  # pylint: disable=no-name-in-module
+else:
+    from typing_extensions import Annotated
+
 try:
     import pystac
     from pystac.utils import datetime_to_str, str_to_datetime
     from rio_stac.stac import create_stac_item
 except ImportError:  # pragma: nocover
     create_stac_item = None  # type: ignore
     pystac = None  # type: ignore
@@ -54,59 +59,91 @@
         ), "'rio-stac' must be installed to use stacExtension"
         assert pystac is not None, "'pystac' must be installed to use stacExtension"
 
         media = [m.value for m in pystac.MediaType] + ["auto"]
 
         @factory.router.get("/stac", response_model=Item, name="Create STAC Item")
         def create_stac(
-            src_path: str = Depends(factory.path_dependency),
-            datetime: Optional[str] = Query(
-                None,
-                description="The date and time of the assets, in UTC (e.g 2020-01-01, 2020-01-01T01:01:01).",
-            ),
-            extensions: Optional[List[str]] = Query(
-                None, description="STAC extension URL the Item implements."
-            ),
-            collection: Optional[str] = Query(
-                None, description="The Collection ID that this item belongs to."
-            ),
-            collection_url: Optional[str] = Query(
-                None, description="Link to the STAC Collection."
-            ),
+            src_path=Depends(factory.path_dependency),
+            datetime: Annotated[
+                Optional[str],
+                Query(
+                    description="The date and time of the assets, in UTC (e.g 2020-01-01, 2020-01-01T01:01:01).",
+                ),
+            ] = None,
+            extensions: Annotated[
+                Optional[List[str]],
+                Query(description="STAC extension URL the Item implements."),
+            ] = None,
+            collection: Annotated[
+                Optional[str],
+                Query(description="The Collection ID that this item belongs to."),
+            ] = None,
+            collection_url: Annotated[
+                Optional[str],
+                Query(description="Link to the STAC Collection."),
+            ] = None,
             # properties: Optional[Dict] = Query(None, description="Additional properties to add in the item."),
-            id: Optional[str] = Query(
-                None,
-                description="Id to assign to the item (default to the source basename).",
-            ),
-            asset_name: Optional[str] = Query(
-                "data", description="asset name for the source (default to 'data')."
-            ),
-            asset_roles: Optional[List[str]] = Query(
-                None, description="list of asset's roles."
-            ),
-            asset_media_type: Literal[tuple(media)] = Query(  # type: ignore
-                "auto", description="Asset's media type"
-            ),
-            asset_href: Optional[str] = Query(
-                None, description="Asset's URI (default to source's path)"
-            ),
-            with_proj: bool = Query(
-                True, description="Add the `projection` extension and properties."
-            ),
-            with_raster: bool = Query(
-                True, description="Add the `raster` extension and properties."
-            ),
-            with_eo: bool = Query(
-                True, description="Add the `eo` extension and properties."
-            ),
-            max_size: Optional[int] = Query(
-                1024,
-                gt=0,
-                description="Limit array size from which to get the raster statistics.",
-            ),
+            id: Annotated[
+                Optional[str],
+                Query(
+                    description="Id to assign to the item (default to the source basename)."
+                ),
+            ] = None,
+            asset_name: Annotated[
+                Optional[str],
+                Query(description="asset name for the source (default to 'data')."),
+            ] = "data",
+            asset_roles: Annotated[
+                Optional[List[str]],
+                Query(description="list of asset's roles."),
+            ] = None,
+            asset_media_type: Annotated[  # type: ignore
+                Optional[Literal[tuple(media)]],
+                Query(description="Asset's media type"),
+            ] = "auto",
+            asset_href: Annotated[
+                Optional[str],
+                Query(description="Asset's URI (default to source's path)"),
+            ] = None,
+            with_proj: Annotated[
+                Optional[bool],
+                Query(description="Add the `projection` extension and properties."),
+            ] = True,
+            with_raster: Annotated[
+                Optional[bool],
+                Query(description="Add the `raster` extension and properties."),
+            ] = True,
+            with_eo: Annotated[
+                Optional[bool],
+                Query(description="Add the `eo` extension and properties."),
+            ] = True,
+            max_size: Annotated[
+                Optional[int],
+                Query(
+                    gt=0,
+                    description="Limit array size from which to get the raster statistics.",
+                ),
+            ] = 1024,
+            geom_densify_pts: Annotated[
+                Optional[int],
+                Query(
+                    alias="geom-densify-pts",
+                    ge=0,
+                    description="Number of points to add to each edge to account for nonlinear edges transformation.",
+                ),
+            ] = 0,
+            geom_precision: Annotated[
+                Optional[int],
+                Query(
+                    alias="geom-precision",
+                    ge=-1,
+                    description="Round geometry coordinates to this number of decimal.",
+                ),
+            ] = -1,
         ):
             """Create STAC item."""
             properties = (
                 {}
             )  # or properties = properties or {} if we add properties in Query
 
             dt = None
@@ -134,8 +171,10 @@
                 asset_roles=asset_roles,
                 asset_media_type=asset_media_type,
                 asset_href=asset_href or src_path,
                 with_proj=with_proj,
                 with_raster=with_raster,
                 with_eo=with_eo,
                 raster_max_size=max_size,
+                geom_densify_pts=geom_densify_pts,
+                geom_precision=geom_precision,
             ).to_dict()
```

### Comparing `titiler.extensions-0.11.7/titiler/extensions/templates/cog_viewer.html` & `titiler.extensions-0.12.0/titiler/extensions/templates/cog_viewer.html`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.7/titiler/extensions/templates/stac_viewer.html` & `titiler.extensions-0.12.0/titiler/extensions/templates/stac_viewer.html`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.7/titiler/extensions/templates/wms_1.0.0.xml` & `titiler.extensions-0.12.0/titiler/extensions/templates/wms_1.0.0.xml`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.7/titiler/extensions/templates/wms_1.1.1.xml` & `titiler.extensions-0.12.0/titiler/extensions/templates/wms_1.1.1.xml`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.7/titiler/extensions/templates/wms_1.3.0.xml` & `titiler.extensions-0.12.0/titiler/extensions/templates/wms_1.3.0.xml`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.7/titiler/extensions/viewer.py` & `titiler.extensions-0.12.0/titiler/extensions/viewer.py`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.7/titiler/extensions/wms.py` & `titiler.extensions-0.12.0/titiler/extensions/wms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """wms Extension."""
 
+import sys
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional
 from urllib.parse import urlencode
 
 import jinja2
 import numpy
 import rasterio
 from fastapi import Depends, HTTPException, Query
 from rasterio.crs import CRS
@@ -16,14 +17,20 @@
 from starlette.responses import Response
 from starlette.templating import Jinja2Templates
 
 from titiler.core.dependencies import RescalingParams
 from titiler.core.factory import BaseTilerFactory, FactoryExtension
 from titiler.core.resources.enums import ImageType, MediaType
 
+if sys.version_info >= (3, 9):
+    from typing import Annotated  # pylint: disable=no-name-in-module
+else:
+    from typing_extensions import Annotated
+
+
 DEFAULT_TEMPLATES = Jinja2Templates(
     directory="",
     loader=jinja2.ChoiceLoader([jinja2.PackageLoader(__package__, "templates")]),
 )  # type:ignore
 
 
 class WMSMediaType(str, Enum):
@@ -33,27 +40,29 @@
     jp2 = "image/jp2"
     png = "image/png"
     jpeg = "image/jpeg"
     jpg = "image/jpg"
     webp = "image/webp"
 
 
+@dataclass
 class OverlayMethod(MosaicMethodBase):
     """Overlay data on top."""
 
-    def feed(self, tile):
-        """Add data to tile."""
-        if self.tile is None:
-            self.tile = tile
-
-        pidex = self.tile.mask & ~tile.mask
-
-        mask = numpy.where(pidex, tile.mask, self.tile.mask)
-        self.tile = numpy.ma.where(pidex, tile, self.tile)
-        self.tile.mask = mask
+    def feed(self, array: numpy.ma.MaskedArray):
+        """Add data to the mosaic array."""
+        if self.mosaic is None:  # type: ignore
+            self.mosaic = array
+
+        else:
+            pidex = self.mosaic.mask & ~array.mask
+
+            mask = numpy.where(pidex, array.mask, self.mosaic.mask)
+            self.mosaic = numpy.ma.where(pidex, array, self.mosaic)
+            self.mosaic.mask = mask
 
 
 @dataclass
 class wmsExtension(FactoryExtension):
     """Add /wms endpoint to a TilerFactory."""
 
     supported_crs: List[str] = field(default_factory=lambda: ["EPSG:4326"])
@@ -263,20 +272,22 @@
         )
         def wms(  # noqa: C901
             request: Request,
             # vendor (titiler) parameters
             layer_params=Depends(factory.layer_dependency),
             dataset_params=Depends(factory.dataset_dependency),
             post_process=Depends(factory.process_dependency),
-            rescale: Optional[List[Tuple[float, ...]]] = Depends(RescalingParams),
-            color_formula: Optional[str] = Query(
-                None,
-                title="Color Formula",
-                description="rio-color formula (info: https://github.com/mapbox/rio-color)",
-            ),
+            rescale=Depends(RescalingParams),
+            color_formula: Annotated[
+                Optional[str],
+                Query(
+                    title="Color Formula",
+                    description="rio-color formula (info: https://github.com/mapbox/rio-color)",
+                ),
+            ] = None,
             colormap=Depends(factory.colormap_dependency),
             reader_params=Depends(factory.reader_dependency),
             env=Depends(factory.environment_dependency),
         ):
             """Return a WMS query for a single COG.
 
             GetCapability will generate a WMS XML definition.
@@ -513,17 +524,19 @@
 
                 if rescale:
                     image.rescale(rescale)
 
                 if color_formula:
                     image.apply_color_formula(color_formula)
 
+                if colormap:
+                    image = image.apply_colormap(colormap)
+
                 content = image.render(
                     img_format=format.driver,
-                    colormap=colormap,
                     add_mask=transparent,
                     **format.profile,
                 )
 
                 return Response(content, media_type=format.mediatype)
 
             elif request_type.lower() == "getfeatureinfo":
```

### Comparing `titiler.extensions-0.11.7/PKG-INFO` & `titiler.extensions-0.12.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.extensions
-Version: 0.11.7
+Version: 0.12.0
 Summary: Extensions for TiTiler Factories.
 License: MIT
 Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile server,GDAL,Rasterio,OGC
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -140,35 +140,35 @@
             ),
             colormap=Depends(factory.colormap_dependency),
             render_params=Depends(factory.render_dependency),
             reader_params=Depends(factory.reader_dependency),
             env=Depends(factory.environment_dependency),
         ):
             with rasterio.Env(**env):
-                with self.reader(src_path, **reader_params) as src_dst:
-                        im = src.preview(
-                            max_size=self.max_size,
-                            **layer_params,
-                            **dataset_params,
-                        )
+                with factory.reader(src_path, **reader_params) as src:
+                    image = src.preview(
+                        max_size=self.max_size,
+                        **layer_params,
+                        **dataset_params,
+                    )
 
             if post_process:
                 image = post_process(image)
 
             if rescale:
                 image.rescale(rescale)
 
             if color_formula:
                 image.apply_color_formula(color_formula)
 
             format = ImageType.jpeg if image.mask.all() else ImageType.png
 
             content = image.render(
                 img_format=format.driver,
-                colormap=colormap or dst_colormap,
+                colormap=colormap,
                 **format.profile,
                 **render_params,
             )
 
             return Response(content, media_type=format.mediatype)
 
 # Use it
```

