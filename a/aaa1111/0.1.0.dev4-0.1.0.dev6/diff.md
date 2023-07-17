# Comparing `tmp/aaa1111-0.1.0.dev4.tar.gz` & `tmp/aaa1111-0.1.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aaa1111-0.1.0.dev4.tar", last modified: Fri Jul 14 13:10:42 2023, max compression
+gzip compressed data, was "aaa1111-0.1.0.dev6.tar", last modified: Mon Jul 17 14:54:34 2023, max compression
```

## Comparing `aaa1111-0.1.0.dev4.tar` & `aaa1111-0.1.0.dev6.tar`

### file list

```diff
@@ -1,16 +1,31 @@
--rw-r--r--   0        0        0     1083 2023-07-13 05:37:34.132225 aaa1111-0.1.0.dev4/LICENSE
--rw-r--r--   0        0        0       88 2023-07-13 15:33:45.322313 aaa1111-0.1.0.dev4/README.md
--rw-r--r--   0        0        0        0 2023-07-13 05:44:31.695257 aaa1111-0.1.0.dev4/aaa1111/__init__.py
--rw-r--r--   0        0        0     6235 2023-07-14 12:34:58.164236 aaa1111-0.1.0.dev4/aaa1111/__main__.py
--rw-r--r--   0        0        0       28 2023-07-14 07:05:38.542707 aaa1111-0.1.0.dev4/aaa1111/__version__.py
--rw-r--r--   0        0        0       52 2023-07-14 05:41:34.045117 aaa1111-0.1.0.dev4/aaa1111/client/__init__.py
--rw-r--r--   0        0        0     3435 2023-07-14 07:07:50.741981 aaa1111-0.1.0.dev4/aaa1111/client/extras.py
--rw-r--r--   0        0        0     3461 2023-07-14 07:08:57.775642 aaa1111-0.1.0.dev4/aaa1111/client/main.py
--rw-r--r--   0        0        0     3387 2023-07-14 06:19:38.538109 aaa1111-0.1.0.dev4/aaa1111/client/toimg.py
--rw-r--r--   0        0        0      386 2023-07-14 06:13:53.739597 aaa1111-0.1.0.dev4/aaa1111/types/__init__.py
--rw-r--r--   0        0        0      427 2023-07-14 12:29:28.450074 aaa1111-0.1.0.dev4/aaa1111/types/base.py
--rw-r--r--   0        0        0     1980 2023-07-14 07:08:09.213639 aaa1111-0.1.0.dev4/aaa1111/types/extras.py
--rw-r--r--   0        0        0     3547 2023-07-14 06:13:46.741195 aaa1111-0.1.0.dev4/aaa1111/types/toimg.py
--rw-r--r--   0        0        0     4724 2023-07-14 12:31:45.041606 aaa1111-0.1.0.dev4/aaa1111/utils.py
--rw-r--r--   0        0        0     1186 2023-07-14 13:10:42.713395 aaa1111-0.1.0.dev4/pyproject.toml
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 aaa1111-0.1.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-13 05:37:34.132225 aaa1111-0.1.0.dev6/LICENSE
+-rw-r--r--   0        0        0       88 2023-07-13 15:33:45.322313 aaa1111-0.1.0.dev6/README.md
+-rw-r--r--   0        0        0       61 2023-07-16 11:12:17.652504 aaa1111-0.1.0.dev6/aaa1111/__init__.py
+-rw-r--r--   0        0        0     6232 2023-07-16 05:29:53.454992 aaa1111-0.1.0.dev6/aaa1111/__main__.py
+-rw-r--r--   0        0        0       28 2023-07-17 12:55:33.157432 aaa1111-0.1.0.dev6/aaa1111/__version__.py
+-rw-r--r--   0        0        0       52 2023-07-14 05:41:34.045117 aaa1111-0.1.0.dev6/aaa1111/client/__init__.py
+-rw-r--r--   0        0        0     2073 2023-07-17 02:54:36.587173 aaa1111-0.1.0.dev6/aaa1111/client/action.py
+-rw-r--r--   0        0        0     3442 2023-07-16 09:11:37.426730 aaa1111-0.1.0.dev6/aaa1111/client/extras.py
+-rw-r--r--   0        0        0     9458 2023-07-16 10:50:01.709231 aaa1111-0.1.0.dev6/aaa1111/client/info.py
+-rw-r--r--   0        0        0     2678 2023-07-17 14:42:44.488541 aaa1111-0.1.0.dev6/aaa1111/client/main.py
+-rw-r--r--   0        0        0      853 2023-07-17 12:19:06.015859 aaa1111-0.1.0.dev6/aaa1111/client/options.py
+-rw-r--r--   0        0        0     5946 2023-07-17 03:32:55.702077 aaa1111-0.1.0.dev6/aaa1111/client/toimg.py
+-rw-r--r--   0        0        0      368 2023-07-16 11:44:07.758916 aaa1111-0.1.0.dev6/aaa1111/types/__init__.py
+-rw-r--r--   0        0        0      587 2023-07-16 09:12:58.603870 aaa1111-0.1.0.dev6/aaa1111/types/base.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:42:28.785881 aaa1111-0.1.0.dev6/aaa1111/types/extension/__init__.py
+-rw-r--r--   0        0        0     1782 2023-07-16 13:38:52.293106 aaa1111-0.1.0.dev6/aaa1111/types/extension/controlnet.py
+-rw-r--r--   0        0        0     2384 2023-07-16 13:38:24.656274 aaa1111-0.1.0.dev6/aaa1111/types/extension/lora_block_weight.py
+-rw-r--r--   0        0        0      306 2023-07-16 13:14:51.579466 aaa1111-0.1.0.dev6/aaa1111/types/extension/misc.py
+-rw-r--r--   0        0        0     1950 2023-07-16 09:12:58.605870 aaa1111-0.1.0.dev6/aaa1111/types/extras.py
+-rw-r--r--   0        0        0     2811 2023-07-16 11:02:56.779986 aaa1111-0.1.0.dev6/aaa1111/types/info.py
+-rw-r--r--   0        0        0     5493 2023-07-17 03:04:40.400483 aaa1111-0.1.0.dev6/aaa1111/types/toimg.py
+-rw-r--r--   0        0        0     5579 2023-07-17 14:00:36.489658 aaa1111-0.1.0.dev6/aaa1111/utils.py
+-rw-r--r--   0        0        0     1230 2023-07-17 14:54:34.930184 aaa1111-0.1.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0      731 2023-07-17 14:27:53.688121 aaa1111-0.1.0.dev6/tests/conftest.py
+-rw-r--r--   0        0        0   573492 2023-07-14 12:24:42.631826 aaa1111-0.1.0.dev6/tests/image/test1.png
+-rw-r--r--   0        0        0   466758 2023-07-17 13:52:38.641903 aaa1111-0.1.0.dev6/tests/image/test2.webp
+-rw-r--r--   0        0        0   132490 2023-07-17 13:53:50.814172 aaa1111-0.1.0.dev6/tests/image/test3.jpg
+-rw-r--r--   0        0        0      349 2023-07-17 14:30:35.485475 aaa1111-0.1.0.dev6/tests/test_action.py
+-rw-r--r--   0        0        0     3833 2023-07-17 14:53:06.259898 aaa1111-0.1.0.dev6/tests/test_info.py
+-rw-r--r--   0        0        0     1165 2023-07-17 14:50:26.087051 aaa1111-0.1.0.dev6/tests/test_misc.py
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 aaa1111-0.1.0.dev6/PKG-INFO
```

### Comparing `aaa1111-0.1.0.dev4/LICENSE` & `aaa1111-0.1.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev4/aaa1111/__main__.py` & `aaa1111-0.1.0.dev6/aaa1111/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 from rich.panel import Panel
 from rich.syntax import Syntax
 from ruamel.yaml import YAML
 from typer import Argument, Option, Typer
 from typing_extensions import Annotated
 
 from aaa1111.client import AAA1111
-from aaa1111.utils import load_dict_file, save_image
+from aaa1111.utils import FILE_EXT, load_from_file, save_image
 
 app_txt2img = Typer()
 app_img2img = Typer()
 
 
 defalut_output = Path("output")
 
 
 @app_txt2img.command(no_args_is_help=True)
 def txt2img(
     params: Annotated[
         List[Path],
         Argument(
             show_default=False,
-            help="Path to params files. .toml, .yaml, .yml, .json available. others will be ignored.",
+            help="Path to params files. .toml, .yaml, .yml, .json, .json5 available. others will be ignored.",
             exists=True,
             rich_help_panel="api",
         ),
     ],
     save_dir: Annotated[
         Path,
         Option(
@@ -81,15 +81,15 @@
 
 @app_img2img.command(no_args_is_help=True)
 def img2img(
     params: Annotated[
         List[Path],
         Argument(
             show_default=False,
-            help="Path to params files. .toml, .yaml, .yml, .json available. others will be ignored.",
+            help="Path to params files. .toml, .yaml, .yml, .json, .json5 available. others will be ignored.",
             exists=True,
             rich_help_panel="api",
         ),
     ],
     save_dir: Annotated[
         Path,
         Option(
@@ -164,15 +164,15 @@
         pg.TimeRemainingColumn(),
         pg.TextColumn("[progress.percentage]{task.percentage:>3.0f}%"),
     )
     pg_task = progress.add_task(task, total=length)
 
     with Live(progress) as live:
         for i in range(length):
-            payload = load_dict_file(params[i])
+            payload = load_from_file(params[i])
             panel = Panel(
                 Syntax(format_payload(payload), "yaml", theme="ansi_dark"),
                 title=f"{task} [green]{i + 1}/{length}[/green]",
             )
             live.update(Group(progress, panel))
 
             if task == "txt2img":
@@ -190,23 +190,23 @@
                     infotext = infotexts[j]
                 else:
                     infotext = None
 
                 save_image(image, save_dir, infotext, save_ext, quality, lossless)
 
             progress.update(pg_task, advance=1)
-            live.refresh()
+
+        live.update(progress)
 
 
 def format_payload(payload: Dict[str, Any]) -> str:
     stream = io.StringIO()
     YAML().dump(payload, stream)
     return stream.getvalue().strip()
 
 
 def filter_paths(paths: List[Path]) -> List[Path]:
-    ext = [".yaml", ".yml", ".json", ".toml"]
-    return [p for p in paths if p.is_file() and p.suffix in ext]
+    return [p for p in paths if p.is_file() and p.suffix.lower() in FILE_EXT]
 
 
 if __name__ == "__main__":
     app_txt2img()
```

### Comparing `aaa1111-0.1.0.dev4/aaa1111/client/extras.py` & `aaa1111-0.1.0.dev6/aaa1111/client/extras.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC
 from pathlib import Path
 from typing import Any, Mapping, Optional, Union
 
 from beartype import beartype
 from httpx import AsyncClient, Client
 
-from aaa1111.types import (
+from aaa1111.types.extras import (
     ExtrasBatchImages,
     ExtrasBatchImagesResponse,
     ExtrasSingleImage,
     ExtrasSingleImageResponse,
 )
 from aaa1111.utils import (
     aimage_to_base64,
```

### Comparing `aaa1111-0.1.0.dev4/aaa1111/client/main.py` & `aaa1111-0.1.0.dev6/aaa1111/client/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import asyncio
 import platform
-from dataclasses import asdict, is_dataclass
 from pathlib import Path
-from typing import Any, Dict, Mapping, Optional, Union
+from typing import Any, Mapping, Optional, Union
 
 from beartype import beartype
-from httpx import AsyncClient, BasicAuth, Client
+from httpx import URL, AsyncClient, BasicAuth, Client, Timeout
 
-from aaa1111.utils import aload_dict_file, load_dict_file
+from aaa1111.utils import load_from_file
 
+from .action import ActionMixin
 from .extras import ExtrasMixin
+from .info import InfoMixin
+from .options import OptionsMixin
 from .toimg import ToImageMixin
 
 if platform.system() == "Windows":
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
 
 @beartype
-class AAA1111(ExtrasMixin, ToImageMixin):
+class AAA1111(OptionsMixin, InfoMixin, ActionMixin, ExtrasMixin, ToImageMixin):
     def __init__(
         self,
         host: str = "127.0.0.1",
         port: int = 7860,
         base_url: Optional[str] = None,
         https: bool = False,
         username: Union[str, bytes, None] = None,
@@ -32,15 +34,15 @@
         if base_url is None:
             pre = "https" if https else "http"
             init_base_url = f"{pre}://{host}:{port}"
         else:
             init_base_url = base_url
 
         if isinstance(defaults, (str, Path)):
-            self.defaults = load_dict_file(defaults)
+            self.defaults = load_from_file(defaults)
         else:
             self.defaults = defaults or {}
 
         auth = BasicAuth(username, password) if username else None
         kwargs = {
             "auth": auth,
             "follow_redirects": True,
@@ -64,44 +66,23 @@
             loop = None
         if loop and loop.is_running():
             loop.create_task(self.aclient.aclose())
         else:
             asyncio.run(self.aclient.aclose())
 
     @property
-    def base_url(self):
+    def base_url(self) -> URL:
         return self.client.base_url
 
     @base_url.setter
-    def base_url(self, url: str):
+    def base_url(self, url: Union[str, URL]):
         self.client.base_url = url
         self.aclient.base_url = url
 
-    @staticmethod
-    def _get_payload(payload: Any) -> Dict[str, Any]:
-        if hasattr(payload, "asdict"):
-            return payload.asdict()
-        if is_dataclass(payload):
-            return asdict(payload)
-        if isinstance(payload, (str, Path)):
-            return load_dict_file(payload)
-        if isinstance(payload, dict):
-            return payload
-        if isinstance(payload, Mapping):
-            return dict(payload)
-        msg = f"Unsupported payload type: {type(payload)}"
-        raise ValueError(msg)
-
-    @staticmethod
-    async def _aget_payload(payload: Any) -> Dict[str, Any]:
-        if hasattr(payload, "asdict"):
-            return payload.asdict()
-        if is_dataclass(payload):
-            return asdict(payload)
-        if isinstance(payload, (str, Path)):
-            return await aload_dict_file(payload)
-        if isinstance(payload, dict):
-            return payload
-        if isinstance(payload, Mapping):
-            return dict(payload)
-        msg = f"Unsupported payload type: {type(payload)}"
-        raise ValueError(msg)
+    @property
+    def timeout(self) -> Timeout:
+        return self.client.timeout
+
+    @timeout.setter
+    def timeout(self, timeout: Any):
+        self.client.timeout = timeout
+        self.aclient.timeout = timeout
```

### Comparing `aaa1111-0.1.0.dev4/aaa1111/types/extras.py` & `aaa1111-0.1.0.dev6/aaa1111/types/extras.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from dataclasses import dataclass, field
 from enum import IntEnum
 from pathlib import Path
-from typing import List, Literal, Union
+from typing import List, Literal, Optional, Union
 
 from beartype import beartype
 from PIL import Image
 
 from aaa1111.utils import base64_to_image
 
-from .base import AsdictMixin
-
-Number = Union[int, float]
+from .base import AsdictMixin, ImageType, Number, PathType
 
 
 class ResizeMode(IntEnum):
     Scale_by = 0
     Scale_to = 1
 
 
@@ -37,25 +35,25 @@
 
     ResizeMode = ResizeMode
 
 
 @beartype
 @dataclass
 class ExtrasSingleImage(ExtraBase):
-    image: Union[str, Path, Image.Image, None] = None
+    image: Optional[ImageType] = None
 
 
 @beartype
 @dataclass
 class FileData:
-    data: Union[str, Path, Image.Image]
+    data: ImageType
     name: str = ""  # never used (v1.4.1)
 
     def __post_init__(self):
-        if isinstance(self.data, (str, Path)) and not self.name:
+        if not self.name and isinstance(self.data, PathType):
             self.name = Path(self.data).name
 
 
 @beartype
 @dataclass
 class ExtrasBatchImages(ExtraBase):
     imageList: List[FileData] = field(default_factory=list)  # noqa: N815
```

### Comparing `aaa1111-0.1.0.dev4/aaa1111/utils.py` & `aaa1111-0.1.0.dev6/aaa1111/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,156 +1,177 @@
 import base64
 import io
 from pathlib import Path
 from typing import Any, Dict, Mapping, Optional, Sequence, Union
 
-import filetype
 import orjson
+import pyjson5
 import rtoml
 from aiofile import async_open
 from PIL import Image, PngImagePlugin
 from ruamel.yaml import YAML
 from ulid import ULID
 
-Image_Type = Union[str, Path, Image.Image]
-DICT_EXT = (".toml", ".yaml", ".yml", ".json")
+ImageType = Union[str, Path, Image.Image]  # prevent circular import
+PathType = Union[str, Path]
 
+FILE_EXT = (".toml", ".yaml", ".yml", ".json", ".json5")
+available_extensions = Image.registered_extensions()
 
-def image_to_base64(img: Image_Type) -> str:
+
+def image_to_base64(img: ImageType) -> str:
     if isinstance(img, Image.Image):
-        buffer = io.BytesIO()
-        img.save(buffer)
-        value = buffer.getvalue()
+        buf = io.BytesIO()
+        # 1. png
+        if "parameters" in img.info:
+            pnginfo = PngImagePlugin.PngInfo()
+            pnginfo.add_text("parameters", img.info["parameters"])
+            img.save(buf, format="png", pnginfo=pnginfo)
+        # 2. else
+        else:
+            img.save(buf, format="webp", lossless=True, exif=img.getexif())
+        value = buf.getvalue()
     else:
         if isinstance(img, str) and not Path(img).is_file():
             # expect img is base64 string
             return img
         with open(img, "rb") as f:
             value = f.read()
     return base64.b64encode(value).decode("utf-8")
 
 
-async def aimage_to_base64(img: Image_Type) -> str:
+async def aimage_to_base64(img: ImageType) -> str:
     if isinstance(img, Image.Image):
-        buffer = io.BytesIO()
-        img.save(buffer)
-        value = buffer.getvalue()
+        buf = io.BytesIO()
+        # 1. png
+        if "parameters" in img.info:
+            pnginfo = PngImagePlugin.PngInfo()
+            pnginfo.add_text("parameters", img.info["parameters"])
+            img.save(buf, format="png", pnginfo=pnginfo)
+        # 2. else
+        else:
+            img.save(buf, format="webp", lossless=True, exif=img.getexif())
+        value = buf.getvalue()
     else:
         if isinstance(img, str) and not Path(img).is_file():
             # expect img is base64 string
             return img
         async with async_open(img, "rb") as f:
             value = await f.read()
     return base64.b64encode(value).decode("utf-8")
 
 
 def base64_to_image(s: str) -> Image.Image:
     return Image.open(io.BytesIO(base64.b64decode(s)))
 
 
-def is_image_file(obj: Any) -> bool:
-    if isinstance(obj, (str, Path)) and Path(obj).is_file():
-        return filetype.image_match(obj) is not None
-    return False
+def is_image(obj: Any) -> bool:
+    if isinstance(obj, (str, Path)) and (p := Path(obj)).is_file():
+        return p.suffix.lower() in available_extensions
+    return isinstance(obj, Image.Image)
 
 
 def _recursive_read_image(item: Any):
     if not isinstance(item, str) and isinstance(item, Sequence):
         return [
-            image_to_base64(v) if is_image_file(v) else _recursive_read_image(v)
+            image_to_base64(v) if is_image(v) else _recursive_read_image(v)
             for v in item
         ]
     if isinstance(item, Mapping):
         return {
-            k: image_to_base64(v) if is_image_file(v) else _recursive_read_image(v)
+            k: image_to_base64(v) if is_image(v) else _recursive_read_image(v)
             for k, v in item.items()
         }
     return item
 
 
 def recursive_read_image(item: Mapping[str, Any]) -> Dict[str, Any]:
     return _recursive_read_image(item)
 
 
 async def _arecursive_read_image(item: Any):
     if not isinstance(item, str) and isinstance(item, Sequence):
         return [
             (await aimage_to_base64(v))
-            if is_image_file(v)
+            if is_image(v)
             else (await _arecursive_read_image(v))
             for v in item
         ]
     if isinstance(item, Mapping):
         return {
             k: (await aimage_to_base64(v))
-            if is_image_file(v)
+            if is_image(v)
             else (await _arecursive_read_image(v))
             for k, v in item.items()
         }
     return item
 
 
 async def arecursive_read_image(item: Mapping[str, Any]) -> Dict[str, Any]:
     return await _arecursive_read_image(item)
 
 
-def is_valid_dict_file(file: Union[str, Path]) -> bool:
-    ext = Path(file).suffix
-    return ext in DICT_EXT
+def is_valid_file(file: PathType) -> bool:
+    ext = Path(file).suffix.lower()
+    return ext in FILE_EXT
 
 
-def load_dict_file(file: Union[str, Path]) -> Dict[str, Any]:
-    if not is_valid_dict_file(file):
+def load_from_file(file: PathType) -> Dict[str, Any]:
+    if not is_valid_file(file):
         msg = f"Unsupported file extension: {file!r}"
         raise ValueError(msg)
-    ext = Path(file).suffix
+    ext = Path(file).suffix.lower()
 
     with open(file, encoding="utf-8") as raw:
         if ext == ".toml":
             return rtoml.load(raw)
         if ext == ".json":
             return orjson.loads(raw.read())
-        yaml = YAML()
-        return dict(yaml.load(raw))
+        if ext == ".json5":
+            return pyjson5.decode_io(raw)
+        return dict(YAML().load(raw))
 
 
-async def aload_dict_file(file: Union[str, Path]) -> Dict[str, Any]:
-    if not is_valid_dict_file(file):
+async def aload_from_file(file: PathType) -> Dict[str, Any]:
+    if not is_valid_file(file):
         msg = f"Unsupported file extension: {file!r}"
         raise ValueError(msg)
-    ext = Path(file).suffix
+    ext = Path(file).suffix.lower()
 
     async with async_open(file, encoding="utf-8") as raw:
         data = await raw.read()
         if ext == ".toml":
             return rtoml.loads(data)
         if ext == ".json":
             return orjson.loads(data)
-        yaml = YAML()
-        return dict(yaml.load(data))
+        if ext == ".json5":
+            return pyjson5.decode(data)
+        return dict(YAML().load(data))
 
 
 def save_image(
     image: Image.Image,
     save_dir: Path,
     infotext: Optional[str] = None,
     ext: str = "png",
     quality: int = 95,
     lossless: bool = True,
-):
+) -> Path:
     if not ext.startswith("."):
         ext = "." + ext
     path = save_dir.joinpath(str(ULID())).with_suffix(ext)
+
     if not infotext:
         image.save(path, quality=quality, lossless=lossless)
-        return
 
-    if ext.lower().endswith("png"):
+    elif ext.lower().endswith("png"):
         pnginfo = PngImagePlugin.PngInfo()
         pnginfo.add_text("parameters", infotext)
         image.save(path, pnginfo=pnginfo, quality=quality)
-        return
 
-    exif = image.getexif()
-    # https://github.com/python-pillow/Pillow/issues/4935#issuecomment-698027721
-    exif[0x9286] = infotext
-    image.save(path, quality=quality, lossless=lossless, exif=exif)
+    else:
+        exif = image.getexif()
+        # https://github.com/python-pillow/Pillow/issues/4935#issuecomment-698027721
+        exif[0x9286] = infotext
+        image.save(path, quality=quality, lossless=lossless, exif=exif)
+
+    return path
```

### Comparing `aaa1111-0.1.0.dev4/pyproject.toml` & `aaa1111-0.1.0.dev6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 description = "An Api for Automatic1111"
 authors = [
     { name = "Bingsu", email = "ks2515@naver.com" },
 ]
 dependencies = [
     "httpx",
     "aiofile",
-    "pillow",
+    "pillow>=9.4.0",
     "orjson",
     "rtoml",
     "ruamel.yaml",
-    "asyncer",
+    "pyjson5",
     "beartype",
-    "filetype",
     "typing-extensions",
     "python-ulid",
     "rich",
-    "typer",
+    "typer>=0.9.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dynamic = []
-version = "0.1.0.dev4"
+version = "0.1.0.dev6"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/Bing-su/AAA1111"
 
@@ -43,14 +42,18 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "black",
     "ruff",
     "pre-commit",
     "ipywidgets",
 ]
+test = [
+    "pytest",
+    "python-dotenv",
+]
 
 [tool.pdm.version]
 source = "file"
 path = "aaa1111/__version__.py"
 
 [tool.ruff]
 select = [
```

### Comparing `aaa1111-0.1.0.dev4/PKG-INFO` & `aaa1111-0.1.0.dev6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: aaa1111
-Version: 0.1.0.dev4
+Version: 0.1.0.dev6
 Summary: An Api for Automatic1111
 Author-Email: Bingsu <ks2515@naver.com>
 License: MIT
 Project-URL: Repository, https://github.com/Bing-su/AAA1111
 Requires-Python: >=3.8
 Requires-Dist: httpx
 Requires-Dist: aiofile
-Requires-Dist: pillow
+Requires-Dist: pillow>=9.4.0
 Requires-Dist: orjson
 Requires-Dist: rtoml
 Requires-Dist: ruamel.yaml
-Requires-Dist: asyncer
+Requires-Dist: pyjson5
 Requires-Dist: beartype
-Requires-Dist: filetype
 Requires-Dist: typing-extensions
 Requires-Dist: python-ulid
 Requires-Dist: rich
-Requires-Dist: typer
+Requires-Dist: typer>=0.9.0
 Description-Content-Type: text/markdown
 
 # AAA1111
 
 An Api for Automatic1111
 
 CLI로 이미지를 만들어보는 시험작
```

