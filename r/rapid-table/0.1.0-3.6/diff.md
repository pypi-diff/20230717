# Comparing `tmp/rapid_table-0.1.0-py3-none-any.whl.zip` & `tmp/rapid_table-3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7077572 bytes, number of entries: 15
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-17 08:53 rapid_table/__init__.py
--rw-r--r--  2.0 unx     3789 b- defN 23-Jul-17 08:53 rapid_table/rapid_table.py
--rw-r--r--  2.0 unx     2701 b- defN 23-Jul-17 08:53 rapid_table/utils.py
+Zip file size: 7077382 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-15 14:14 rapid_table/__init__.py
+-rw-r--r--  2.0 unx     2759 b- defN 23-Jun-15 14:14 rapid_table/rapid_table.py
+-rw-r--r--  2.0 unx     2707 b- defN 23-Jun-15 14:14 rapid_table/utils.py
 -rw-r--r--  2.0 unx  7704409 b- defN 22-Dec-19 09:03 rapid_table/models/en_ppstructure_mobile_v2_SLANet.onnx
--rw-r--r--  2.0 unx      106 b- defN 23-Jul-17 08:53 rapid_table/table_matcher/__init__.py
--rw-r--r--  2.0 unx     4760 b- defN 23-Jul-17 08:53 rapid_table/table_matcher/matcher.py
--rw-r--r--  2.0 unx     9671 b- defN 23-Jul-17 08:53 rapid_table/table_matcher/utils.py
--rw-r--r--  2.0 unx      653 b- defN 23-Jul-17 08:53 rapid_table/table_structure/__init__.py
--rw-r--r--  2.0 unx     1933 b- defN 23-Jul-17 08:53 rapid_table/table_structure/table_structure.py
--rw-r--r--  2.0 unx    11920 b- defN 23-Jul-17 08:53 rapid_table/table_structure/utils.py
--rw-r--r--  2.0 unx     5141 b- defN 23-Jul-17 08:53 rapid_table-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 08:53 rapid_table-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 23-Jul-17 08:53 rapid_table-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-17 08:53 rapid_table-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1336 b- defN 23-Jul-17 08:53 rapid_table-0.1.0.dist-info/RECORD
-15 files, 7746694 bytes uncompressed, 7075330 bytes compressed:  8.7%
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-15 14:14 rapid_table/table_matcher/__init__.py
+-rw-r--r--  2.0 unx     6670 b- defN 23-Jun-15 14:14 rapid_table/table_matcher/matcher.py
+-rw-r--r--  2.0 unx    10019 b- defN 23-Jun-15 14:14 rapid_table/table_matcher/utils.py
+-rw-r--r--  2.0 unx      653 b- defN 23-Jun-15 14:14 rapid_table/table_structure/__init__.py
+-rw-r--r--  2.0 unx     1945 b- defN 23-Jun-15 14:14 rapid_table/table_structure/table_structure.py
+-rw-r--r--  2.0 unx    12009 b- defN 23-Jun-15 14:14 rapid_table/table_structure/utils.py
+-rw-r--r--  2.0 unx     4967 b- defN 23-Jun-15 14:15 rapid_table-3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 14:15 rapid_table-3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-15 14:15 rapid_table-3.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-15 14:15 rapid_table-3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-15 14:15 rapid_table-3.6.dist-info/RECORD
+15 files, 7747846 bytes uncompressed, 7075160 bytes compressed:  8.7%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: rapid_table/table_structure/table_structure.py
 Comment: 
 
 Filename: rapid_table/table_structure/utils.py
 Comment: 
 
-Filename: rapid_table-0.1.0.dist-info/METADATA
+Filename: rapid_table-3.6.dist-info/METADATA
 Comment: 
 
-Filename: rapid_table-0.1.0.dist-info/WHEEL
+Filename: rapid_table-3.6.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_table-0.1.0.dist-info/entry_points.txt
+Filename: rapid_table-3.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_table-0.1.0.dist-info/top_level.txt
+Filename: rapid_table-3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_table-0.1.0.dist-info/RECORD
+Filename: rapid_table-3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_table/rapid_table.py

```diff
@@ -1,74 +1,55 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 import argparse
 import copy
-import importlib
 import time
 from pathlib import Path
-from typing import List, Optional, Tuple, Union
+from typing import Union
 
 import cv2
 import numpy as np
+from rapidocr_onnxruntime import RapidOCR
 
 from .table_matcher import TableMatch
 from .table_structure import TableStructurer
 from .utils import LoadImage, vis_table
 
 root_dir = Path(__file__).resolve().parent
 
 
-class RapidTable:
-    def __init__(
-        self,
-        model_path: Optional[str] = None,
-    ):
+class RapidTable():
+    def __init__(self, model_path: str = None):
+        self.ocr_sys = RapidOCR()
+
         if model_path is None:
-            model_path = str(
-                root_dir / "models" / "en_ppstructure_mobile_v2_SLANet.onnx"
-            )
+            model_path = str(root_dir / 'models' / 'en_ppstructure_mobile_v2_SLANet.onnx')
 
-        self.load_img = LoadImage()
         self.table_structure = TableStructurer(model_path)
         self.table_matcher = TableMatch()
 
-        try:
-            self.ocr_engine = importlib.import_module("rapidocr_onnxruntime").RapidOCR()
-        except ModuleNotFoundError:
-            self.ocr_engine = None
-
-    def __call__(
-        self,
-        img_content: Union[str, np.ndarray, bytes, Path],
-        ocr_result: List[Union[List[List[float]], str, str]] = None,
-    ) -> Tuple[str, float]:
-        if self.ocr_engine is None and ocr_result is None:
-            raise ValueError(
-                "One of two conditions must be met: ocr_result is not empty, or rapidocr_onnxruntime is installed."
-            )
+        self.load_img = LoadImage()
 
+    def __call__(self, img_content: Union[str, np.ndarray, bytes, Path]):
         img = self.load_img(img_content)
 
         s = time.time()
-        h, w = img.shape[:2]
-
-        if ocr_result is None:
-            ocr_result, _ = self.ocr_engine(img)
-        dt_boxes, rec_res = self.get_boxes_recs(ocr_result, h, w)
+        dt_boxes, rec_res = self._ocr(copy.deepcopy(img))
 
         structure_res, _ = self.table_structure(copy.deepcopy(img))
         pred_html = self.table_matcher(structure_res, dt_boxes, rec_res)
 
         elapse = time.time() - s
         return pred_html, elapse
 
-    def get_boxes_recs(
-        self, ocr_result: List[Union[List[List[float]], str, str]], h: int, w: int
-    ) -> Tuple[np.ndarray, Tuple[str, str]]:
+    def _ocr(self, img):
+        h, w = img.shape[:2]
+
+        ocr_result, _ = self.ocr_sys(img)
         dt_boxes, rec_res, scores = list(zip(*ocr_result))
         rec_res = list(zip(rec_res, scores))
 
         r_boxes = []
         for box in dt_boxes:
             box = np.array(box)
             x_min = max(0, box[:, 0].min() - 1)
@@ -79,48 +60,30 @@
             r_boxes.append(box)
         dt_boxes = np.array(r_boxes)
         return dt_boxes, rec_res
 
 
 def main() -> None:
     parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-v",
-        "--vis",
-        action="store_true",
-        help="Wheter to visualize the layout results.",
-    )
-    parser.add_argument(
-        "-img", "--img_path", type=str, required=True, help="Path to image for layout."
-    )
-    parser.add_argument(
-        "-m",
-        "--model_path",
-        type=str,
-        default=str(root_dir / "models" / "en_ppstructure_mobile_v2_SLANet.onnx"),
-        help="The model path used for inference.",
-    )
+    parser.add_argument('-v', '--vis', action='store_true',
+                        help='Wheter to visualize the layout results.')
+    parser.add_argument('-img', '--img_path', type=str, required=True,
+                        help='Path to image for layout.')
+    parser.add_argument('-m', '--model_path', type=str,
+                        default=str(root_dir / 'models' / 'en_ppstructure_mobile_v2_SLANet.onnx'),
+                        help='The model path used for inference.')
     args = parser.parse_args()
 
-    try:
-        ocr_engine = importlib.import_module("rapidocr_onnxruntime").RapidOCR()
-    except ModuleNotFoundError as exc:
-        raise ModuleNotFoundError(
-            "Please install the rapidocr_onnxruntime by pip install rapidocr_onnxruntime."
-        ) from exc
-
     rapid_table = RapidTable(args.model_path)
 
     img = cv2.imread(args.img_path)
-
-    ocr_result, _ = ocr_engine(img)
-    table_html_str, elapse = rapid_table(img, ocr_result)
+    table_html_str, elapse = rapid_table(img)
     print(table_html_str)
 
     if args.vis:
         img_path = Path(args.img_path)
-        save_path = img_path.resolve().parent / f"vis_{img_path.stem}.html"
+        save_path = img_path.resolve().parent / f'vis_{img_path.stem}.html'
         vis_table(table_html_str, str(save_path))
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     main()
```

## rapid_table/utils.py

```diff
@@ -8,25 +8,22 @@
 import cv2
 import numpy as np
 from PIL import Image, UnidentifiedImageError
 
 InputType = Union[str, np.ndarray, bytes, Path]
 
 
-class LoadImage:
-    def __init__(
-        self,
-    ):
+class LoadImage():
+    def __init__(self, ):
         pass
 
     def __call__(self, img: InputType) -> np.ndarray:
         if not isinstance(img, InputType.__args__):
             raise LoadImageError(
-                f"The img type {type(img)} does not in {InputType.__args__}"
-            )
+                f'The img type {type(img)} does not in {InputType.__args__}')
 
         img = self.load_img(img)
 
         if img.ndim == 2:
             return cv2.cvtColor(img, cv2.COLOR_GRAY2BGR)
 
         if img.ndim == 3 and img.shape[2] == 4:
@@ -37,53 +34,55 @@
     def load_img(self, img: InputType) -> np.ndarray:
         if isinstance(img, (str, Path)):
             self.verify_exist(img)
             try:
                 img = np.array(Image.open(img))
                 img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
             except UnidentifiedImageError as e:
-                raise LoadImageError(f"cannot identify image file {img}") from e
+                raise LoadImageError(
+                    f'cannot identify image file {img}') from e
             return img
 
         if isinstance(img, bytes):
             img = np.array(Image.open(BytesIO(img)))
             img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
             return img
 
         if isinstance(img, np.ndarray):
             return img
 
-        raise LoadImageError(f"{type(img)} is not supported!")
+        raise LoadImageError(f'{type(img)} is not supported!')
 
     @staticmethod
     def cvt_four_to_three(img: np.ndarray) -> np.ndarray:
-        """RGBA → RGB"""
+        '''RGBA → RGB
+        '''
         r, g, b, a = cv2.split(img)
         new_img = cv2.merge((b, g, r))
 
         not_a = cv2.bitwise_not(a)
         not_a = cv2.cvtColor(not_a, cv2.COLOR_GRAY2BGR)
 
         new_img = cv2.bitwise_and(new_img, new_img, mask=a)
         new_img = cv2.add(new_img, not_a)
         return new_img
 
     @staticmethod
     def verify_exist(file_path: Union[str, Path]):
         if not Path(file_path).exists():
-            raise LoadImageError(f"{file_path} does not exist.")
+            raise LoadImageError(f'{file_path} does not exist.')
 
 
 class LoadImageError(Exception):
     pass
 
 
 def vis_table(table_res: str, save_path: str) -> None:
-    style_res = """<style>td {border-left: 1px solid;border-bottom:1px solid;}
+    style_res = '''<style>td {border-left: 1px solid;border-bottom:1px solid;}
                    table, th {border-top:1px solid;font-size: 10px;
                    border-collapse: collapse;border-right: 1px solid;}
-                </style>"""
-    prefix_table, suffix_table = table_res.split("<body>")
-    new_table_res = f"{prefix_table}{style_res}<body>{suffix_table}"
-    with open(save_path, "w", encoding="utf-8") as f:
+                </style>'''
+    prefix_table, suffix_table = table_res.split('<body>')
+    new_table_res = f'{prefix_table}{style_res}<body>{suffix_table}'
+    with open(save_path, 'w', encoding='utf-8') as f:
         f.write(new_table_res)
-    print(f"The infer result has saved in {save_path}")
+    print(f'The infer result has saved in {save_path}')
```

## rapid_table/table_matcher/matcher.py

```diff
@@ -10,112 +10,144 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # -*- encoding: utf-8 -*-
 import numpy as np
 
-from .utils import compute_iou, distance
+from .utils import compute_iou, deal_bb, distance
 
 
-class TableMatch:
+class TableMatch():
     def __init__(self, filter_ocr_result=True, use_master=False):
         self.filter_ocr_result = filter_ocr_result
         self.use_master = use_master
 
     def __call__(self, structure_res, dt_boxes, rec_res):
         pred_structures, pred_bboxes = structure_res
         if self.filter_ocr_result:
-            dt_boxes, rec_res = self._filter_ocr_result(pred_bboxes, dt_boxes, rec_res)
+            dt_boxes, rec_res = self._filter_ocr_result(pred_bboxes, dt_boxes,
+                                                        rec_res)
         matched_index = self.match_result(dt_boxes, pred_bboxes)
-        pred_html, pred = self.get_pred_html(pred_structures, matched_index, rec_res)
+        pred_html, pred = self.get_pred_html(pred_structures,
+                                             matched_index,
+                                             rec_res)
         return pred_html
 
     def match_result(self, dt_boxes, pred_bboxes):
         matched = {}
         for i, gt_box in enumerate(dt_boxes):
             distances = []
             for j, pred_box in enumerate(pred_bboxes):
                 if len(pred_box) == 8:
                     pred_box = [
-                        np.min(pred_box[0::2]),
-                        np.min(pred_box[1::2]),
-                        np.max(pred_box[0::2]),
-                        np.max(pred_box[1::2]),
+                        np.min(pred_box[0::2]), np.min(pred_box[1::2]),
+                        np.max(pred_box[0::2]), np.max(pred_box[1::2])
                     ]
-                distances.append(
-                    (distance(gt_box, pred_box), 1.0 - compute_iou(gt_box, pred_box))
-                )  # compute iou and l1 distance
+                distances.append((distance(gt_box, pred_box),
+                                  1. - compute_iou(gt_box, pred_box)
+                                  ))  # compute iou and l1 distance
             sorted_distances = distances.copy()
             # select det box by iou and l1 distance
             sorted_distances = sorted(
-                sorted_distances, key=lambda item: (item[1], item[0])
-            )
+                sorted_distances, key=lambda item: (item[1], item[0]))
             if distances.index(sorted_distances[0]) not in matched.keys():
                 matched[distances.index(sorted_distances[0])] = [i]
             else:
                 matched[distances.index(sorted_distances[0])].append(i)
         return matched
 
     def get_pred_html(self, pred_structures, matched_index, ocr_contents):
         end_html = []
         td_index = 0
         for tag in pred_structures:
-            if "</td>" not in tag:
+            if '</td>' in tag:
+                if '<td></td>' == tag:
+                    end_html.extend('<td>')
+                if td_index in matched_index.keys():
+                    b_with = False
+                    if '<b>' in ocr_contents[matched_index[td_index][0]] \
+                            and len(matched_index[td_index]) > 1:
+                        b_with = True
+                        end_html.extend('<b>')
+                    for i, td_index_index in enumerate(matched_index[td_index]):
+                        content = ocr_contents[td_index_index][0]
+                        if len(matched_index[td_index]) > 1:
+                            if len(content) == 0:
+                                continue
+
+                            if content[0] == ' ':
+                                content = content[1:]
+
+                            if '<b>' in content:
+                                content = content[3:]
+
+                            if '</b>' in content:
+                                content = content[:-4]
+
+                            if len(content) == 0:
+                                continue
+
+                            if i != len(matched_index[td_index]) - 1 \
+                                    and ' ' != content[-1]:
+                                content += ' '
+                        end_html.extend(content)
+                    if b_with:
+                        end_html.extend('</b>')
+
+                if '<td></td>' == tag:
+                    end_html.append('</td>')
+                else:
+                    end_html.append(tag)
+                td_index += 1
+            else:
                 end_html.append(tag)
-                continue
-
-            if "<td></td>" == tag:
-                end_html.extend("<td>")
+        return ''.join(end_html), end_html
 
-            if td_index in matched_index.keys():
+    def get_pred_html_master(self, pred_structures, matched_index,
+                             ocr_contents):
+        end_html = []
+        td_index = 0
+        for token in pred_structures:
+            if '</td>' in token:
+                txt = ''
                 b_with = False
-                if (
-                    "<b>" in ocr_contents[matched_index[td_index][0]]
-                    and len(matched_index[td_index]) > 1
-                ):
-                    b_with = True
-                    end_html.extend("<b>")
-
-                for i, td_index_index in enumerate(matched_index[td_index]):
-                    content = ocr_contents[td_index_index][0]
-                    if len(matched_index[td_index]) > 1:
-                        if len(content) == 0:
-                            continue
-
-                        if content[0] == " ":
-                            content = content[1:]
-
-                        if "<b>" in content:
-                            content = content[3:]
-
-                        if "</b>" in content:
-                            content = content[:-4]
-
-                        if len(content) == 0:
-                            continue
-
-                        if i != len(matched_index[td_index]) - 1 and " " != content[-1]:
-                            content += " "
-                    end_html.extend(content)
-
+                if td_index in matched_index.keys():
+                    if '<b>' in ocr_contents[matched_index[td_index][
+                            0]] and len(matched_index[td_index]) > 1:
+                        b_with = True
+                    for i, td_index_index in enumerate(matched_index[td_index]):
+                        content = ocr_contents[td_index_index][0]
+                        if len(matched_index[td_index]) > 1:
+                            if len(content) == 0:
+                                continue
+                            if content[0] == ' ':
+                                content = content[1:]
+                            if '<b>' in content:
+                                content = content[3:]
+                            if '</b>' in content:
+                                content = content[:-4]
+                            if len(content) == 0:
+                                continue
+                            if i != len(matched_index[
+                                    td_index]) - 1 and ' ' != content[-1]:
+                                content += ' '
+                        txt += content
                 if b_with:
-                    end_html.extend("</b>")
-
-            if "<td></td>" == tag:
-                end_html.append("</td>")
-            else:
-                end_html.append(tag)
-
-            td_index += 1
-
-        # Filter <thead></thead><tbody></tbody> elements
-        filter_elements = ["<thead>", "</thead>", "<tbody>", "</tbody>"]
-        end_html = [v for v in end_html if v not in filter_elements]
-        return "".join(end_html), end_html
+                    txt = '<b>{}</b>'.format(txt)
+                if '<td></td>' == token:
+                    token = '<td>{}</td>'.format(txt)
+                else:
+                    token = '{}</td>'.format(txt)
+                td_index += 1
+            token = deal_eb_token(token)
+            end_html.append(token)
+        html = ''.join(end_html)
+        html = deal_bb(html)
+        return html, end_html
 
     def _filter_ocr_result(self, pred_bboxes, dt_boxes, rec_res):
         y1 = pred_bboxes[:, 1::2].min()
         new_dt_boxes = []
         new_rec_res = []
 
         for box, rec in zip(dt_boxes, rec_res):
```

## rapid_table/table_matcher/utils.py

```diff
@@ -22,37 +22,33 @@
     Deal with isolate span cases in this function.
     It causes by wrong prediction in structure recognition model.
     eg. predict <td rowspan="2"></td> to <td></td> rowspan="2"></b></td>.
     :param thead_part:
     :return:
     """
     # 1. find out isolate span tokens.
-    isolate_pattern = (
-        '<td></td> rowspan="(\d)+" colspan="(\d)+"></b></td>|'
-        '<td></td> colspan="(\d)+" rowspan="(\d)+"></b></td>|'
-        '<td></td> rowspan="(\d)+"></b></td>|'
-        '<td></td> colspan="(\d)+"></b></td>'
-    )
+    isolate_pattern = "<td></td> rowspan=\"(\d)+\" colspan=\"(\d)+\"></b></td>|" \
+                      "<td></td> colspan=\"(\d)+\" rowspan=\"(\d)+\"></b></td>|" \
+                      "<td></td> rowspan=\"(\d)+\"></b></td>|" \
+                      "<td></td> colspan=\"(\d)+\"></b></td>"
     isolate_iter = re.finditer(isolate_pattern, thead_part)
     isolate_list = [i.group() for i in isolate_iter]
 
     # 2. find out span number, by step 1 results.
-    span_pattern = (
-        ' rowspan="(\d)+" colspan="(\d)+"|'
-        ' colspan="(\d)+" rowspan="(\d)+"|'
-        ' rowspan="(\d)+"|'
-        ' colspan="(\d)+"'
-    )
+    span_pattern = " rowspan=\"(\d)+\" colspan=\"(\d)+\"|" \
+                   " colspan=\"(\d)+\" rowspan=\"(\d)+\"|" \
+                   " rowspan=\"(\d)+\"|" \
+                   " colspan=\"(\d)+\""
     corrected_list = []
     for isolate_item in isolate_list:
         span_part = re.search(span_pattern, isolate_item)
         spanStr_in_isolateItem = span_part.group()
         # 3. merge the span number into the span token format string.
         if spanStr_in_isolateItem is not None:
-            corrected_item = "<td{}></td>".format(spanStr_in_isolateItem)
+            corrected_item = '<td{}></td>'.format(spanStr_in_isolateItem)
             corrected_list.append(corrected_item)
         else:
             corrected_list.append(None)
 
     # 4. replace original isolated token.
     for corrected_item, isolate_item in zip(corrected_list, isolate_list):
         if corrected_item is not None:
@@ -66,33 +62,32 @@
     """
     Deal duplicate <b> or </b> after replace.
     Keep one <b></b> in a <td></td> token.
     :param thead_part:
     :return:
     """
     # 1. find out <td></td> in <thead></thead>.
-    td_pattern = (
-        '<td rowspan="(\d)+" colspan="(\d)+">(.+?)</td>|'
-        '<td colspan="(\d)+" rowspan="(\d)+">(.+?)</td>|'
-        '<td rowspan="(\d)+">(.+?)</td>|'
-        '<td colspan="(\d)+">(.+?)</td>|'
-        "<td>(.*?)</td>"
-    )
+    td_pattern = "<td rowspan=\"(\d)+\" colspan=\"(\d)+\">(.+?)</td>|" \
+                 "<td colspan=\"(\d)+\" rowspan=\"(\d)+\">(.+?)</td>|" \
+                 "<td rowspan=\"(\d)+\">(.+?)</td>|" \
+                 "<td colspan=\"(\d)+\">(.+?)</td>|" \
+                 "<td>(.*?)</td>"
     td_iter = re.finditer(td_pattern, thead_part)
     td_list = [t.group() for t in td_iter]
 
     # 2. is multiply <b></b> in <td></td> or not?
     new_td_list = []
     for td_item in td_list:
-        if td_item.count("<b>") > 1 or td_item.count("</b>") > 1:
+        if td_item.count('<b>') > 1 or td_item.count('</b>') > 1:
             # multiply <b></b> in <td></td> case.
             # 1. remove all <b></b>
-            td_item = td_item.replace("<b>", "").replace("</b>", "")
+            td_item = td_item.replace('<b>', '').replace('</b>', '')
             # 2. replace <tb> -> <tb><b>, </tb> -> </b></tb>.
-            td_item = td_item.replace("<td>", "<td><b>").replace("</td>", "</b></td>")
+            td_item = td_item.replace('<td>', '<td><b>').replace('</td>',
+                                                                 '</b></td>')
             new_td_list.append(td_item)
         else:
             new_td_list.append(td_item)
 
     # 3. replace original thead part.
     for td_item, new_td_item in zip(td_list, new_td_list):
         thead_part = thead_part.replace(td_item, new_td_item)
@@ -103,72 +98,71 @@
     """
     In our opinion, <b></b> always occurs in <thead></thead> text's context.
     This function will find out all tokens in <thead></thead> and insert <b></b> by manual.
     :param result_token:
     :return:
     """
     # find out <thead></thead> parts.
-    thead_pattern = "<thead>(.*?)</thead>"
+    thead_pattern = '<thead>(.*?)</thead>'
     if re.search(thead_pattern, result_token) is None:
         return result_token
     thead_part = re.search(thead_pattern, result_token).group()
     origin_thead_part = copy.deepcopy(thead_part)
 
     # check "rowspan" or "colspan" occur in <thead></thead> parts or not .
-    span_pattern = '<td rowspan="(\d)+" colspan="(\d)+">|<td colspan="(\d)+" rowspan="(\d)+">|<td rowspan="(\d)+">|<td colspan="(\d)+">'
+    span_pattern = "<td rowspan=\"(\d)+\" colspan=\"(\d)+\">|<td colspan=\"(\d)+\" rowspan=\"(\d)+\">|<td rowspan=\"(\d)+\">|<td colspan=\"(\d)+\">"
     span_iter = re.finditer(span_pattern, thead_part)
     span_list = [s.group() for s in span_iter]
     has_span_in_head = True if len(span_list) > 0 else False
 
     if not has_span_in_head:
         # <thead></thead> not include "rowspan" or "colspan" branch 1.
         # 1. replace <td> to <td><b>, and </td> to </b></td>
         # 2. it is possible to predict text include <b> or </b> by Text-line recognition,
         #    so we replace <b><b> to <b>, and </b></b> to </b>
-        thead_part = (
-            thead_part.replace("<td>", "<td><b>")
-            .replace("</td>", "</b></td>")
-            .replace("<b><b>", "<b>")
-            .replace("</b></b>", "</b>")
-        )
+        thead_part = thead_part.replace('<td>', '<td><b>')\
+            .replace('</td>', '</b></td>')\
+            .replace('<b><b>', '<b>')\
+            .replace('</b></b>', '</b>')
     else:
         # <thead></thead> include "rowspan" or "colspan" branch 2.
         # Firstly, we deal rowspan or colspan cases.
         # 1. replace > to ><b>
         # 2. replace </td> to </b></td>
         # 3. it is possible to predict text include <b> or </b> by Text-line recognition,
         #    so we replace <b><b> to <b>, and </b><b> to </b>
 
         # Secondly, deal ordinary cases like branch 1
 
         # replace ">" to "<b>"
         replaced_span_list = []
         for sp in span_list:
-            replaced_span_list.append(sp.replace(">", "><b>"))
+            replaced_span_list.append(sp.replace('>', '><b>'))
         for sp, rsp in zip(span_list, replaced_span_list):
             thead_part = thead_part.replace(sp, rsp)
 
         # replace "</td>" to "</b></td>"
-        thead_part = thead_part.replace("</td>", "</b></td>")
+        thead_part = thead_part.replace('</td>', '</b></td>')
 
         # remove duplicated <b> by re.sub
         mb_pattern = "(<b>)+"
         single_b_string = "<b>"
         thead_part = re.sub(mb_pattern, single_b_string, thead_part)
 
         mgb_pattern = "(</b>)+"
         single_gb_string = "</b>"
         thead_part = re.sub(mgb_pattern, single_gb_string, thead_part)
 
         # ordinary cases like branch 1
-        thead_part = thead_part.replace("<td>", "<td><b>").replace("<b><b>", "<b>")
+        thead_part = thead_part.replace('<td>', '<td><b>').replace('<b><b>',
+                                                                   '<b>')
 
     # convert <tb><b></b></tb> back to <tb></tb>, empty cell has no <b></b>.
     # but space cell(<tb> </tb>)  is suitable for <td><b> </b></td>
-    thead_part = thead_part.replace("<td><b></b></td>", "<td></td>")
+    thead_part = thead_part.replace('<td><b></b></td>', '<td></td>')
     # deal with duplicated <b></b>
     thead_part = deal_duplicate_bb(thead_part)
     # deal with isolate span tokens, which causes by wrong predict by structure prediction.
     # eg.PMC5994107_011_00.png
     thead_part = deal_isolate_span(thead_part)
     # replace original result with new thead part.
     result_token = result_token.replace(origin_thead_part, thead_part)
@@ -190,27 +184,28 @@
         "['<b>', '<i>', ' ', '</i>', '</b>']": '<eb8></eb8>',
         "['<i>', '</i>']": '<eb9></eb9>',
         "['<b>', ' ', '\\u2028', ' ', '\\u2028', ' ', '</b>']": '<eb10></eb10>',
     }
     :param master_token:
     :return:
     """
-    master_token = master_token.replace("<eb></eb>", "<td></td>")
-    master_token = master_token.replace("<eb1></eb1>", "<td> </td>")
-    master_token = master_token.replace("<eb2></eb2>", "<td><b> </b></td>")
-    master_token = master_token.replace("<eb3></eb3>", "<td>\u2028\u2028</td>")
-    master_token = master_token.replace("<eb4></eb4>", "<td><sup> </sup></td>")
-    master_token = master_token.replace("<eb5></eb5>", "<td><b></b></td>")
-    master_token = master_token.replace("<eb6></eb6>", "<td><i> </i></td>")
-    master_token = master_token.replace("<eb7></eb7>", "<td><b><i></i></b></td>")
-    master_token = master_token.replace("<eb8></eb8>", "<td><b><i> </i></b></td>")
-    master_token = master_token.replace("<eb9></eb9>", "<td><i></i></td>")
-    master_token = master_token.replace(
-        "<eb10></eb10>", "<td><b> \u2028 \u2028 </b></td>"
-    )
+    master_token = master_token.replace('<eb></eb>', '<td></td>')
+    master_token = master_token.replace('<eb1></eb1>', '<td> </td>')
+    master_token = master_token.replace('<eb2></eb2>', '<td><b> </b></td>')
+    master_token = master_token.replace('<eb3></eb3>', '<td>\u2028\u2028</td>')
+    master_token = master_token.replace('<eb4></eb4>', '<td><sup> </sup></td>')
+    master_token = master_token.replace('<eb5></eb5>', '<td><b></b></td>')
+    master_token = master_token.replace('<eb6></eb6>', '<td><i> </i></td>')
+    master_token = master_token.replace('<eb7></eb7>',
+                                        '<td><b><i></i></b></td>')
+    master_token = master_token.replace('<eb8></eb8>',
+                                        '<td><b><i> </i></b></td>')
+    master_token = master_token.replace('<eb9></eb9>', '<td><i></i></td>')
+    master_token = master_token.replace('<eb10></eb10>',
+                                        '<td><b> \u2028 \u2028 </b></td>')
     return master_token
 
 
 def distance(box_1, box_2):
     x1, y1, x2, y2 = box_1
     x3, y3, x4, y4 = box_2
     dis = abs(x3 - x1) + abs(y3 - y1) + abs(x4 - x2) + abs(y4 - y2)
```

## rapid_table/table_structure/table_structure.py

```diff
@@ -10,47 +10,48 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import time
 import numpy as np
 
-from .utils import OrtInferSession, TableLabelDecode, TablePreprocess
+from .utils import (OrtInferSession, TableLabelDecode, TablePreprocess)
 
 
-class TableStructurer:
+class TableStructurer():
     def __init__(self, model_path: str):
         self.preprocess_op = TablePreprocess()
 
         self.session = OrtInferSession(model_path)
 
         self.character = self.session.get_metadata()
         self.postprocess_op = TableLabelDecode(self.character)
 
     def __call__(self, img):
         starttime = time.time()
-        data = {"image": img}
+        data = {'image': img}
         data = self.preprocess_op(data)
         img = data[0]
         if img is None:
             return None, 0
         img = np.expand_dims(img, axis=0)
         img = img.copy()
 
         outputs = self.session(img)
 
-        preds = {"loc_preds": outputs[0], "structure_probs": outputs[1]}
+        preds = {
+            'loc_preds': outputs[0],
+            'structure_probs': outputs[1]
+        }
 
         shape_list = np.expand_dims(data[-1], axis=0)
         post_result = self.postprocess_op(preds, [shape_list])
 
-        bbox_list = post_result["bbox_batch_list"][0]
+        bbox_list = post_result['bbox_batch_list'][0]
 
-        structure_str_list = post_result["structure_batch_list"][0]
+        structure_str_list = post_result['structure_batch_list'][0]
         structure_str_list = structure_str_list[0]
-        structure_str_list = (
-            ["<html>", "<body>", "<table>"]
-            + structure_str_list
-            + ["</table>", "</body>", "</html>"]
-        )
+        structure_str_list = [
+            '<html>', '<body>', '<table>'
+        ] + structure_str_list + ['</table>', '</body>', '</html>']
         elapse = time.time() - starttime
         return (structure_str_list, bbox_list), elapse
```

## rapid_table/table_structure/utils.py

```diff
@@ -14,100 +14,99 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
 from pathlib import Path
 
 import cv2
 import numpy as np
-from onnxruntime import GraphOptimizationLevel, InferenceSession, SessionOptions
+from onnxruntime import (GraphOptimizationLevel, InferenceSession,
+                         SessionOptions)
 
 
-class OrtInferSession:
+class OrtInferSession():
     def __init__(self, onnx_path: str):
         self._verify_model(onnx_path)
 
         sess_opt = SessionOptions()
         sess_opt.log_severity_level = 4
         sess_opt.enable_cpu_mem_arena = False
         sess_opt.graph_optimization_level = GraphOptimizationLevel.ORT_ENABLE_ALL
 
-        cpu_ep = "CPUExecutionProvider"
-        cpu_provider_options = {
-            "arena_extend_strategy": "kSameAsRequested",
-        }
+        cpu_ep = 'CPUExecutionProvider'
+        cpu_provider_options = {"arena_extend_strategy": "kSameAsRequested",}
         EP_list = [(cpu_ep, cpu_provider_options)]
 
         self._verify_model(onnx_path)
-        self.session = InferenceSession(
-            onnx_path, sess_options=sess_opt, providers=EP_list
-        )
+        self.session = InferenceSession(onnx_path,
+                                        sess_options=sess_opt,
+                                        providers=EP_list)
 
     def __call__(self, input_content: np.ndarray) -> np.ndarray:
         input_dict = dict(zip(self.get_input_names(), [input_content]))
         try:
             return self.session.run(self.get_output_names(), input_dict)
         except Exception as e:
-            raise ONNXRuntimeError("ONNXRuntime inferece failed.") from e
+            raise ONNXRuntimeError('ONNXRuntime inferece failed.') from e
 
-    def get_input_names(
-        self,
-    ):
+    def get_input_names(self, ):
         return [v.name for v in self.session.get_inputs()]
 
-    def get_output_names(
-        self,
-    ):
+    def get_output_names(self,):
         return [v.name for v in self.session.get_outputs()]
 
-    def get_metadata(self, key: str = "character") -> list:
+    def get_metadata(self, key: str = 'character') -> list:
         meta_dict = self.session.get_modelmeta().custom_metadata_map
         content_list = meta_dict[key].splitlines()
         return content_list
 
     @staticmethod
     def _verify_model(model_path):
         model_path = Path(model_path)
         if not model_path.exists():
-            raise FileNotFoundError(f"{model_path} does not exists.")
+            raise FileNotFoundError(f'{model_path} does not exists.')
         if not model_path.is_file():
-            raise FileExistsError(f"{model_path} is not a file.")
+            raise FileExistsError(f'{model_path} is not a file.')
 
 
 class ONNXRuntimeError(Exception):
     pass
 
 
-class TableLabelDecode:
-    def __init__(self, dict_character, merge_no_span_structure=True, **kwargs):
+class TableLabelDecode():
+    def __init__(self,
+                 dict_character,
+                 merge_no_span_structure=True,
+                 **kwargs):
         if merge_no_span_structure:
             if "<td></td>" not in dict_character:
                 dict_character.append("<td></td>")
             if "<td>" in dict_character:
                 dict_character.remove("<td>")
 
         dict_character = self.add_special_char(dict_character)
         self.dict = {}
         for i, char in enumerate(dict_character):
             self.dict[char] = i
         self.character = dict_character
-        self.td_token = ["<td>", "<td", "<td></td>"]
+        self.td_token = ['<td>', '<td', '<td></td>']
 
     def __call__(self, preds, batch=None):
-        structure_probs = preds["structure_probs"]
-        bbox_preds = preds["loc_preds"]
+        structure_probs = preds['structure_probs']
+        bbox_preds = preds['loc_preds']
         shape_list = batch[-1]
         result = self.decode(structure_probs, bbox_preds, shape_list)
         if len(batch) == 1:  # only contains shape
             return result
 
         label_decode_result = self.decode_label(batch)
         return result, label_decode_result
 
     def decode(self, structure_probs, bbox_preds, shape_list):
-        """convert text-label into text-index."""
+        """convert text-label into text-index.
+        """
         ignored_tokens = self.get_ignored_tokens()
         end_idx = self.dict[self.end_str]
 
         structure_idx = structure_probs.argmax(axis=2)
         structure_probs = structure_probs.max(axis=2)
 
         structure_batch_list = []
@@ -131,21 +130,22 @@
                     bbox = self._bbox_decode(bbox, shape_list[batch_idx])
                     bbox_list.append(bbox)
                 structure_list.append(text)
                 score_list.append(structure_probs[batch_idx, idx])
             structure_batch_list.append([structure_list, np.mean(score_list)])
             bbox_batch_list.append(np.array(bbox_list))
         result = {
-            "bbox_batch_list": bbox_batch_list,
-            "structure_batch_list": structure_batch_list,
+            'bbox_batch_list': bbox_batch_list,
+            'structure_batch_list': structure_batch_list,
         }
         return result
 
     def decode_label(self, batch):
-        """convert text-label into text-index."""
+        """convert text-label into text-index.
+        """
         structure_idx = batch[1]
         gt_bbox_list = batch[2]
         shape_list = batch[-1]
         ignored_tokens = self.get_ignored_tokens()
         end_idx = self.dict[self.end_str]
 
         structure_batch_list = []
@@ -165,16 +165,16 @@
                 bbox = gt_bbox_list[batch_idx][idx]
                 if bbox.sum() != 0:
                     bbox = self._bbox_decode(bbox, shape_list[batch_idx])
                     bbox_list.append(bbox)
             structure_batch_list.append(structure_list)
             bbox_batch_list.append(bbox_list)
         result = {
-            "bbox_batch_list": bbox_batch_list,
-            "structure_batch_list": structure_batch_list,
+            'bbox_batch_list': bbox_batch_list,
+            'structure_batch_list': structure_batch_list,
         }
         return result
 
     def _bbox_decode(self, bbox, shape):
         h, w = shape[:2]
         bbox[0::2] *= w
         bbox[1::2] *= h
@@ -187,167 +187,159 @@
 
     def get_beg_end_flag_idx(self, beg_or_end):
         if beg_or_end == "beg":
             idx = np.array(self.dict[self.beg_str])
         elif beg_or_end == "end":
             idx = np.array(self.dict[self.end_str])
         else:
-            assert False, "unsupport type %s in get_beg_end_flag_idx" % beg_or_end
+            assert False, "unsupport type %s in get_beg_end_flag_idx" \
+                          % beg_or_end
         return idx
 
     def add_special_char(self, dict_character):
         self.beg_str = "sos"
         self.end_str = "eos"
         dict_character = [self.beg_str] + dict_character + [self.end_str]
         return dict_character
 
 
-class TablePreprocess:
+class TablePreprocess():
     def __init__(self):
         self.table_max_len = 488
         self.build_pre_process_list()
         self.ops = self.create_operators()
 
     def __call__(self, data):
-        """transform"""
+        """ transform """
         if self.ops is None:
             self.ops = []
 
         for op in self.ops:
             data = op(data)
             if data is None:
                 return None
         return data
 
-    def create_operators(
-        self,
-    ):
+    def create_operators(self,):
         """
         create operators based on the config
 
         Args:
             params(list): a dict list, used to create some operators
         """
-        assert isinstance(
-            self.pre_process_list, list
-        ), "operator config should be a list"
+        assert isinstance(self.pre_process_list, list), ('operator config should be a list')
         ops = []
         for operator in self.pre_process_list:
-            assert (
-                isinstance(operator, dict) and len(operator) == 1
-            ), "yaml format error"
+            assert isinstance(operator,
+                            dict) and len(operator) == 1, "yaml format error"
             op_name = list(operator)[0]
             param = {} if operator[op_name] is None else operator[op_name]
             op = eval(op_name)(**param)
             ops.append(op)
         return ops
 
     def build_pre_process_list(self):
-        resize_op = {
-            "ResizeTableImage": {
-                "max_len": self.table_max_len,
-            }
-        }
+        resize_op = {'ResizeTableImage': {'max_len': self.table_max_len, }}
         pad_op = {
-            "PaddingTableImage": {"size": [self.table_max_len, self.table_max_len]}
+            'PaddingTableImage': {
+                'size': [self.table_max_len, self.table_max_len]
+            }
         }
         normalize_op = {
-            "NormalizeImage": {
-                "std": [0.229, 0.224, 0.225],
-                "mean": [0.485, 0.456, 0.406],
-                "scale": "1./255.",
-                "order": "hwc",
+            'NormalizeImage': {
+                'std': [0.229, 0.224, 0.225],
+                'mean': [0.485, 0.456, 0.406],
+                'scale': '1./255.',
+                'order': 'hwc'
             }
         }
-        to_chw_op = {"ToCHWImage": None}
-        keep_keys_op = {"KeepKeys": {"keep_keys": ["image", "shape"]}}
+        to_chw_op = {'ToCHWImage': None}
+        keep_keys_op = {'KeepKeys': {'keep_keys': ['image', 'shape']}}
         self.pre_process_list = [
-            resize_op,
-            normalize_op,
-            pad_op,
-            to_chw_op,
-            keep_keys_op,
+            resize_op, normalize_op, pad_op, to_chw_op, keep_keys_op
         ]
 
 
-class ResizeTableImage:
+class ResizeTableImage():
     def __init__(self, max_len, resize_bboxes=False, infer_mode=False):
         super(ResizeTableImage, self).__init__()
         self.max_len = max_len
         self.resize_bboxes = resize_bboxes
         self.infer_mode = infer_mode
 
     def __call__(self, data):
-        img = data["image"]
+        img = data['image']
         height, width = img.shape[0:2]
         ratio = self.max_len / (max(height, width) * 1.0)
         resize_h = int(height * ratio)
         resize_w = int(width * ratio)
         resize_img = cv2.resize(img, (resize_w, resize_h))
         if self.resize_bboxes and not self.infer_mode:
-            data["bboxes"] = data["bboxes"] * ratio
-        data["image"] = resize_img
-        data["src_img"] = img
-        data["shape"] = np.array([height, width, ratio, ratio])
-        data["max_len"] = self.max_len
+            data['bboxes'] = data['bboxes'] * ratio
+        data['image'] = resize_img
+        data['src_img'] = img
+        data['shape'] = np.array([height, width, ratio, ratio])
+        data['max_len'] = self.max_len
         return data
 
 
-class PaddingTableImage:
+class PaddingTableImage():
     def __init__(self, size, **kwargs):
         super(PaddingTableImage, self).__init__()
         self.size = size
 
     def __call__(self, data):
-        img = data["image"]
+        img = data['image']
         pad_h, pad_w = self.size
         padding_img = np.zeros((pad_h, pad_w, 3), dtype=np.float32)
         height, width = img.shape[0:2]
         padding_img[0:height, 0:width, :] = img.copy()
-        data["image"] = padding_img
-        shape = data["shape"].tolist()
+        data['image'] = padding_img
+        shape = data['shape'].tolist()
         shape.extend([pad_h, pad_w])
-        data["shape"] = np.array(shape)
+        data['shape'] = np.array(shape)
         return data
 
 
-class NormalizeImage:
-    """normalize image such as substract mean, divide std"""
-
-    def __init__(self, scale=None, mean=None, std=None, order="chw", **kwargs):
+class NormalizeImage():
+    """ normalize image such as substract mean, divide std
+    """
+    def __init__(self, scale=None, mean=None, std=None, order='chw', **kwargs):
         if isinstance(scale, str):
             scale = eval(scale)
         self.scale = np.float32(scale if scale is not None else 1.0 / 255.0)
         mean = mean if mean is not None else [0.485, 0.456, 0.406]
         std = std if std is not None else [0.229, 0.224, 0.225]
 
-        shape = (3, 1, 1) if order == "chw" else (1, 1, 3)
-        self.mean = np.array(mean).reshape(shape).astype("float32")
-        self.std = np.array(std).reshape(shape).astype("float32")
+        shape = (3, 1, 1) if order == 'chw' else (1, 1, 3)
+        self.mean = np.array(mean).reshape(shape).astype('float32')
+        self.std = np.array(std).reshape(shape).astype('float32')
 
     def __call__(self, data):
-        img = np.array(data["image"])
-        assert isinstance(img, np.ndarray), "invalid input 'img' in NormalizeImage"
-        data["image"] = (img.astype("float32") * self.scale - self.mean) / self.std
+        img = np.array(data['image'])
+        assert isinstance(img,
+                        np.ndarray), "invalid input 'img' in NormalizeImage"
+        data['image'] = (
+            img.astype('float32') * self.scale - self.mean) / self.std
         return data
 
 
-class ToCHWImage:
-    """convert hwc image to chw image"""
-
+class ToCHWImage():
+    """ convert hwc image to chw image
+    """
     def __init__(self, **kwargs):
         pass
 
     def __call__(self, data):
-        img = np.array(data["image"])
-        data["image"] = img.transpose((2, 0, 1))
+        img = np.array(data['image'])
+        data['image'] = img.transpose((2, 0, 1))
         return data
 
 
-class KeepKeys:
+class KeepKeys():
     def __init__(self, keep_keys, **kwargs):
         self.keep_keys = keep_keys
 
     def __call__(self, data):
         data_list = []
         for key in self.keep_keys:
             data_list.append(data[key])
```

## Comparing `rapid_table-0.1.0.dist-info/METADATA` & `rapid_table-3.6.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,74 +1,68 @@
 Metadata-Version: 2.1
 Name: rapid-table
-Version: 0.1.0
+Version: 3.6
 Summary: Tools for parsing table structures based ONNXRuntime.
 Home-page: https://github.com/RapidAI/RapidStructure
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: ppstructure,table,rapidocr,rapid_table
 Platform: Any
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6,<3.12
+Requires-Python: >=3.6,<=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: onnxruntime (>=1.7.0)
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: opencv-python (>=4.5.1.48)
 Requires-Dist: numpy (>=1.21.6)
+Requires-Dist: rapidocr-onnxruntime (>=1.1.18)
 Requires-Dist: Pillow
 
 ## rapid-table
 <p align="left">
-    <a href=""><img src="https://img.shields.io/badge/Python->=3.6,<3.12-aff.svg"></a>
+    <a href=""><img src="https://img.shields.io/badge/Python->=3.6,<=3.11-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
     <a href="https://pypi.org/project/rapid-table/"><img alt="PyPI" src="https://img.shields.io/pypi/v/rapid-table"></a>
     <a href="https://pepy.tech/project/rapid-table"><img src="https://static.pepy.tech/personalized-badge/rapid-table?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
 </p>
 
-
 ### 1. Install package by pypi.
-⚠️Attention: After `rapid_table>=v0.1.0`, you need to install `rapidocr_onnxruntime` package firstly.
 ```bash
-pip install rapidocr_onnxruntime
-pip install rapid-table
+$ pip install rapid-table
 ```
 
 ### 2. Run by script.
 - RapidTable has the default `model_path` value, you can set the different value of `model_path` to use different models, e.g. `table_engine = RapidTable(model_path='ch_ppstructure_mobile_v2_SLANet.onnx')`
 - See details, for [README_Table](https://github.com/RapidAI/RapidStructure/blob/main/docs/README_Table.md) .
 - 📌 `table.jpg` source: [link](https://github.com/RapidAI/RapidStructure/blob/main/test_images/table.jpg)
 
-    ````python
-    from rapid_table import RapidTable
-    from rapidocr_onnxruntime import RapidOCR
-
-    table_engine = RapidTable()
-    ocr_engine = RapidOCR()
+```python
+from rapid_table import RapidTable
 
-    img_path = 'test_images/table.jpg'
+table_engine = RapidTable()
 
-    ocr_result, _ = ocr_engine(img_path)
-    table_html_str, _ = table_engine(img_path, ocr_result)
-
-    print(table_html_str)
-    ````
+with open('table.jpg', 'rb') as f:
+    img = f.read()
+table_html_str, _ = table_engine(img)
+print(table_html_str)
+```
 
 ### 3. Run by command line.
 ```bash
-rapid_table -v -img table.jpg
+$ rapid_table -v -img table.jpg
 ```
 
 ### 4. Result.
 - Return value.
     ```html
-    <html><body><table><tr><td>Methods</td><td></td><td></td><td></td><td>FPS</td></tr><tr><td>SegLink [26]</td><td>70.0</td><td>86d><td.0</td><td>77.0</td><td>8.9</td></tr><tr><td>PixelLink [4]</td><td>73.2</td><td>83.0</td><td>77.8</td><td></td></tr><tr><td>TextSnake [18]</td><td>73.9</td><td>83.2</td><td>78.3</td><td>1.1</td></tr><tr><td>TextField [37]</td><td>75.9</td><td>87.4</td><td>81.3</td><td>5.2</td></tr><tr><td>MSR[38]</td><td>76.7</td><td>87.87.4</td><td>81.7</td><td></td></tr><tr><td>FTSN [3]</td><td>77.1</td><td>87.6</td><td>82.0</td><td></td></tr><tr><td>LSE[30]</td><td>81.7</td><td>84.2</td><td>82.9</td><><ttd></td></tr><tr><td>CRAFT [2]</td><td>78.2</td><td>88.2</td><td>82.9</td><td>8.6</td></tr><tr><td>MCN[16]</td><td>79</td><td>88</td><td>83</td><td></td></tr><tr><td>ATRR</>[35]</td><td>82.1</td><td>85.2</td><td>83.6</td><td></td></tr><tr><td>PAN [34]</td><td>83.8</td><td>84.4</td><td>84.1</td><td>30.2</td></tr><tr><td>DB[12]</td><td>79.2</t91/d><td>91.5</td><td>84.9</td><td>32.0</td></tr><tr><td>DRRG[41]</td><td>82.30</td><td>88.05</td><td>85.08</td><td></td></tr><tr><td>Ours (SynText)</td><td>80.68</td><td>85<t..40</td><td>82.97</td><td>12.68</td></tr><tr><td>Ours (MLT-17)</td><td>84.54</td><td>86.62</td><td>85.57</td><td>12.31</td></tr></table></body></html>
+    <html><body><table><thead><tr><td>Methods</td><td></td><td></td><td></td><td>FPS</td></tr></thead><tbody><tr><td>SegLink [26]</td><td>70.0</td><td>86d><td.0</td><td>77.0</td><td>8.9</td></tr><tr><td>PixelLink [4]</td><td>73.2</td><td>83.0</td><td>77.8</td><td></td></tr><tr><td>TextSnake [18]</td><td>73.9</td><td>83.2</td><td>78.3</td><td>1.1</td></tr><tr><td>TextField [37]</td><td>75.9</td><td>87.4</td><td>81.3</td><td>5.2</td></tr><tr><td>MSR[38]</td><td>76.7</td><td>87.87.4</td><td>81.7</td><td></td></tr><tr><td>FTSN [3]</td><td>77.1</td><td>87.6</td><td>82.0</td><td></td></tr><tr><td>LSE[30]</td><td>81.7</td><td>84.2</td><td>82.9</td><><ttd></td></tr><tr><td>CRAFT [2]</td><td>78.2</td><td>88.2</td><td>82.9</td><td>8.6</td></tr><tr><td>MCN[16]</td><td>79</td><td>88</td><td>83</td><td></td></tr><tr><td>ATRR</>[35]</td><td>82.1</td><td>85.2</td><td>83.6</td><td></td></tr><tr><td>PAN [34]</td><td>83.8</td><td>84.4</td><td>84.1</td><td>30.2</td></tr><tr><td>DB[12]</td><td>79.2</t91/d><td>91.5</td><td>84.9</td><td>32.0</td></tr><tr><td>DRRG[41]</td><td>82.30</td><td>88.05</td><td>85.08</td><td></td></tr><tr><td>Ours (SynText)</td><td>80.68</td><td>85<t..40</td><td>82.97</td><td>12.68</td></tr><tr><td>Ours (MLT-17)</td><td>84.54</td><td>86.62</td><td>85.57</td><td>12.31</td></tr></tbody></table></body></html>
     ```
 - Visualize result.
     <div align="center">
-        <table><tr><td>Methods</td><td></td><td></td><td></td><td>FPS</td></tr><tr><td>SegLink [26]</td><td>70.0</td><td>86d><td.0</td><td>77.0</td><td>8.9</td></tr><tr><td>PixelLink [4]</td><td>73.2</td><td>83.0</td><td>77.8</td><td></td></tr><tr><td>TextSnake [18]</td><td>73.9</td><td>83.2</td><td>78.3</td><td>1.1</td></tr><tr><td>TextField [37]</td><td>75.9</td><td>87.4</td><td>81.3</td><td>5.2</td></tr><tr><td>MSR[38]</td><td>76.7</td><td>87.87.4</td><td>81.7</td><td></td></tr><tr><td>FTSN [3]</td><td>77.1</td><td>87.6</td><td>82.0</td><td></td></tr><tr><td>LSE[30]</td><td>81.7</td><td>84.2</td><td>82.9</td><><ttd></td></tr><tr><td>CRAFT [2]</td><td>78.2</td><td>88.2</td><td>82.9</td><td>8.6</td></tr><tr><td>MCN[16]</td><td>79</td><td>88</td><td>83</td><td></td></tr><tr><td>ATRR</>[35]</td><td>82.1</td><td>85.2</td><td>83.6</td><td></td></tr><tr><td>PAN [34]</td><td>83.8</td><td>84.4</td><td>84.1</td><td>30.2</td></tr><tr><td>DB[12]</td><td>79.2</t91/d><td>91.5</td><td>84.9</td><td>32.0</td></tr><tr><td>DRRG[41]</td><td>82.30</td><td>88.05</td><td>85.08</td><td></td></tr><tr><td>Ours (SynText)</td><td>80.68</td><td>85<t..40</td><td>82.97</td><td>12.68</td></tr><tr><td>Ours (MLT-17)</td><td>84.54</td><td>86.62</td><td>85.57</td><td>12.31</td></tr></table>
+        <table><thead><tr><td>Methods</td><td></td><td></td><td></td><td>FPS</td></tr></thead><tbody><tr><td>SegLink [26]</td><td>70.0</td><td>86d><td.0</td><td>77.0</td><td>8.9</td></tr><tr><td>PixelLink [4]</td><td>73.2</td><td>83.0</td><td>77.8</td><td></td></tr><tr><td>TextSnake [18]</td><td>73.9</td><td>83.2</td><td>78.3</td><td>1.1</td></tr><tr><td>TextField [37]</td><td>75.9</td><td>87.4</td><td>81.3</td><td>5.2</td></tr><tr><td>MSR[38]</td><td>76.7</td><td>87.87.4</td><td>81.7</td><td></td></tr><tr><td>FTSN [3]</td><td>77.1</td><td>87.6</td><td>82.0</td><td></td></tr><tr><td>LSE[30]</td><td>81.7</td><td>84.2</td><td>82.9</td><><ttd></td></tr><tr><td>CRAFT [2]</td><td>78.2</td><td>88.2</td><td>82.9</td><td>8.6</td></tr><tr><td>MCN[16]</td><td>79</td><td>88</td><td>83</td><td></td></tr><tr><td>ATRR</>[35]</td><td>82.1</td><td>85.2</td><td>83.6</td><td></td></tr><tr><td>PAN [34]</td><td>83.8</td><td>84.4</td><td>84.1</td><td>30.2</td></tr><tr><td>DB[12]</td><td>79.2</t91/d><td>91.5</td><td>84.9</td><td>32.0</td></tr><tr><td>DRRG[41]</td><td>82.30</td><td>88.05</td><td>85.08</td><td></td></tr><tr><td>Ours (SynText)</td><td>80.68</td><td>85<t..40</td><td>82.97</td><td>12.68</td></tr><tr><td>Ours (MLT-17)</td><td>84.54</td><td>86.62</td><td>85.57</td><td>12.31</td></tr></tbody></table>
     </div>
```

### html2text {}

```diff
@@ -1,38 +1,34 @@
-Metadata-Version: 2.1 Name: rapid-table Version: 0.1.0 Summary: Tools for
-parsing table structures based ONNXRuntime. Home-page: https://github.com/
-RapidAI/RapidStructure Author: SWHL Author-email: liekkaskono@163.com License:
-Apache-2.0 Keywords: ppstructure,table,rapidocr,rapid_table Platform: Any
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6,<3.12 Description-Content-Type: text/markdown Requires-
-Dist: onnxruntime (>=1.7.0) Requires-Dist: PyYAML (>=6.0) Requires-Dist:
-opencv-python (>=4.5.1.48) Requires-Dist: numpy (>=1.21.6) Requires-Dist:
-Pillow ## rapid-table
-[https://img.shields.io/badge/Python->=3.6,<3.12-aff.svg] [https://
+Metadata-Version: 2.1 Name: rapid-table Version: 3.6 Summary: Tools for parsing
+table structures based ONNXRuntime. Home-page: https://github.com/RapidAI/
+RapidStructure Author: SWHL Author-email: liekkaskono@163.com License: Apache-
+2.0 Keywords: ppstructure,table,rapidocr,rapid_table Platform: Any Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.6,<=3.11 Description-Content-Type: text/markdown Requires-Dist:
+onnxruntime (>=1.7.0) Requires-Dist: PyYAML (>=6.0) Requires-Dist: opencv-
+python (>=4.5.1.48) Requires-Dist: numpy (>=1.21.6) Requires-Dist: rapidocr-
+onnxruntime (>=1.1.18) Requires-Dist: Pillow ## rapid-table
+[https://img.shields.io/badge/Python->=3.6,<=3.11-aff.svg] [https://
 img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
 static.pepy.tech/personalized-badge/rapid-
 table?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
-### 1. Install package by pypi. â ï¸Attention: After `rapid_table>=v0.1.0`,
-you need to install `rapidocr_onnxruntime` package firstly. ```bash pip install
-rapidocr_onnxruntime pip install rapid-table ``` ### 2. Run by script. -
-RapidTable has the default `model_path` value, you can set the different value
-of `model_path` to use different models, e.g. `table_engine = RapidTable
-(model_path='ch_ppstructure_mobile_v2_SLANet.onnx')` - See details, for
-[README_Table](https://github.com/RapidAI/RapidStructure/blob/main/docs/
+### 1. Install package by pypi. ```bash $ pip install rapid-table ``` ### 2.
+Run by script. - RapidTable has the default `model_path` value, you can set the
+different value of `model_path` to use different models, e.g. `table_engine =
+RapidTable(model_path='ch_ppstructure_mobile_v2_SLANet.onnx')` - See details,
+for [README_Table](https://github.com/RapidAI/RapidStructure/blob/main/docs/
 README_Table.md) . - ð `table.jpg` source: [link](https://github.com/
-RapidAI/RapidStructure/blob/main/test_images/table.jpg) ````python from
-rapid_table import RapidTable from rapidocr_onnxruntime import RapidOCR
-table_engine = RapidTable() ocr_engine = RapidOCR() img_path = 'test_images/
-table.jpg' ocr_result, _ = ocr_engine(img_path) table_html_str, _ =
-table_engine(img_path, ocr_result) print(table_html_str) ```` ### 3. Run by
-command line. ```bash rapid_table -v -img table.jpg ``` ### 4. Result. - Return
-value. ```html
+RapidAI/RapidStructure/blob/main/test_images/table.jpg) ```python from
+rapid_table import RapidTable table_engine = RapidTable() with open
+('table.jpg', 'rb') as f: img = f.read() table_html_str, _ = table_engine(img)
+print(table_html_str) ``` ### 3. Run by command line. ```bash $ rapid_table -
+v -img table.jpg ``` ### 4. Result. - Return value. ```html
 Methods                            FPS
 SegLink [26]   70.0  86d>    77.0  8.9
                      0
 PixelLink [4]  73.2  83.0    77.8
 TextSnake [18] 73.9  83.2    78.3  1.1
 TextField [37] 75.9  87.4    81.3  5.2
 MSR[38]        76.7  87.87.4 81.7
```

## Comparing `rapid_table-0.1.0.dist-info/RECORD` & `rapid_table-3.6.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 rapid_table/__init__.py,sha256=qdYnOhgN-tNAExRe48Dzib6eorDhoWQTJ0FHAMws1kI,110
-rapid_table/rapid_table.py,sha256=vNfdZhFkfUhTyGTJkDX48HCP4ZPHa8B1kMsGhVjKDtk,3789
-rapid_table/utils.py,sha256=UUCWgs0kAr6afAIpsRQJoLZ2XcpxkteUo3sOQDp-z5w,2701
+rapid_table/rapid_table.py,sha256=-U88HJT20ClcKsX9-Yj3N2tAAyeRjxOkxihJ8MWqFus,2759
+rapid_table/utils.py,sha256=EERheshF9IFWMALJ1_GnANxWonGihmexZtiPHfUbm8s,2707
 rapid_table/models/en_ppstructure_mobile_v2_SLANet.onnx,sha256=LK4X0WoW-d9yKeIWZf4_vgbzyoWyAkdy7j4xQulVqmA,7704409
 rapid_table/table_matcher/__init__.py,sha256=MG5RnW1TllQdYPDoCEAWjhcAKEez44kaNHegLOW--Gk,106
-rapid_table/table_matcher/matcher.py,sha256=yiR7ekoI6Afyzfz_UvwSqYT2xfmuv7z2lXJzzB956t0,4760
-rapid_table/table_matcher/utils.py,sha256=JAPrLqiL8DAd4TDrqPNWyYWZ3EajjBPLMHtRtnDYDtU,9671
+rapid_table/table_matcher/matcher.py,sha256=A8gVZ2XQJqWA87HK5b-_Ql8raY94rauS9g3QOjnha6w,6670
+rapid_table/table_matcher/utils.py,sha256=2TbkdclD0Y9lOVO_xuqlGcdR_kVwpuAYW4eu3UJwUvA,10019
 rapid_table/table_structure/__init__.py,sha256=N_1OGAgiMrF4LB5_sP_OSOrh6pnBGZrrnph8RfQ3VHA,653
-rapid_table/table_structure/table_structure.py,sha256=EiaP5PgGtGYN1Y5Y5enqp452izgc4tCP5xzH_wg-2yc,1933
-rapid_table/table_structure/utils.py,sha256=ND2T1qlF90uVUbsONUAkfvjabUdgjeJn-leC6OK24_8,11920
-rapid_table-0.1.0.dist-info/METADATA,sha256=QO3lS7tp8pzJ9-7LZkpO4DxmobOc8Zcpgi26zAenXf4,5141
-rapid_table-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rapid_table-0.1.0.dist-info/entry_points.txt,sha256=a4UsMSxd7Ex1mZvdIT5AmkuiUAvB__awLj-NeYU8bsQ,61
-rapid_table-0.1.0.dist-info/top_level.txt,sha256=DkBPZpaze8SaoAvCufxilNpITY4n-rHH1lgHr6KHPgA,12
-rapid_table-0.1.0.dist-info/RECORD,,
+rapid_table/table_structure/table_structure.py,sha256=0QyKU9c6J-H5kCGET09NVjkHV-xa5pMC-JERvMnY-Ow,1945
+rapid_table/table_structure/utils.py,sha256=fDK5G9N6DfG-IGE_fZ4l85ypjXSR33cK4R5P5X5l1Ws,12009
+rapid_table-3.6.dist-info/METADATA,sha256=e83v94q0OqFaLMB5fOatNvPnY_AiwvuLwhICSDVyJvo,4967
+rapid_table-3.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rapid_table-3.6.dist-info/entry_points.txt,sha256=a4UsMSxd7Ex1mZvdIT5AmkuiUAvB__awLj-NeYU8bsQ,61
+rapid_table-3.6.dist-info/top_level.txt,sha256=DkBPZpaze8SaoAvCufxilNpITY4n-rHH1lgHr6KHPgA,12
+rapid_table-3.6.dist-info/RECORD,,
```

