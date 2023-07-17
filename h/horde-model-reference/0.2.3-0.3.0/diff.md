# Comparing `tmp/horde_model_reference-0.2.3-py3-none-any.whl.zip` & `tmp/horde_model_reference-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,34 +1,24 @@
-Zip file size: 88122 bytes, number of entries: 32
--rw-rw-rw-  2.0 fat      760 b- defN 23-Jun-12 20:15 horde_model_reference/__init__.py
--rw-rw-rw-  2.0 fat     1121 b- defN 23-Jun-05 23:50 horde_model_reference/blip.json
--rw-rw-rw-  2.0 fat     2545 b- defN 23-Jun-05 23:50 horde_model_reference/clip.json
--rw-rw-rw-  2.0 fat      676 b- defN 23-Jun-05 23:50 horde_model_reference/codeformer.json
--rw-rw-rw-  2.0 fat    11397 b- defN 23-Jun-05 23:50 horde_model_reference/controlnet.json
--rw-rw-rw-  2.0 fat     4230 b- defN 23-Jun-05 23:50 horde_model_reference/esrgan.json
--rw-rw-rw-  2.0 fat     1358 b- defN 23-Jun-05 23:50 horde_model_reference/gfpgan.json
--rw-rw-rw-  2.0 fat     2254 b- defN 23-Jun-05 23:50 horde_model_reference/meta_consts.py
--rw-rw-rw-  2.0 fat     6149 b- defN 23-Jun-21 19:14 horde_model_reference/model_reference_records.py
--rw-rw-rw-  2.0 fat     4201 b- defN 23-Jun-22 12:22 horde_model_reference/path_consts.py
--rw-rw-rw-  2.0 fat     1329 b- defN 23-Jun-05 23:50 horde_model_reference/safety_checker.json
--rw-rw-rw-  2.0 fat   191369 b- defN 23-Jun-05 23:50 horde_model_reference/stable_diffusion.json
--rw-rw-rw-  2.0 fat      500 b- defN 23-Jun-05 21:44 horde_model_reference/util.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 21:44 horde_model_reference/embeddings/hypernetworks/add_hypernetworks_here.txt
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 21:44 horde_model_reference/embeddings/lora/add_loras_here.txt
+Zip file size: 49913 bytes, number of entries: 22
+-rw-rw-rw-  2.0 fat      760 b- defN 23-Jul-14 14:58 horde_model_reference/__init__.py
+-rw-rw-rw-  2.0 fat     2143 b- defN 23-Jul-17 17:46 horde_model_reference/meta_consts.py
+-rw-rw-rw-  2.0 fat     6691 b- defN 23-Jul-17 17:46 horde_model_reference/model_reference_records.py
+-rw-rw-rw-  2.0 fat     4201 b- defN 23-Jul-17 17:47 horde_model_reference/path_consts.py
+-rw-rw-rw-  2.0 fat      471 b- defN 23-Jul-17 17:46 horde_model_reference/util.py
 -rw-rw-rw-  2.0 fat      879 b- defN 23-Jun-05 23:50 horde_model_reference/legacy/README.md
 -rw-rw-rw-  2.0 fat      221 b- defN 23-Jun-05 23:50 horde_model_reference/legacy/__init__.py
--rw-rw-rw-  2.0 fat    14178 b- defN 23-Jun-21 19:52 horde_model_reference/legacy/add_to_legacy_sd.py
--rw-rw-rw-  2.0 fat     1999 b- defN 23-Jun-21 19:57 horde_model_reference/legacy/convert_all_legacy_dbs.py
--rw-rw-rw-  2.0 fat     3450 b- defN 23-Jun-25 20:29 horde_model_reference/legacy/download_live_legacy_dbs.py
--rw-rw-rw-  2.0 fat     3420 b- defN 23-Jun-21 19:57 horde_model_reference/legacy/validate_sd.py
+-rw-rw-rw-  2.0 fat    14307 b- defN 23-Jul-17 17:46 horde_model_reference/legacy/add_to_legacy_sd.py
+-rw-rw-rw-  2.0 fat     1999 b- defN 23-Jul-17 17:46 horde_model_reference/legacy/convert_all_legacy_dbs.py
+-rw-rw-rw-  2.0 fat     3450 b- defN 23-Jul-14 17:19 horde_model_reference/legacy/download_live_legacy_dbs.py
+-rw-rw-rw-  2.0 fat     3613 b- defN 23-Jul-17 17:46 horde_model_reference/legacy/validate_sd.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 21:44 horde_model_reference/legacy/classes/__init__.py
--rw-rw-rw-  2.0 fat    32660 b- defN 23-Jun-21 20:33 horde_model_reference/legacy/classes/legacy_converters.py
--rw-rw-rw-  2.0 fat     2061 b- defN 23-Jun-21 01:43 horde_model_reference/legacy/classes/raw_legacy_model_database_records.py
--rw-rw-rw-  2.0 fat     4397 b- defN 23-Jun-21 19:13 horde_model_reference/legacy/classes/staging_model_database_records.py
+-rw-rw-rw-  2.0 fat    32829 b- defN 23-Jul-17 17:46 horde_model_reference/legacy/classes/legacy_converters.py
+-rw-rw-rw-  2.0 fat     1475 b- defN 23-Jul-17 17:46 horde_model_reference/legacy/classes/raw_legacy_model_database_records.py
+-rw-rw-rw-  2.0 fat     4099 b- defN 23-Jul-17 17:46 horde_model_reference/legacy/classes/staging_model_database_records.py
 -rw-rw-rw-  2.0 fat     1430 b- defN 23-Jun-22 12:21 horde_model_reference/showcase/README.md
--rw-rw-rw-  2.0 fat    35184 b- defN 23-Jun-25 20:33 horde_model_reference-0.2.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    44597 b- defN 23-Jun-25 20:33 horde_model_reference-0.2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-25 20:33 horde_model_reference-0.2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       85 b- defN 23-Jun-25 20:33 horde_model_reference-0.2.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       22 b- defN 23-Jun-25 20:33 horde_model_reference-0.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     3204 b- defN 23-Jun-25 20:33 horde_model_reference-0.2.3.dist-info/RECORD
-32 files, 375768 bytes uncompressed, 82774 bytes compressed:  78.0%
+-rw-rw-rw-  2.0 fat    35184 b- defN 23-Jul-17 17:48 horde_model_reference-0.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    44644 b- defN 23-Jul-17 17:48 horde_model_reference-0.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 17:48 horde_model_reference-0.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       85 b- defN 23-Jul-17 17:48 horde_model_reference-0.3.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       22 b- defN 23-Jul-17 17:48 horde_model_reference-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2223 b- defN 23-Jul-17 17:48 horde_model_reference-0.3.0.dist-info/RECORD
+22 files, 160818 bytes uncompressed, 46155 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -1,52 +1,22 @@
 Filename: horde_model_reference/__init__.py
 Comment: 
 
-Filename: horde_model_reference/blip.json
-Comment: 
-
-Filename: horde_model_reference/clip.json
-Comment: 
-
-Filename: horde_model_reference/codeformer.json
-Comment: 
-
-Filename: horde_model_reference/controlnet.json
-Comment: 
-
-Filename: horde_model_reference/esrgan.json
-Comment: 
-
-Filename: horde_model_reference/gfpgan.json
-Comment: 
-
 Filename: horde_model_reference/meta_consts.py
 Comment: 
 
 Filename: horde_model_reference/model_reference_records.py
 Comment: 
 
 Filename: horde_model_reference/path_consts.py
 Comment: 
 
-Filename: horde_model_reference/safety_checker.json
-Comment: 
-
-Filename: horde_model_reference/stable_diffusion.json
-Comment: 
-
 Filename: horde_model_reference/util.py
 Comment: 
 
-Filename: horde_model_reference/embeddings/hypernetworks/add_hypernetworks_here.txt
-Comment: 
-
-Filename: horde_model_reference/embeddings/lora/add_loras_here.txt
-Comment: 
-
 Filename: horde_model_reference/legacy/README.md
 Comment: 
 
 Filename: horde_model_reference/legacy/__init__.py
 Comment: 
 
 Filename: horde_model_reference/legacy/add_to_legacy_sd.py
@@ -72,26 +42,26 @@
 
 Filename: horde_model_reference/legacy/classes/staging_model_database_records.py
 Comment: 
 
 Filename: horde_model_reference/showcase/README.md
 Comment: 
 
-Filename: horde_model_reference-0.2.3.dist-info/LICENSE
+Filename: horde_model_reference-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: horde_model_reference-0.2.3.dist-info/METADATA
+Filename: horde_model_reference-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: horde_model_reference-0.2.3.dist-info/WHEEL
+Filename: horde_model_reference-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: horde_model_reference-0.2.3.dist-info/entry_points.txt
+Filename: horde_model_reference-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: horde_model_reference-0.2.3.dist-info/top_level.txt
+Filename: horde_model_reference-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: horde_model_reference-0.2.3.dist-info/RECORD
+Filename: horde_model_reference-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## horde_model_reference/meta_consts.py

```diff
@@ -1,19 +1,21 @@
-from enum import Enum
+from enum import auto
 
+from strenum import StrEnum
 
-class MODEL_STYLES(str, Enum):
+
+class MODEL_STYLES(StrEnum):
     """An enum of all the model styles."""
 
-    generalist = "generalist"
-    anime = "anime"
-    furry = "furry"
-    artistic = "artistic"
-    other = "other"
-    realistic = "realistic"
+    generalist = auto()
+    anime = auto()
+    furry = auto()
+    artistic = auto()
+    other = auto()
+    realistic = auto()
 
 
 KNOWN_TAGS = [
     "anime",
     "manga",
     "cyberpunk",
     "tv show",
@@ -30,55 +32,55 @@
     "comic",
     "cartoon",
     "painting",
     "game",
 ]
 
 
-class MODEL_REFERENCE_CATEGORIES(str, Enum):
+class MODEL_REFERENCE_CATEGORIES(StrEnum):
     """The categories of model reference entries."""
 
-    BLIP = "blip"
-    CLIP = "clip"
-    CODEFORMER = "codeformer"
-    CONTROLNET = "controlnet"
-    ESRGAN = "esrgan"
-    GFPGAN = "gfpgan"
-    SAFETY_CHECKER = "safety_checker"
-    STABLE_DIFFUSION = "stable_diffusion"
+    blip = auto()
+    clip = auto()
+    codeformer = auto()
+    controlnet = auto()
+    esrgan = auto()
+    gfpgan = auto()
+    safety_checker = auto()
+    stable_diffusion = auto()
 
 
-class MODEL_PURPOSE(str, Enum):
-    image_generation = "image_generation"
+class MODEL_PURPOSE(StrEnum):
+    image_generation = auto()
     """The model is for image generation."""
 
-    controlnet = "controlnet"
+    controlnet = auto()
     """The model is a controlnet."""
 
-    clip = "clip"
+    clip = auto()
     """The model is a CLIP model."""
 
-    blip = "blip"
+    blip = auto()
     """The model is a BLIP model."""
 
-    post_processor = "post_processor"
+    post_processor = auto()
     """The model is a post processor (after image generation) of some variety."""
 
 
-class STABLE_DIFFUSION_BASELINE_CATEGORIES(str, Enum):
+class STABLE_DIFFUSION_BASELINE_CATEGORIES(StrEnum):
     """An enum of all the stable diffusion baselines."""
 
-    stable_diffusion_1 = "stable_diffusion_1"
-    stable_diffusion_2_768 = "stable_diffusion_2_768"
-    stable_diffusion_2_512 = "stable_diffusion_2_512"
+    stable_diffusion_1 = auto()
+    stable_diffusion_2_768 = auto()
+    stable_diffusion_2_512 = auto()
 
 
 MODEL_PURPOSE_LOOKUP: dict[MODEL_REFERENCE_CATEGORIES, MODEL_PURPOSE] = {
-    MODEL_REFERENCE_CATEGORIES.CLIP: MODEL_PURPOSE.clip,
-    MODEL_REFERENCE_CATEGORIES.BLIP: MODEL_PURPOSE.blip,
-    MODEL_REFERENCE_CATEGORIES.CODEFORMER: MODEL_PURPOSE.post_processor,
-    MODEL_REFERENCE_CATEGORIES.CONTROLNET: MODEL_PURPOSE.controlnet,
-    MODEL_REFERENCE_CATEGORIES.ESRGAN: MODEL_PURPOSE.post_processor,
-    MODEL_REFERENCE_CATEGORIES.GFPGAN: MODEL_PURPOSE.post_processor,
-    MODEL_REFERENCE_CATEGORIES.SAFETY_CHECKER: MODEL_PURPOSE.post_processor,
-    MODEL_REFERENCE_CATEGORIES.STABLE_DIFFUSION: MODEL_PURPOSE.image_generation,
+    MODEL_REFERENCE_CATEGORIES.clip: MODEL_PURPOSE.clip,
+    MODEL_REFERENCE_CATEGORIES.blip: MODEL_PURPOSE.blip,
+    MODEL_REFERENCE_CATEGORIES.codeformer: MODEL_PURPOSE.post_processor,
+    MODEL_REFERENCE_CATEGORIES.controlnet: MODEL_PURPOSE.controlnet,
+    MODEL_REFERENCE_CATEGORIES.esrgan: MODEL_PURPOSE.post_processor,
+    MODEL_REFERENCE_CATEGORIES.gfpgan: MODEL_PURPOSE.post_processor,
+    MODEL_REFERENCE_CATEGORIES.safety_checker: MODEL_PURPOSE.post_processor,
+    MODEL_REFERENCE_CATEGORIES.stable_diffusion: MODEL_PURPOSE.image_generation,
 }
```

## horde_model_reference/model_reference_records.py

```diff
@@ -1,11 +1,13 @@
 """The model database pydantic models and associate enums/lookups."""
+from __future__ import annotations
+
 from collections.abc import Mapping
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict, model_validator
 
 from horde_model_reference import (
     MODEL_PURPOSE,
     MODEL_REFERENCE_CATEGORIES,
     MODEL_STYLES,
     STABLE_DIFFUSION_BASELINE_CATEGORIES,
 )
@@ -33,117 +35,126 @@
     version: str | None
     """The version of the  model (not the version of SD it is based on, see `baseline` for that info)."""
     style: MODEL_STYLES | str | None  # TODO remove str
     """The style of the model."""
     config: Mapping[str, list[DownloadRecord]]
     """A dictionary of any configuration files and information on where to download the model file(s)."""
 
-    model_purpose: MODEL_PURPOSE
+    purpose: MODEL_PURPOSE
     """The purpose of the model."""
 
 
 class StableDiffusion_ModelRecord(Generic_ModelRecord):
     """A model entry in the model reference."""
 
-    class Config:
-        extra = "forbid"
+    model_config = ConfigDict(extra="ignore")
 
-    inpainting: bool | None
+    inpainting: bool | None = False
     """If this is an inpainting model or not."""
     baseline: STABLE_DIFFUSION_BASELINE_CATEGORIES
     """The model on which this model is based."""
-    tags: list[str] | None
+    tags: list[str] | None = []
     """Any tags associated with the model which may be useful for searching."""
-    showcases: list[str] | None
+    showcases: list[str] | None = []
     """Links to any showcases of the model which illustrate its style."""
-    min_bridge_version: int | None
+    min_bridge_version: int | None = None
     """The minimum version of AI-Horde-Worker required to use this model."""
-    trigger: list[str] | None
+    trigger: list[str] | None = []
     """A list of trigger words or phrases which can be used to activate the model."""
-    homepage: str | None
+    homepage: str | None = None
     """A link to the model's homepage."""
     nsfw: bool
     """Whether the model is NSFW or not."""
 
+    @model_validator(mode="after")  # type: ignore # FIXME
+    def validator_set_arrays_to_empty_if_none(self) -> StableDiffusion_ModelRecord:
+        """Set any `None` values to empty lists."""
+        if self.tags is None:
+            self.tags = []
+        if self.showcases is None:
+            self.showcases = []
+        if self.trigger is None:
+            self.trigger = []
+        return self
+
 
 class CLIP_ModelRecord(Generic_ModelRecord):
     pretrained_name: str | None
     # TODO docstring
 
 
 class Generic_ModelReference(BaseModel):
     models: Mapping[str, Generic_ModelRecord]
     """A dictionary of all the models."""
 
 
 class StableDiffusion_ModelReference(Generic_ModelReference):
     """The combined metadata and model list."""
 
-    class Config:
-        extra = "forbid"
+    model_config = ConfigDict(extra="forbid")
 
     baseline: Mapping[STABLE_DIFFUSION_BASELINE_CATEGORIES, int]
     """A dictionary of all the baseline types and how many models use them."""
     styles: Mapping[MODEL_STYLES, int]
     """A dictionary of all the styles and how many models use them."""
     tags: Mapping[str, int]
     """A dictionary of all the tags and how many models use them."""
-    model_hosts: Mapping[str, int]
+    models_hosts: Mapping[str, int]
     """A dictionary of all the model hosts and how many models use them."""
     models: Mapping[str, StableDiffusion_ModelRecord]
     """A dictionary of all the models."""
 
 
 def create_stablediffusion_modelreference(
     models: Mapping[str, StableDiffusion_ModelRecord],
 ) -> StableDiffusion_ModelReference:
     """Create a StableDiffusion_ModelReference from a mapping of {str: StableDiffusion_ModelRecords}."""
     baseline_categories: dict[STABLE_DIFFUSION_BASELINE_CATEGORIES, int] = {}
     styles: dict[MODEL_STYLES, int] = {}
     tags: dict[str, int] = {}
-    model_hosts: dict[str, int] = {}
+    download_hosts: dict[str, int] = {}
     for model in models.values():
         baseline_categories[model.baseline] = baseline_categories.get(model.baseline, 0) + 1
-        if model.style is not None and model.style in MODEL_STYLES:
+        if model.style is not None and model.style in MODEL_STYLES.__members__:
             styles[MODEL_STYLES(model.style)] = styles.get(MODEL_STYLES(model.style), 0) + 1
         if model.tags is not None:
             for tag in model.tags:
                 tags[tag] = tags.get(tag, 0) + 1
         for host in model.config:
-            model_hosts[host] = model_hosts.get(host, 0) + 1
+            download_hosts[host] = download_hosts.get(host, 0) + 1
     return StableDiffusion_ModelReference(
         baseline=baseline_categories,
         styles=styles,
         tags=tags,
-        model_hosts=model_hosts,
+        models_hosts=download_hosts,
         models=models,
     )
 
 
 class CLIP_ModelReference(Generic_ModelReference):
     models: Mapping[str, CLIP_ModelRecord]
     """A dictionary of all the models."""
 
 
 MODEL_REFERENCE_RECORD_TYPE_LOOKUP: dict[MODEL_REFERENCE_CATEGORIES, type[Generic_ModelRecord]] = {
-    MODEL_REFERENCE_CATEGORIES.STABLE_DIFFUSION: StableDiffusion_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.CONTROLNET: Generic_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.CLIP: CLIP_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.BLIP: Generic_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.ESRGAN: Generic_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.GFPGAN: Generic_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.SAFETY_CHECKER: Generic_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.CODEFORMER: Generic_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.stable_diffusion: StableDiffusion_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.controlnet: Generic_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.clip: CLIP_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.blip: Generic_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.esrgan: Generic_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.gfpgan: Generic_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.safety_checker: Generic_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.codeformer: Generic_ModelRecord,
 }
 """A lookup for the model record type based on the model category. See also `MODEL_REFERENCE_TYPE_LOOKUP`."""
 
 MODEL_REFERENCE_TYPE_LOOKUP: dict[MODEL_REFERENCE_CATEGORIES, type[Generic_ModelReference]] = {
-    MODEL_REFERENCE_CATEGORIES.STABLE_DIFFUSION: StableDiffusion_ModelReference,
-    MODEL_REFERENCE_CATEGORIES.CONTROLNET: Generic_ModelReference,
-    MODEL_REFERENCE_CATEGORIES.CLIP: CLIP_ModelReference,
-    MODEL_REFERENCE_CATEGORIES.BLIP: Generic_ModelReference,
-    MODEL_REFERENCE_CATEGORIES.ESRGAN: Generic_ModelReference,
-    MODEL_REFERENCE_CATEGORIES.GFPGAN: Generic_ModelReference,
-    MODEL_REFERENCE_CATEGORIES.SAFETY_CHECKER: Generic_ModelReference,
-    MODEL_REFERENCE_CATEGORIES.CODEFORMER: Generic_ModelReference,
+    MODEL_REFERENCE_CATEGORIES.stable_diffusion: StableDiffusion_ModelReference,
+    MODEL_REFERENCE_CATEGORIES.controlnet: Generic_ModelReference,
+    MODEL_REFERENCE_CATEGORIES.clip: CLIP_ModelReference,
+    MODEL_REFERENCE_CATEGORIES.blip: Generic_ModelReference,
+    MODEL_REFERENCE_CATEGORIES.esrgan: Generic_ModelReference,
+    MODEL_REFERENCE_CATEGORIES.gfpgan: Generic_ModelReference,
+    MODEL_REFERENCE_CATEGORIES.safety_checker: Generic_ModelReference,
+    MODEL_REFERENCE_CATEGORIES.codeformer: Generic_ModelReference,
 }
 """A lookup for the model reference type based on the model category. See also `MODEL_REFERENCE_RECORD_TYPE_LOOKUP`."""
```

## horde_model_reference/util.py

```diff
@@ -8,9 +8,8 @@
         model_name (str): The model name to convert.
 
     Returns:
         str: This is a lowercase, sanitized version of the model name.
     """
     model_name = model_name.lower()
     model_name = model_name.replace("'", "")
-    model_name = re.sub(r"[^a-z0-9]", "_", model_name)
-    return model_name
+    return re.sub(r"[^a-z0-9]", "_", model_name)
```

## horde_model_reference/legacy/add_to_legacy_sd.py

```diff
@@ -31,24 +31,24 @@
     def __init__(self, target_folder: str | pathlib.Path):
         if not isinstance(target_folder, pathlib.Path):
             target_folder = pathlib.Path(target_folder)
         self.target_folder = target_folder
 
     def load_legacy_sd_model_reference(self) -> dict[str, RawLegacy_StableDiffusion_ModelRecord]:
         path_to_legacy_stablediffusion = get_model_reference_file_path(
-            MODEL_REFERENCE_CATEGORIES.STABLE_DIFFUSION,
+            MODEL_REFERENCE_CATEGORIES.stable_diffusion,
             base_path=LEGACY_REFERENCE_FOLDER,
         )
         sd_legacy_model_reference: dict[str, RawLegacy_StableDiffusion_ModelRecord] = {}
         with open(str(path_to_legacy_stablediffusion)) as f:
             raw_json = json.load(f)
 
             for raw_record_key, raw_record_contents in raw_json.items():
                 try:
-                    sd_legacy_model_reference[raw_record_key] = RawLegacy_StableDiffusion_ModelRecord.parse_obj(
+                    sd_legacy_model_reference[raw_record_key] = RawLegacy_StableDiffusion_ModelRecord.model_validate(
                         raw_record_contents,
                     )
                 except Exception as e:
                     logger.exception(f"Failed to parse {raw_record_key} due to {e}")
 
         return sd_legacy_model_reference
 
@@ -62,15 +62,15 @@
         self,
         model_filename: str,
         sd_legacy_model_reference: dict[str, RawLegacy_StableDiffusion_ModelRecord],
     ):
         for legacy_model_record in sd_legacy_model_reference.values():
             download = legacy_model_record.config["download"][0]
             if not isinstance(download, RawLegacy_DownloadRecord):
-                raise ValueError(f"Expected download to be a DownloadRecord, got {download}")
+                raise TypeError(f"Expected download to be a DownloadRecord, got {download}")
             if download.file_name == str(model_filename):
                 # print(f"Found {model_on_disk} in legacy model reference")
                 return True
         return False
 
     def add_models_from_disk(self, file_out: pathlib.Path) -> None:
         all_sd_models_on_disk = self.get_sd_models_on_disk()
@@ -268,15 +268,19 @@
 
         if len(new_models) == 0:
             print("No new models found")
         sd_legacy_model_reference.update(new_models)
 
         jsonable_out = {}
         for model_name, model_record in sd_legacy_model_reference.items():
-            jsonable_out[model_name] = model_record.dict()
+            jsonable_out[model_name] = model_record.model_dump(
+                exclude_none=True,
+                exclude_unset=True,
+                by_alias=True,
+            )
 
         with open(str(file_out), "w") as f:
             f.write(json.dumps(jsonable_out, indent=4))
 
 
 if __name__ == "__main__":
     arg_parser = argparse.ArgumentParser()
```

## horde_model_reference/legacy/convert_all_legacy_dbs.py

```diff
@@ -20,16 +20,16 @@
         legacy_folder_path=legacy_path,
         target_file_folder=target_path,
         debug_mode=False,
     )
     clip_converter.normalize_and_convert()
 
     non_generic_converter_categories = [
-        MODEL_REFERENCE_CATEGORIES.STABLE_DIFFUSION,
-        MODEL_REFERENCE_CATEGORIES.CLIP,
+        MODEL_REFERENCE_CATEGORIES.stable_diffusion,
+        MODEL_REFERENCE_CATEGORIES.clip,
     ]
 
     generic_converted_categories = [x for x in MODEL_REFERENCE_CATEGORIES if x not in non_generic_converter_categories]
 
     for model_category in generic_converted_categories:
         converter = BaseLegacyConverter(
             legacy_folder_path=legacy_path,
```

## horde_model_reference/legacy/validate_sd.py

```diff
@@ -20,18 +20,28 @@
         logger.exception(f"ERROR: The stable diffusion database specified ({sd_db}) is not a valid json file.")
         if __name__ == "__main__":
             exit(1)
         else:
             return False
 
     parsed_db_records: dict[str, RawLegacy_StableDiffusion_ModelRecord] = {
-        k: RawLegacy_StableDiffusion_ModelRecord.parse_obj(v) for k, v in loaded_json_sd_db.items()
+        k: RawLegacy_StableDiffusion_ModelRecord.model_validate(v) for k, v in loaded_json_sd_db.items()
     }
 
-    correct_json_layout = json.dumps({k: v.dict() for k, v in parsed_db_records.items()}, indent=4)
+    correct_json_layout = json.dumps(
+        {
+            k: v.model_dump(
+                exclude_none=True,
+                exclude_unset=True,
+                by_alias=True,
+            )
+            for k, v in parsed_db_records.items()
+        },
+        indent=4,
+    )
     correct_json_layout += "\n"  # Add a newline to the end of the file, for consistency with formatters.
 
     if raw_json_sd_db != correct_json_layout:
         logger.error("Invalid stable diffusion model database.")
         if write_to_path:
             logger.info(f"Writing the correct stable diffusion model database json to {write_to_path}")
             with open(write_to_path, "w") as corrected_sd_db_file:
```

## horde_model_reference/legacy/classes/legacy_converters.py

```diff
@@ -16,24 +16,23 @@
     LOG_FOLDER,
     MODEL_PURPOSE_LOOKUP,
     MODEL_REFERENCE_CATEGORIES,
     path_consts,
 )
 from horde_model_reference.legacy.classes.staging_model_database_records import (
     MODEL_REFERENCE_LEGACY_TYPE_LOOKUP,
-    Legacy_Generic_ModelReference,
     Legacy_StableDiffusion_ModelRecord,
     Staging_StableDiffusion_ModelReference,
     StagingLegacy_Config_DownloadRecord,
     StagingLegacy_Config_FileRecord,
     StagingLegacy_Generic_ModelRecord,
 )
+from horde_model_reference.meta_consts import MODEL_PURPOSE
 from horde_model_reference.model_reference_records import (
-    MODEL_REFERENCE_TYPE_LOOKUP,
-    StableDiffusion_ModelReference,
+    StableDiffusion_ModelRecord,
 )
 from horde_model_reference.path_consts import (
     GITHUB_REPO_URL,
     PACKAGE_NAME,
 )
 from horde_model_reference.util import model_name_to_showcase_folder_name
 
@@ -161,15 +160,15 @@
                     del model_record_contents["config"]["showcases"]
                 record_as_conversion_class = model_record_type(**model_record_contents)
                 self.all_model_records[model_record_key] = record_as_conversion_class
                 yield model_record_key, record_as_conversion_class
             except ValidationError as e:
                 error = f"CRITICAL: Error parsing {model_record_key}:\n{e}"
                 self.add_validation_error_to_log(model_record_key=model_record_key, error=error)
-                raise e
+                raise
 
     def config_record_pre_parse(
         self,
         model_record_key: str,
         model_record_contents: dict,
     ) -> list[StagingLegacy_Config_DownloadRecord]:
         """Parse the config record of the legacy model reference. Changes `model_record_contents`.
@@ -197,16 +196,19 @@
                     sha_lookup[parsed_file_record.path] = parsed_file_record.sha256sum
                     parsed_file_record.sha256sum = None
 
                     parsed_record_config_files_list.append(parsed_file_record)
 
             elif config_entry == "download":
                 for download in model_record_contents["config"][config_entry]:
-                    parsed_download_record = StagingLegacy_Config_DownloadRecord(**download)
-                    parsed_download_record.sha256sum = sha_lookup[parsed_download_record.file_name]
+                    sha_dict = {}
+                    if download.get("file_name") and download["file_name"] in sha_lookup:
+                        sha_dict = {"sha256sum": sha_lookup[download["file_name"]]}
+                    all_params = {**download, **sha_dict}
+                    parsed_download_record = StagingLegacy_Config_DownloadRecord(**all_params)
 
                     if parsed_download_record.sha256sum is None:
                         error = f"{model_record_key} has a download record without a sha256sum."
                         self.add_validation_error_to_log(model_record_key=model_record_key, error=error)
                         parsed_download_record.sha256sum = "FIXME"
                     parsed_record_config_download_list.append(parsed_download_record)
 
@@ -228,19 +230,18 @@
             self.add_validation_error_to_log(model_record_key=model_record_key, error=error)
 
         if record.available:
             error = f"{model_record_key} is flagged 'available'."
 
             self.add_validation_error_to_log(model_record_key=model_record_key, error=error)
 
-        if record.download_all:
-            if self.debug_mode:
-                error = f"{model_record_key} has download_all set."
+        if record.download_all and self.debug_mode:
+            error = f"{model_record_key} has download_all set."
 
-                self.add_validation_error_to_log(model_record_key=model_record_key, error=error)
+            self.add_validation_error_to_log(model_record_key=model_record_key, error=error)
 
         if record.config is None:
             error = f"{model_record_key} has no config."
 
             self.add_validation_error_to_log(model_record_key=model_record_key, error=error)
 
         if record.description is None:
@@ -262,41 +263,32 @@
         model_record_in_progress: StagingLegacy_Generic_ModelRecord,
     ) -> None:
         """Override and call super().parse_record(..) to perform any model category specific parsing."""
 
     def post_parse_records(self) -> None:
         """Override and call super().post_parse_records() to perform any model category specific post parsing."""
         for model_record in self.all_model_records.values():
-            model_record.model_purpose = MODEL_PURPOSE_LOOKUP[self.model_reference_category]
+            model_record.purpose = MODEL_PURPOSE_LOOKUP[self.model_reference_category]
         pass
 
     def write_out_records(self) -> None:
         """Write out the parsed records."""
-        new_reference = None
-        type_to_convert_to = MODEL_REFERENCE_TYPE_LOOKUP[self.model_reference_category]
-        try:
-            _ = Legacy_Generic_ModelReference(models=self.all_model_records)
-            new_reference = type_to_convert_to(models=_.models)
-            pass
-        except ValidationError as e:
-            logger.exception(f"CRITICAL: Failed to convert to new model reference type {type_to_convert_to}.")
-            raise e
-
         if self.dry_run:
             return
 
         with open(self.converted_database_file_path, "w") as new_model_reference_file:
-            new_model_reference_file.write(
-                new_reference.json(
-                    indent=4,
-                    exclude_defaults=True,
+            json.dump(
+                self.all_model_records,
+                new_model_reference_file,
+                indent=4,
+                default=lambda o: o.model_dump(
                     exclude_none=True,
                     exclude_unset=True,
-                )
-                + "\n",
+                    by_alias=True,
+                ),
             )
 
     def add_validation_error_to_log(
         self,
         *,
         model_record_key: str,
         error: str,
@@ -330,15 +322,15 @@
 
     all_baseline_categories: dict[str, int]
     """A dictionary of all the baseline types found and the number of times they appear."""
     all_styles: dict[str, int]
     """A dictionary of all the styles found and the number of times they appear."""
     all_tags: dict[str, int]
     """A dictionary of all the tags found and the number of times they appear."""
-    all_model_hosts: dict[str, int]
+    all_download_hosts: dict[str, int]
     """A dictionary of all the model hosts found and the number of times they appear."""
 
     existing_showcase_files: dict[str, list[str]]
     """The pre-existing showcase files found in the target folder."""
 
     def __init__(
         self,
@@ -353,21 +345,21 @@
             legacy_folder_path (str | Path, optional): The legacy database folder. Defaults to LEGACY_REFERENCE_FOLDER.
             target_file_folder (str | Path): The folder to write the converted database to.
             debug_mode (bool, optional): If true, include extra information in the error log. Defaults to False.
         """
         super().__init__(
             legacy_folder_path=legacy_folder_path,
             target_file_folder=target_file_folder,
-            model_reference_category=path_consts.MODEL_REFERENCE_CATEGORIES.STABLE_DIFFUSION,
+            model_reference_category=path_consts.MODEL_REFERENCE_CATEGORIES.stable_diffusion,
             debug_mode=debug_mode,
         )
         self.all_baseline_categories = {}
         self.all_styles = {}
         self.all_tags = {}
-        self.all_model_hosts = {}
+        self.all_download_hosts = {}
 
     @override
     def pre_parse_records(self) -> None:
         existing_showcase_folders = glob.glob(self.showcase_glob_pattern, recursive=True)
         self.existing_showcase_files = self.get_existing_showcases(existing_showcase_folders)
 
     @override
@@ -454,15 +446,15 @@
             config_entries=config_entries,
         )
 
         #
         # Increment host counter
         #
         for found_host in found_hosts:
-            self.all_model_hosts[found_host] = self.all_model_hosts.get(found_host, 0) + 1
+            self.all_download_hosts[found_host] = self.all_download_hosts.get(found_host, 0) + 1
 
     @override
     def post_parse_records(self) -> None:
         super().post_parse_records()
         final_on_disk_showcase_folders = glob.glob(self.showcase_glob_pattern, recursive=True)
         for folder in final_on_disk_showcase_folders:
             parsed_folder = Path(folder)
@@ -486,15 +478,15 @@
                 error = f"folder '{folder}' is not in the model records."
                 self.add_validation_error_to_log(model_record_key=folder, error=error)
 
         print()
         logger.debug(f"{self.all_styles=}")
         logger.debug(f"{self.all_baseline_categories=}")
         logger.debug(f"{self.all_tags=}")
-        logger.debug(f"{self.all_model_hosts=}")
+        logger.debug(f"{self.all_download_hosts=}")
         print()
         logger.info(f"Total number of models: {len(self.all_model_records)}")
         logger.info(f"Total number of showcase folders: {len(final_on_disk_showcase_folders_names)}")
         print()
         logger.info(f"Total number of models with validation issues: {len(self.all_validation_errors_log)}")
 
     @override
@@ -503,38 +495,54 @@
             key: value
             for key, value in self.all_model_records.items()
             if isinstance(value, Legacy_StableDiffusion_ModelRecord)
         }
         if len(sanity_check) != len(self.all_model_records):
             raise ValueError("CRITICAL: Not all records are of the correct type.")
 
-        modelReference = Staging_StableDiffusion_ModelReference(
+        Staging_StableDiffusion_ModelReference(
             baseline=self.all_baseline_categories,
             styles=self.all_styles,
             tags=self.all_tags,
-            model_hosts=self.all_model_hosts,
+            download_hosts=self.all_download_hosts,
             models=sanity_check,
         )
 
-        models_in_doc_root = {k: v.dict() for k, v in self.all_model_records.items()}
+        models_in_doc_root = {
+            k: v.model_dump(
+                exclude_none=True,
+                exclude_unset=True,
+                by_alias=True,
+            )
+            for k, v in self.all_model_records.items()
+        }
 
         try:
             # If this fails, we have a problem. By definition, the model reference should be converted by this point
             # and ready to be cast to the new model reference type.
-            StableDiffusion_ModelReference(**json.loads(modelReference.json()))
+            for model_entry in sanity_check.values():
+                model_entry_as_dict = model_entry.model_dump(by_alias=True)
+                model_entry_as_dict["purpose"] = MODEL_PURPOSE.image_generation
+                StableDiffusion_ModelRecord(**model_entry_as_dict)
         except ValidationError as e:
             logger.exception(e)
             logger.exception("CRITICAL: Failed to convert to new model reference type.")
-            raise e
+            raise
 
         if self.dry_run:
             return
 
         with open(self.converted_database_file_path, "w") as testfile:
-            testfile.write(json.dumps(models_in_doc_root, indent=4) + "\n")
+            testfile.write(
+                json.dumps(
+                    models_in_doc_root,
+                    indent=4,
+                )
+                + "\n",
+            )
 
         logger.info("Converted database passes validation and was written to disk successfully.")
         logger.info(f"Converted database written to: {self.converted_database_file_path}")
 
     def get_existing_showcases(
         self,
         existing_showcase_folders: list[str],
@@ -611,15 +619,16 @@
                         self.add_validation_error_to_log(model_record_key=model_record_key, error=error)
 
                     if ".yaml" in config_file.path:
                         if config_file.path != "v2-inference-v.yaml" and config_file.path != "v1-inference.yaml":
                             error = f"{model_record_key} has a non-standard config."
                             self.add_validation_error_to_log(model_record_key=model_record_key, error=error)
                         continue
-                    elif ".ckpt" not in config_file.path:
+
+                    if ".ckpt" not in config_file.path:
                         error = f"{model_record_key} has a config file with an invalid path."
                         self.add_validation_error_to_log(model_record_key=model_record_key, error=error)
 
                     if config_file.sha256sum is None or config_file.sha256sum == "":
                         error = f"{model_record_key} has a config file with no sha256sum."
                         self.add_validation_error_to_log(model_record_key=model_record_key, error=error)
                     else:
@@ -649,18 +658,18 @@
 
                     if "civitai" in download.file_url:
                         download.known_slow_download = True
 
                     try:
                         host = urllib.parse.urlparse(download.file_url).netloc
                         download_hosts[host] = download_hosts.get(host, 0) + 1
-                    except Exception as e:
+                    except Exception:
                         error = f"{model_record_key} has a download with an invalid file_url."
                         self.add_validation_error_to_log(model_record_key=model_record_key, error=error)
-                        raise e
+                        raise
 
         return download_hosts
 
 
 class LegacyClipConverter(BaseLegacyConverter):
     def __init__(
         self,
@@ -668,15 +677,15 @@
         legacy_folder_path: str | Path = LEGACY_REFERENCE_FOLDER,
         target_file_folder: str | Path = BASE_PATH,
         debug_mode: bool = False,
     ):
         super().__init__(
             legacy_folder_path=legacy_folder_path,
             target_file_folder=target_file_folder,
-            model_reference_category=MODEL_REFERENCE_CATEGORIES.CLIP,
+            model_reference_category=MODEL_REFERENCE_CATEGORIES.clip,
             debug_mode=debug_mode,
         )
 
     @override
     def config_record_pre_parse(
         self,
         model_record_key: str,
@@ -685,15 +694,15 @@
         new_record_config_download_list: list[StagingLegacy_Config_DownloadRecord] = []
         if len(model_record_contents["config"]) > 2:
             error = f"{model_record_key} has more than 2 config entries."
             self.add_validation_error_to_log(model_record_key=model_record_key, error=error)
         for config_entry in model_record_contents["config"]:
             if config_entry == "files":
                 continue
-            elif config_entry == "download":
+            if config_entry == "download":
                 for download in model_record_contents["config"][config_entry]:
                     # Skip if file_url is missing
                     if download.get("file_url") is None or download.get("file_url") == "":
                         continue
                     parsed_download_record = StagingLegacy_Config_DownloadRecord(**download)
                     parsed_download_record.file_name = model_record_key.replace("/", "-") + ".pt"
                     parsed_download_record.sha256sum = "FIXME"
```

## horde_model_reference/legacy/classes/raw_legacy_model_database_records.py

```diff
@@ -1,11 +1,11 @@
 """The classes which can represent a legacy model reference file."""
 from collections.abc import Mapping
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 
 class RawLegacy_DownloadRecord(BaseModel):
     """An entry in the `config` field of a `RawLegacy_StableDiffusion_ModelRecord`."""
 
     file_name: str
     file_path: str
@@ -17,52 +17,30 @@
 
     path: str
     md5sum: str | None = None
     sha256sum: str | None = None
 
 
 class RawLegacy_StableDiffusion_ModelRecord(BaseModel):
-    """A model entry in the legacy model reference. Note that `.dict()` exports to the new model reference format."""
+    """A model entry in the legacy model reference."""
 
     # This is a better representation of the legacy model reference than the one in `staging_model_database_records.py`
     # which is a hybrid representation of the legacy model reference and the new model reference format.
 
-    class Config:
-        extra = "forbid"
+    model_config = ConfigDict(extra="forbid")
 
     name: str
     baseline: str
     type: str  # noqa: A003
     inpainting: bool
-    description: str | None
-    tags: list[str] | None
-    showcases: list[str] | None
-    min_bridge_version: int | None
+    description: str | None = None
+    tags: list[str] | None = None
+    showcases: list[str] | None = None
+    min_bridge_version: int | None = None
     version: str
-    style: str | None
-    trigger: list[str] | None
-    homepage: str | None
+    style: str | None = None
+    trigger: list[str] | None = None
+    homepage: str | None = None
     nsfw: bool
     download_all: bool
     config: Mapping[str, list[RawLegacy_FileRecord | RawLegacy_DownloadRecord]]
-    available: bool | None
-
-    def dict(  # noqa: A003
-        self,
-        *,
-        include=None,
-        exclude=None,
-        by_alias: bool = False,
-        skip_defaults: bool | None = None,
-        exclude_unset: bool = False,
-        exclude_defaults: bool = False,
-        exclude_none: bool = False,
-    ):
-        return super().dict(
-            include=include,
-            exclude=exclude,
-            by_alias=by_alias,
-            skip_defaults=skip_defaults,
-            exclude_unset=True,
-            exclude_defaults=exclude_defaults,
-            exclude_none=True,
-        )
+    available: bool | None = None
```

## horde_model_reference/legacy/classes/staging_model_database_records.py

```diff
@@ -4,124 +4,110 @@
 # a set of classes exactly representative of the legacy model reference. It's
 # more of a hybrid representation of the legacy model reference and the new model.
 
 # These classes will only persist until the legacy model reference is fully deprecated.
 
 from collections.abc import Mapping
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict, model_validator
 
 from horde_model_reference.model_reference_records import MODEL_PURPOSE
 from horde_model_reference.path_consts import MODEL_REFERENCE_CATEGORIES
 
 
 class StagingLegacy_Config_FileRecord(BaseModel):
     """An entry in the `config` field of a `StagingLegacy_Generic_ModelRecord`."""
 
     # class Config:
     #     extra = "forbid"
 
     path: str
     # md5sum: str | None
-    sha256sum: str | None
+    sha256sum: str | None = None
+
+    @model_validator(mode="after")
+    def validate_model_file_has_sha256sum(self):
+        if ".yaml" in self.path or ".json" in self.path:
+            return self
+
+        if self.sha256sum is None:
+            raise ValueError("A model file must have a sha256sum.")
+
+        return self
 
 
 class StagingLegacy_Config_DownloadRecord(BaseModel):
     """An entry in the `config` field of a `StagingLegacy_Generic_ModelRecord`."""
 
-    class Config:
-        extra = "forbid"
+    model_config = ConfigDict(extra="forbid")
 
     file_name: str
     file_path: str = ""
     file_url: str
-    sha256sum: str | None
-    known_slow_download: bool | None
+    sha256sum: str | None = None
+    known_slow_download: bool | None = False
 
 
 class StagingLegacy_Generic_ModelRecord(BaseModel):
     """This is a helper class, a hybrid representation of the legacy model reference and the new format."""
 
-    class Config:
-        extra = "forbid"
+    model_config = ConfigDict(extra="forbid")
 
     name: str
     type: str  # noqa: A003
-    description: str | None
-    version: str | None
-    style: str | None
-    nsfw: bool | None
-    download_all: bool | None
+    description: str | None = None
+    version: str | None = None
+    style: str | None = None
+    nsfw: bool | None = None
+    download_all: bool | None = None
     config: dict[str, list[StagingLegacy_Config_FileRecord | StagingLegacy_Config_DownloadRecord]]
-    available: bool | None
+    available: bool | None = None
 
-    model_purpose: MODEL_PURPOSE | None
+    purpose: MODEL_PURPOSE | None = None
 
 
 class Legacy_CLIP_ModelRecord(StagingLegacy_Generic_ModelRecord):
-    """A model entry in the legacy model reference. Note that `.dict()` exports to the new model reference format."""
+    """A model entry in the legacy model reference."""
 
-    pretrained_name: str | None
+    pretrained_name: str | None = None
 
 
 class Legacy_StableDiffusion_ModelRecord(StagingLegacy_Generic_ModelRecord):
-    """A model entry in the legacy model reference. Note that `.dict()` exports to the new model reference format."""
+    """A model entry in the legacy model reference."""
 
-    inpainting: bool | None
+    inpainting: bool
     baseline: str
-    tags: list[str] | None
-    showcases: list[str] | None
-    min_bridge_version: int | None
-    trigger: list[str] | None
-    homepage: str | None
-
-    def dict(  # noqa: A003
-        self,
-        *,
-        include=None,
-        exclude=None,
-        by_alias: bool = False,
-        skip_defaults: bool | None = None,
-        exclude_unset: bool = False,
-        exclude_defaults: bool = False,
-        exclude_none: bool = False,
-    ):
-        return super().dict(
-            include=include,
-            exclude={"available", "type", "download_all"},
-            by_alias=by_alias,
-            skip_defaults=skip_defaults,
-            exclude_unset=True,
-            exclude_defaults=True,
-            exclude_none=True,
-        )
+    tags: list[str] | None = None
+    showcases: list[str] | None = None
+    min_bridge_version: int | None = None
+    trigger: list[str] | None = None
+    homepage: str | None = None
 
 
 class Legacy_Generic_ModelReference(BaseModel):
     """A helper class to convert the legacy model reference to the new model reference format."""
 
-    class Config:
-        extra = "forbid"
+    model_config = ConfigDict(extra="forbid")
 
     models: Mapping[str, StagingLegacy_Generic_ModelRecord]
 
 
 class Staging_StableDiffusion_ModelReference(Legacy_Generic_ModelReference):
     """A helper class to convert the legacy model reference to the new model reference format."""
 
     baseline: dict[str, int]
     styles: dict[str, int]
     tags: dict[str, int]
-    model_hosts: dict[str, int]
+    download_hosts: dict[str, int]
     models: Mapping[str, Legacy_StableDiffusion_ModelRecord]
 
 
 MODEL_REFERENCE_LEGACY_TYPE_LOOKUP: dict[MODEL_REFERENCE_CATEGORIES, type[StagingLegacy_Generic_ModelRecord]] = {
-    MODEL_REFERENCE_CATEGORIES.BLIP: StagingLegacy_Generic_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.CLIP: Legacy_CLIP_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.CODEFORMER: StagingLegacy_Generic_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.CONTROLNET: StagingLegacy_Generic_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.ESRGAN: StagingLegacy_Generic_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.GFPGAN: StagingLegacy_Generic_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.SAFETY_CHECKER: StagingLegacy_Generic_ModelRecord,
-    MODEL_REFERENCE_CATEGORIES.STABLE_DIFFUSION: Legacy_StableDiffusion_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.blip: StagingLegacy_Generic_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.clip: Legacy_CLIP_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.codeformer: StagingLegacy_Generic_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.controlnet: StagingLegacy_Generic_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.esrgan: StagingLegacy_Generic_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.gfpgan: StagingLegacy_Generic_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.safety_checker: StagingLegacy_Generic_ModelRecord,
+    MODEL_REFERENCE_CATEGORIES.stable_diffusion: Legacy_StableDiffusion_ModelRecord,
 }
```

## Comparing `horde_model_reference-0.2.3.dist-info/LICENSE` & `horde_model_reference-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `horde_model_reference-0.2.3.dist-info/METADATA` & `horde_model_reference-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horde-model-reference
-Version: 0.2.3
+Version: 0.3.0
 Summary: A helper library providing a way to work with the lists of diffusion models, utility models, and any other related files required for AI-Horde.
 Author-email: tazlin <tazlin.on.github@gmail.com>, db0 <mail@dbzer0.com>, Jug <jugdev@proton.me>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -672,14 +672,16 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: typing-extensions
+Requires-Dist: loguru
+Requires-Dist: strenum
 
 # Horde Model Reference
 
 This package provides some tools to help manage the models which power the [AI-Horde](https://github.com/db0/AI-Horde).
 
 ## Reference info (.json files)
 For now, the legacy reference format will be availible as before at the [original official repo](https://github.com/Haidra-Org/AI-Horde-image-model-reference) used in the past.
```

## Comparing `horde_model_reference-0.2.3.dist-info/RECORD` & `horde_model_reference-0.3.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,22 @@
 horde_model_reference/__init__.py,sha256=edi3P1jpV0M41qOuZYpHLsFx9B7eyBvpJxHmwai0mLY,760
-horde_model_reference/blip.json,sha256=BabSA0Ervw8bOnC3AQYksKmAYrhwj-sjLnoHiC4KFd0,1121
-horde_model_reference/clip.json,sha256=FHqmv5t1km4uHn9ffiSK8djs-93WDb0ASGscGRHv5GI,2545
-horde_model_reference/codeformer.json,sha256=3DNDGJJZa3cJTQPjwY0MNS7fURcLWdRWuq4pIPc_x6s,676
-horde_model_reference/controlnet.json,sha256=i-JAc3hmGt-oR08TYQtDXv6g3-Pf0VyjUJBmlUYp-bY,11397
-horde_model_reference/esrgan.json,sha256=TeYUtIKTY3g9DOIYCiX44roPViu1fM2QREGjuW-5Mzg,4230
-horde_model_reference/gfpgan.json,sha256=bIp6VknP3U54iui87Jl3KlI_HuueJD29TeaIwn3nEjY,1358
-horde_model_reference/meta_consts.py,sha256=HrgIGDuU_nBX01x5XHHE31LaiwYyV-fW3OFApKW8dQg,2254
-horde_model_reference/model_reference_records.py,sha256=iO3gdvv1mzNGXOVukpVB9JAUOUIUiNF6_FtoB3xgMqg,6149
+horde_model_reference/meta_consts.py,sha256=R0DZWTyIhhnDI5PuVwAiiWUubjeQygziFFeRibuYDm0,2143
+horde_model_reference/model_reference_records.py,sha256=GR4vmsml28y1qF8ieEPCSQT68eV-zxoSa5qom7tGHa8,6691
 horde_model_reference/path_consts.py,sha256=Bj--0A9by18scyyXGDIYWRwzlJBRsZn4RiatqO96Kyc,4201
-horde_model_reference/safety_checker.json,sha256=yyXZP3ufIntfMeDRehYdUzL-aI0fkEqGrB-4ehpcfK4,1329
-horde_model_reference/stable_diffusion.json,sha256=toGpwb1syWcqXLpNXtkvXknDbPhN2VYtQYGaeHVjwCM,191369
-horde_model_reference/util.py,sha256=Fnt95izYz1KpzaUL5UTl1dGogNiCNIpe2-QziraxVp8,500
-horde_model_reference/embeddings/hypernetworks/add_hypernetworks_here.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-horde_model_reference/embeddings/lora/add_loras_here.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+horde_model_reference/util.py,sha256=ZNzoGmgHUT2KSUvCL2slNKaqaQxAbz9dXa-sXdU0f5I,471
 horde_model_reference/legacy/README.md,sha256=WbkgdvkrIDhhRiPlqW2YoPSzr590ZP_A71uulSjQQ70,879
 horde_model_reference/legacy/__init__.py,sha256=ww6Vh68nQ1X30tdkQWj9bOFdZ2s3dhc_OAstLa4zjYw,221
-horde_model_reference/legacy/add_to_legacy_sd.py,sha256=5mqOo9OjCM74fgK9r0aN-mLjy8Tbu6ypCZ4fbEryamQ,14178
-horde_model_reference/legacy/convert_all_legacy_dbs.py,sha256=Wv6Lf33gosl67Jw4OcByN1hjHCLN6Mvgf07yhZbqFyg,1999
+horde_model_reference/legacy/add_to_legacy_sd.py,sha256=r3y2eDYY4yHmfB0q3OlgTIo5K6HICLpoG2aCJTKOLdw,14307
+horde_model_reference/legacy/convert_all_legacy_dbs.py,sha256=emUJ-5kYvXN-hfjWWk9oh_l7dXjhsz8LsYZ4AbWAp4E,1999
 horde_model_reference/legacy/download_live_legacy_dbs.py,sha256=asdEnlzJFcIZICRen_bLlWGltBp2AIXr6QR49GEdkB8,3450
-horde_model_reference/legacy/validate_sd.py,sha256=fOH0A4RzwG6GII267e4C-H5n8co9vfdaOp_eAqdgx5Y,3420
+horde_model_reference/legacy/validate_sd.py,sha256=xnMKHL0xWB6ONZ-fqO2LakmTkF9Rb1KivBKXRDNwJoE,3613
 horde_model_reference/legacy/classes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-horde_model_reference/legacy/classes/legacy_converters.py,sha256=uQL6py_oy57xgR0ldAT08J63B1xW6Hmx2ZhaUON1FZA,32660
-horde_model_reference/legacy/classes/raw_legacy_model_database_records.py,sha256=xYkT8CbXwLJnDyV12pBIBABiMv_llLxUBR-D8n1x_D8,2061
-horde_model_reference/legacy/classes/staging_model_database_records.py,sha256=u8_TJRSIOKKA51UNMyTntClPw69_pquNlI61iOjRLMU,4397
+horde_model_reference/legacy/classes/legacy_converters.py,sha256=ymH7M-k6JlpFFc3ricfQdiAg2w-ss2hAEQN7L71KUCc,32829
+horde_model_reference/legacy/classes/raw_legacy_model_database_records.py,sha256=iG69-vBzKZ332ClQx51Ay4ySNIGmGwGomIkWd1YodvQ,1475
+horde_model_reference/legacy/classes/staging_model_database_records.py,sha256=fBnlQR9u0_CBeD5QOT5IhdInNwwW93fJ4qjLlljJOp8,4099
 horde_model_reference/showcase/README.md,sha256=h-CSQLFQcFlLENtBMgaSQmQh0IfF7C5Kqs7B0-OiMgM,1430
-horde_model_reference-0.2.3.dist-info/LICENSE,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
-horde_model_reference-0.2.3.dist-info/METADATA,sha256=Q3y06TKeRYTt63cRzcG8_2HGYEUiwZBDrB3Z8tuKn1Y,44597
-horde_model_reference-0.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-horde_model_reference-0.2.3.dist-info/entry_points.txt,sha256=_LjrCGpRgF-adj35rjBZvjk13JFrRZT0L2mxiaphd6Y,85
-horde_model_reference-0.2.3.dist-info/top_level.txt,sha256=2wj98-jSCXgbXKdbmQMwlE_8AYWjfPDZYs_gxc4Xumc,22
-horde_model_reference-0.2.3.dist-info/RECORD,,
+horde_model_reference-0.3.0.dist-info/LICENSE,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
+horde_model_reference-0.3.0.dist-info/METADATA,sha256=ZICZthGS2HJMdo9ZzOXv7GXKSy8EWBMv9YdiV4ldI4Q,44644
+horde_model_reference-0.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+horde_model_reference-0.3.0.dist-info/entry_points.txt,sha256=_LjrCGpRgF-adj35rjBZvjk13JFrRZT0L2mxiaphd6Y,85
+horde_model_reference-0.3.0.dist-info/top_level.txt,sha256=2wj98-jSCXgbXKdbmQMwlE_8AYWjfPDZYs_gxc4Xumc,22
+horde_model_reference-0.3.0.dist-info/RECORD,,
```

