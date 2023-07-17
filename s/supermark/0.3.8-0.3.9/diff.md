# Comparing `tmp/supermark-0.3.8.tar.gz` & `tmp/supermark-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supermark-0.3.8.tar", last modified: Mon Dec 13 20:30:25 2021, max compression
+gzip compressed data, was "supermark-0.3.9.tar", last modified: Sun Feb 27 14:23:26 2022, max compression
```

## Comparing `supermark-0.3.8.tar` & `supermark-0.3.9.tar`

### file list

```diff
@@ -1,126 +1,135 @@
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.683465 supermark-0.3.8/
--rw-r--r--   0 kraemer    (501) staff       (20)      891 2021-12-13 20:30:25.683757 supermark-0.3.8/PKG-INFO
--rw-r--r--   0 kraemer    (501) staff       (20)       40 2017-11-26 20:50:12.000000 supermark-0.3.8/setup.cfg
--rw-r--r--   0 kraemer    (501) staff       (20)     3255 2021-12-12 19:42:46.534831 supermark-0.3.8/setup.py
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.570080 supermark-0.3.8/supermark/
--rw-r--r--   0 kraemer    (501) staff       (20)      596 2021-12-13 20:30:01.702307 supermark-0.3.8/supermark/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)     1121 2021-08-03 16:31:58.403868 supermark-0.3.8/supermark/base.py
--rw-r--r--   0 kraemer    (501) staff       (20)     8781 2021-11-14 08:32:49.000000 supermark-0.3.8/supermark/build_html.py
--rw-r--r--   0 kraemer    (501) staff       (20)     5007 2021-07-11 12:54:57.796553 supermark-0.3.8/supermark/build_latex.py
--rw-r--r--   0 kraemer    (501) staff       (20)    13940 2021-12-13 18:18:39.520563 supermark-0.3.8/supermark/chunks.py
--rw-r--r--   0 kraemer    (501) staff       (20)     2029 2021-07-28 21:02:05.243732 supermark-0.3.8/supermark/code.py
--rw-r--r--   0 kraemer    (501) staff       (20)     4588 2021-11-14 21:12:14.354519 supermark-0.3.8/supermark/command.py
--rw-r--r--   0 kraemer    (501) staff       (20)     9279 2021-11-13 19:06:59.000000 supermark-0.3.8/supermark/core.py
--rw-r--r--   0 kraemer    (501) staff       (20)     4587 2021-07-30 10:07:30.511454 supermark-0.3.8/supermark/extend.py
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.570964 supermark-0.3.8/supermark/extensions/
--rw-r--r--   0 kraemer    (501) staff       (20)        1 2021-07-28 21:43:35.677365 supermark-0.3.8/supermark/extensions/__init__.py
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.573207 supermark-0.3.8/supermark/extensions/abstract/
--rw-r--r--   0 kraemer    (501) staff       (20)      176 2021-08-01 08:25:18.960233 supermark-0.3.8/supermark/extensions/abstract/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)       59 2021-08-01 08:27:40.835777 supermark-0.3.8/supermark/extensions/abstract/abstract.css
--rw-r--r--   0 kraemer    (501) staff       (20)       10 2021-08-01 08:24:59.560820 supermark-0.3.8/supermark/extensions/abstract/doc.md
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.574863 supermark-0.3.8/supermark/extensions/boxes/
--rw-r--r--   0 kraemer    (501) staff       (20)      175 2021-07-28 09:10:55.879880 supermark-0.3.8/supermark/extensions/boxes/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      106 2021-07-28 09:11:33.932233 supermark-0.3.8/supermark/extensions/boxes/boxes.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.576447 supermark-0.3.8/supermark/extensions/button/
--rw-r--r--   0 kraemer    (501) staff       (20)      811 2021-07-20 16:58:17.715938 supermark-0.3.8/supermark/extensions/button/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      547 2021-03-06 19:00:29.082771 supermark-0.3.8/supermark/extensions/button/button.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.579585 supermark-0.3.8/supermark/extensions/check/
--rw-r--r--   0 kraemer    (501) staff       (20)      167 2021-07-28 09:36:05.647441 supermark-0.3.8/supermark/extensions/check/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      334 2021-07-28 08:12:33.136427 supermark-0.3.8/supermark/extensions/check/check.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.582305 supermark-0.3.8/supermark/extensions/checklistbox/
--rw-r--r--   0 kraemer    (501) staff       (20)      152 2021-11-21 13:36:38.000000 supermark-0.3.8/supermark/extensions/checklistbox/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      545 2021-11-21 13:36:56.000000 supermark-0.3.8/supermark/extensions/checklistbox/checklistbox.css
--rw-r--r--   0 kraemer    (501) staff       (20)      103 2021-07-30 07:23:09.000000 supermark-0.3.8/supermark/extensions/checklistbox/doc.md
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.583725 supermark-0.3.8/supermark/extensions/code/
--rw-r--r--   0 kraemer    (501) staff       (20)     1835 2021-03-06 18:54:18.371080 supermark-0.3.8/supermark/extensions/code/code.css
--rw-r--r--   0 kraemer    (501) staff       (20)     1482 2021-07-30 06:56:32.442594 supermark-0.3.8/supermark/extensions/code/doc.md
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.585338 supermark-0.3.8/supermark/extensions/coursetable/
--rw-r--r--   0 kraemer    (501) staff       (20)      173 2021-11-20 20:39:51.000000 supermark-0.3.8/supermark/extensions/coursetable/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      678 2021-11-21 14:35:10.000000 supermark-0.3.8/supermark/extensions/coursetable/coursetable.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.587344 supermark-0.3.8/supermark/extensions/definition/
--rw-r--r--   0 kraemer    (501) staff       (20)      156 2021-08-01 08:36:07.406930 supermark-0.3.8/supermark/extensions/definition/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      305 2021-08-01 08:35:55.129520 supermark-0.3.8/supermark/extensions/definition/definition.css
--rw-r--r--   0 kraemer    (501) staff       (20)       10 2021-08-01 08:24:59.560820 supermark-0.3.8/supermark/extensions/definition/doc.md
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.590000 supermark-0.3.8/supermark/extensions/delivery/
--rw-r--r--   0 kraemer    (501) staff       (20)      152 2021-07-30 09:33:02.167446 supermark-0.3.8/supermark/extensions/delivery/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      334 2021-07-30 09:33:14.888927 supermark-0.3.8/supermark/extensions/delivery/delivery.css
--rw-r--r--   0 kraemer    (501) staff       (20)      179 2021-07-30 07:22:28.660264 supermark-0.3.8/supermark/extensions/delivery/doc.md
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.592845 supermark-0.3.8/supermark/extensions/double/
--rw-r--r--   0 kraemer    (501) staff       (20)      148 2021-08-01 08:46:26.375147 supermark-0.3.8/supermark/extensions/double/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)       10 2021-08-01 08:24:59.560820 supermark-0.3.8/supermark/extensions/double/doc.md
--rw-r--r--   0 kraemer    (501) staff       (20)       30 2021-08-01 08:46:10.176225 supermark-0.3.8/supermark/extensions/double/double.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.597139 supermark-0.3.8/supermark/extensions/figure/
--rw-r--r--   0 kraemer    (501) staff       (20)     4723 2021-07-28 18:05:13.174834 supermark-0.3.8/supermark/extensions/figure/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      249 2021-07-29 22:16:53.216039 supermark-0.3.8/supermark/extensions/figure/doc.md
--rw-r--r--   0 kraemer    (501) staff       (20)      156 2021-07-13 06:43:45.501000 supermark-0.3.8/supermark/extensions/figure/example.md
--rw-r--r--   0 kraemer    (501) staff       (20)      167 2021-07-21 10:07:58.236446 supermark-0.3.8/supermark/extensions/figure/figure.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.599643 supermark-0.3.8/supermark/extensions/goals/
--rw-r--r--   0 kraemer    (501) staff       (20)      146 2021-07-28 07:50:04.492850 supermark-0.3.8/supermark/extensions/goals/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      173 2021-07-30 07:16:48.786620 supermark-0.3.8/supermark/extensions/goals/doc.md
--rw-r--r--   0 kraemer    (501) staff       (20)      334 2021-03-06 18:15:54.562299 supermark-0.3.8/supermark/extensions/goals/goals.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.601887 supermark-0.3.8/supermark/extensions/guideline/
--rw-r--r--   0 kraemer    (501) staff       (20)      154 2021-08-01 08:35:03.989010 supermark-0.3.8/supermark/extensions/guideline/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)       10 2021-08-01 08:24:59.560820 supermark-0.3.8/supermark/extensions/guideline/doc.md
--rw-r--r--   0 kraemer    (501) staff       (20)      292 2021-08-01 08:33:56.674274 supermark-0.3.8/supermark/extensions/guideline/guideline.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.604242 supermark-0.3.8/supermark/extensions/hints/
--rw-r--r--   0 kraemer    (501) staff       (20)     1980 2021-07-28 18:16:55.194071 supermark-0.3.8/supermark/extensions/hints/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      850 2021-07-30 07:17:19.732416 supermark-0.3.8/supermark/extensions/hints/doc.md
--rw-r--r--   0 kraemer    (501) staff       (20)      442 2021-03-06 18:31:38.027474 supermark-0.3.8/supermark/extensions/hints/hints.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.604771 supermark-0.3.8/supermark/extensions/lines/
--rw-r--r--   0 kraemer    (501) staff       (20)      772 2021-08-01 08:43:11.245407 supermark-0.3.8/supermark/extensions/lines/__init__.py
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.606679 supermark-0.3.8/supermark/extensions/qna/
--rw-r--r--   0 kraemer    (501) staff       (20)     1588 2021-12-13 19:55:19.550512 supermark-0.3.8/supermark/extensions/qna/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      273 2021-12-13 20:06:17.922352 supermark-0.3.8/supermark/extensions/qna/qna.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.608134 supermark-0.3.8/supermark/extensions/rat/
--rw-r--r--   0 kraemer    (501) staff       (20)      142 2021-07-18 06:52:26.991358 supermark-0.3.8/supermark/extensions/rat/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)       46 2021-03-06 18:55:29.224764 supermark-0.3.8/supermark/extensions/rat/rat.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.610714 supermark-0.3.8/supermark/extensions/report/
--rw-r--r--   0 kraemer    (501) staff       (20)      148 2021-07-28 09:27:05.139210 supermark-0.3.8/supermark/extensions/report/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      230 2021-07-28 09:26:51.876894 supermark-0.3.8/supermark/extensions/report/report.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.612954 supermark-0.3.8/supermark/extensions/rubrics/
--rw-r--r--   0 kraemer    (501) staff       (20)      172 2021-07-28 21:45:07.099919 supermark-0.3.8/supermark/extensions/rubrics/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)     1920 2021-03-06 18:50:46.656566 supermark-0.3.8/supermark/extensions/rubrics/rubric.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.616203 supermark-0.3.8/supermark/extensions/steplist/
--rw-r--r--   0 kraemer    (501) staff       (20)      149 2021-11-21 20:01:49.437880 supermark-0.3.8/supermark/extensions/steplist/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)     4061 2021-07-30 07:21:47.292453 supermark-0.3.8/supermark/extensions/steplist/doc.md
--rw-r--r--   0 kraemer    (501) staff       (20)      586 2021-11-21 18:47:03.037000 supermark-0.3.8/supermark/extensions/steplist/steplist.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.619035 supermark-0.3.8/supermark/extensions/steps/
--rw-r--r--   0 kraemer    (501) staff       (20)      146 2021-07-27 12:58:29.516413 supermark-0.3.8/supermark/extensions/steps/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)     4061 2021-07-30 07:21:47.292453 supermark-0.3.8/supermark/extensions/steps/doc.md
--rw-r--r--   0 kraemer    (501) staff       (20)      689 2021-07-27 12:59:07.331165 supermark-0.3.8/supermark/extensions/steps/steps.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.621075 supermark-0.3.8/supermark/extensions/table/
--rw-r--r--   0 kraemer    (501) staff       (20)     7566 2021-11-20 21:25:00.000000 supermark-0.3.8/supermark/extensions/table/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      672 2021-07-30 06:52:26.153754 supermark-0.3.8/supermark/extensions/table/doc.md
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.622570 supermark-0.3.8/supermark/extensions/task/
--rw-r--r--   0 kraemer    (501) staff       (20)      144 2021-07-28 09:28:42.649524 supermark-0.3.8/supermark/extensions/task/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      188 2021-07-28 09:28:33.641000 supermark-0.3.8/supermark/extensions/task/task.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.625272 supermark-0.3.8/supermark/extensions/tips/
--rw-r--r--   0 kraemer    (501) staff       (20)      164 2021-07-23 19:04:45.556122 supermark-0.3.8/supermark/extensions/tips/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      103 2021-07-30 07:23:09.967390 supermark-0.3.8/supermark/extensions/tips/doc.md
--rw-r--r--   0 kraemer    (501) staff       (20)      114 2021-07-28 07:50:25.662047 supermark-0.3.8/supermark/extensions/tips/tips.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.636170 supermark-0.3.8/supermark/extensions/tipsbox/
--rw-r--r--   0 kraemer    (501) staff       (20)      147 2021-11-21 13:34:55.000000 supermark-0.3.8/supermark/extensions/tipsbox/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      493 2021-11-21 13:46:36.000000 supermark-0.3.8/supermark/extensions/tipsbox/tipsbox.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.646996 supermark-0.3.8/supermark/extensions/tree/
--rw-r--r--   0 kraemer    (501) staff       (20)      144 2021-07-29 07:16:08.080458 supermark-0.3.8/supermark/extensions/tree/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      538 2021-07-29 07:15:14.032000 supermark-0.3.8/supermark/extensions/tree/tree.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.662847 supermark-0.3.8/supermark/extensions/video/
--rw-r--r--   0 kraemer    (501) staff       (20)     4624 2021-07-28 18:20:02.742540 supermark-0.3.8/supermark/extensions/video/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      260 2021-07-30 06:51:45.634459 supermark-0.3.8/supermark/extensions/video/doc.md
--rw-r--r--   0 kraemer    (501) staff       (20)       80 2021-07-13 06:46:42.410890 supermark-0.3.8/supermark/extensions/video/example-00.md
--rw-r--r--   0 kraemer    (501) staff       (20)       96 2021-07-13 06:46:39.405215 supermark-0.3.8/supermark/extensions/video/example-01.md
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.668411 supermark-0.3.8/supermark/extensions/warning/
--rw-r--r--   0 kraemer    (501) staff       (20)      171 2021-07-28 09:20:53.275766 supermark-0.3.8/supermark/extensions/warning/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      179 2021-07-30 07:22:28.660264 supermark-0.3.8/supermark/extensions/warning/doc.md
--rw-r--r--   0 kraemer    (501) staff       (20)      239 2021-07-28 09:19:11.754769 supermark-0.3.8/supermark/extensions/warning/warning.css
-drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2021-12-13 20:30:25.683049 supermark-0.3.8/supermark/extensions/weekplan/
--rw-r--r--   0 kraemer    (501) staff       (20)      230 2021-08-24 10:54:12.000000 supermark-0.3.8/supermark/extensions/weekplan/__init__.py
--rw-r--r--   0 kraemer    (501) staff       (20)      314 2021-05-24 14:54:38.848910 supermark-0.3.8/supermark/extensions/weekplan/example.md
--rw-r--r--   0 kraemer    (501) staff       (20)      409 2021-11-20 18:06:09.841986 supermark-0.3.8/supermark/extensions/weekplan/weekplan.css
--rw-r--r--   0 kraemer    (501) staff       (20)      151 2021-05-24 14:52:31.855466 supermark-0.3.8/supermark/extensions/weekplan/weekplan.md
--rw-r--r--   0 kraemer    (501) staff       (20)     1083 2021-07-29 22:01:28.014012 supermark-0.3.8/supermark/pandoc.py
--rw-r--r--   0 kraemer    (501) staff       (20)     8467 2021-11-13 19:22:45.000000 supermark-0.3.8/supermark/parse.py
--rw-r--r--   0 kraemer    (501) staff       (20)     7430 2021-09-03 19:13:59.256893 supermark-0.3.8/supermark/report.py
--rw-r--r--   0 kraemer    (501) staff       (20)     1146 2021-11-14 20:17:12.968039 supermark-0.3.8/supermark/setup.py
--rw-r--r--   0 kraemer    (501) staff       (20)     5148 2021-07-28 09:12:56.282231 supermark-0.3.8/supermark/style.css
--rw-r--r--   0 kraemer    (501) staff       (20)     1716 2021-07-18 08:36:19.088834 supermark-0.3.8/supermark/utils.py
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.912725 supermark-0.3.9/
+-rw-r--r--   0 kraemer    (501) staff       (20)      694 2022-02-27 14:23:26.912820 supermark-0.3.9/PKG-INFO
+-rw-r--r--   0 kraemer    (501) staff       (20)       40 2017-11-26 20:50:12.000000 supermark-0.3.9/setup.cfg
+-rw-r--r--   0 kraemer    (501) staff       (20)     3151 2022-01-16 21:12:53.196278 supermark-0.3.9/setup.py
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.896967 supermark-0.3.9/supermark/
+-rw-r--r--   0 kraemer    (501) staff       (20)      596 2022-02-27 14:23:22.325187 supermark-0.3.9/supermark/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     1213 2022-01-16 21:12:53.196571 supermark-0.3.9/supermark/base.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     9016 2022-01-16 21:12:53.196751 supermark-0.3.9/supermark/build_html.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     5007 2022-01-16 21:12:53.196906 supermark-0.3.9/supermark/build_latex.py
+-rw-r--r--   0 kraemer    (501) staff       (20)    13940 2022-01-16 21:12:53.197091 supermark-0.3.9/supermark/chunks.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     2029 2022-01-16 21:12:53.197233 supermark-0.3.9/supermark/code.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     5539 2022-01-16 21:28:14.636492 supermark-0.3.9/supermark/command.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     9517 2022-01-16 21:12:53.197561 supermark-0.3.9/supermark/core.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     4589 2022-01-16 21:40:15.523899 supermark-0.3.9/supermark/extend.py
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.897157 supermark-0.3.9/supermark/extensions/
+-rw-r--r--   0 kraemer    (501) staff       (20)        1 2022-01-16 21:12:53.200509 supermark-0.3.9/supermark/extensions/__init__.py
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.897705 supermark-0.3.9/supermark/extensions/abstract/
+-rw-r--r--   0 kraemer    (501) staff       (20)      176 2022-01-16 21:12:53.200628 supermark-0.3.9/supermark/extensions/abstract/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)       59 2022-01-16 21:12:53.200728 supermark-0.3.9/supermark/extensions/abstract/abstract.css
+-rw-r--r--   0 kraemer    (501) staff       (20)       10 2022-01-16 21:12:53.200819 supermark-0.3.9/supermark/extensions/abstract/doc.md
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.898063 supermark-0.3.9/supermark/extensions/boxes/
+-rw-r--r--   0 kraemer    (501) staff       (20)      175 2022-01-16 21:12:53.200931 supermark-0.3.9/supermark/extensions/boxes/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      106 2022-01-16 21:12:53.201036 supermark-0.3.9/supermark/extensions/boxes/boxes.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.898440 supermark-0.3.9/supermark/extensions/button/
+-rw-r--r--   0 kraemer    (501) staff       (20)      811 2022-01-16 21:12:53.201166 supermark-0.3.9/supermark/extensions/button/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      548 2022-01-16 21:25:06.722774 supermark-0.3.9/supermark/extensions/button/button.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.898787 supermark-0.3.9/supermark/extensions/check/
+-rw-r--r--   0 kraemer    (501) staff       (20)      167 2022-01-16 21:12:53.201378 supermark-0.3.9/supermark/extensions/check/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      334 2022-01-16 21:12:53.201475 supermark-0.3.9/supermark/extensions/check/check.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.899331 supermark-0.3.9/supermark/extensions/checklistbox/
+-rw-r--r--   0 kraemer    (501) staff       (20)      152 2022-01-16 21:12:53.201602 supermark-0.3.9/supermark/extensions/checklistbox/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      568 2022-01-17 19:38:03.696256 supermark-0.3.9/supermark/extensions/checklistbox/checklistbox.css
+-rw-r--r--   0 kraemer    (501) staff       (20)      103 2022-01-16 21:12:53.201793 supermark-0.3.9/supermark/extensions/checklistbox/doc.md
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.899668 supermark-0.3.9/supermark/extensions/code/
+-rw-r--r--   0 kraemer    (501) staff       (20)     1835 2022-01-16 21:12:53.203730 supermark-0.3.9/supermark/extensions/code/code.css
+-rw-r--r--   0 kraemer    (501) staff       (20)     1482 2022-01-16 21:12:53.203930 supermark-0.3.9/supermark/extensions/code/doc.md
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.900165 supermark-0.3.9/supermark/extensions/coursetable/
+-rw-r--r--   0 kraemer    (501) staff       (20)      173 2022-01-16 21:12:53.204219 supermark-0.3.9/supermark/extensions/coursetable/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     1358 2022-01-16 21:12:53.204361 supermark-0.3.9/supermark/extensions/coursetable/coursetable.css
+-rw-r--r--   0 kraemer    (501) staff       (20)      943 2022-01-16 21:12:53.204481 supermark-0.3.9/supermark/extensions/coursetable/doc.md
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.900667 supermark-0.3.9/supermark/extensions/definition/
+-rw-r--r--   0 kraemer    (501) staff       (20)      156 2022-01-16 21:12:53.204600 supermark-0.3.9/supermark/extensions/definition/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      305 2022-01-16 21:12:53.224918 supermark-0.3.9/supermark/extensions/definition/definition.css
+-rw-r--r--   0 kraemer    (501) staff       (20)       10 2022-01-16 21:12:53.225149 supermark-0.3.9/supermark/extensions/definition/doc.md
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.901167 supermark-0.3.9/supermark/extensions/delivery/
+-rw-r--r--   0 kraemer    (501) staff       (20)      152 2022-01-16 21:12:53.225296 supermark-0.3.9/supermark/extensions/delivery/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      334 2022-01-16 21:12:53.225416 supermark-0.3.9/supermark/extensions/delivery/delivery.css
+-rw-r--r--   0 kraemer    (501) staff       (20)      179 2022-01-16 21:12:53.226309 supermark-0.3.9/supermark/extensions/delivery/doc.md
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.901750 supermark-0.3.9/supermark/extensions/double/
+-rw-r--r--   0 kraemer    (501) staff       (20)      148 2022-01-16 21:12:53.226443 supermark-0.3.9/supermark/extensions/double/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)       10 2022-01-16 21:12:53.226528 supermark-0.3.9/supermark/extensions/double/doc.md
+-rw-r--r--   0 kraemer    (501) staff       (20)       30 2022-01-16 21:12:53.226634 supermark-0.3.9/supermark/extensions/double/double.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.902443 supermark-0.3.9/supermark/extensions/figure/
+-rw-r--r--   0 kraemer    (501) staff       (20)     4737 2022-01-16 21:12:53.239771 supermark-0.3.9/supermark/extensions/figure/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      249 2022-01-16 21:12:53.227057 supermark-0.3.9/supermark/extensions/figure/doc.md
+-rw-r--r--   0 kraemer    (501) staff       (20)      156 2022-01-16 21:12:53.227165 supermark-0.3.9/supermark/extensions/figure/example.md
+-rw-r--r--   0 kraemer    (501) staff       (20)      167 2022-01-16 21:12:53.227253 supermark-0.3.9/supermark/extensions/figure/figure.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.903024 supermark-0.3.9/supermark/extensions/goals/
+-rw-r--r--   0 kraemer    (501) staff       (20)      146 2022-01-16 21:12:53.227344 supermark-0.3.9/supermark/extensions/goals/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      173 2022-01-16 21:12:53.227428 supermark-0.3.9/supermark/extensions/goals/doc.md
+-rw-r--r--   0 kraemer    (501) staff       (20)      334 2022-01-16 21:12:53.227601 supermark-0.3.9/supermark/extensions/goals/goals.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.903856 supermark-0.3.9/supermark/extensions/guideline/
+-rw-r--r--   0 kraemer    (501) staff       (20)      154 2022-01-16 21:12:53.227743 supermark-0.3.9/supermark/extensions/guideline/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)       10 2022-01-16 21:12:53.227884 supermark-0.3.9/supermark/extensions/guideline/doc.md
+-rw-r--r--   0 kraemer    (501) staff       (20)      292 2022-01-16 21:12:53.227989 supermark-0.3.9/supermark/extensions/guideline/guideline.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.904489 supermark-0.3.9/supermark/extensions/hints/
+-rw-r--r--   0 kraemer    (501) staff       (20)     1980 2022-01-16 21:12:53.228095 supermark-0.3.9/supermark/extensions/hints/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      850 2022-01-16 21:12:53.228188 supermark-0.3.9/supermark/extensions/hints/doc.md
+-rw-r--r--   0 kraemer    (501) staff       (20)      442 2022-01-16 21:12:53.228365 supermark-0.3.9/supermark/extensions/hints/hints.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.904794 supermark-0.3.9/supermark/extensions/lines/
+-rw-r--r--   0 kraemer    (501) staff       (20)      772 2022-01-16 21:12:53.228459 supermark-0.3.9/supermark/extensions/lines/__init__.py
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.905301 supermark-0.3.9/supermark/extensions/qna/
+-rw-r--r--   0 kraemer    (501) staff       (20)     1588 2022-01-16 21:12:53.228562 supermark-0.3.9/supermark/extensions/qna/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      257 2022-01-16 21:32:43.854662 supermark-0.3.9/supermark/extensions/qna/qna.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.906541 supermark-0.3.9/supermark/extensions/quiz/
+-rw-r--r--   0 kraemer    (501) staff       (20)     4609 2022-01-16 21:12:53.228820 supermark-0.3.9/supermark/extensions/quiz/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      260 2022-01-16 21:12:53.228911 supermark-0.3.9/supermark/extensions/quiz/doc.md
+-rw-r--r--   0 kraemer    (501) staff       (20)      428 2022-01-16 21:12:53.229014 supermark-0.3.9/supermark/extensions/quiz/example-00.md
+-rw-r--r--   0 kraemer    (501) staff       (20)      457 2022-01-16 21:12:53.229117 supermark-0.3.9/supermark/extensions/quiz/example-01.md
+-rw-r--r--   0 kraemer    (501) staff       (20)     1554 2022-01-16 21:12:53.229215 supermark-0.3.9/supermark/extensions/quiz/example-02.md
+-rw-r--r--   0 kraemer    (501) staff       (20)     1139 2022-01-16 21:12:53.229312 supermark-0.3.9/supermark/extensions/quiz/quiz.css
+-rw-r--r--   0 kraemer    (501) staff       (20)     2318 2022-01-16 21:12:53.229418 supermark-0.3.9/supermark/extensions/quiz/quiz.js
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.906880 supermark-0.3.9/supermark/extensions/rat/
+-rw-r--r--   0 kraemer    (501) staff       (20)      142 2022-01-16 21:12:53.229530 supermark-0.3.9/supermark/extensions/rat/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)       46 2022-01-16 21:12:53.229621 supermark-0.3.9/supermark/extensions/rat/rat.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.907223 supermark-0.3.9/supermark/extensions/report/
+-rw-r--r--   0 kraemer    (501) staff       (20)      148 2022-01-16 21:12:53.229711 supermark-0.3.9/supermark/extensions/report/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      230 2022-01-16 21:12:53.229814 supermark-0.3.9/supermark/extensions/report/report.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.907608 supermark-0.3.9/supermark/extensions/rubrics/
+-rw-r--r--   0 kraemer    (501) staff       (20)      172 2022-01-16 21:12:53.229918 supermark-0.3.9/supermark/extensions/rubrics/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     1920 2022-01-16 21:36:56.511846 supermark-0.3.9/supermark/extensions/rubrics/rubric.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.908182 supermark-0.3.9/supermark/extensions/steplist/
+-rw-r--r--   0 kraemer    (501) staff       (20)      149 2022-01-16 21:12:53.230104 supermark-0.3.9/supermark/extensions/steplist/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     4061 2022-01-16 21:12:53.230205 supermark-0.3.9/supermark/extensions/steplist/doc.md
+-rw-r--r--   0 kraemer    (501) staff       (20)      586 2022-01-16 21:12:53.230300 supermark-0.3.9/supermark/extensions/steplist/steplist.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.908888 supermark-0.3.9/supermark/extensions/steps/
+-rw-r--r--   0 kraemer    (501) staff       (20)      146 2022-01-16 21:12:53.230388 supermark-0.3.9/supermark/extensions/steps/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     4061 2022-01-16 21:12:53.230485 supermark-0.3.9/supermark/extensions/steps/doc.md
+-rw-r--r--   0 kraemer    (501) staff       (20)      538 2022-01-16 21:35:02.452595 supermark-0.3.9/supermark/extensions/steps/steps.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.909222 supermark-0.3.9/supermark/extensions/table/
+-rw-r--r--   0 kraemer    (501) staff       (20)     7566 2022-01-16 21:12:53.230703 supermark-0.3.9/supermark/extensions/table/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      672 2022-01-16 21:12:53.230792 supermark-0.3.9/supermark/extensions/table/doc.md
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.909560 supermark-0.3.9/supermark/extensions/task/
+-rw-r--r--   0 kraemer    (501) staff       (20)      144 2022-01-16 21:12:53.230880 supermark-0.3.9/supermark/extensions/task/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      188 2022-01-16 21:12:53.230963 supermark-0.3.9/supermark/extensions/task/task.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.910063 supermark-0.3.9/supermark/extensions/tips/
+-rw-r--r--   0 kraemer    (501) staff       (20)      164 2022-01-16 21:12:53.231050 supermark-0.3.9/supermark/extensions/tips/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      103 2022-01-16 21:12:53.231126 supermark-0.3.9/supermark/extensions/tips/doc.md
+-rw-r--r--   0 kraemer    (501) staff       (20)      114 2022-01-16 21:12:53.231305 supermark-0.3.9/supermark/extensions/tips/tips.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.910415 supermark-0.3.9/supermark/extensions/tipsbox/
+-rw-r--r--   0 kraemer    (501) staff       (20)      147 2022-01-16 21:12:53.231394 supermark-0.3.9/supermark/extensions/tipsbox/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      493 2022-01-16 21:12:53.231606 supermark-0.3.9/supermark/extensions/tipsbox/tipsbox.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.910747 supermark-0.3.9/supermark/extensions/tree/
+-rw-r--r--   0 kraemer    (501) staff       (20)      144 2022-01-16 21:12:53.231703 supermark-0.3.9/supermark/extensions/tree/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      538 2022-01-16 21:12:53.231791 supermark-0.3.9/supermark/extensions/tree/tree.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.911461 supermark-0.3.9/supermark/extensions/video/
+-rw-r--r--   0 kraemer    (501) staff       (20)     4624 2022-01-16 21:12:53.239498 supermark-0.3.9/supermark/extensions/video/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      260 2022-01-16 21:12:53.231983 supermark-0.3.9/supermark/extensions/video/doc.md
+-rw-r--r--   0 kraemer    (501) staff       (20)       80 2022-01-16 21:12:53.232060 supermark-0.3.9/supermark/extensions/video/example-00.md
+-rw-r--r--   0 kraemer    (501) staff       (20)       96 2022-01-16 21:12:53.232147 supermark-0.3.9/supermark/extensions/video/example-01.md
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.911988 supermark-0.3.9/supermark/extensions/warning/
+-rw-r--r--   0 kraemer    (501) staff       (20)      171 2022-01-16 21:12:53.232235 supermark-0.3.9/supermark/extensions/warning/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      179 2022-01-16 21:12:53.232325 supermark-0.3.9/supermark/extensions/warning/doc.md
+-rw-r--r--   0 kraemer    (501) staff       (20)      239 2022-01-16 21:12:53.232408 supermark-0.3.9/supermark/extensions/warning/warning.css
+drwxr-xr-x   0 kraemer    (501) staff       (20)        0 2022-02-27 14:23:26.912679 supermark-0.3.9/supermark/extensions/weekplan/
+-rw-r--r--   0 kraemer    (501) staff       (20)      230 2022-01-16 21:12:53.232496 supermark-0.3.9/supermark/extensions/weekplan/__init__.py
+-rw-r--r--   0 kraemer    (501) staff       (20)      314 2022-01-16 21:12:53.232577 supermark-0.3.9/supermark/extensions/weekplan/example.md
+-rw-r--r--   0 kraemer    (501) staff       (20)      409 2022-01-16 21:12:53.232660 supermark-0.3.9/supermark/extensions/weekplan/weekplan.css
+-rw-r--r--   0 kraemer    (501) staff       (20)      151 2022-01-16 21:12:53.232742 supermark-0.3.9/supermark/extensions/weekplan/weekplan.md
+-rw-r--r--   0 kraemer    (501) staff       (20)     1231 2022-02-13 08:15:48.091001 supermark-0.3.9/supermark/pandoc.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     8512 2022-01-16 21:12:53.233023 supermark-0.3.9/supermark/parse.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     7584 2022-01-16 21:12:53.233163 supermark-0.3.9/supermark/report.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     1146 2022-01-16 21:12:53.233248 supermark-0.3.9/supermark/setup.py
+-rw-r--r--   0 kraemer    (501) staff       (20)     5148 2022-01-16 21:12:53.233343 supermark-0.3.9/supermark/style.css
+-rw-r--r--   0 kraemer    (501) staff       (20)     1716 2022-01-16 21:12:53.233433 supermark-0.3.9/supermark/utils.py
```

### Comparing `supermark-0.3.8/PKG-INFO` & `supermark-0.3.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 1.1
 Name: supermark
-Version: 0.3.8
+Version: 0.3.9
 Summary: Pandoc-based transformation tool for documents containing different markup languages.
 Home-page: https://github.com/falkr/supermark
 Author: Frank Alexander Kraemer
 Author-email: kraemer.frank@gmail.com
 License: GPLv3
 Download-URL: https://github.com/falkr/supermark/archive/0.2.tar.gz
 Description: UNKNOWN
 Keywords: education
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
```

### Comparing `supermark-0.3.8/setup.py` & `supermark-0.3.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         "supermark.extensions.double",
         "supermark.extensions.figure",
         "supermark.extensions.goals",
         "supermark.extensions.guideline",
         "supermark.extensions.hints",
         "supermark.extensions.lines",
         "supermark.extensions.qna",
+        "supermark.extensions.quiz",
         "supermark.extensions.rat",
         "supermark.extensions.report",
         "supermark.extensions.rubrics",
         "supermark.extensions.steplist",
         "supermark.extensions.steps",
         "supermark.extensions.table",
         "supermark.extensions.task",
@@ -57,43 +58,41 @@
         "click",
         "openpyxl",
         "progressbar2",
         "pygments",
         "wikitextparser",
         "requests",
         "cairosvg",
-        "pathlib",
+        "pathlib2",
         "tqdm",
         "indentation",
         "blindspin",
         # "beepy",
         "watchdog",
         "pretty_errors",
         "rich",
         "icecream",
         "black",
         "blindspin",
+        "toml",
+        " markdown-it-py",
     ],
     package_data={
-        "": ["*.tex", "*.pdf", "*.css", "*.md"],
+        "": ["*.tex", "*.pdf", "*.css", "*.md", "*.js"],
     },
     include_package_data=True,
     author="Frank Alexander Kraemer",
     author_email="kraemer.frank@gmail.com",
     license="GPLv3",
     url="https://github.com/falkr/supermark",
     download_url="https://github.com/falkr/supermark/archive/0.2.tar.gz",
     keywords=["education"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Education",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     entry_points={"console_scripts": ["supermark=supermark.command:supermark"]},
 )
```

### Comparing `supermark-0.3.8/supermark/__init__.py` & `supermark-0.3.9/supermark/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     YAMLChunk,
     YAMLDataChunk,
 )
 from .core import Core
 from .extend import Extension, ParagraphExtension, TableClassExtension, YamlExtension
 from .report import Report
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 
 __all__ = [
     "Core",
     "Report",
     "RawChunk",
     "Chunk",
     "YAMLChunk",
```

### Comparing `supermark-0.3.8/supermark/base.py` & `supermark-0.3.9/supermark/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,17 @@
             ) as open_file:
                 string += open_file.read()
         return string
 
     def get_css(self) -> str:
         return self.files_to_string(self._find_files("*.css"))
 
+    def get_js(self) -> str:
+        return self.files_to_string(self._find_files("*.js"))
+
     def get_examples(self):
         return self._find_files("examples/*.md")
 
     def get_doc(self) -> Optional[Path]:
         files = self._find_files("doc.md")
         if len(files) > 0:
             return files[0]
```

### Comparing `supermark-0.3.8/supermark/build_html.py` & `supermark-0.3.9/supermark/build_html.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     def _transform_page_to_html(
         self,
         chunks: Sequence[Chunk],
         template: str,
         filepath: Path,
         report: Report,
         css: str,
+        js: str,
     ) -> str:
         content: Sequence[str] = []
         content.append('<div class="page">')
         if len(chunks) == 0:
             pass
         else:
             first_chunk = chunks[0]
@@ -76,20 +77,20 @@
                 add_notnone(chunk.to_html(self), content)
                 for aside in chunk.asides:
                     add_notnone(aside.to_html(self), content)
 
         content.append("    </section>")
         content.append("</div>")
         content = "\n".join(content)
-        for tag in ["content", "css"]:
+        for tag in ["content", "css", "js"]:
             if "{" + tag + "}" not in template:
                 self.report.warning(
                     "The template does not contain insertion tag {" + tag + "}"
                 )
-        return template.format_map({"content": content, "css": css})
+        return template.format_map({"content": content, "css": css, "js": js})
 
     def _create_target(
         self,
         source_file_path: Path,
         target_file_path: Path,
         template_file_path: Path,
         overwrite: bool,
@@ -113,19 +114,24 @@
     ):
 
         extensions_used: Set[Extension] = set()
         chunks = self.parse_file(source_file_path, extensions_used)
         if not chunks:
             # TODO warn that the page is empty, and therefore nothing is written
             return
-        css = self.core.get_css(self.extensions_used)
         html = self._transform_page_to_html(
-            chunks, template, source_file_path, self.report, css
+            chunks,
+            template,
+            source_file_path,
+            self.report,
+            self.core.get_css(self.extensions_used),
+            self.core.get_js(self.extensions_used),
         )
         write_file(html, target_file_path, self.report)
+        self.report.info("Translated", path=target_file_path)
 
     def _default_html_template(self) -> str:
         html: Sequence[str] = []
         html.append('<head><title></title><style type="text/css">{css}</style></head>')
         html.append("<body>")
         html.append("{content}")
         html.append("</body>")
@@ -182,25 +188,25 @@
             return
         elif len(jobs) == 0:
             self.report.conclude(
                 "No changed files detected. To re-build all unchanged files, use the [bold]--all[/bold] option."
             )
             return
         if len(jobs) == 1:
-            print("1")
+            self.report.info("Using single thread.")
             with Progress(transient=True) as progress:
                 progress.add_task("[orange]Building 1 page", start=False)
                 self._process_file(
                     jobs[0]["source_file_path"],
                     jobs[0]["target_file_path"],
                     jobs[0]["template"],
                 )
         else:
             with ThreadPoolExecutor() as e:
-                print("2")
+                self.report.info("Using threadpool.")
                 with Progress(
                     "[progress.description]{task.description}",
                     BarColumn(),
                     "[progress.percentage]{task.percentage:>3.0f}%",
                     transient=True,
                 ) as progress:
                     task = progress.add_task(
```

### Comparing `supermark-0.3.8/supermark/build_latex.py` & `supermark-0.3.9/supermark/build_latex.py`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/chunks.py` & `supermark-0.3.9/supermark/chunks.py`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/code.py` & `supermark-0.3.9/supermark/code.py`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/command.py` & `supermark-0.3.9/supermark/command.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 from .pandoc import print_pandoc_info
 
 # from .build_latex import build_latex
 from .report import Report
 from rich import print
 
+import toml
+
 
 def logo(version: str) -> str:
     return (
         R""" ___ __  __ ____ ____ ____ __  __   __   ____ _  _
 / __|  )(  |  _ ( ___|  _ (  \/  ) /__\ (  _ ( )/ )
 \__ \)(__)( )___/)__) )   /)    ( /(__)\ )   /)  (
 (___(______|__) (____|_)\_|_/\/\_|__)(__|_)\_|_)\_) """
@@ -79,14 +81,21 @@
     "-c",
     "--continuous",
     is_flag=True,
     default=False,
     help="Observe the source directory and run continuously.",
 )
 @click.option(
+    "-p",
+    "--path",
+    "path",
+    type=click.Path(exists=True, readable=True, path_type=Path),
+    help="Base path pointing to the folder that contains input, template, output path and an optional config file.",
+)
+@click.option(
     "-i",
     "--input",
     "input",
     type=click.Path(exists=True, readable=True, path_type=Path),
     help="Input directory containing the source files.",
 )
 @click.option(
@@ -118,67 +127,86 @@
     help="Write messages to a log file instead of standard output.",
 )
 def build(
     all: bool,
     verbose: bool,
     draft: bool,
     continuous: bool,
+    path: Optional[Path] = None,
     input: Optional[Path] = None,
     output: Optional[Path] = None,
     template: Optional[Path] = None,
     reformat: bool = False,
     log: bool = False,
 ):
     report = Report()
     core = Core(report=report)
     print(logo_2(__version__))
     print_pandoc_info()
+
+    path = ensure_path(path)
     input = ensure_path(input)
     output = ensure_path(output)
+    template = ensure_path(template)
+
+    base_path = path or Path.cwd()
+    input_path = None
+    output_path = None
+    template_path = None
+
+    # read configuration file
+    config_file = Path("config.toml")
+    if config_file.exists():
+        report.info("Found configuration file.", path=config_file)
+        config = toml.load(config_file)
+        if "input" in config and input is None:
+            input_path = base_path / config["input"]
+        if "output" in config and output is None:
+            output_path = base_path / config["output"]
+        if "template" in config and template is None:
+            template_path = base_path / config["template"]
+
+    if input_path is None:
+        input_path = base_path / "pages"
+    if output_path is None:
+        output_path = output or Path.cwd()
+    if template_path is None:
+        template_path = template or (base_path / "templates/page.html")
+
     format = "html"
-    base_path = input or Path.cwd()
-    input_path = base_path / "pages"
-    output_path = output or Path.cwd()
-    template_path = template or (base_path / "templates/page.html")
-    # print(template_path)
-
-    # if format == "pdf":
-    #     build_latex(
-    #         input_path,
-    #         output_path,
-    #     )
-    # else:
+    
     builder = HTMLBuilder(
         input_path,
         output_path,
         template_path,
         report,
         rebuild_all_pages=all,
         abort_draft=not draft,
         verbose=verbose,
         reformat=reformat,
     )
     builder.set_core(core)
     builder.build()
     if log:
-        report.print_to_file(base_path / ".log")
+        report.print_to_file(base_path / "supermark.log")
     else:
-        report.print()
+        report.print(verbose=verbose)
     if report.has_error():
         # beep(3)  # sad error
         ex = ClickException("Something is wrong.")
         ex.exit_code = 1
         raise ex
     # else:
     # beep(5)
 
 
 @supermark.command(help="Show info about a project and installation.")
 def info():
-    core = Core()
+    report = Report()
+    core = Core(report=report)
     core.info()
 
 
 @supermark.command(help="Setup a project.")
 @click.option(
     "-g",
     "--githubaction",
```

### Comparing `supermark-0.3.8/supermark/core.py` & `supermark-0.3.9/supermark/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,20 @@
 
     def get_css(self, used_extensions: Set[Extension]) -> str:
         all_css: str = ""
         for extension in sorted(list(used_extensions), key=lambda e: e.folder):
             all_css += extension.get_css() + "\n"
         return all_css
 
+    def get_js(self, used_extensions: Set[Extension]) -> str:
+        all_js: str = ""
+        for extension in sorted(list(used_extensions), key=lambda e: e.folder):
+            all_js += extension.get_js() + "\n"
+        return all_js
+
     def info(self):
         tree = Tree("Supermark Extensions")
         for extension_point in self.extension_points.values():
             ep_tree = tree.add(extension_point.name)
             for extension in extension_point.extensions.values():
                 ep_tree.add(str(extension))
         rich.print(tree)
```

### Comparing `supermark-0.3.8/supermark/extend.py` & `supermark-0.3.9/supermark/extend.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,18 +43,18 @@
     """For extension that are based on Yaml chunks."""
 
     def __init__(self) -> None:
         super().__init__("yaml")
         self.extensions: Dict[str, YamlExtension] = {}
 
     def register(self, extension: YamlExtension):
-        for type in (
+        for ttype in (
             [extension.type] if isinstance(extension.type, str) else extension.type
         ):
-            self.extensions[type] = extension
+            self.extensions[ttype] = extension
 
     def cast_yaml(
         self,
         raw: RawChunk,
         type: str,
         dictionary: Dict[str, Any],
         page_variables: Dict[str, Any],
```

### Comparing `supermark-0.3.8/supermark/extensions/button/__init__.py` & `supermark-0.3.9/supermark/extensions/button/__init__.py`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/extensions/button/button.css` & `supermark-0.3.9/supermark/extensions/button/button.css`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 a.ntnu-button {
     font: 600 14px "Source Sans Pro", Georgia, serif;
     background: #fff;
     color: #00509e;
     border: 1px solid #00509e;
-    border-color: #00509e !important
+    border-color: #00509e !important;
     border-style: solid !important;
     border-radius: 10rem;
     display: inline-block;
     padding: 5px 15px;
     height: auto;
     font-weight: bold;
     line-height: 1.5em;
```

### Comparing `supermark-0.3.8/supermark/extensions/checklistbox/checklistbox.css` & `supermark-0.3.9/supermark/extensions/checklistbox/checklistbox.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 div.checklistbox {
   width: 18rem;
   float: right;
   padding: 10px;
-  margin-left: 10px;
+  margin-left: 30px;
+  margin-bottom: 30px;
   background-color: #EFF7FF;
   border-radius: 0px;
   border-top: 6px solid #00509e
   }
   
 div.checklistbox::before { 
   content: "Checklist:";
```

### Comparing `supermark-0.3.8/supermark/extensions/code/code.css` & `supermark-0.3.9/supermark/extensions/code/code.css`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/extensions/code/doc.md` & `supermark-0.3.9/supermark/extensions/code/doc.md`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/extensions/figure/__init__.py` & `supermark-0.3.9/supermark/extensions/figure/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import os
 from typing import Any, Dict, Optional, Sequence
 
-import cairosvg
-
-
 from ... import YAMLChunk, YamlExtension, RawChunk, Builder
 
 
 class FigureExtension(YamlExtension):
     def __init__(self):
         super().__init__(type="figure", chunk_class=Figure)
 
@@ -101,14 +98,15 @@
                 level=self.WARNING,
             )
             return None
         if figure_file.suffix == ".svg":
             # file = Path(file)
             target_path = self.get_dir_cached() / "{}.pdf".format(figure_file.stem)
             if not target_path.exists():
+                import cairosvg
                 # file = self.raw_chunk.parent_path / self.dictionary['source']
                 cairosvg.svg2pdf(url=str(figure_file), write_to=str(target_path))
             # s.append('\\includegraphics[width=\\linewidth]{{{}}}%'.format(target_path))
             figure_file = target_path
         figure_file = figure_file.relative_to(builder.output_file.parent)
         # print('figure_file: {}'.format(figure_file))
         s.append("\\includegraphics[width=\\linewidth]{{{}}}%".format(figure_file))
```

### Comparing `supermark-0.3.8/supermark/extensions/hints/__init__.py` & `supermark-0.3.9/supermark/extensions/hints/__init__.py`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/extensions/hints/doc.md` & `supermark-0.3.9/supermark/extensions/hints/doc.md`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/extensions/lines/__init__.py` & `supermark-0.3.9/supermark/extensions/lines/__init__.py`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/extensions/qna/__init__.py` & `supermark-0.3.9/supermark/extensions/qna/__init__.py`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/extensions/rubrics/rubric.css` & `supermark-0.3.9/supermark/extensions/rubrics/rubric.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 th.rubric_f {background-color: #EBBCB9}
 
 table.rubric th {border-top: 2px black solid; border-bottom: 2px black solid; text-align: center;
 	vertical-align:top;}
 table.rubric td {width:22%; border-bottom: 1px black solid;}}*/
 
 .rubric p {margin: 0px}
+.rubric th {border-top: 1.4px black solid; border-bottom: 1.4px black solid; text-align: center; padding:6px;}
+.rubric td {border-bottom: 0.7px black solid; vertical-align:top; font-size:12px; padding:6px;}
+.rubric th {font-size:12px; vertical-align:top; }
 .rubric td:nth-child(2), .rubric th:nth-child(2){background-color: #D0E8DC; width:22%}
 .rubric td:nth-child(3), .rubric th:nth-child(3){background-color: #FCFDE3; width:22%}
 .rubric td:nth-child(4), .rubric th:nth-child(4){background-color: #F8D9C2; width:22%}
 .rubric td:nth-child(5), .rubric th:nth-child(5){background-color: #EBBCB9; width:22%}
-.rubric th {border-top: 1.4px black solid; border-bottom: 1.4px black solid; text-align: center; padding:6px;}
-.rubric td {border-bottom: 0.7px black solid; vertical-align:top; font-size:12px; padding:6px;}
-.rubric th {font-size:12px; vertical-align:top; }
 .rubric tfoot td {text-align:right; border-bottom: none; padding: 1px;}
 .rubric tfoot a {font-size: 12px; font-style: italic; color: gray}
```

### Comparing `supermark-0.3.8/supermark/extensions/steplist/doc.md` & `supermark-0.3.9/supermark/extensions/steplist/doc.md`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/extensions/steplist/steplist.css` & `supermark-0.3.9/supermark/extensions/steplist/steplist.css`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/extensions/steps/doc.md` & `supermark-0.3.9/supermark/extensions/steps/doc.md`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/extensions/table/__init__.py` & `supermark-0.3.9/supermark/extensions/table/__init__.py`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/extensions/table/doc.md` & `supermark-0.3.9/supermark/extensions/table/doc.md`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/extensions/tree/tree.css` & `supermark-0.3.9/supermark/extensions/tree/tree.css`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/extensions/video/__init__.py` & `supermark-0.3.9/supermark/extensions/video/__init__.py`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/pandoc.py` & `supermark-0.3.9/supermark/pandoc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 import pypandoc
 from packaging import version
 from rich import print
+from markdown_it import MarkdownIt
+
+
+md = MarkdownIt()
 
 
 def print_pandoc_info():
     installed_pandoc_version = pypandoc.get_pandoc_version()
     print("Installed Pandoc version: {}".format(installed_pandoc_version))
     if version.parse(installed_pandoc_version) < version.parse("2.14"):
         print(
             "There exists a newer version of Pandoc. Update via [link=https://pandoc.org]pandoc.org[/link]."
         )
     # print(pypandoc.get_pandoc_path())
     # print(pypandoc.get_pandoc_formats())
 
 
 def convert(source: str, target_format: str, source_format: str = "md") -> str:
+
+    if source_format == "md" and target_format == "html":
+        return md.render(source)
+
     if source_format == "mediawiki":
         extra_args = ["--from", "mediawiki", "--to", "html"]
     else:
         extra_args = []
     return pypandoc.convert_text(
         source, target_format, format=source_format, extra_args=extra_args
     ).strip()
```

### Comparing `supermark-0.3.8/supermark/parse.py` & `supermark-0.3.9/supermark/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,14 @@
                 if empty_lines > 1:
                     previous_yaml_chunk.post_yaml = current_lines
                     state = ParserState.MARKDOWN
                     current_lines = []
                 else:
                     current_lines.append(line)
                 start_line_number = line_number + 1
-            # TODO also handle that file is ending, and the post-yaml is the last content in the file
             else:
                 empty_lines = 0
                 current_lines.append(line)
         elif state == ParserState.CODE:
             if code_stop(s_line):
                 current_lines.append(line)
                 chunks.append(
@@ -208,40 +207,42 @@
                 current_lines.append(line)
                 start_line_number = line_number
                 empty_lines = 0
             else:
                 current_lines.append(line)
                 empty_lines = 0
     # create last chunk
+    if state == ParserState.AFTER_YAML_CONTENT:
+        previous_yaml_chunk.post_yaml = current_lines
+    else:
+        def parser_state_to_chunk_type(state: ParserState) -> RawChunkType:
+            if state == ParserState.MARKDOWN:
+                return RawChunkType.MARKDOWN
+            elif (
+                (state == ParserState.YAML)
+                or (state == ParserState.AFTER_YAML)
+            ):
+                return RawChunkType.YAML
+            elif state == ParserState.HTML:
+                return RawChunkType.HTML
+            elif state == ParserState.CODE:
+                return RawChunkType.CODE
+            else:
+                assert False
 
-    def parser_state_to_chunk_type(state: ParserState) -> RawChunkType:
-        if state == ParserState.MARKDOWN:
-            return RawChunkType.MARKDOWN
-        elif (
-            (state == ParserState.YAML)
-            or (state == ParserState.AFTER_YAML)
-            or (state == ParserState.AFTER_YAML_CONTENT)
-        ):
-            return RawChunkType.YAML
-        elif state == ParserState.HTML:
-            return RawChunkType.HTML
-        elif state == ParserState.CODE:
-            return RawChunkType.CODE
-        else:
-            assert False
-
-    chunks.append(
-        RawChunk(
-            current_lines,
-            parser_state_to_chunk_type(state),
-            start_line_number,
-            path,
-            report,
+        chunks.append(
+            RawChunk(
+                current_lines,
+                parser_state_to_chunk_type(state),
+                start_line_number,
+                path,
+                report,
+            )
         )
-    )
+
     # TODO remove chunks that turn out to be empty
     chunks = [item for item in chunks if not item.is_empty()]
     chunks = expand_reference_chunks(chunks, path, report)
     return chunks
 
 
 def expand_reference_chunks(
```

### Comparing `supermark-0.3.8/supermark/report.py` & `supermark-0.3.9/supermark/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 from typing import Dict, List, Optional, Set
 
 from rich import print as pprint
 from rich.panel import Panel
 from rich.tree import Tree
+from rich.console import Console
 
 from colorama import Fore, Back, Style
 import indentation
 
 COLOR_1 = Fore.LIGHTBLUE_EX
 COLOR_2 = Fore.LIGHTGREEN_EX
 
@@ -163,15 +164,15 @@
                 f":banana: Finished with {self.warnings} warning{plural}.",
                 expand=False,
                 style="dark_orange",
             )
         else:
             return Panel(":shamrock: Finished.", expand=False, style="dark_sea_green")
 
-    def print(self, verbose: bool = False):
+    def _get_tree(self, verbose: bool) -> Tree:
         panel = self._get_conclusion_panel()
         tree = Tree(panel, guide_style="grey50")
         levels = (
             [Report.ERROR, Report.WARNING, Report.INFO]
             if verbose
             else [Report.ERROR, Report.WARNING]
         )
@@ -191,22 +192,28 @@
                             else "dark_sea_green4"
                         )
                         hashes[entry.get_hash()] = tree.add(
                             entry.message, style=f"bold {level_color}"
                         )
                         if entry.path is not None:
                             hashes[entry.get_hash()].add(entry.get_styled_location())
+        return tree
+
+    def print(self, verbose: bool = False):
+        tree = self._get_tree(verbose=verbose)
         pprint(tree)
 
     def print_to_file(self, log: Path):
         with open(log, "w") as file:
-            for level in [Report.ERROR, Report.WARNING, Report.INFO]:
-                for entry in self.messages:
-                    if entry.level == level:
-                        file.write(entry.message + "\n")
+            tree = self._get_tree(verbose=True)
+            console = Console(record=True)
+            with console.capture() as capture:
+                console.print(tree)
+            file.write(console.export_text())
+
 
     # @staticmethod
     # def print_reports(verbose: bool = False) -> int:
     #     levels = (
     #         [Report.ERROR, Report.WARNING, Report.INFO]
     #         if verbose
     #         else [Report.ERROR, Report.WARNING]
```

### Comparing `supermark-0.3.8/supermark/setup.py` & `supermark-0.3.9/supermark/setup.py`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/style.css` & `supermark-0.3.9/supermark/style.css`

 * *Files identical despite different names*

### Comparing `supermark-0.3.8/supermark/utils.py` & `supermark-0.3.9/supermark/utils.py`

 * *Files identical despite different names*

