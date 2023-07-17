# Comparing `tmp/nbconvert-7.7.0.tar.gz` & `tmp/nbconvert-7.7.1.tar.gz`

## Comparing `nbconvert-7.7.0.tar` & `nbconvert-7.7.1.tar`

### file list

```diff
@@ -1,278 +1,278 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.mailmap
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.prettierignore
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.readthedocs.yaml
--rw-r--r--   0        0        0    76987 2020-02-02 00:00:00.000000 nbconvert-7.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 nbconvert-7.7.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 nbconvert-7.7.0/RELEASE.md
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 nbconvert-7.7.0/check_requirements.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/Makefile
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/README.md
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/autogen_config.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/make.bat
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/make_html.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/quiz_notebook.py
--rw-r--r--   0        0        0    36829 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/media/image1.png
--rw-r--r--   0        0        0   176383 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/media/image2.png
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/conf.json
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2
--rw-r--r--   0        0        0   266255 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css
--rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/architecture.rst
--rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/conf.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/customizing.rst
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/dejavu.rst
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/development_release.rst
--rw-r--r--   0        0        0     7875 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/execute_api.rst
--rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/external_exporters.rst
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/highlighting.rst
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/index.rst
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/install.rst
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/latex_citations.rst
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/nbconvert_library.ipynb
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/need_help.rst
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/removing_cells.rst
--rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/usage.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/_static/empty.txt
--rw-r--r--   0        0        0    36971 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/_static/exporter_inheritance.png
--rw-r--r--   0        0        0    65726 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/_static/preprocessor_inheritance.png
--rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/_static/writer_inheritance.png
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/exporters.rst
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/filters.rst
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/index.rst
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/nbconvertapp.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/postprocessors.rst
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/preprocessors.rst
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/writers.rst
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/__main__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/_version.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/conftest.py
--rwxr-xr-x   0        0        0    24121 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/nbconvertapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/py.typed
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/__init__.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/asciidoc.py
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/base.py
--rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/exporter.py
--rw-r--r--   0        0        0    12735 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/html.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/latex.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/markdown.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/notebook.py
--rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/pdf.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/python.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/qt_exporter.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/qt_screenshot.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/qtpdf.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/qtpng.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/rst.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/script.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/slides.py
--rw-r--r--   0        0        0    27014 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/templateexporter.py
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/webpdf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/__init__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/base.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/cheese.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_asciidoc.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_export.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_exporter.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_html.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_latex.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_markdown.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_notebook.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_pdf.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_python.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_qtpdf.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_qtpng.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_rst.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_script.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_slides.py
--rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_templateexporter.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_webpdf.py
--rw-r--r--   0        0        0    45585 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/attachment.ipynb
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/lablike.html.j2
--rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/notebook2.ipynb
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/notebook3.ipynb
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/notebook_inject.ipynb
--rw-r--r--   0        0        0    16782 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/pngmetadata.ipynb
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/rawtest.ipynb
--rw-r--r--   0        0        0    19943 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/svg.ipynb
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/__init__.py
--rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/ansi.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/citation.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/datatypefilter.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/filter_links.py
--rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/highlight.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/latex.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/markdown.py
--rw-r--r--   0        0        0    18261 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/markdown_mistune.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/metadata.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/pandoc.py
--rw-r--r--   0        0        0     7461 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/strings.py
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/widgetsdatatypefilter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_ansi.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_citation.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_datatypefilter.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_highlight.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_latex.py
--rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_markdown.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_metadata.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_pandoc.py
--rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_strings.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/postprocessors/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/postprocessors/base.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/postprocessors/serve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/postprocessors/tests/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/postprocessors/tests/test_serve.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/__init__.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/base.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/clearmetadata.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/clearoutput.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/coalescestreams.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/convertfigures.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/csshtmlheader.py
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/execute.py
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/extractattachments.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/extractoutput.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/highlightmagics.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/latex.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/regexremove.py
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/sanitize.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/svg2pdf.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tagremove.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/__init__.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/base.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/fake_kernelmanager.py
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_clearmetadata.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_clearoutput.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_coalescestreams.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_csshtmlheader.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_execute.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_extractattachments.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_extractoutput.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_highlightmagics.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_latex.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_regexremove.py
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_sanitize.py
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_svg2pdf.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_tagremove.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/files/HelloWorld.ipynb
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/resources/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/templates/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/templates/skeleton/Makefile
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/templates/skeleton/README.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/__init__.py
--rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/base.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/fake_exporters.py
--rw-r--r--   0        0        0    28724 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/test_nbconvertapp.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/utils.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/exporter_entrypoint/eptest.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/exporter_entrypoint/eptest-0.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/Unexecuted_widget.ipynb
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb
--rw-r--r--   0        0        0    96479 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/Widget_List.ipynb
--rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/containerized_deployments.jpeg
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/hello.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/jupyter_nbconvert_config.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/latex-linked-image.ipynb
--rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/markdown_display_priority.ipynb
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook1.ipynb
--rw-r--r--   0        0        0   125459 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook2.ipynb
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook3_with_errors.ipynb
--rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook4_jpeg.ipynb
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook5_embed_images.ipynb
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook_jl.ipynb
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook_tags.ipynb
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/override.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/testimage.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/_contextlib_chdir.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/base.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/exceptions.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/io.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/iso639_1.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/lexers.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/pandoc.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/text.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/tests/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/tests/test_io.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/tests/test_pandoc.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/tests/test_version.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/__init__.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/base.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/debug.py
--rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/files.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/stdout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/tests/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/tests/test_debug.py
--rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/tests/test_files.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/tests/test_stdout.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/asciidoc/conf.json
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/asciidoc/index.asciidoc.j2
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/base/cell_id_anchor.j2
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/base/celltags.j2
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/base/display_priority.j2
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/base/jupyter_widgets.html.j2
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/base/mathjax.html.j2
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/base/null.j2
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/basic/conf.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/basic/index.html.j2
--rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/classic/base.html.j2
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/classic/conf.json
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/classic/index.html.j2
--rw-r--r--   0        0        0   265101 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/classic/static/style.css
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/compatibility/display_priority.tpl
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/compatibility/full.tpl
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/base.html.j2
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/conf.json
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/index.html.j2
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/mermaidjs.html.j2
--rw-r--r--   0        0        0   240379 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/static/index.css
--rw-r--r--   0        0        0    17102 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/static/theme-dark.css
--rw-r--r--   0        0        0    16019 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/static/theme-light.css
--rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/base.tex.j2
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/conf.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/display_priority.j2
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/document_contents.tex.j2
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/index.tex.j2
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/null.j2
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/report.tex.j2
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/style_bw_ipython.tex.j2
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/style_bw_python.tex.j2
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/style_ipython.tex.j2
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/style_jupyter.tex.j2
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/style_python.tex.j2
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/markdown/conf.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/markdown/index.md.j2
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/python/conf.json
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/python/index.py.j2
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/reveal/base.html.j2
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/reveal/cellslidedata.j2
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/reveal/conf.json
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/reveal/index.html.j2
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/reveal/static/custom_reveal.css
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/rst/conf.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/rst/index.rst.j2
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/script/conf.json
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/script/script.j2
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/webpdf/conf.json
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/webpdf/index.pdf.j2
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.gitignore
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbconvert-7.7.0/LICENSE
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 nbconvert-7.7.0/README.md
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 nbconvert-7.7.0/hatch_build.py
--rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 nbconvert-7.7.0/pyproject.toml
--rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 nbconvert-7.7.0/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.mailmap
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.prettierignore
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.readthedocs.yaml
+-rw-r--r--   0        0        0    77566 2020-02-02 00:00:00.000000 nbconvert-7.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 nbconvert-7.7.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 nbconvert-7.7.1/RELEASE.md
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 nbconvert-7.7.1/check_requirements.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/Makefile
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/README.md
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/autogen_config.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/make.bat
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/api_examples/template_path/make_html.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/api_examples/template_path/quiz_notebook.py
+-rw-r--r--   0        0        0    36829 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/api_examples/template_path/media/image1.png
+-rw-r--r--   0        0        0   176383 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/api_examples/template_path/media/image2.png
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/conf.json
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2
+-rw-r--r--   0        0        0   266255 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css
+-rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/architecture.rst
+-rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/conf.py
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/customizing.rst
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/dejavu.rst
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/development_release.rst
+-rw-r--r--   0        0        0     7875 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/execute_api.rst
+-rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/external_exporters.rst
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/highlighting.rst
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/index.rst
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/install.rst
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/latex_citations.rst
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/nbconvert_library.ipynb
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/need_help.rst
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/removing_cells.rst
+-rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/usage.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/_static/empty.txt
+-rw-r--r--   0        0        0    36971 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/_static/exporter_inheritance.png
+-rw-r--r--   0        0        0    65726 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/_static/preprocessor_inheritance.png
+-rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/_static/writer_inheritance.png
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/api/exporters.rst
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/api/filters.rst
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/api/index.rst
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/api/nbconvertapp.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/api/postprocessors.rst
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/api/preprocessors.rst
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nbconvert-7.7.1/docs/source/api/writers.rst
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/__main__.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/_version.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/conftest.py
+-rwxr-xr-x   0        0        0    24121 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/nbconvertapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/py.typed
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/__init__.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/asciidoc.py
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/base.py
+-rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/exporter.py
+-rw-r--r--   0        0        0    12735 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/html.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/latex.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/markdown.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/notebook.py
+-rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/pdf.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/python.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/qt_exporter.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/qt_screenshot.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/qtpdf.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/qtpng.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/rst.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/script.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/slides.py
+-rw-r--r--   0        0        0    27014 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/templateexporter.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/webpdf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/__init__.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/base.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/cheese.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_asciidoc.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_export.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_exporter.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_html.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_latex.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_markdown.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_notebook.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_pdf.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_python.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_qtpdf.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_qtpng.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_rst.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_script.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_slides.py
+-rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_templateexporter.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/test_webpdf.py
+-rw-r--r--   0        0        0    45585 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/files/attachment.ipynb
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/files/lablike.html.j2
+-rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/files/notebook2.ipynb
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/files/notebook3.ipynb
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/files/notebook_inject.ipynb
+-rw-r--r--   0        0        0    16782 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/files/pngmetadata.ipynb
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/files/prompt_numbers.ipynb
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/files/rawtest.ipynb
+-rw-r--r--   0        0        0    19943 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/exporters/tests/files/svg.ipynb
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/__init__.py
+-rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/ansi.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/citation.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/datatypefilter.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/filter_links.py
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/highlight.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/latex.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/markdown.py
+-rw-r--r--   0        0        0    18261 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/markdown_mistune.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/metadata.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/pandoc.py
+-rw-r--r--   0        0        0     7461 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/strings.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/widgetsdatatypefilter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/tests/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/tests/test_ansi.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/tests/test_citation.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/tests/test_datatypefilter.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/tests/test_highlight.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/tests/test_latex.py
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/tests/test_markdown.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/tests/test_metadata.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/tests/test_pandoc.py
+-rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/filters/tests/test_strings.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/postprocessors/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/postprocessors/base.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/postprocessors/serve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/postprocessors/tests/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/postprocessors/tests/test_serve.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/__init__.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/base.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/clearmetadata.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/clearoutput.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/coalescestreams.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/convertfigures.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/csshtmlheader.py
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/execute.py
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/extractattachments.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/extractoutput.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/highlightmagics.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/latex.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/regexremove.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/sanitize.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/svg2pdf.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tagremove.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/__init__.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/base.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/fake_kernelmanager.py
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/test_clearmetadata.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/test_clearoutput.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/test_coalescestreams.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/test_csshtmlheader.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/test_execute.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/test_extractattachments.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/test_extractoutput.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/test_highlightmagics.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/test_latex.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/test_regexremove.py
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/test_sanitize.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/test_svg2pdf.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/test_tagremove.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/files/HelloWorld.ipynb
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/resources/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/templates/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/templates/skeleton/Makefile
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/templates/skeleton/README.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/__init__.py
+-rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/base.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/fake_exporters.py
+-rw-r--r--   0        0        0    28724 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/test_nbconvertapp.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/utils.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/exporter_entrypoint/eptest.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/exporter_entrypoint/eptest-0.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/Unexecuted_widget.ipynb
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/Unexecuted_widget_2.ipynb
+-rw-r--r--   0        0        0    96479 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/Widget_List.ipynb
+-rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/containerized_deployments.jpeg
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/hello.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/jupyter_nbconvert_config.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/latex-linked-image.ipynb
+-rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/markdown_display_priority.ipynb
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/notebook1.ipynb
+-rw-r--r--   0        0        0   125459 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/notebook2.ipynb
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/notebook3_with_errors.ipynb
+-rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/notebook4_jpeg.ipynb
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/notebook5_embed_images.ipynb
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/notebook_jl.ipynb
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/notebook_tags.ipynb
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/override.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/tests/files/testimage.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/_contextlib_chdir.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/base.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/exceptions.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/io.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/iso639_1.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/lexers.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/pandoc.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/text.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/tests/test_io.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/tests/test_pandoc.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/utils/tests/test_version.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/writers/__init__.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/writers/base.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/writers/debug.py
+-rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/writers/files.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/writers/stdout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/writers/tests/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/writers/tests/test_debug.py
+-rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/writers/tests/test_files.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 nbconvert-7.7.1/nbconvert/writers/tests/test_stdout.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/asciidoc/conf.json
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/asciidoc/index.asciidoc.j2
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/base/cell_id_anchor.j2
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/base/celltags.j2
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/base/display_priority.j2
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/base/jupyter_widgets.html.j2
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/base/mathjax.html.j2
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/base/null.j2
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/basic/conf.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/basic/index.html.j2
+-rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/classic/base.html.j2
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/classic/conf.json
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/classic/index.html.j2
+-rw-r--r--   0        0        0   265101 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/classic/static/style.css
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/compatibility/display_priority.tpl
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/compatibility/full.tpl
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/lab/base.html.j2
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/lab/conf.json
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/lab/index.html.j2
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/lab/mermaidjs.html.j2
+-rw-r--r--   0        0        0   240379 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/lab/static/index.css
+-rw-r--r--   0        0        0    17102 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/lab/static/theme-dark.css
+-rw-r--r--   0        0        0    16019 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/lab/static/theme-light.css
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/latex/base.tex.j2
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/latex/conf.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/latex/display_priority.j2
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/latex/document_contents.tex.j2
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/latex/index.tex.j2
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/latex/null.j2
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/latex/report.tex.j2
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/latex/style_bw_ipython.tex.j2
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/latex/style_bw_python.tex.j2
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/latex/style_ipython.tex.j2
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/latex/style_jupyter.tex.j2
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/latex/style_python.tex.j2
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/markdown/conf.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/markdown/index.md.j2
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/python/conf.json
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/python/index.py.j2
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/reveal/base.html.j2
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/reveal/cellslidedata.j2
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/reveal/conf.json
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/reveal/index.html.j2
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/reveal/static/custom_reveal.css
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/rst/conf.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/rst/index.rst.j2
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/script/conf.json
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/script/script.j2
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/webpdf/conf.json
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 nbconvert-7.7.1/share/templates/webpdf/index.pdf.j2
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nbconvert-7.7.1/.gitignore
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbconvert-7.7.1/LICENSE
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 nbconvert-7.7.1/README.md
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 nbconvert-7.7.1/hatch_build.py
+-rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 nbconvert-7.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 nbconvert-7.7.1/PKG-INFO
```

### Comparing `nbconvert-7.7.0/.mailmap` & `nbconvert-7.7.1/.mailmap`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/.pre-commit-config.yaml` & `nbconvert-7.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/CHANGELOG.md` & `nbconvert-7.7.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changes in nbconvert
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 7.7.1
+
+([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.7.0...86cebfc16920fcdddef557620a7b8a23d84072d6))
+
+### Bugs fixed
+
+- Restore 'media=print' option [#2022](https://github.com/jupyter/nbconvert/pull/2022) ([@brichet](https://github.com/brichet))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/nbconvert/graphs/contributors?from=2023-07-17&to=2023-07-17&type=c))
+
+[@brichet](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Abrichet+updated%3A2023-07-17..2023-07-17&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 7.7.0
 
 ([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.6.0...f2fc3e13fe8e8836324550dac5286bbb0e4315bb))
 
 ### Enhancements made
 
 - \[Accessibility\] some accessibility improvements [#2021](https://github.com/jupyter/nbconvert/pull/2021) ([@brichet](https://github.com/brichet))
@@ -24,16 +40,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/nbconvert/graphs/contributors?from=2023-06-19&to=2023-07-17&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Ablink1073+updated%3A2023-06-19..2023-07-17&type=Issues) | [@brichet](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Abrichet+updated%3A2023-06-19..2023-07-17&type=Issues) | [@jstorrs](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Ajstorrs+updated%3A2023-06-19..2023-07-17&type=Issues) | [@maartenbreddels](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Amaartenbreddels+updated%3A2023-06-19..2023-07-17&type=Issues) | [@manzt](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Amanzt+updated%3A2023-06-19..2023-07-17&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3AmartinRenou+updated%3A2023-06-19..2023-07-17&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Apre-commit-ci+updated%3A2023-06-19..2023-07-17&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 7.6.0
 
 ([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.5.0...60af6d897c083444586829c636f278d84ae81962))
 
 ### Maintenance and upkeep improvements
 
 - Update to Mistune v3 [#1820](https://github.com/jupyter/nbconvert/pull/1820) ([@TiagodePAlves](https://github.com/TiagodePAlves))
```

### Comparing `nbconvert-7.7.0/CONTRIBUTING.md` & `nbconvert-7.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/RELEASE.md` & `nbconvert-7.7.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/check_requirements.py` & `nbconvert-7.7.1/check_requirements.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/.github/workflows/docs.yml` & `nbconvert-7.7.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/.github/workflows/prep-release.yml` & `nbconvert-7.7.1/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/.github/workflows/publish-release.yml` & `nbconvert-7.7.1/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/.github/workflows/tests.yml` & `nbconvert-7.7.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/Makefile` & `nbconvert-7.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/README.md` & `nbconvert-7.7.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/autogen_config.py` & `nbconvert-7.7.1/docs/autogen_config.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/make.bat` & `nbconvert-7.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/api_examples/template_path/make_html.py` & `nbconvert-7.7.1/docs/api_examples/template_path/make_html.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/api_examples/template_path/quiz_notebook.py` & `nbconvert-7.7.1/docs/api_examples/template_path/quiz_notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/api_examples/template_path/media/image1.png` & `nbconvert-7.7.1/docs/api_examples/template_path/media/image1.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/api_examples/template_path/media/image2.png` & `nbconvert-7.7.1/docs/api_examples/template_path/media/image2.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2` & `nbconvert-7.7.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css` & `nbconvert-7.7.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/architecture.rst` & `nbconvert-7.7.1/docs/source/architecture.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/conf.py` & `nbconvert-7.7.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/customizing.rst` & `nbconvert-7.7.1/docs/source/customizing.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/dejavu.rst` & `nbconvert-7.7.1/docs/source/dejavu.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/development_release.rst` & `nbconvert-7.7.1/docs/source/development_release.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/execute_api.rst` & `nbconvert-7.7.1/docs/source/execute_api.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/external_exporters.rst` & `nbconvert-7.7.1/docs/source/external_exporters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/highlighting.rst` & `nbconvert-7.7.1/docs/source/highlighting.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/index.rst` & `nbconvert-7.7.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/install.rst` & `nbconvert-7.7.1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/latex_citations.rst` & `nbconvert-7.7.1/docs/source/latex_citations.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/nbconvert_library.ipynb` & `nbconvert-7.7.1/docs/source/nbconvert_library.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/need_help.rst` & `nbconvert-7.7.1/docs/source/need_help.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/removing_cells.rst` & `nbconvert-7.7.1/docs/source/removing_cells.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/usage.rst` & `nbconvert-7.7.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/_static/exporter_inheritance.png` & `nbconvert-7.7.1/docs/source/_static/exporter_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/_static/preprocessor_inheritance.png` & `nbconvert-7.7.1/docs/source/_static/preprocessor_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/_static/writer_inheritance.png` & `nbconvert-7.7.1/docs/source/_static/writer_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/api/exporters.rst` & `nbconvert-7.7.1/docs/source/api/exporters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/api/filters.rst` & `nbconvert-7.7.1/docs/source/api/filters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/docs/source/api/preprocessors.rst` & `nbconvert-7.7.1/docs/source/api/preprocessors.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/nbconvertapp.py` & `nbconvert-7.7.1/nbconvert/nbconvertapp.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/__init__.py` & `nbconvert-7.7.1/nbconvert/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/asciidoc.py` & `nbconvert-7.7.1/nbconvert/exporters/asciidoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/base.py` & `nbconvert-7.7.1/nbconvert/exporters/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/exporter.py` & `nbconvert-7.7.1/nbconvert/exporters/exporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/html.py` & `nbconvert-7.7.1/nbconvert/exporters/html.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/latex.py` & `nbconvert-7.7.1/nbconvert/exporters/latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/markdown.py` & `nbconvert-7.7.1/nbconvert/exporters/markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/notebook.py` & `nbconvert-7.7.1/nbconvert/exporters/notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/pdf.py` & `nbconvert-7.7.1/nbconvert/exporters/pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/python.py` & `nbconvert-7.7.1/nbconvert/exporters/python.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/qt_exporter.py` & `nbconvert-7.7.1/nbconvert/exporters/qt_exporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/qt_screenshot.py` & `nbconvert-7.7.1/nbconvert/exporters/qt_screenshot.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/qtpdf.py` & `nbconvert-7.7.1/nbconvert/exporters/qtpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/rst.py` & `nbconvert-7.7.1/nbconvert/exporters/rst.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/script.py` & `nbconvert-7.7.1/nbconvert/exporters/script.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/slides.py` & `nbconvert-7.7.1/nbconvert/exporters/slides.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/templateexporter.py` & `nbconvert-7.7.1/nbconvert/exporters/templateexporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/webpdf.py` & `nbconvert-7.7.1/nbconvert/exporters/webpdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,15 @@
                     "No suitable chromium executable found on the system. "
                     "Please use '--allow-chromium-download' to allow downloading one,"
                     "or install it using `playwright install chromium`."
                 )
                 raise RuntimeError(msg) from e
 
             page = await browser.new_page()
+            await page.emulate_media(media="print")
             await page.goto(f"file://{temp_file.name}", wait_until="networkidle")
 
             pdf_params = {"print_background": True}
             if not self.paginate:
                 # Floating point precision errors cause the printed
                 # PDF from spilling over a new page by a pixel fraction.
                 dimensions = await page.evaluate(
```

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/base.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/cheese.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/cheese.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_asciidoc.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_asciidoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_export.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_exporter.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_html.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_latex.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_markdown.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_notebook.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_pdf.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_python.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_qtpdf.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_qtpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_qtpng.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_qtpng.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_rst.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_rst.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_script.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_slides.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_slides.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_templateexporter.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_templateexporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/test_webpdf.py` & `nbconvert-7.7.1/nbconvert/exporters/tests/test_webpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/files/attachment.ipynb` & `nbconvert-7.7.1/nbconvert/exporters/tests/files/attachment.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/files/notebook2.ipynb` & `nbconvert-7.7.1/nbconvert/exporters/tests/files/notebook2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/files/notebook3.ipynb` & `nbconvert-7.7.1/nbconvert/exporters/tests/files/notebook3.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/files/notebook_inject.ipynb` & `nbconvert-7.7.1/nbconvert/exporters/tests/files/notebook_inject.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/files/pngmetadata.ipynb` & `nbconvert-7.7.1/nbconvert/exporters/tests/files/pngmetadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb` & `nbconvert-7.7.1/nbconvert/exporters/tests/files/prompt_numbers.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/files/rawtest.ipynb` & `nbconvert-7.7.1/nbconvert/exporters/tests/files/rawtest.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/exporters/tests/files/svg.ipynb` & `nbconvert-7.7.1/nbconvert/exporters/tests/files/svg.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/ansi.py` & `nbconvert-7.7.1/nbconvert/filters/ansi.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/citation.py` & `nbconvert-7.7.1/nbconvert/filters/citation.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/datatypefilter.py` & `nbconvert-7.7.1/nbconvert/filters/datatypefilter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/filter_links.py` & `nbconvert-7.7.1/nbconvert/filters/filter_links.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/highlight.py` & `nbconvert-7.7.1/nbconvert/filters/highlight.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/latex.py` & `nbconvert-7.7.1/nbconvert/filters/latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/markdown.py` & `nbconvert-7.7.1/nbconvert/filters/markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/markdown_mistune.py` & `nbconvert-7.7.1/nbconvert/filters/markdown_mistune.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/pandoc.py` & `nbconvert-7.7.1/nbconvert/filters/pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/strings.py` & `nbconvert-7.7.1/nbconvert/filters/strings.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/widgetsdatatypefilter.py` & `nbconvert-7.7.1/nbconvert/filters/widgetsdatatypefilter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/tests/test_ansi.py` & `nbconvert-7.7.1/nbconvert/filters/tests/test_ansi.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/tests/test_citation.py` & `nbconvert-7.7.1/nbconvert/filters/tests/test_citation.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/tests/test_datatypefilter.py` & `nbconvert-7.7.1/nbconvert/filters/tests/test_datatypefilter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/tests/test_highlight.py` & `nbconvert-7.7.1/nbconvert/filters/tests/test_highlight.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/tests/test_latex.py` & `nbconvert-7.7.1/nbconvert/filters/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/tests/test_markdown.py` & `nbconvert-7.7.1/nbconvert/filters/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/tests/test_metadata.py` & `nbconvert-7.7.1/nbconvert/filters/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/tests/test_pandoc.py` & `nbconvert-7.7.1/nbconvert/filters/tests/test_pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/filters/tests/test_strings.py` & `nbconvert-7.7.1/nbconvert/filters/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/postprocessors/base.py` & `nbconvert-7.7.1/nbconvert/postprocessors/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/postprocessors/serve.py` & `nbconvert-7.7.1/nbconvert/postprocessors/serve.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/postprocessors/tests/test_serve.py` & `nbconvert-7.7.1/nbconvert/postprocessors/tests/test_serve.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/__init__.py` & `nbconvert-7.7.1/nbconvert/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/base.py` & `nbconvert-7.7.1/nbconvert/preprocessors/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/clearmetadata.py` & `nbconvert-7.7.1/nbconvert/preprocessors/clearmetadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/clearoutput.py` & `nbconvert-7.7.1/nbconvert/preprocessors/clearoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/coalescestreams.py` & `nbconvert-7.7.1/nbconvert/preprocessors/coalescestreams.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/convertfigures.py` & `nbconvert-7.7.1/nbconvert/preprocessors/convertfigures.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/csshtmlheader.py` & `nbconvert-7.7.1/nbconvert/preprocessors/csshtmlheader.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/execute.py` & `nbconvert-7.7.1/nbconvert/preprocessors/execute.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/extractattachments.py` & `nbconvert-7.7.1/nbconvert/preprocessors/extractattachments.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/extractoutput.py` & `nbconvert-7.7.1/nbconvert/preprocessors/extractoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/highlightmagics.py` & `nbconvert-7.7.1/nbconvert/preprocessors/highlightmagics.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/latex.py` & `nbconvert-7.7.1/nbconvert/preprocessors/latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/regexremove.py` & `nbconvert-7.7.1/nbconvert/preprocessors/regexremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/sanitize.py` & `nbconvert-7.7.1/nbconvert/preprocessors/sanitize.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/svg2pdf.py` & `nbconvert-7.7.1/nbconvert/preprocessors/svg2pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tagremove.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tagremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/base.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/fake_kernelmanager.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/fake_kernelmanager.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_clearmetadata.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/test_clearmetadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_clearoutput.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/test_clearoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_coalescestreams.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/test_coalescestreams.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_csshtmlheader.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/test_csshtmlheader.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_execute.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_extractattachments.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/test_extractattachments.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_extractoutput.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/test_extractoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_highlightmagics.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/test_highlightmagics.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_latex.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_regexremove.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/test_regexremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_sanitize.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_svg2pdf.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/test_svg2pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_tagremove.py` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/test_tagremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb` & `nbconvert-7.7.1/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/templates/skeleton/Makefile` & `nbconvert-7.7.1/nbconvert/templates/skeleton/Makefile`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/base.py` & `nbconvert-7.7.1/nbconvert/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/fake_exporters.py` & `nbconvert-7.7.1/nbconvert/tests/fake_exporters.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/test_nbconvertapp.py` & `nbconvert-7.7.1/nbconvert/tests/test_nbconvertapp.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/files/Unexecuted_widget.ipynb` & `nbconvert-7.7.1/nbconvert/tests/files/Unexecuted_widget.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb` & `nbconvert-7.7.1/nbconvert/tests/files/Unexecuted_widget_2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/files/Widget_List.ipynb` & `nbconvert-7.7.1/nbconvert/tests/files/Widget_List.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/files/containerized_deployments.jpeg` & `nbconvert-7.7.1/nbconvert/tests/files/containerized_deployments.jpeg`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/files/latex-linked-image.ipynb` & `nbconvert-7.7.1/nbconvert/tests/files/latex-linked-image.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/files/markdown_display_priority.ipynb` & `nbconvert-7.7.1/nbconvert/tests/files/markdown_display_priority.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/files/notebook1.ipynb` & `nbconvert-7.7.1/nbconvert/tests/files/notebook1.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/files/notebook2.ipynb` & `nbconvert-7.7.1/nbconvert/tests/files/notebook2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/files/notebook3_with_errors.ipynb` & `nbconvert-7.7.1/nbconvert/tests/files/notebook3_with_errors.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/files/notebook4_jpeg.ipynb` & `nbconvert-7.7.1/nbconvert/tests/files/notebook4_jpeg.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/files/notebook5_embed_images.ipynb` & `nbconvert-7.7.1/nbconvert/tests/files/notebook5_embed_images.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/files/notebook_tags.ipynb` & `nbconvert-7.7.1/nbconvert/tests/files/notebook_tags.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/tests/files/testimage.png` & `nbconvert-7.7.1/nbconvert/tests/files/testimage.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/utils/_contextlib_chdir.py` & `nbconvert-7.7.1/nbconvert/utils/_contextlib_chdir.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/utils/base.py` & `nbconvert-7.7.1/nbconvert/utils/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/utils/exceptions.py` & `nbconvert-7.7.1/nbconvert/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/utils/io.py` & `nbconvert-7.7.1/nbconvert/utils/io.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/utils/iso639_1.py` & `nbconvert-7.7.1/nbconvert/utils/iso639_1.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/utils/pandoc.py` & `nbconvert-7.7.1/nbconvert/utils/pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/utils/text.py` & `nbconvert-7.7.1/nbconvert/utils/text.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/utils/version.py` & `nbconvert-7.7.1/nbconvert/utils/version.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/utils/tests/test_io.py` & `nbconvert-7.7.1/nbconvert/utils/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/utils/tests/test_pandoc.py` & `nbconvert-7.7.1/nbconvert/utils/tests/test_pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/writers/base.py` & `nbconvert-7.7.1/nbconvert/writers/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/writers/debug.py` & `nbconvert-7.7.1/nbconvert/writers/debug.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/writers/files.py` & `nbconvert-7.7.1/nbconvert/writers/files.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/writers/stdout.py` & `nbconvert-7.7.1/nbconvert/writers/stdout.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/writers/tests/test_debug.py` & `nbconvert-7.7.1/nbconvert/writers/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/writers/tests/test_files.py` & `nbconvert-7.7.1/nbconvert/writers/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/nbconvert/writers/tests/test_stdout.py` & `nbconvert-7.7.1/nbconvert/writers/tests/test_stdout.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/asciidoc/index.asciidoc.j2` & `nbconvert-7.7.1/share/templates/asciidoc/index.asciidoc.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/base/display_priority.j2` & `nbconvert-7.7.1/share/templates/base/display_priority.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/base/jupyter_widgets.html.j2` & `nbconvert-7.7.1/share/templates/base/jupyter_widgets.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/base/mathjax.html.j2` & `nbconvert-7.7.1/share/templates/base/mathjax.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/base/null.j2` & `nbconvert-7.7.1/share/templates/base/null.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/classic/base.html.j2` & `nbconvert-7.7.1/share/templates/classic/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/classic/index.html.j2` & `nbconvert-7.7.1/share/templates/classic/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/classic/static/style.css` & `nbconvert-7.7.1/share/templates/classic/static/style.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/lab/base.html.j2` & `nbconvert-7.7.1/share/templates/lab/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/lab/index.html.j2` & `nbconvert-7.7.1/share/templates/lab/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/lab/mermaidjs.html.j2` & `nbconvert-7.7.1/share/templates/lab/mermaidjs.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/lab/static/index.css` & `nbconvert-7.7.1/share/templates/lab/static/index.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/lab/static/theme-dark.css` & `nbconvert-7.7.1/share/templates/lab/static/theme-dark.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/lab/static/theme-light.css` & `nbconvert-7.7.1/share/templates/lab/static/theme-light.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/latex/base.tex.j2` & `nbconvert-7.7.1/share/templates/latex/base.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/latex/display_priority.j2` & `nbconvert-7.7.1/share/templates/latex/display_priority.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/latex/document_contents.tex.j2` & `nbconvert-7.7.1/share/templates/latex/document_contents.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/latex/null.j2` & `nbconvert-7.7.1/share/templates/latex/null.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/latex/report.tex.j2` & `nbconvert-7.7.1/share/templates/latex/report.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/latex/style_bw_ipython.tex.j2` & `nbconvert-7.7.1/share/templates/latex/style_bw_ipython.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/latex/style_ipython.tex.j2` & `nbconvert-7.7.1/share/templates/latex/style_ipython.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/latex/style_jupyter.tex.j2` & `nbconvert-7.7.1/share/templates/latex/style_jupyter.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/latex/style_python.tex.j2` & `nbconvert-7.7.1/share/templates/latex/style_python.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/markdown/index.md.j2` & `nbconvert-7.7.1/share/templates/markdown/index.md.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/reveal/base.html.j2` & `nbconvert-7.7.1/share/templates/reveal/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/reveal/index.html.j2` & `nbconvert-7.7.1/share/templates/reveal/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/reveal/static/custom_reveal.css` & `nbconvert-7.7.1/share/templates/reveal/static/custom_reveal.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/share/templates/rst/index.rst.j2` & `nbconvert-7.7.1/share/templates/rst/index.rst.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/.gitignore` & `nbconvert-7.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/LICENSE` & `nbconvert-7.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/README.md` & `nbconvert-7.7.1/README.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/hatch_build.py` & `nbconvert-7.7.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/pyproject.toml` & `nbconvert-7.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.7.0/PKG-INFO` & `nbconvert-7.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbconvert
-Version: 7.7.0
+Version: 7.7.1
 Summary: Converting Jupyter Notebooks
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
         - Copyright (c) 2001-2015, IPython Development Team
         - Copyright (c) 2015-, Jupyter Development Team
```

