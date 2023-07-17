# Comparing `tmp/nbconvert-7.6.0.tar.gz` & `tmp/nbconvert-7.7.0.tar.gz`

## Comparing `nbconvert-7.6.0.tar` & `nbconvert-7.7.0.tar`

### file list

```diff
@@ -1,279 +1,278 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.mailmap
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.prettierignore
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.readthedocs.yaml
--rw-r--r--   0        0        0    74702 2020-02-02 00:00:00.000000 nbconvert-7.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 nbconvert-7.6.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 nbconvert-7.6.0/RELEASE.md
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 nbconvert-7.6.0/check_requirements.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.github/dependabot.yml
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/Makefile
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/README.md
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/autogen_config.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/make.bat
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/api_examples/template_path/make_html.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/api_examples/template_path/quiz_notebook.py
--rw-r--r--   0        0        0    36829 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/api_examples/template_path/media/image1.png
--rw-r--r--   0        0        0   176383 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/api_examples/template_path/media/image2.png
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/conf.json
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2
--rw-r--r--   0        0        0   266255 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css
--rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/architecture.rst
--rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/conf.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/customizing.rst
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/dejavu.rst
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/development_release.rst
--rw-r--r--   0        0        0     7875 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/execute_api.rst
--rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/external_exporters.rst
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/highlighting.rst
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/index.rst
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/install.rst
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/latex_citations.rst
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/nbconvert_library.ipynb
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/need_help.rst
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/removing_cells.rst
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/usage.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/_static/empty.txt
--rw-r--r--   0        0        0    36971 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/_static/exporter_inheritance.png
--rw-r--r--   0        0        0    65726 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/_static/preprocessor_inheritance.png
--rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/_static/writer_inheritance.png
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/api/exporters.rst
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/api/filters.rst
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/api/index.rst
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/api/nbconvertapp.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/api/postprocessors.rst
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/api/preprocessors.rst
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nbconvert-7.6.0/docs/source/api/writers.rst
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/__main__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/_version.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/conftest.py
--rwxr-xr-x   0        0        0    24129 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/nbconvertapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/py.typed
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/__init__.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/asciidoc.py
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/base.py
--rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/exporter.py
--rw-r--r--   0        0        0    11557 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/html.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/latex.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/markdown.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/notebook.py
--rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/pdf.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/python.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/qt_exporter.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/qt_screenshot.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/qtpdf.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/qtpng.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/rst.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/script.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/slides.py
--rw-r--r--   0        0        0    26970 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/templateexporter.py
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/webpdf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/__init__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/base.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/cheese.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_asciidoc.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_export.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_exporter.py
--rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_html.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_latex.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_markdown.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_notebook.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_pdf.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_python.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_qtpdf.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_qtpng.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_rst.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_script.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_slides.py
--rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_templateexporter.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/test_webpdf.py
--rw-r--r--   0        0        0    45585 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/files/attachment.ipynb
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/files/lablike.html.j2
--rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/files/notebook2.ipynb
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/files/notebook3.ipynb
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/files/notebook_inject.ipynb
--rw-r--r--   0        0        0    16782 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/files/pngmetadata.ipynb
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/files/rawtest.ipynb
--rw-r--r--   0        0        0    19943 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/exporters/tests/files/svg.ipynb
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/__init__.py
--rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/ansi.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/citation.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/datatypefilter.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/filter_links.py
--rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/highlight.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/latex.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/markdown.py
--rw-r--r--   0        0        0    18261 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/markdown_mistune.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/metadata.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/pandoc.py
--rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/strings.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/svg_constants.py
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/widgetsdatatypefilter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/tests/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/tests/test_ansi.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/tests/test_citation.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/tests/test_datatypefilter.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/tests/test_highlight.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/tests/test_latex.py
--rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/tests/test_markdown.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/tests/test_metadata.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/tests/test_pandoc.py
--rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/filters/tests/test_strings.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/postprocessors/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/postprocessors/base.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/postprocessors/serve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/postprocessors/tests/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/postprocessors/tests/test_serve.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/__init__.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/base.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/clearmetadata.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/clearoutput.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/coalescestreams.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/convertfigures.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/csshtmlheader.py
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/execute.py
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/extractattachments.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/extractoutput.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/highlightmagics.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/latex.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/regexremove.py
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/sanitize.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/svg2pdf.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tagremove.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/__init__.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/base.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/fake_kernelmanager.py
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/test_clearmetadata.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/test_clearoutput.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/test_coalescestreams.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/test_csshtmlheader.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/test_execute.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/test_extractattachments.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/test_extractoutput.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/test_highlightmagics.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/test_latex.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/test_regexremove.py
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/test_sanitize.py
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/test_svg2pdf.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/test_tagremove.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/files/HelloWorld.ipynb
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/resources/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/templates/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/templates/skeleton/Makefile
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/templates/skeleton/README.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/__init__.py
--rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/base.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/fake_exporters.py
--rw-r--r--   0        0        0    29353 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/test_nbconvertapp.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/utils.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/exporter_entrypoint/eptest.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/exporter_entrypoint/eptest-0.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/Unexecuted_widget.ipynb
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb
--rw-r--r--   0        0        0    96479 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/Widget_List.ipynb
--rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/containerized_deployments.jpeg
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/hello.py
--rw-r--r--   0        0        0    18524 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/issue1849_svg.ipynb
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/jupyter_nbconvert_config.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/latex-linked-image.ipynb
--rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/markdown_display_priority.ipynb
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/notebook1.ipynb
--rw-r--r--   0        0        0   125459 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/notebook2.ipynb
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/notebook3_with_errors.ipynb
--rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/notebook4_jpeg.ipynb
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/notebook5_embed_images.ipynb
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/notebook_jl.ipynb
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/notebook_tags.ipynb
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/override.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/tests/files/testimage.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/utils/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/utils/_contextlib_chdir.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/utils/base.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/utils/exceptions.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/utils/io.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/utils/lexers.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/utils/pandoc.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/utils/text.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/utils/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/utils/tests/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/utils/tests/test_io.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/utils/tests/test_pandoc.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/utils/tests/test_version.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/writers/__init__.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/writers/base.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/writers/debug.py
--rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/writers/files.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/writers/stdout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/writers/tests/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/writers/tests/test_debug.py
--rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/writers/tests/test_files.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 nbconvert-7.6.0/nbconvert/writers/tests/test_stdout.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/asciidoc/conf.json
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/asciidoc/index.asciidoc.j2
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/base/cell_id_anchor.j2
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/base/celltags.j2
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/base/display_priority.j2
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/base/jupyter_widgets.html.j2
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/base/mathjax.html.j2
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/base/null.j2
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/basic/conf.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/basic/index.html.j2
--rw-r--r--   0        0        0     8261 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/classic/base.html.j2
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/classic/conf.json
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/classic/index.html.j2
--rw-r--r--   0        0        0   265101 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/classic/static/style.css
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/compatibility/display_priority.tpl
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/compatibility/full.tpl
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/lab/base.html.j2
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/lab/conf.json
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/lab/index.html.j2
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/lab/mermaidjs.html.j2
--rw-r--r--   0        0        0   581722 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/lab/static/index.css
--rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/lab/static/theme-dark.css
--rw-r--r--   0        0        0    15637 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/lab/static/theme-light.css
--rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/latex/base.tex.j2
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/latex/conf.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/latex/display_priority.j2
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/latex/document_contents.tex.j2
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/latex/index.tex.j2
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/latex/null.j2
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/latex/report.tex.j2
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/latex/style_bw_ipython.tex.j2
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/latex/style_bw_python.tex.j2
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/latex/style_ipython.tex.j2
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/latex/style_jupyter.tex.j2
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/latex/style_python.tex.j2
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/markdown/conf.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/markdown/index.md.j2
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/python/conf.json
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/python/index.py.j2
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/reveal/base.html.j2
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/reveal/cellslidedata.j2
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/reveal/conf.json
--rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/reveal/index.html.j2
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/reveal/static/custom_reveal.css
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/rst/conf.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/rst/index.rst.j2
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/script/conf.json
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/script/script.j2
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/webpdf/conf.json
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 nbconvert-7.6.0/share/templates/webpdf/index.pdf.j2
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nbconvert-7.6.0/.gitignore
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbconvert-7.6.0/LICENSE
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 nbconvert-7.6.0/README.md
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 nbconvert-7.6.0/hatch_build.py
--rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 nbconvert-7.6.0/pyproject.toml
--rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 nbconvert-7.6.0/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.mailmap
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.prettierignore
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    76987 2020-02-02 00:00:00.000000 nbconvert-7.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 nbconvert-7.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 nbconvert-7.7.0/RELEASE.md
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 nbconvert-7.7.0/check_requirements.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/Makefile
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/README.md
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/autogen_config.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/make.bat
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/make_html.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/quiz_notebook.py
+-rw-r--r--   0        0        0    36829 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/media/image1.png
+-rw-r--r--   0        0        0   176383 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/media/image2.png
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/conf.json
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2
+-rw-r--r--   0        0        0   266255 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css
+-rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/architecture.rst
+-rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/conf.py
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/customizing.rst
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/dejavu.rst
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/development_release.rst
+-rw-r--r--   0        0        0     7875 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/execute_api.rst
+-rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/external_exporters.rst
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/highlighting.rst
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/index.rst
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/install.rst
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/latex_citations.rst
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/nbconvert_library.ipynb
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/need_help.rst
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/removing_cells.rst
+-rw-r--r--   0        0        0    11751 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/usage.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/_static/empty.txt
+-rw-r--r--   0        0        0    36971 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/_static/exporter_inheritance.png
+-rw-r--r--   0        0        0    65726 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/_static/preprocessor_inheritance.png
+-rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/_static/writer_inheritance.png
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/exporters.rst
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/filters.rst
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/index.rst
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/nbconvertapp.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/postprocessors.rst
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/preprocessors.rst
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nbconvert-7.7.0/docs/source/api/writers.rst
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/__main__.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/_version.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/conftest.py
+-rwxr-xr-x   0        0        0    24121 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/nbconvertapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/py.typed
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/__init__.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/asciidoc.py
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/base.py
+-rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/exporter.py
+-rw-r--r--   0        0        0    12735 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/html.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/latex.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/markdown.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/notebook.py
+-rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/pdf.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/python.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/qt_exporter.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/qt_screenshot.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/qtpdf.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/qtpng.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/rst.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/script.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/slides.py
+-rw-r--r--   0        0        0    27014 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/templateexporter.py
+-rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/webpdf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/__init__.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/base.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/cheese.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_asciidoc.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_export.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_exporter.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_html.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_latex.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_markdown.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_notebook.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_pdf.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_python.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_qtpdf.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_qtpng.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_rst.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_script.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_slides.py
+-rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_templateexporter.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/test_webpdf.py
+-rw-r--r--   0        0        0    45585 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/attachment.ipynb
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/lablike.html.j2
+-rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/notebook2.ipynb
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/notebook3.ipynb
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/notebook_inject.ipynb
+-rw-r--r--   0        0        0    16782 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/pngmetadata.ipynb
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/rawtest.ipynb
+-rw-r--r--   0        0        0    19943 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/exporters/tests/files/svg.ipynb
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/__init__.py
+-rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/ansi.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/citation.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/datatypefilter.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/filter_links.py
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/highlight.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/latex.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/markdown.py
+-rw-r--r--   0        0        0    18261 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/markdown_mistune.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/metadata.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/pandoc.py
+-rw-r--r--   0        0        0     7461 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/strings.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/widgetsdatatypefilter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_ansi.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_citation.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_datatypefilter.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_highlight.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_latex.py
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_markdown.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_metadata.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_pandoc.py
+-rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/filters/tests/test_strings.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/postprocessors/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/postprocessors/base.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/postprocessors/serve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/postprocessors/tests/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/postprocessors/tests/test_serve.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/__init__.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/base.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/clearmetadata.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/clearoutput.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/coalescestreams.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/convertfigures.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/csshtmlheader.py
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/execute.py
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/extractattachments.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/extractoutput.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/highlightmagics.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/latex.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/regexremove.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/sanitize.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/svg2pdf.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tagremove.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/__init__.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/base.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/fake_kernelmanager.py
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_clearmetadata.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_clearoutput.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_coalescestreams.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_csshtmlheader.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_execute.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_extractattachments.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_extractoutput.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_highlightmagics.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_latex.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_regexremove.py
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_sanitize.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_svg2pdf.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/test_tagremove.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/files/HelloWorld.ipynb
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/resources/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/templates/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/templates/skeleton/Makefile
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/templates/skeleton/README.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/__init__.py
+-rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/base.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/fake_exporters.py
+-rw-r--r--   0        0        0    28724 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/test_nbconvertapp.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/utils.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/exporter_entrypoint/eptest.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/exporter_entrypoint/eptest-0.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/Unexecuted_widget.ipynb
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb
+-rw-r--r--   0        0        0    96479 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/Widget_List.ipynb
+-rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/containerized_deployments.jpeg
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/hello.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/jupyter_nbconvert_config.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/latex-linked-image.ipynb
+-rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/markdown_display_priority.ipynb
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook1.ipynb
+-rw-r--r--   0        0        0   125459 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook2.ipynb
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook3_with_errors.ipynb
+-rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook4_jpeg.ipynb
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook5_embed_images.ipynb
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook_jl.ipynb
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/notebook_tags.ipynb
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/override.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/tests/files/testimage.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/_contextlib_chdir.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/base.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/exceptions.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/io.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/iso639_1.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/lexers.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/pandoc.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/text.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/tests/test_io.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/tests/test_pandoc.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/utils/tests/test_version.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/__init__.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/base.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/debug.py
+-rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/files.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/stdout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/tests/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/tests/test_debug.py
+-rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/tests/test_files.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 nbconvert-7.7.0/nbconvert/writers/tests/test_stdout.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/asciidoc/conf.json
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/asciidoc/index.asciidoc.j2
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/base/cell_id_anchor.j2
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/base/celltags.j2
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/base/display_priority.j2
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/base/jupyter_widgets.html.j2
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/base/mathjax.html.j2
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/base/null.j2
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/basic/conf.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/basic/index.html.j2
+-rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/classic/base.html.j2
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/classic/conf.json
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/classic/index.html.j2
+-rw-r--r--   0        0        0   265101 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/classic/static/style.css
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/compatibility/display_priority.tpl
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/compatibility/full.tpl
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/base.html.j2
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/conf.json
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/index.html.j2
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/mermaidjs.html.j2
+-rw-r--r--   0        0        0   240379 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/static/index.css
+-rw-r--r--   0        0        0    17102 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/static/theme-dark.css
+-rw-r--r--   0        0        0    16019 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/lab/static/theme-light.css
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/base.tex.j2
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/conf.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/display_priority.j2
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/document_contents.tex.j2
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/index.tex.j2
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/null.j2
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/report.tex.j2
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/style_bw_ipython.tex.j2
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/style_bw_python.tex.j2
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/style_ipython.tex.j2
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/style_jupyter.tex.j2
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/latex/style_python.tex.j2
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/markdown/conf.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/markdown/index.md.j2
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/python/conf.json
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/python/index.py.j2
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/reveal/base.html.j2
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/reveal/cellslidedata.j2
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/reveal/conf.json
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/reveal/index.html.j2
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/reveal/static/custom_reveal.css
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/rst/conf.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/rst/index.rst.j2
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/script/conf.json
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/script/script.j2
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/webpdf/conf.json
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 nbconvert-7.7.0/share/templates/webpdf/index.pdf.j2
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nbconvert-7.7.0/.gitignore
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbconvert-7.7.0/LICENSE
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 nbconvert-7.7.0/README.md
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 nbconvert-7.7.0/hatch_build.py
+-rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 nbconvert-7.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 nbconvert-7.7.0/PKG-INFO
```

### Comparing `nbconvert-7.6.0/.mailmap` & `nbconvert-7.7.0/.mailmap`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/.pre-commit-config.yaml` & `nbconvert-7.7.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.23.1
+    rev: 0.23.2
     hooks:
       - id: check-github-workflows
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
@@ -31,12 +31,12 @@
           [mdformat-gfm, mdformat-frontmatter, mdformat-footnote]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.270
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.276
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `nbconvert-7.6.0/CHANGELOG.md` & `nbconvert-7.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,53 @@
 # Changes in nbconvert
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 7.7.0
+
+([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.6.0...f2fc3e13fe8e8836324550dac5286bbb0e4315bb))
+
+### Enhancements made
+
+- \[Accessibility\] some accessibility improvements [#2021](https://github.com/jupyter/nbconvert/pull/2021) ([@brichet](https://github.com/brichet))
+- Adopt playwright [#2013](https://github.com/jupyter/nbconvert/pull/2013) ([@brichet](https://github.com/brichet))
+- Update to Jupyterlab 4 [#2012](https://github.com/jupyter/nbconvert/pull/2012) ([@brichet](https://github.com/brichet))
+
+### Bugs fixed
+
+- html: write image/svg+xml data as base64 and skip clean_html [#2018](https://github.com/jupyter/nbconvert/pull/2018) ([@jstorrs](https://github.com/jstorrs))
+- Remove HTML escaping JSON-encoded widget state [#1934](https://github.com/jupyter/nbconvert/pull/1934) ([@manzt](https://github.com/manzt))
+
+### Maintenance and upkeep improvements
+
+- Fix lint error [#2010](https://github.com/jupyter/nbconvert/pull/2010) ([@blink1073](https://github.com/blink1073))
+- Support Python 3.8-3.12 [#2008](https://github.com/jupyter/nbconvert/pull/2008) ([@blink1073](https://github.com/blink1073))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/nbconvert/graphs/contributors?from=2023-06-19&to=2023-07-17&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Ablink1073+updated%3A2023-06-19..2023-07-17&type=Issues) | [@brichet](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Abrichet+updated%3A2023-06-19..2023-07-17&type=Issues) | [@jstorrs](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Ajstorrs+updated%3A2023-06-19..2023-07-17&type=Issues) | [@maartenbreddels](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Amaartenbreddels+updated%3A2023-06-19..2023-07-17&type=Issues) | [@manzt](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Amanzt+updated%3A2023-06-19..2023-07-17&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3AmartinRenou+updated%3A2023-06-19..2023-07-17&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Apre-commit-ci+updated%3A2023-06-19..2023-07-17&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 7.6.0
 
 ([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.5.0...60af6d897c083444586829c636f278d84ae81962))
 
 ### Maintenance and upkeep improvements
 
 - Update to Mistune v3 [#1820](https://github.com/jupyter/nbconvert/pull/1820) ([@TiagodePAlves](https://github.com/TiagodePAlves))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/nbconvert/graphs/contributors?from=2023-06-13&to=2023-06-19&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Ablink1073+updated%3A2023-06-13..2023-06-19&type=Issues) | [@kloczek](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Akloczek+updated%3A2023-06-13..2023-06-19&type=Issues) | [@TiagodePAlves](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3ATiagodePAlves+updated%3A2023-06-13..2023-06-19&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 7.5.0
 
 ([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.4.0...3dd3a67bf16474042efac25519ef257d708a8d7b))
 
 ### Enhancements made
 
 - Add mermaidjs 10.2.3 [#1957](https://github.com/jupyter/nbconvert/pull/1957) ([@bollwyvl](https://github.com/bollwyvl))
```

### Comparing `nbconvert-7.6.0/CONTRIBUTING.md` & `nbconvert-7.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/RELEASE.md` & `nbconvert-7.7.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/check_requirements.py` & `nbconvert-7.7.0/check_requirements.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/.github/workflows/docs.yml` & `nbconvert-7.7.0/.github/workflows/docs.yml`

 * *Files 19% similar despite different names*

```diff
@@ -10,25 +10,25 @@
   cancel-in-progress: true
 
 jobs:
   generate-docs:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.10"]
+        python-version: ["3.8", "3.11"]
     steps:
       - name: Check out repository code
         uses: actions/checkout@v3
       - name: Install dependencies
         run: |
           sudo apt-get update
           sudo apt-get install texlive-plain-generic inkscape texlive-xetex latexmk enchant-2
 
           # pandoc is not up to date in the ubuntu repos, so we install directly
-          wget https://github.com/jgm/pandoc/releases/download/2.14.2/pandoc-2.14.2-1-amd64.deb && sudo dpkg -i pandoc-2.14.2-1-amd64.deb
+          wget https://github.com/jgm/pandoc/releases/download/3.1.2/pandoc-3.1.2-1-amd64.deb && sudo dpkg -i pandoc-3.1.2-1-amd64.deb
 
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       - name: Install
         run: pip install -v ".[all]"
       - name: List installed packages
         run: |
           pip freeze
```

### Comparing `nbconvert-7.6.0/.github/workflows/prep-release.yml` & `nbconvert-7.7.0/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/.github/workflows/publish-release.yml` & `nbconvert-7.7.0/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/.github/workflows/tests.yml` & `nbconvert-7.7.0/.github/workflows/tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
   run-tests:
     runs-on: ${{ matrix.os }}
     env:
       NBFORMAT_VALIDATOR: jsonschema
     strategy:
       matrix:
         os: ["ubuntu-20.04", "macos-latest", "windows-latest"]
-        python-version: ["3.7", "3.10"]
+        python-version: ["3.8", "3.11"]
         include:
           - os: "windows-latest"
-            python-version: "3.8"
-          - os: "ubuntu-20.04"
             python-version: "3.9"
+          - os: "ubuntu-20.04"
+            python-version: "3.10"
       fail-fast: false
     steps:
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
 
       - name: Install Linux dependencies
         if: startsWith(runner.os, 'Linux')
@@ -48,18 +48,27 @@
         if: ${{ startsWith(runner.os, 'linux') }}
         run: |
           xvfb-run --auto-servernum hatch run cov:test
 
       - name: Run tests on other platforms
         if: ${{ !startsWith(runner.os, 'linux')  }}
         run: |
-          hatch run cov:test
+          hatch run cov:nowarn
 
       - uses: jupyterlab/maintainer-tools/.github/actions/upload-coverage@v1
 
+  python312:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
+        with:
+          python_version: "3.12"
+      - run: hatch run test:test
+
   coverage:
     runs-on: ubuntu-latest
     needs:
       - run-tests
     steps:
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/report-coverage@v1
```

### Comparing `nbconvert-7.6.0/docs/Makefile` & `nbconvert-7.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/README.md` & `nbconvert-7.7.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/autogen_config.py` & `nbconvert-7.7.0/docs/autogen_config.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/make.bat` & `nbconvert-7.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/api_examples/template_path/make_html.py` & `nbconvert-7.7.0/docs/api_examples/template_path/make_html.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/api_examples/template_path/quiz_notebook.py` & `nbconvert-7.7.0/docs/api_examples/template_path/quiz_notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/api_examples/template_path/media/image1.png` & `nbconvert-7.7.0/docs/api_examples/template_path/media/image1.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/api_examples/template_path/media/image2.png` & `nbconvert-7.7.0/docs/api_examples/template_path/media/image2.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2` & `nbconvert-7.7.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css` & `nbconvert-7.7.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/architecture.rst` & `nbconvert-7.7.0/docs/source/architecture.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/conf.py` & `nbconvert-7.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/customizing.rst` & `nbconvert-7.7.0/docs/source/customizing.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/dejavu.rst` & `nbconvert-7.7.0/docs/source/dejavu.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/development_release.rst` & `nbconvert-7.7.0/docs/source/development_release.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/execute_api.rst` & `nbconvert-7.7.0/docs/source/execute_api.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/external_exporters.rst` & `nbconvert-7.7.0/docs/source/external_exporters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/highlighting.rst` & `nbconvert-7.7.0/docs/source/highlighting.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/index.rst` & `nbconvert-7.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/install.rst` & `nbconvert-7.7.0/docs/source/install.rst`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     conda install nbconvert
 
 The `Miniconda <https://docs.conda.io/en/latest/miniconda.html>`_ and `Miniforge <https://github.com/conda-forge/miniforge/>`_ distributions both provide a minimal conda installation.
 
 .. important::
 
     To unlock its full capabilities, nbconvert requires Pandoc, TeX
-    (specifically, XeLaTeX) and Pyppeteer. These must be installed separately.
+    (specifically, XeLaTeX) and playwright. These must be installed separately.
 
 Installing Pandoc
 -----------------
 
 For converting markdown to formats other than HTML, nbconvert uses
 `Pandoc <https://pandoc.org>`_ (1.12.1 or later).
 
@@ -76,21 +76,21 @@
 may not be able to use nbconvert's standard tooling to convert
 notebooks to PDF.
 
 Installing Chromium
 -------------------
 
 For converting notebooks to PDF with ``--to webpdf``, nbconvert requires the
-`Pyppeteer <https://github.com/pyppeteer/pyppeteer>`_ Chromium automation library.
+`playwright <https://github.com/microsoft/playwright-python>`_ Chromium automation library.
 
-Pyppeteer makes use of a specific version of Chromium. If it does not find a suitable
+Playwright makes use of a specific version of Chromium. If it does not find a suitable
 installation of the web browser, it can automatically download it if the ``--allow-chromium-download``
 flag is passed to the command line.
 
-To install a suitable version of pyppeteer, you can pip install ``nbconvert[webpdf]``.
+To install a suitable version of playwright, you can pip install ``nbconvert[webpdf]``.
 
 PDF conversion on a limited TeX environment
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If you are only able to install a limited TeX environment, there are two main routes you could take to convert to PDF:
 
 1. Using TeX by hand
```

### Comparing `nbconvert-7.6.0/docs/source/latex_citations.rst` & `nbconvert-7.7.0/docs/source/latex_citations.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/nbconvert_library.ipynb` & `nbconvert-7.7.0/docs/source/nbconvert_library.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/need_help.rst` & `nbconvert-7.7.0/docs/source/need_help.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/removing_cells.rst` & `nbconvert-7.7.0/docs/source/removing_cells.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/usage.rst` & `nbconvert-7.7.0/docs/source/usage.rst`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 WebPDF
 ~~~~~~
 * ``--to webpdf``
 
   Generates a PDF by first rendering to HTML, rendering the HTML Chromium headless, and
   exporting to PDF. This exporter supports the same templates as ``--to html``.
 
-  The webpdf exporter requires the ``pyppeteer`` Chromium automation library, which
+  The webpdf exporter requires the ``playwright`` Chromium automation library, which
   can be installed via ``nbconvert[webpdf]``.
 
 .. _convert_revealjs:
 
 Reveal.js HTML slideshow
 ~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `nbconvert-7.6.0/docs/source/_static/exporter_inheritance.png` & `nbconvert-7.7.0/docs/source/_static/exporter_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/_static/preprocessor_inheritance.png` & `nbconvert-7.7.0/docs/source/_static/preprocessor_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/_static/writer_inheritance.png` & `nbconvert-7.7.0/docs/source/_static/writer_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/api/exporters.rst` & `nbconvert-7.7.0/docs/source/api/exporters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/api/filters.rst` & `nbconvert-7.7.0/docs/source/api/filters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/docs/source/api/preprocessors.rst` & `nbconvert-7.7.0/docs/source/api/preprocessors.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/nbconvertapp.py` & `nbconvert-7.7.0/nbconvert/nbconvertapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,15 @@
                     filenames.append(filename)
         self.notebooks = filenames
 
     def init_writer(self):
         """Initialize the writer (which is stateless)"""
         self._writer_class_changed({"new": self.writer_class})
         self.writer = self.writer_factory(parent=self)
-        if hasattr(self.writer, "build_directory") and self.writer.build_directory != "":  # noqa
+        if hasattr(self.writer, "build_directory") and self.writer.build_directory != "":
             self.use_output_suffix = False
 
     def init_postprocessor(self):
         """Initialize the postprocessor (which is stateless)"""
         self._postprocessor_class_changed({"new": self.postprocessor_class})
         if self.postprocessor_factory:
             self.postprocessor = self.postprocessor_factory(parent=self)
```

### Comparing `nbconvert-7.6.0/nbconvert/exporters/__init__.py` & `nbconvert-7.7.0/nbconvert/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/asciidoc.py` & `nbconvert-7.7.0/nbconvert/exporters/asciidoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/base.py` & `nbconvert-7.7.0/nbconvert/exporters/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/exporter.py` & `nbconvert-7.7.0/nbconvert/exporters/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         `**kw`
             Ignored
 
         """
         # Pull the metadata from the filesystem.
         if resources is None:
             resources = ResourcesDict()
-        if "metadata" not in resources or resources["metadata"] == "":  # noqa
+        if "metadata" not in resources or resources["metadata"] == "":
             resources["metadata"] = ResourcesDict()
         path, basename = os.path.split(filename)
         notebook_name = os.path.splitext(basename)[0]
         resources["metadata"]["name"] = notebook_name
         resources["metadata"]["path"] = path
 
         modified_date = datetime.datetime.fromtimestamp(
```

### Comparing `nbconvert-7.6.0/nbconvert/exporters/html.py` & `nbconvert-7.7.0/nbconvert/exporters/html.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,29 +8,31 @@
 import mimetypes
 import os
 from pathlib import Path
 from typing import Any, Dict, Optional, Tuple
 
 import jinja2
 import markupsafe
+from bs4 import BeautifulSoup
 from jupyter_core.paths import jupyter_path
-from traitlets import Bool, Unicode, default
+from traitlets import Bool, Unicode, default, validate
 from traitlets.config import Config
 
 if tuple(int(x) for x in jinja2.__version__.split(".")[:3]) < (3, 0, 0):
     from jinja2 import contextfilter  # type:ignore
 else:
     from jinja2 import pass_context as contextfilter
 
 from jinja2.loaders import split_template_path
 from nbformat import NotebookNode
 
 from nbconvert.filters.highlight import Highlight2HTML
 from nbconvert.filters.markdown_mistune import IPythonRenderer, MarkdownWithMath
 from nbconvert.filters.widgetsdatatypefilter import WidgetsDataTypeFilter
+from nbconvert.utils.iso639_1 import iso639_1
 
 from .templateexporter import TemplateExporter
 
 
 def find_lab_theme(theme_name):
     """
     Find a JupyterLab theme location by name.
@@ -198,14 +200,28 @@
         )
         if super().default_config:
             c2 = super().default_config.copy()
             c2.merge(c)
             c = c2
         return c
 
+    language_code = Unicode(
+        "en", help="Language code of the content, should be one of the ISO639-1"
+    ).tag(config=True)
+
+    @validate("language_code")
+    def _valid_language_code(self, proposal):
+        if self.language_code not in iso639_1:
+            self.log.warn(
+                f'"{self.language_code}" is not an ISO 639-1 language code. '
+                'It has been replaced by the default value "en".'
+            )
+            return proposal["trait"].default_value
+        return proposal["value"]
+
     @contextfilter
     def markdown2html(self, context, source):
         """Markdown to HTML filter respecting the anchor_link_text setting"""
         cell = context.get("cell", {})
         attachments = cell.get("attachments", {})
         path = context.get("resources", {}).get("metadata", {}).get("path", "")
 
@@ -236,15 +252,26 @@
 
         filter_data_type = WidgetsDataTypeFilter(
             notebook_metadata=self._nb_metadata, parent=self, resources=resources
         )
 
         self.register_filter("highlight_code", highlight_code)
         self.register_filter("filter_data_type", filter_data_type)
-        return super().from_notebook_node(nb, resources, **kw)
+        html, resources = super().from_notebook_node(nb, resources, **kw)
+        soup = BeautifulSoup(html, features="html.parser")
+        # Add image's alternative text
+        for elem in soup.select("img:not([alt])"):
+            elem.attrs["alt"] = "Image"
+        # Set input and output focusable
+        for elem in soup.select(".jp-Notebook div.jp-Cell-inputWrapper"):
+            elem.attrs["tabindex"] = "0"
+        for elem in soup.select(".jp-Notebook div.jp-OutputArea-output"):
+            elem.attrs["tabindex"] = "0"
+
+        return str(soup), resources
 
     def _init_resources(self, resources):  # noqa
         def resources_include_css(name):
             env = self.environment
             code = """<style type="text/css">\n%s</style>""" % (env.loader.get_source(env, name)[0])
             return markupsafe.Markup(code)
 
@@ -314,8 +341,9 @@
         resources["mathjax_url"] = self.mathjax_url
         resources["mermaid_js_url"] = self.mermaid_js_url
         resources["jquery_url"] = self.jquery_url
         resources["jupyter_widgets_base_url"] = self.jupyter_widgets_base_url
         resources["widget_renderer_url"] = self.widget_renderer_url
         resources["html_manager_semver_range"] = self.html_manager_semver_range
         resources["should_sanitize_html"] = self.sanitize_html
+        resources["language_code"] = self.language_code
         return resources
```

### Comparing `nbconvert-7.6.0/nbconvert/exporters/latex.py` & `nbconvert-7.7.0/nbconvert/exporters/latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/markdown.py` & `nbconvert-7.7.0/nbconvert/exporters/markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/notebook.py` & `nbconvert-7.7.0/nbconvert/exporters/notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/pdf.py` & `nbconvert-7.7.0/nbconvert/exporters/pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/python.py` & `nbconvert-7.7.0/nbconvert/exporters/python.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/qt_exporter.py` & `nbconvert-7.7.0/nbconvert/exporters/qt_exporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/qt_screenshot.py` & `nbconvert-7.7.0/nbconvert/exporters/qt_screenshot.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/qtpdf.py` & `nbconvert-7.7.0/nbconvert/exporters/qtpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/rst.py` & `nbconvert-7.7.0/nbconvert/exporters/rst.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/script.py` & `nbconvert-7.7.0/nbconvert/exporters/script.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/slides.py` & `nbconvert-7.7.0/nbconvert/exporters/slides.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/templateexporter.py` & `nbconvert-7.7.0/nbconvert/exporters/templateexporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     "prevent_list_blocks": filters.prevent_list_blocks,
     "get_metadata": filters.get_metadata,
     "convert_pandoc": filters.convert_pandoc,
     "json_dumps": json.dumps,
     # For removing any HTML
     "escape_html": lambda s: html.escape(str(s)),
     "escape_html_keep_quotes": lambda s: html.escape(str(s), quote=False),
+    "escape_html_script": lambda s: s.replace("/", "\\/"),
     # For sanitizing HTML for any XSS
     "clean_html": filters.clean_html,
     "strip_trailing_newline": filters.strip_trailing_newline,
     "text_base64": filters.text_base64,
 }
 
 
@@ -535,15 +536,15 @@
         super()._init_preprocessors()
         conf = self._get_conf()
         preprocessors = conf.get("preprocessors", {})
         # preprocessors is a dict for three reasons
         #  * We rely on recursive_update, which can only merge dicts, lists will be overwritten
         #  * We can use the key with numerical prefixing to guarantee ordering (/etc/*.d/XY-file style)
         #  * We can disable preprocessors by overwriting the value with None
-        for _, preprocessor in sorted(preprocessors.items(), key=lambda x: x[0]):  # type:ignore
+        for _, preprocessor in sorted(preprocessors.items(), key=lambda x: x[0]):
             if preprocessor is not None:
                 kwargs = preprocessor.copy()
                 preprocessor_cls = kwargs.pop("type")
                 preprocessor_cls = import_item(preprocessor_cls)
                 if preprocessor_cls.__name__ in self.config:
                     kwargs.update(self.config[preprocessor_cls.__name__])
                 preprocessor = preprocessor_cls(**kwargs)  # noqa
```

### Comparing `nbconvert-7.6.0/nbconvert/exporters/webpdf.py` & `nbconvert-7.7.0/nbconvert/exporters/webpdf.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 
 import asyncio
 import concurrent.futures
 import os
+import subprocess
+import sys
 import tempfile
 from importlib import util as importlib_util
 
 from traitlets import Bool, default
 
 from .html import HTMLExporter
 
-PYPPETEER_INSTALLED = importlib_util.find_spec("pyppeteer") is not None
+PLAYWRIGHT_INSTALLED = importlib_util.find_spec("playwright") is not None
+IS_WINDOWS = os.name == 'nt'
 
 
 class WebPDFExporter(HTMLExporter):
     """Writer designed to write to PDF files.
 
     This inherits from :class:`HTMLExporter`. It creates the HTML using the
-    template machinery, and then run pyppeteer to create a pdf.
+    template machinery, and then run playwright to create a pdf.
     """
 
     export_from_notebook = "PDF via HTML"
 
     allow_chromium_download = Bool(
         False,
         help="Whether to allow downloading Chromium if no suitable version is found on the system.",
@@ -61,48 +64,52 @@
         ``https://github.com/puppeteer/puppeteer/blob/main@%7B2020-12-14T17:22:24Z%7D/docs/troubleshooting.md#setting-up-chrome-linux-sandbox``
         has more information.
 
         This is required for webpdf to work inside most container environments.
         """,
     ).tag(config=True)
 
-    def _check_launch_reqs(self):
-        try:
-            from pyppeteer import launch  # type: ignore[import]
-            from pyppeteer.util import check_chromium  # type:ignore
-        except ModuleNotFoundError as e:
-            msg = (
-                "Pyppeteer is not installed to support Web PDF conversion. "
-                "Please install `nbconvert[webpdf]` to enable."
-            )
-            raise RuntimeError(msg) from e
-        if not self.allow_chromium_download and not check_chromium():
-            msg = (
-                "No suitable chromium executable found on the system. "
-                "Please use '--allow-chromium-download' to allow downloading one."
-            )
-            raise RuntimeError(msg)
-        return launch
-
-    def run_pyppeteer(self, html):
-        """Run pyppeteer."""
+    def run_playwright(self, html):
+        """Run playwright."""
 
         async def main(temp_file):
-            """Run main pyppeteer script."""
+            """Run main playwright script."""
             args = ["--no-sandbox"] if self.disable_sandbox else []
-            browser = await self._check_launch_reqs()(
-                handleSIGINT=False, handleSIGTERM=False, handleSIGHUP=False, args=args
-            )
-            page = await browser.newPage()
-            await page.emulateMedia("print")
-            await page.waitFor(100)
-            await page.goto(f"file://{temp_file.name}", waitUntil="networkidle0")
-            await page.waitFor(100)
+            try:
+                from playwright.async_api import async_playwright  # type: ignore[import]
+            except ModuleNotFoundError as e:
+                msg = (
+                    "Playwright is not installed to support Web PDF conversion. "
+                    "Please install `nbconvert[webpdf]` to enable."
+                )
+                raise RuntimeError(msg) from e
 
-            pdf_params = {"printBackground": True}
+            if self.allow_chromium_download:
+                cmd = [sys.executable, "-m", "playwright", "install", "chromium"]
+                subprocess.check_call(cmd)  # noqa
+
+            playwright = await async_playwright().start()
+            chromium = playwright.chromium
+
+            try:
+                browser = await chromium.launch(
+                    handle_sigint=False, handle_sigterm=False, handle_sighup=False, args=args
+                )
+            except Exception as e:
+                msg = (
+                    "No suitable chromium executable found on the system. "
+                    "Please use '--allow-chromium-download' to allow downloading one,"
+                    "or install it using `playwright install chromium`."
+                )
+                raise RuntimeError(msg) from e
+
+            page = await browser.new_page()
+            await page.goto(f"file://{temp_file.name}", wait_until="networkidle")
+
+            pdf_params = {"print_background": True}
             if not self.paginate:
                 # Floating point precision errors cause the printed
                 # PDF from spilling over a new page by a pixel fraction.
                 dimensions = await page.evaluate(
                     """() => {
                     const rect = document.body.getBoundingClientRect();
                     return {
@@ -116,15 +123,15 @@
                 # 200 inches is the maximum size for Adobe Acrobat Reader.
                 pdf_params.update(
                     {
                         "width": min(width, 200 * 72),
                         "height": min(height, 200 * 72),
                     }
                 )
-            pdf_data = await page.pdf(pdf_params)
+            pdf_data = await page.pdf(**pdf_params)
 
             await browser.close()
             return pdf_data
 
         pool = concurrent.futures.ThreadPoolExecutor()
         # Create a temporary file to pass the HTML code to Chromium:
         # Unfortunately, tempfile on Windows does not allow for an already open
@@ -135,31 +142,35 @@
         with temp_file:
             temp_file.write(html.encode("utf-8"))
         try:
             # TODO: when dropping Python 3.6, use
             # pdf_data = pool.submit(asyncio.run, main(temp_file)).result()
             def run_coroutine(coro):
                 """Run an internal coroutine."""
-                loop = asyncio.new_event_loop()
+                loop = (
+                    asyncio.ProactorEventLoop()  # type:ignore
+                    if IS_WINDOWS
+                    else asyncio.new_event_loop()
+                )
+
                 asyncio.set_event_loop(loop)
                 return loop.run_until_complete(coro)
 
             pdf_data = pool.submit(run_coroutine, main(temp_file)).result()
         finally:
-            # Ensure the file is deleted even if pypeteer raises an exception
+            # Ensure the file is deleted even if playwright raises an exception
             os.unlink(temp_file.name)
         return pdf_data
 
     def from_notebook_node(self, nb, resources=None, **kw):
         """Convert from a notebook node."""
-        self._check_launch_reqs()
         html, resources = super().from_notebook_node(nb, resources=resources, **kw)
 
         self.log.info("Building PDF")
-        pdf_data = self.run_pyppeteer(html)
+        pdf_data = self.run_playwright(html)
         self.log.info("PDF successfully created")
 
         # convert output extension to pdf
         # the writer above required it to be html
         resources["output_extension"] = ".pdf"
 
         return pdf_data, resources
```

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/base.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/cheese.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/cheese.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_asciidoc.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_asciidoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_export.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_exporter.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_html.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_html.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,20 +72,20 @@
     def test_png_metadata(self):
         """
         Does HTMLExporter with the 'classic' template treat pngs with width/height metadata correctly?
         """
         (output, resources) = HTMLExporter(template_name="classic").from_filename(
             self._get_notebook(nb_name="pngmetadata.ipynb")
         )
-        check_for_png = re.compile(r'<img src="[^"]*?"([^>]*?)>')
+        check_for_png = re.compile(r'<img alt="Image"([^>]*?)>')
         result = check_for_png.search(output)
         assert result
         attr_string = result.group(1)
-        assert "width" in attr_string
-        assert "height" in attr_string
+        assert "width=" in attr_string
+        assert "height=" in attr_string
 
     def test_javascript_output(self):
         nb = v4.new_notebook(
             cells=[
                 v4.new_code_cell(
                     outputs=[
                         v4.new_output(
@@ -99,21 +99,20 @@
         (output, resources) = HTMLExporter(template_name="classic").from_notebook_node(nb)
         self.assertIn("javascript_output", output)
 
     def test_attachments(self):
         (output, resources) = HTMLExporter(template_name="classic").from_file(
             self._get_notebook(nb_name="attachment.ipynb")
         )
-        check_for_png = re.compile(r'<img src="[^"]*?"([^>]*?)>')
+        check_for_png = re.compile(r'<img alt="image.png" src="([^"]*?)"/>')
         result = check_for_png.search(output)
         assert result
-        self.assertTrue(result.group(0).strip().startswith('<img src="data:image/png;base64,iVBOR'))
-        self.assertTrue(result.group(1).strip().startswith('alt="image.png"'))
+        self.assertTrue(result.group(1).strip().startswith('data:image/png;base64,iVBOR'))
 
-        check_for_data = re.compile(r'<img src="(?P<url>[^"]*?)"')
+        check_for_data = re.compile(r'<img alt="image.png" src="(?P<url>[^"]*?)"')
         results = check_for_data.findall(output)
         assert results[0] != results[1], "attachments only need to be unique within a cell"
         assert "image/svg" in results[1], "second image should use svg"
 
     def test_custom_filter_highlight_code(self):
         # Overwriting filters takes place at: Exporter.from_notebook_node
         nb = v4.new_notebook()
```

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_latex.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_markdown.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_notebook.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_pdf.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_python.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_qtpdf.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_qtpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_qtpng.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_qtpng.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_rst.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_rst.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_script.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_slides.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_slides.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_templateexporter.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_templateexporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/test_webpdf.py` & `nbconvert-7.7.0/nbconvert/exporters/tests/test_webpdf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 """Tests for the latex preprocessor"""
 
 # Copyright (c) IPython Development Team.
 # Distributed under the terms of the Modified BSD License.
 
+import builtins
 from unittest.mock import patch
 
 import pytest
 
-from ..webpdf import PYPPETEER_INSTALLED, WebPDFExporter
+from ..exporter import Exporter
+from ..webpdf import PLAYWRIGHT_INSTALLED, WebPDFExporter
 from .base import ExportersTestsBase
 
+real_import = builtins.__import__
 
-@pytest.mark.skipif(not PYPPETEER_INSTALLED, reason="Pyppeteer not installed")
+
+class FakeBrowser:
+    executable_path: str = ''
+
+
+def monkey_import_notfound(name, globals_ctx=None, locals_ctx=None, fromlist=(), level=0):
+    if name == "playwright.async_api":
+        msg = 'Fake missing'
+        raise ModuleNotFoundError(msg)
+    return real_import(name, globals=globals_ctx, locals=locals_ctx, fromlist=fromlist, level=level)
+
+
+@pytest.mark.skipif(not PLAYWRIGHT_INSTALLED, reason="Playwright not installed")
 class TestWebPDFExporter(ExportersTestsBase):
     """Contains test functions for webpdf.py"""
 
     exporter_class = WebPDFExporter  # type:ignore
 
     @pytest.mark.network
     def test_export(self):
@@ -23,26 +38,27 @@
         Can a TemplateExporter export something?
         """
         (output, resources) = WebPDFExporter(allow_chromium_download=True).from_filename(
             self._get_notebook()
         )
         assert len(output) > 0
 
-    @patch("pyppeteer.util.check_chromium", return_value=False)
-    def test_webpdf_without_chromium(self, mock_check_chromium):
+    @patch("playwright.async_api._generated.Playwright.chromium", return_value=FakeBrowser())
+    def test_webpdf_without_chromium(self, mock_chromium):
         """
         Generate PDFs if chromium not present?
         """
         with pytest.raises(RuntimeError):
             WebPDFExporter(allow_chromium_download=False).from_filename(self._get_notebook())
 
-    def test_webpdf_without_pyppeteer(self):
+    @patch("builtins.__import__", monkey_import_notfound)
+    def test_webpdf_without_playwright(self):
         """
-        Generate PDFs if chromium not present?
+        Generate PDFs if playwright not installed?
         """
         with pytest.raises(RuntimeError):
+            base_exporter = Exporter()
             exporter = WebPDFExporter()
             with open(self._get_notebook(), encoding="utf-8") as f:
-                nb = exporter.from_file(f, resources={})
+                nb = base_exporter.from_file(f, resources={})[0]
                 # Have to do this as the very last action as traitlets do dynamic importing often
-                with patch("builtins.__import__", side_effect=ModuleNotFoundError("Fake missing")):
-                    exporter.from_notebook_node(nb)
+                exporter.from_notebook_node(nb)
```

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/files/attachment.ipynb` & `nbconvert-7.7.0/nbconvert/exporters/tests/files/attachment.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/files/notebook2.ipynb` & `nbconvert-7.7.0/nbconvert/exporters/tests/files/notebook2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/files/notebook3.ipynb` & `nbconvert-7.7.0/nbconvert/exporters/tests/files/notebook3.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/files/notebook_inject.ipynb` & `nbconvert-7.7.0/nbconvert/exporters/tests/files/notebook_inject.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/files/pngmetadata.ipynb` & `nbconvert-7.7.0/nbconvert/exporters/tests/files/pngmetadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb` & `nbconvert-7.7.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/files/rawtest.ipynb` & `nbconvert-7.7.0/nbconvert/exporters/tests/files/rawtest.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/exporters/tests/files/svg.ipynb` & `nbconvert-7.7.0/nbconvert/exporters/tests/files/svg.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/ansi.py` & `nbconvert-7.7.0/nbconvert/filters/ansi.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/citation.py` & `nbconvert-7.7.0/nbconvert/filters/citation.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/datatypefilter.py` & `nbconvert-7.7.0/nbconvert/filters/datatypefilter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/filter_links.py` & `nbconvert-7.7.0/nbconvert/filters/filter_links.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/highlight.py` & `nbconvert-7.7.0/nbconvert/filters/highlight.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/latex.py` & `nbconvert-7.7.0/nbconvert/filters/latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/markdown.py` & `nbconvert-7.7.0/nbconvert/filters/markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/markdown_mistune.py` & `nbconvert-7.7.0/nbconvert/filters/markdown_mistune.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/pandoc.py` & `nbconvert-7.7.0/nbconvert/filters/pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/strings.py` & `nbconvert-7.7.0/nbconvert/filters/strings.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,16 +37,14 @@
     "add_prompts",
     "ascii_only",
     "prevent_list_blocks",
     "strip_trailing_newline",
     "text_base64",
 ]
 
-from nbconvert.filters.svg_constants import ALLOWED_SVG_ATTRIBUTES, ALLOWED_SVG_TAGS
-
 
 def wrap_text(text, width=100):
     """
     Intelligently wrap text.
     Wrap text without breaking words if possible.
 
     Parameters
@@ -87,19 +85,17 @@
     element = element.decode() if isinstance(element, bytes) else str(element)
     kwargs = {}
     css_sanitizer = _get_default_css_sanitizer()
     if css_sanitizer:
         kwargs['css_sanitizer'] = css_sanitizer
     return bleach.clean(
         element,
-        tags=[*bleach.ALLOWED_TAGS, *ALLOWED_SVG_TAGS, "div", "pre", "code", "span"],
-        strip_comments=False,
+        tags=[*bleach.ALLOWED_TAGS, "div", "pre", "code", "span"],
         attributes={
             **bleach.ALLOWED_ATTRIBUTES,
-            **{svg_tag: list(ALLOWED_SVG_ATTRIBUTES) for svg_tag in ALLOWED_SVG_TAGS},
             "*": ["class", "id"],
         },
         **kwargs,
     )
 
 
 def _convert_header_id(header_contents):
```

### Comparing `nbconvert-7.6.0/nbconvert/filters/widgetsdatatypefilter.py` & `nbconvert-7.7.0/nbconvert/filters/widgetsdatatypefilter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/tests/test_ansi.py` & `nbconvert-7.7.0/nbconvert/filters/tests/test_ansi.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/tests/test_citation.py` & `nbconvert-7.7.0/nbconvert/filters/tests/test_citation.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/tests/test_datatypefilter.py` & `nbconvert-7.7.0/nbconvert/filters/tests/test_datatypefilter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/tests/test_highlight.py` & `nbconvert-7.7.0/nbconvert/filters/tests/test_highlight.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,16 +75,14 @@
 
     @pytest.mark.filterwarnings("ignore")
     def test_inject_html(self):
         out = highlight2html(self.tests[0], 'ipython3-foo"><script>alert(1)</script>')
         assert "<script>alert(1)</script>" not in out
 
     def _extract_tokens(self, root, cls):
-        return set(  # noqa
-            map(lambda x: x.text, root.findall(".//*[@class='" + cls + "']"))  # type:ignore
-        )
+        return set(map(lambda x: x.text, root.findall(".//*[@class='" + cls + "']")))  # noqa
 
     def _try_highlight(self, method, test, tokens):
         """Try highlighting source, look for key tokens"""
         results = method(test)
         for token in tokens:
             assert token in results
```

### Comparing `nbconvert-7.6.0/nbconvert/filters/tests/test_latex.py` & `nbconvert-7.7.0/nbconvert/filters/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/tests/test_markdown.py` & `nbconvert-7.7.0/nbconvert/filters/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/tests/test_metadata.py` & `nbconvert-7.7.0/nbconvert/filters/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/tests/test_pandoc.py` & `nbconvert-7.7.0/nbconvert/filters/tests/test_pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/filters/tests/test_strings.py` & `nbconvert-7.7.0/nbconvert/filters/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/postprocessors/base.py` & `nbconvert-7.7.0/nbconvert/postprocessors/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/postprocessors/serve.py` & `nbconvert-7.7.0/nbconvert/postprocessors/serve.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/postprocessors/tests/test_serve.py` & `nbconvert-7.7.0/nbconvert/postprocessors/tests/test_serve.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/__init__.py` & `nbconvert-7.7.0/nbconvert/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/base.py` & `nbconvert-7.7.0/nbconvert/preprocessors/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/clearmetadata.py` & `nbconvert-7.7.0/nbconvert/preprocessors/clearmetadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/clearoutput.py` & `nbconvert-7.7.0/nbconvert/preprocessors/clearoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/coalescestreams.py` & `nbconvert-7.7.0/nbconvert/preprocessors/coalescestreams.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/convertfigures.py` & `nbconvert-7.7.0/nbconvert/preprocessors/convertfigures.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/csshtmlheader.py` & `nbconvert-7.7.0/nbconvert/preprocessors/csshtmlheader.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/execute.py` & `nbconvert-7.7.0/nbconvert/preprocessors/execute.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/extractattachments.py` & `nbconvert-7.7.0/nbconvert/preprocessors/extractattachments.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/extractoutput.py` & `nbconvert-7.7.0/nbconvert/preprocessors/extractoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/highlightmagics.py` & `nbconvert-7.7.0/nbconvert/preprocessors/highlightmagics.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/latex.py` & `nbconvert-7.7.0/nbconvert/preprocessors/latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/regexremove.py` & `nbconvert-7.7.0/nbconvert/preprocessors/regexremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/sanitize.py` & `nbconvert-7.7.0/nbconvert/preprocessors/sanitize.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/svg2pdf.py` & `nbconvert-7.7.0/nbconvert/preprocessors/svg2pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tagremove.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tagremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/base.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/fake_kernelmanager.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/fake_kernelmanager.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/test_clearmetadata.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_clearmetadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/test_clearoutput.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_clearoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/test_coalescestreams.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_coalescestreams.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/test_csshtmlheader.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_csshtmlheader.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/test_execute.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/test_extractattachments.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_extractattachments.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/test_extractoutput.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_extractoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/test_highlightmagics.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_highlightmagics.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/test_latex.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/test_regexremove.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_regexremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/test_sanitize.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/test_svg2pdf.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_svg2pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/test_tagremove.py` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/test_tagremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb` & `nbconvert-7.7.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/templates/skeleton/Makefile` & `nbconvert-7.7.0/nbconvert/templates/skeleton/Makefile`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/base.py` & `nbconvert-7.7.0/nbconvert/tests/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,14 +122,17 @@
         if not os.path.isdir(dest):
             os.makedirs(dest)
         files_path = self._get_files_path()
         for pattern in copy_filenames:
             files = glob.glob(os.path.join(files_path, pattern))
             assert files
             for match in files:
+                # Avoid copying the Julia file unless it is explicitly asked for.
+                if 'jl' in match and "jl" not in pattern:
+                    continue
                 shutil.copyfile(match, os.path.join(dest, os.path.basename(match)))
 
     def _get_files_path(self):
         # Get the relative path to this module in the IPython directory.
         names = self.__module__.split(".")[1:-1]
         names.append("files")
```

### Comparing `nbconvert-7.6.0/nbconvert/tests/fake_exporters.py` & `nbconvert-7.7.0/nbconvert/tests/fake_exporters.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/test_nbconvertapp.py` & `nbconvert-7.7.0/nbconvert/tests/test_nbconvertapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 # Distributed under the terms of the Modified BSD License.
 
 import os
 from tempfile import TemporaryDirectory
 
 import nbformat
 import pytest
+from flaky import flaky  # type:ignore
 from traitlets.tests.utils import check_help_all_output
 
 from nbconvert.exporters import HTMLExporter
-from nbconvert.exporters.webpdf import PYPPETEER_INSTALLED
+from nbconvert.exporters.webpdf import PLAYWRIGHT_INSTALLED
 
 from ..postprocessors import PostProcessorBase
 from ..tests.utils import onlyif_cmds_exist
 from .base import TestsBase
 
 # -----------------------------------------------------------------------------
 # Classes and functions
@@ -144,16 +145,17 @@
                 "--log-level 0 --to pdf"
                 ' "notebook with spaces"'
                 " --PDFExporter.latex_count=1"
                 " --PDFExporter.verbose=True"
             )
             assert os.path.isfile("notebook with spaces.pdf")
 
+    @flaky
     @pytest.mark.network
-    @pytest.mark.skipif(not PYPPETEER_INSTALLED, reason="Pyppeeter not installed")
+    @pytest.mark.skipif(not PLAYWRIGHT_INSTALLED, reason="Playwright not installed")
     def test_webpdf_with_chromium(self):
         """
         Generate PDFs if chromium allowed to be downloaded?
         """
         with self.create_temp_cwd(["notebook2.ipynb"]):
             self.nbconvert('--to webpdf --allow-chromium-download "notebook2"')
             assert os.path.isfile("notebook2.pdf")
@@ -331,21 +333,21 @@
         Verify that the html has no prompts when given --no-prompt.
         """
         with self.create_temp_cwd(["notebook1.ipynb"]):
             self.nbconvert("notebook1.ipynb --log-level 0 --no-prompt --to html")
             assert os.path.isfile("notebook1.html")
             with open("notebook1.html", encoding="utf8") as f:
                 text = f.read()
-                assert "In&nbsp;[" not in text
+                assert "In\xa0[" not in text
                 assert "Out[6]" not in text
             self.nbconvert("notebook1.ipynb --log-level 0 --to html")
             assert os.path.isfile("notebook1.html")
             with open("notebook1.html", encoding="utf8") as f:
                 text2 = f.read()
-                assert "In&nbsp;[" in text2
+                assert "In\xa0[" in text2
                 assert "Out[6]" in text2
 
     def test_cell_tag_output(self):
         """
         Verify that the html has tags in cell attributes if they exist.
         """
         with self.create_temp_cwd(["notebook_tags.ipynb"]):
@@ -365,28 +367,28 @@
             '<span class="p">,</span>'
             '<span class="n">y</span>'
             '<span class="p">,</span>'
             '<span class="n">z</span> '
             '<span class="o">=</span> '
             '<span class="n">symbols</span>'
             '<span class="p">(</span>'
-            '<span class="s1">&#39;x y z&#39;</span>'
+            '<span class="s1">\'x y z\'</span>'
             '<span class="p">)</span>'
         )
         for no_input_flag in (False, True):
             with self.create_temp_cwd(["notebook1.ipynb"]):
                 command = "notebook1.ipynb --log-level 0 --to html"
                 if no_input_flag:
                     command += " --no-input"
                 self.nbconvert(command)
                 assert os.path.isfile("notebook1.html")
 
                 with open("notebook1.html", encoding="utf8") as f:
                     text = f.read()
-                    assert no_input_flag == ("In&nbsp;[" not in text)
+                    assert no_input_flag == ("In\xa0[" not in text)
                     assert no_input_flag == ("Out[6]" not in text)
                     assert no_input_flag == (input_content_html not in text)
 
     def test_allow_errors(self):
         """
         Verify that conversion is aborted with '--execute' if an error is
         encountered, but that conversion continues if '--allow-errors' is
@@ -576,15 +578,15 @@
             ["notebook5_embed_images.ipynb", "containerized_deployments.jpeg"]
         ):
             self.nbconvert("notebook5_embed_images --log-level 0 --to html")
             assert os.path.isfile("notebook5_embed_images.html")
             with open("notebook5_embed_images.html", encoding="utf8") as f:
                 text = f.read()
                 assert "./containerized_deployments.jpeg" in text
-                assert "src='./containerized_deployments.jpeg'" in text
+                assert 'src="./containerized_deployments.jpeg"' in text
                 assert text.count("data:image/jpeg;base64") == 0
 
     def test_embedding_images_htmlexporter(self):
         """Check that the HTMLExporter embeds images if needed"""
 
         with self.create_temp_cwd(
             ["notebook5_embed_images.ipynb", "containerized_deployments.jpeg"]
@@ -593,27 +595,14 @@
             assert os.path.isfile("notebook5_embed_images.html")
             with open("notebook5_embed_images.html", encoding="utf8") as f:
                 text = f.read()
                 assert "./containerized_deployments.jpeg" not in text
                 assert "src='./containerized_deployments.jpeg'" not in text
                 assert text.count("data:image/jpeg;base64") == 3
 
-    def test_embedded_svg_remains(self):
-        """Check that the HTMLExporter doesn't scrub SVG"""
-
-        with self.create_temp_cwd(["issue1849_svg.ipynb"]):
-            self.nbconvert("issue1849_svg --log-level 0 --to html")
-            assert os.path.isfile("issue1849_svg.html")
-            with open("issue1849_svg.html", encoding="utf8") as f:
-                text = f.read()
-                assert '<g id="line2d_2">' in text  # Must not be escaped
-                # TODO: these currently break...
-                # assert '<use xlink:href=\"#m361cdeea3f\"' in text  # Must not be escaped
-                assert "<!-- 1.6 -->" in text  # Must not be stripped
-
     def test_execute_widgets_from_nbconvert(self):
         """Check jupyter widgets render"""
         notebook_name = "Unexecuted_widget"
         with self.create_temp_cwd([f"{notebook_name}.ipynb"]):
             self.nbconvert(f"{notebook_name}.ipynb --execute --log-level 0 --to html")
             assert os.path.isfile(f"{notebook_name}.html")
             with open(f"{notebook_name}.html", encoding="utf8") as f:
```

### Comparing `nbconvert-7.6.0/nbconvert/tests/files/Unexecuted_widget.ipynb` & `nbconvert-7.7.0/nbconvert/tests/files/Unexecuted_widget.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb` & `nbconvert-7.7.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/files/Widget_List.ipynb` & `nbconvert-7.7.0/nbconvert/tests/files/Widget_List.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/files/containerized_deployments.jpeg` & `nbconvert-7.7.0/nbconvert/tests/files/containerized_deployments.jpeg`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/files/latex-linked-image.ipynb` & `nbconvert-7.7.0/nbconvert/tests/files/latex-linked-image.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/files/markdown_display_priority.ipynb` & `nbconvert-7.7.0/nbconvert/tests/files/markdown_display_priority.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/files/notebook1.ipynb` & `nbconvert-7.7.0/nbconvert/tests/files/notebook1.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/files/notebook2.ipynb` & `nbconvert-7.7.0/nbconvert/tests/files/notebook2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/files/notebook3_with_errors.ipynb` & `nbconvert-7.7.0/nbconvert/tests/files/notebook3_with_errors.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/files/notebook4_jpeg.ipynb` & `nbconvert-7.7.0/nbconvert/tests/files/notebook4_jpeg.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/files/notebook5_embed_images.ipynb` & `nbconvert-7.7.0/nbconvert/tests/files/notebook5_embed_images.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/files/notebook_tags.ipynb` & `nbconvert-7.7.0/nbconvert/tests/files/notebook_tags.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/tests/files/testimage.png` & `nbconvert-7.7.0/nbconvert/tests/files/testimage.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/utils/_contextlib_chdir.py` & `nbconvert-7.7.0/nbconvert/utils/_contextlib_chdir.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/utils/base.py` & `nbconvert-7.7.0/nbconvert/utils/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/utils/exceptions.py` & `nbconvert-7.7.0/nbconvert/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/utils/io.py` & `nbconvert-7.7.0/nbconvert/utils/io.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/utils/pandoc.py` & `nbconvert-7.7.0/nbconvert/utils/pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/utils/text.py` & `nbconvert-7.7.0/nbconvert/utils/text.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/utils/version.py` & `nbconvert-7.7.0/nbconvert/utils/version.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/utils/tests/test_io.py` & `nbconvert-7.7.0/nbconvert/utils/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/utils/tests/test_pandoc.py` & `nbconvert-7.7.0/nbconvert/utils/tests/test_pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/writers/base.py` & `nbconvert-7.7.0/nbconvert/writers/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/writers/debug.py` & `nbconvert-7.7.0/nbconvert/writers/debug.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/writers/files.py` & `nbconvert-7.7.0/nbconvert/writers/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
         # Copy referenced files to output directory
         if build_directory:
             for filename in self.files:
                 # Copy files that match search pattern
                 for matching_filename in glob.glob(filename):
                     # compute the relative path for the filename
-                    if relpath != "":  # noqa
+                    if relpath != "":
                         dest_filename = os.path.relpath(matching_filename, relpath)
                     else:
                         dest_filename = matching_filename
 
                     # Make sure folder exists.
                     dest = os.path.join(build_directory, dest_filename)
                     path = os.path.dirname(dest)
```

### Comparing `nbconvert-7.6.0/nbconvert/writers/stdout.py` & `nbconvert-7.7.0/nbconvert/writers/stdout.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/writers/tests/test_debug.py` & `nbconvert-7.7.0/nbconvert/writers/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/writers/tests/test_files.py` & `nbconvert-7.7.0/nbconvert/writers/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/nbconvert/writers/tests/test_stdout.py` & `nbconvert-7.7.0/nbconvert/writers/tests/test_stdout.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/asciidoc/index.asciidoc.j2` & `nbconvert-7.7.0/share/templates/asciidoc/index.asciidoc.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/base/display_priority.j2` & `nbconvert-7.7.0/share/templates/base/display_priority.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/base/jupyter_widgets.html.j2` & `nbconvert-7.7.0/share/templates/base/jupyter_widgets.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/base/mathjax.html.j2` & `nbconvert-7.7.0/share/templates/base/mathjax.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/base/null.j2` & `nbconvert-7.7.0/share/templates/base/null.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/classic/base.html.j2` & `nbconvert-7.7.0/share/templates/classic/base.html.j2`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 {%- endblock stream_stderr %}
 
 {% block data_svg scoped -%}
 <div class="output_svg output_subarea {{ extra_class }}">
 {%- if output.svg_filename %}
 <img src="{{ output.svg_filename | posix_path | escape_html }}">
 {%- else %}
-{{ output.data['image/svg+xml'].encode("utf-8") | clean_html }}
+<img src="data:image/svg+xml;base64,{{ output.data['image/svg+xml'] | text_base64 | escape_html }}">
 {%- endif %}
 </div>
 {%- endblock data_svg %}
 
 {% block data_html scoped -%}
 <div class="output_html rendered_html output_subarea {{ extra_class }}">
 {%- if resources.should_sanitize_html %}
@@ -265,24 +265,24 @@
 {% set datatype_list = output.data | filter_data_type %}
 {% set datatype = datatype_list[0]%}
 <div id="{{ div_id }}" class="output_subarea output_widget_view {{ extra_class }}">
 <script type="text/javascript">
 var element = $('#{{ div_id }}');
 </script>
 <script type="{{ datatype }}">
-{{ output.data[datatype] | json_dumps | escape_html_keep_quotes }}
+{{ output.data[datatype] | json_dumps | escape_html_script }}
 </script>
 </div>
 {%- endif %}
 {%- endblock data_widget_view -%}
 
 {%- block footer %}
 {%- if not resources.should_sanitize_html %}
 {% set mimetype = 'application/vnd.jupyter.widget-state+json'%}
 {% if mimetype in nb.metadata.get("widgets",{})%}
 <script type="{{ mimetype }}">
-{{ nb.metadata.widgets[mimetype] | json_dumps | escape_html_keep_quotes }}
+{{ nb.metadata.widgets[mimetype] | json_dumps | escape_html_script }}
 </script>
 {% endif %}
 {%- endif %}
 {{ super() }}
 {%- endblock footer-%}
```

### Comparing `nbconvert-7.6.0/share/templates/classic/index.html.j2` & `nbconvert-7.7.0/share/templates/classic/index.html.j2`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {%- extends 'base.html.j2' -%}
 {% from 'mathjax.html.j2' import mathjax %}
 {% from 'jupyter_widgets.html.j2' import jupyter_widgets %}
 
 {%- block header -%}
 <!DOCTYPE html>
-<html>
+<html lang="{{ resources.language_code }}">
 <head>
 {%- block html_head -%}
 <meta charset="utf-8" />
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 {% set nb_title = nb.metadata.get('title', resources['metadata']['name']) | escape_html_keep_quotes %}
 <title>{{nb_title}}</title>
 
@@ -88,21 +88,23 @@
 
 {%- endblock html_head -%}
 </head>
 {%- endblock header -%}
 
 {% block body_header %}
 <body>
-  <div tabindex="-1" id="notebook" class="border-box-sizing">
-    <div class="container" id="notebook-container">
+  <main>
+    <div tabindex="-1" id="notebook" class="border-box-sizing">
+      <div class="container" id="notebook-container">
 {% endblock body_header %}
 
 {% block body_footer %}
+      </div>
     </div>
-  </div>
+  </main>
 </body>
 {% endblock body_footer %}
 
 {% block footer %}
 {% block footer_js %}
 {% endblock footer_js %}
 {{ super() }}
```

### Comparing `nbconvert-7.6.0/share/templates/classic/static/style.css` & `nbconvert-7.7.0/share/templates/classic/static/style.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/lab/base.html.j2` & `nbconvert-7.7.0/share/templates/lab/base.html.j2`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {{ super() }}
 </div>
 </div>
 {% endblock input_group %}
 
 {% block input %}
 <div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
-     <div class="CodeMirror cm-s-jupyter">
+     <div class="cm-editor cm-s-jupyter">
 {{ cell.source | highlight_code(metadata=cell.metadata) | clean_html }}
      </div>
 </div>
 {%- endblock input %}
 
 {% block output_group %}
 <div class="jp-Cell-outputWrapper">
@@ -160,15 +160,15 @@
 {%- endblock stream_stdin %}
 
 {% block data_svg scoped -%}
 <div class="jp-RenderedSVG jp-OutputArea-output {{ extra_class }}" data-mime-type="image/svg+xml">
 {%- if output.svg_filename %}
 <img src="{{ output.svg_filename | posix_path | escape_html }}">
 {%- else %}
-{{ output.data['image/svg+xml'].encode("utf-8") | clean_html }}
+<img src="data:image/svg+xml;base64,{{ output.data['image/svg+xml'] | text_base64 | escape_html }}">
 {%- endif %}
 </div>
 {%- endblock data_svg %}
 
 {% block data_html scoped -%}
 <div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output {{ extra_class }}" data-mime-type="text/html">
 {%- if resources.should_sanitize_html %}
@@ -299,21 +299,21 @@
 {% set datatype_list = output.data | filter_data_type %}
 {% set datatype = datatype_list[0]%}
 <div id="{{ div_id }}" class="jupyter-widgets jp-OutputArea-output {{ extra_class }}">
 <script type="text/javascript">
 var element = document.getElementById('{{ div_id }}');
 </script>
 <script type="{{ datatype }}">
-{{ output.data[datatype] | json_dumps | escape_html_keep_quotes }}
+{{ output.data[datatype] | json_dumps | escape_html_script }}
 </script>
 </div>
 {%- endblock data_widget_view -%}
 
 {%- block footer %}
 {% set mimetype = 'application/vnd.jupyter.widget-state+json'%}
 {% if mimetype in nb.metadata.get("widgets",{})%}
 <script type="{{ mimetype }}">
-{{ nb.metadata.widgets[mimetype] | json_dumps | escape_html_keep_quotes }}
+{{ nb.metadata.widgets[mimetype] | json_dumps | escape_html_script }}
 </script>
 {% endif %}
 {{ super() }}
 {%- endblock footer-%}
```

### Comparing `nbconvert-7.6.0/share/templates/lab/index.html.j2` & `nbconvert-7.7.0/share/templates/lab/index.html.j2`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {%- extends 'base.html.j2' -%}
 {% from 'mathjax.html.j2' import mathjax %}
 {% from 'mermaidjs.html.j2' import mermaid_js %}
 {% from 'jupyter_widgets.html.j2' import jupyter_widgets %}
 
 {%- block header -%}
 <!DOCTYPE html>
-<html>
+<html lang="{{ resources.language_code }}">
 <head>
 {%- block html_head -%}
 <meta charset="utf-8" />
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 {% set nb_title = nb.metadata.get('title', resources['metadata']['name']) | escape_html_keep_quotes %}
 <title>{{nb_title}}</title>
 
@@ -59,16 +59,16 @@
   overflow: hidden;
 }
 
 .jp-InputArea-editor {
   overflow: hidden;
 }
 
-.CodeMirror.cm-s-jupyter .highlight pre {
-/* weird, but --jp-code-padding defined to be 5px but 4px horizontal padding is hardcoded for pre.CodeMirror-line */
+.cm-editor.cm-s-jupyter .highlight pre {
+/* weird, but --jp-code-padding defined to be 5px but 4px horizontal padding is hardcoded for pre.cm-line */
   padding: var(--jp-code-padding) 4px;
   margin: 0;
 
   font-family: inherit;
   font-size: inherit;
   line-height: inherit;
   color: inherit;
@@ -81,70 +81,28 @@
 }
 
 .jp-RenderedText pre {
   color: var(--jp-content-font-color1);
   font-size: var(--jp-code-font-size);
 }
 
-/* Using table instead of flexbox so that we can use break-inside property */
-/* CSS rules under this comment should not be required anymore after we move to the JupyterLab 4.0 CSS */
-
-
-.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
-  min-width: calc(
-    var(--jp-cell-prompt-width) - var(--jp-private-cell-scrolling-output-offset)
-  );
-}
-
-.jp-OutputArea-child {
-  display: table;
-  width: 100%;
-}
-
-.jp-OutputPrompt {
-  display: table-cell;
-  vertical-align: top;
-  min-width: var(--jp-cell-prompt-width);
-}
-
-body[data-format='mobile'] .jp-OutputPrompt {
-  display: table-row;
-}
-
-.jp-OutputArea-output {
-  display: table-cell;
-  width: 100%;
-}
-
-body[data-format='mobile'] .jp-OutputArea-child .jp-OutputArea-output {
-  display: table-row;
-}
-
-.jp-OutputArea-output.jp-OutputArea-executeResult {
-  width: 100%;
-}
-
 /* Hiding the collapser by default */
 .jp-Collapser {
   display: none;
 }
 
 @page {
     margin: 0.5in; /* Margin for each printed piece of paper */
 }
 
 @media print {
   .jp-Cell-inputWrapper,
   .jp-Cell-outputWrapper {
     display: block;
   }
-
-  .jp-OutputArea-child {
-    break-inside: avoid-page;
-  }
 }
 </style>
 
 {% endblock notebook_css %}
 
 {%- block html_head_js_mathjax -%}
 {{ mathjax(resources.mathjax_url) }}
@@ -163,17 +121,19 @@
 
 {%- block body_header -%}
 {% if resources.theme == 'dark' %}
 <body class="jp-Notebook" data-jp-theme-light="false" data-jp-theme-name="JupyterLab Dark">
 {% else %}
 <body class="jp-Notebook" data-jp-theme-light="true" data-jp-theme-name="JupyterLab Light">
 {% endif %}
+<main>
 {%- endblock body_header -%}
 
 {% block body_footer %}
+</main>
 </body>
 {% endblock body_footer %}
 
 {% block footer %}
 {% block footer_js %}
 {% endblock footer_js %}
 {{ super() }}
```

#### html2text {}

```diff
@@ -21,11 +21,11 @@
 (resources.mathjax_url) }} {%- endblock html_head_js_mathjax -%} {%- block
 html_head_js_mermaidjs -%} {{ mermaid_js(resources.mermaid_js_url) }} {%-
 endblock html_head_js_mermaidjs -%} {%- block html_head_css -%} {%- endblock
 html_head_css -%} {%- endblock html_head -%}
 {%- endblock header -%} {%- block body_header -%} {% if resources.theme ==
 'dark' %}
 {% else %}
-{% endif %} {%- endblock body_header -%} {% block body_footer %}
+{% endif %}  {%- endblock body_header -%} {% block body_footer %}
 {% endblock body_footer %} {% block footer %} {% block footer_js %} {% endblock
 footer_js %} {{ super() }}
 {% endblock footer %}
```

### Comparing `nbconvert-7.6.0/share/templates/lab/mermaidjs.html.j2` & `nbconvert-7.7.0/share/templates/lab/mermaidjs.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/lab/static/theme-dark.css` & `nbconvert-7.7.0/share/templates/lab/static/theme-dark.css`

 * *Files 4% similar despite different names*

```diff
@@ -51,41 +51,41 @@
   --jp-shadow-ambient-color: rgba(
     var(--jp-shadow-base-lightness),
     var(--jp-shadow-base-lightness),
     var(--jp-shadow-base-lightness),
     0.12
   );
   --jp-elevation-z0: none;
-  --jp-elevation-z1: 0px 2px 1px -1px var(--jp-shadow-umbra-color),
-    0px 1px 1px 0px var(--jp-shadow-penumbra-color),
-    0px 1px 3px 0px var(--jp-shadow-ambient-color);
-  --jp-elevation-z2: 0px 3px 1px -2px var(--jp-shadow-umbra-color),
-    0px 2px 2px 0px var(--jp-shadow-penumbra-color),
-    0px 1px 5px 0px var(--jp-shadow-ambient-color);
-  --jp-elevation-z4: 0px 2px 4px -1px var(--jp-shadow-umbra-color),
-    0px 4px 5px 0px var(--jp-shadow-penumbra-color),
-    0px 1px 10px 0px var(--jp-shadow-ambient-color);
-  --jp-elevation-z6: 0px 3px 5px -1px var(--jp-shadow-umbra-color),
-    0px 6px 10px 0px var(--jp-shadow-penumbra-color),
-    0px 1px 18px 0px var(--jp-shadow-ambient-color);
-  --jp-elevation-z8: 0px 5px 5px -3px var(--jp-shadow-umbra-color),
-    0px 8px 10px 1px var(--jp-shadow-penumbra-color),
-    0px 3px 14px 2px var(--jp-shadow-ambient-color);
-  --jp-elevation-z12: 0px 7px 8px -4px var(--jp-shadow-umbra-color),
-    0px 12px 17px 2px var(--jp-shadow-penumbra-color),
-    0px 5px 22px 4px var(--jp-shadow-ambient-color);
-  --jp-elevation-z16: 0px 8px 10px -5px var(--jp-shadow-umbra-color),
-    0px 16px 24px 2px var(--jp-shadow-penumbra-color),
-    0px 6px 30px 5px var(--jp-shadow-ambient-color);
-  --jp-elevation-z20: 0px 10px 13px -6px var(--jp-shadow-umbra-color),
-    0px 20px 31px 3px var(--jp-shadow-penumbra-color),
-    0px 8px 38px 7px var(--jp-shadow-ambient-color);
-  --jp-elevation-z24: 0px 11px 15px -7px var(--jp-shadow-umbra-color),
-    0px 24px 38px 3px var(--jp-shadow-penumbra-color),
-    0px 9px 46px 8px var(--jp-shadow-ambient-color);
+  --jp-elevation-z1: 0 2px 1px -1px var(--jp-shadow-umbra-color),
+    0 1px 1px 0 var(--jp-shadow-penumbra-color),
+    0 1px 3px 0 var(--jp-shadow-ambient-color);
+  --jp-elevation-z2: 0 3px 1px -2px var(--jp-shadow-umbra-color),
+    0 2px 2px 0 var(--jp-shadow-penumbra-color),
+    0 1px 5px 0 var(--jp-shadow-ambient-color);
+  --jp-elevation-z4: 0 2px 4px -1px var(--jp-shadow-umbra-color),
+    0 4px 5px 0 var(--jp-shadow-penumbra-color),
+    0 1px 10px 0 var(--jp-shadow-ambient-color);
+  --jp-elevation-z6: 0 3px 5px -1px var(--jp-shadow-umbra-color),
+    0 6px 10px 0 var(--jp-shadow-penumbra-color),
+    0 1px 18px 0 var(--jp-shadow-ambient-color);
+  --jp-elevation-z8: 0 5px 5px -3px var(--jp-shadow-umbra-color),
+    0 8px 10px 1px var(--jp-shadow-penumbra-color),
+    0 3px 14px 2px var(--jp-shadow-ambient-color);
+  --jp-elevation-z12: 0 7px 8px -4px var(--jp-shadow-umbra-color),
+    0 12px 17px 2px var(--jp-shadow-penumbra-color),
+    0 5px 22px 4px var(--jp-shadow-ambient-color);
+  --jp-elevation-z16: 0 8px 10px -5px var(--jp-shadow-umbra-color),
+    0 16px 24px 2px var(--jp-shadow-penumbra-color),
+    0 6px 30px 5px var(--jp-shadow-ambient-color);
+  --jp-elevation-z20: 0 10px 13px -6px var(--jp-shadow-umbra-color),
+    0 20px 31px 3px var(--jp-shadow-penumbra-color),
+    0 8px 38px 7px var(--jp-shadow-ambient-color);
+  --jp-elevation-z24: 0 11px 15px -7px var(--jp-shadow-umbra-color),
+    0 24px 38px 3px var(--jp-shadow-penumbra-color),
+    0 9px 46px 8px var(--jp-shadow-ambient-color);
 
   /* Borders
    *
    * The following variables, specify the visual styling of borders in JupyterLab.
    */
 
   --jp-border-width: 1px;
@@ -107,17 +107,17 @@
    */
 
   --jp-ui-font-scale-factor: 1.2;
   --jp-ui-font-size0: 0.83333em;
   --jp-ui-font-size1: 13px; /* Base font size */
   --jp-ui-font-size2: 1.2em;
   --jp-ui-font-size3: 1.44em;
-
-  --jp-ui-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica,
-    Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
+  --jp-ui-font-family: system-ui, -apple-system, blinkmacsystemfont, 'Segoe UI',
+    helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
+    'Segoe UI Symbol';
 
   /*
    * Use these font colors against the corresponding main layout colors.
    * In a light theme, these go from dark to light.
    */
 
   /* Defaults use Material Design specification */
@@ -152,42 +152,39 @@
   --jp-content-font-size2: 1.2em;
   --jp-content-font-size3: 1.44em;
   --jp-content-font-size4: 1.728em;
   --jp-content-font-size5: 2.0736em;
 
   /* This gives a magnification of about 125% in presentation mode over normal. */
   --jp-content-presentation-font-size1: 17px;
-
   --jp-content-heading-line-height: 1;
   --jp-content-heading-margin-top: 1.2em;
   --jp-content-heading-margin-bottom: 0.8em;
   --jp-content-heading-font-weight: 500;
 
   /* Defaults use Material Design specification */
   --jp-content-font-color0: rgba(255, 255, 255, 1);
   --jp-content-font-color1: rgba(255, 255, 255, 1);
   --jp-content-font-color2: rgba(255, 255, 255, 0.7);
   --jp-content-font-color3: rgba(255, 255, 255, 0.5);
-
   --jp-content-link-color: var(--md-blue-300);
-
-  --jp-content-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI',
-    Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
-    'Segoe UI Symbol';
+  --jp-content-font-family: system-ui, -apple-system, blinkmacsystemfont,
+    'Segoe UI', helvetica, arial, sans-serif, 'Apple Color Emoji',
+    'Segoe UI Emoji', 'Segoe UI Symbol';
 
   /*
    * Code Fonts
    *
    * Code font variables are used for typography of code and other monospaces content.
    */
 
   --jp-code-font-size: 13px;
   --jp-code-line-height: 1.3077; /* 17px for 13px base */
   --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
-  --jp-code-font-family-default: Menlo, Consolas, 'DejaVu Sans Mono', monospace;
+  --jp-code-font-family-default: menlo, consolas, 'DejaVu Sans Mono', monospace;
   --jp-code-font-family: var(--jp-code-font-family-default);
 
   /* This gives a magnification of about 125% in presentation mode over normal. */
   --jp-code-presentation-font-size: 16px;
 
   /* may need to tweak cursor width if you change font size */
   --jp-code-cursor-width0: 1.4px;
@@ -196,15 +193,15 @@
 
   /* Layout
    *
    * The following are the main layout colors use in JupyterLab. In a light
    * theme these would go from light to dark.
    */
 
-  --jp-layout-color0: #111111;
+  --jp-layout-color0: #111;
   --jp-layout-color1: var(--md-grey-900);
   --jp-layout-color2: var(--md-grey-800);
   --jp-layout-color3: var(--md-grey-700);
   --jp-layout-color4: var(--md-grey-600);
 
   /* Inverse Layout
    *
@@ -221,66 +218,60 @@
   /* Brand/accent */
 
   --jp-brand-color0: var(--md-blue-700);
   --jp-brand-color1: var(--md-blue-500);
   --jp-brand-color2: var(--md-blue-300);
   --jp-brand-color3: var(--md-blue-100);
   --jp-brand-color4: var(--md-blue-50);
-
   --jp-accent-color0: var(--md-green-700);
   --jp-accent-color1: var(--md-green-500);
   --jp-accent-color2: var(--md-green-300);
   --jp-accent-color3: var(--md-green-100);
 
   /* State colors (warn, error, success, info) */
 
   --jp-warn-color0: var(--md-orange-700);
   --jp-warn-color1: var(--md-orange-500);
   --jp-warn-color2: var(--md-orange-300);
   --jp-warn-color3: var(--md-orange-100);
-
   --jp-error-color0: var(--md-red-700);
   --jp-error-color1: var(--md-red-500);
   --jp-error-color2: var(--md-red-300);
   --jp-error-color3: var(--md-red-100);
-
   --jp-success-color0: var(--md-green-700);
   --jp-success-color1: var(--md-green-500);
   --jp-success-color2: var(--md-green-300);
   --jp-success-color3: var(--md-green-100);
-
   --jp-info-color0: var(--md-cyan-700);
   --jp-info-color1: var(--md-cyan-500);
   --jp-info-color2: var(--md-cyan-300);
   --jp-info-color3: var(--md-cyan-100);
 
   /* Cell specific styles */
 
   --jp-cell-padding: 5px;
-
   --jp-cell-collapser-width: 8px;
   --jp-cell-collapser-min-height: 20px;
   --jp-cell-collapser-not-active-hover-opacity: 0.6;
-
   --jp-cell-editor-background: var(--jp-layout-color1);
   --jp-cell-editor-border-color: var(--md-grey-700);
   --jp-cell-editor-box-shadow: inset 0 0 2px var(--md-blue-300);
   --jp-cell-editor-active-background: var(--jp-layout-color0);
   --jp-cell-editor-active-border-color: var(--jp-brand-color1);
-
   --jp-cell-prompt-width: 64px;
   --jp-cell-prompt-font-family: var(--jp-code-font-family-default);
-  --jp-cell-prompt-letter-spacing: 0px;
+  --jp-cell-prompt-letter-spacing: 0;
   --jp-cell-prompt-opacity: 1;
   --jp-cell-prompt-not-active-opacity: 1;
   --jp-cell-prompt-not-active-font-color: var(--md-grey-300);
 
   /* A custom blend of MD grey and blue 600
    * See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex */
   --jp-cell-inprompt-font-color: #307fc1;
+
   /* A custom blend of MD grey and orange 600
    * https://meyerweb.com/eric/tools/color-blend/#546E7A:F4511E:5:hex */
   --jp-cell-outprompt-font-color: #bf5b3d;
 
   /* Notebook specific styles */
 
   --jp-notebook-padding: 10px;
@@ -313,16 +304,16 @@
   --jp-console-padding: 10px;
 
   /* Toolbar specific styles */
 
   --jp-toolbar-border-color: var(--jp-border-color2);
   --jp-toolbar-micro-height: 8px;
   --jp-toolbar-background: var(--jp-layout-color1);
-  --jp-toolbar-box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.8);
-  --jp-toolbar-header-margin: 4px 4px 0px 4px;
+  --jp-toolbar-box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.8);
+  --jp-toolbar-header-margin: 4px 4px 0 4px;
   --jp-toolbar-active-background: var(--jp-layout-color0);
 
   /* Statusbar specific styles */
 
   --jp-statusbar-height: 24px;
 
   /* Input field styles */
@@ -344,23 +335,23 @@
   /* Code mirror specific styles */
 
   --jp-mirror-editor-keyword-color: var(--md-green-500);
   --jp-mirror-editor-atom-color: var(--md-blue-300);
   --jp-mirror-editor-number-color: var(--md-green-400);
   --jp-mirror-editor-def-color: var(--md-blue-600);
   --jp-mirror-editor-variable-color: var(--md-grey-300);
-  --jp-mirror-editor-variable-2-color: var(--md-blue-400);
+  --jp-mirror-editor-variable-2-color: var(--md-blue-500);
   --jp-mirror-editor-variable-3-color: var(--md-green-600);
   --jp-mirror-editor-punctuation-color: var(--md-blue-400);
   --jp-mirror-editor-property-color: var(--md-blue-400);
-  --jp-mirror-editor-operator-color: #aa22ff;
+  --jp-mirror-editor-operator-color: #a2f;
   --jp-mirror-editor-comment-color: #408080;
   --jp-mirror-editor-string-color: #ff7070;
   --jp-mirror-editor-string-2-color: var(--md-purple-300);
-  --jp-mirror-editor-meta-color: #aa22ff;
+  --jp-mirror-editor-meta-color: #a2f;
   --jp-mirror-editor-qualifier-color: #555;
   --jp-mirror-editor-builtin-color: var(--md-green-600);
   --jp-mirror-editor-bracket-color: #997;
   --jp-mirror-editor-tag-color: var(--md-green-700);
   --jp-mirror-editor-attribute-color: var(--md-blue-700);
   --jp-mirror-editor-header-color: var(--md-blue-500);
   --jp-mirror-editor-quote-color: var(--md-green-300);
@@ -404,28 +395,38 @@
 
   /* scrollbar related styles. Supports every browser except Edge. */
 
   /* colors based on JetBrain's Darcula theme */
 
   --jp-scrollbar-background-color: #3f4244;
   --jp-scrollbar-thumb-color: 88, 96, 97; /* need to specify thumb color as an RGB triplet */
-
   --jp-scrollbar-endpad: 3px; /* the minimum gap between the thumb and the ends of a scrollbar */
 
   /* hacks for setting the thumb shape. These do nothing in Firefox */
 
   --jp-scrollbar-thumb-margin: 3.5px; /* the space in between the sides of the thumb and the track */
   --jp-scrollbar-thumb-radius: 9px; /* set to a large-ish value for rounded endcaps on the thumb */
 
   /* Icon colors that work well with light or dark backgrounds */
   --jp-icon-contrast-color0: var(--md-purple-600);
   --jp-icon-contrast-color1: var(--md-green-600);
   --jp-icon-contrast-color2: var(--md-pink-600);
   --jp-icon-contrast-color3: var(--md-blue-600);
 
+  /* Button colors */
+  --jp-accept-color-normal: var(--md-blue-700);
+  --jp-accept-color-hover: var(--md-blue-800);
+  --jp-accept-color-active: var(--md-blue-900);
+  --jp-warn-color-normal: var(--md-red-700);
+  --jp-warn-color-hover: var(--md-red-800);
+  --jp-warn-color-active: var(--md-red-900);
+  --jp-reject-color-normal: var(--md-grey-600);
+  --jp-reject-color-hover: var(--md-grey-700);
+  --jp-reject-color-active: var(--md-grey-800);
+
   /* File or activity icons and switch semantic variables */
   --jp-jupyter-icon-color: #f37626;
   --jp-notebook-icon-color: #f37626;
   --jp-json-icon-color: var(--md-orange-500);
   --jp-console-icon-background-color: var(--md-blue-500);
   --jp-console-icon-color: white;
   --jp-terminal-icon-background-color: var(--md-grey-200);
```

### Comparing `nbconvert-7.6.0/share/templates/lab/static/theme-light.css` & `nbconvert-7.7.0/share/templates/lab/static/theme-light.css`

 * *Files 4% similar despite different names*

```diff
@@ -49,41 +49,41 @@
   --jp-shadow-ambient-color: rgba(
     var(--jp-shadow-base-lightness),
     var(--jp-shadow-base-lightness),
     var(--jp-shadow-base-lightness),
     0.12
   );
   --jp-elevation-z0: none;
-  --jp-elevation-z1: 0px 2px 1px -1px var(--jp-shadow-umbra-color),
-    0px 1px 1px 0px var(--jp-shadow-penumbra-color),
-    0px 1px 3px 0px var(--jp-shadow-ambient-color);
-  --jp-elevation-z2: 0px 3px 1px -2px var(--jp-shadow-umbra-color),
-    0px 2px 2px 0px var(--jp-shadow-penumbra-color),
-    0px 1px 5px 0px var(--jp-shadow-ambient-color);
-  --jp-elevation-z4: 0px 2px 4px -1px var(--jp-shadow-umbra-color),
-    0px 4px 5px 0px var(--jp-shadow-penumbra-color),
-    0px 1px 10px 0px var(--jp-shadow-ambient-color);
-  --jp-elevation-z6: 0px 3px 5px -1px var(--jp-shadow-umbra-color),
-    0px 6px 10px 0px var(--jp-shadow-penumbra-color),
-    0px 1px 18px 0px var(--jp-shadow-ambient-color);
-  --jp-elevation-z8: 0px 5px 5px -3px var(--jp-shadow-umbra-color),
-    0px 8px 10px 1px var(--jp-shadow-penumbra-color),
-    0px 3px 14px 2px var(--jp-shadow-ambient-color);
-  --jp-elevation-z12: 0px 7px 8px -4px var(--jp-shadow-umbra-color),
-    0px 12px 17px 2px var(--jp-shadow-penumbra-color),
-    0px 5px 22px 4px var(--jp-shadow-ambient-color);
-  --jp-elevation-z16: 0px 8px 10px -5px var(--jp-shadow-umbra-color),
-    0px 16px 24px 2px var(--jp-shadow-penumbra-color),
-    0px 6px 30px 5px var(--jp-shadow-ambient-color);
-  --jp-elevation-z20: 0px 10px 13px -6px var(--jp-shadow-umbra-color),
-    0px 20px 31px 3px var(--jp-shadow-penumbra-color),
-    0px 8px 38px 7px var(--jp-shadow-ambient-color);
-  --jp-elevation-z24: 0px 11px 15px -7px var(--jp-shadow-umbra-color),
-    0px 24px 38px 3px var(--jp-shadow-penumbra-color),
-    0px 9px 46px 8px var(--jp-shadow-ambient-color);
+  --jp-elevation-z1: 0 2px 1px -1px var(--jp-shadow-umbra-color),
+    0 1px 1px 0 var(--jp-shadow-penumbra-color),
+    0 1px 3px 0 var(--jp-shadow-ambient-color);
+  --jp-elevation-z2: 0 3px 1px -2px var(--jp-shadow-umbra-color),
+    0 2px 2px 0 var(--jp-shadow-penumbra-color),
+    0 1px 5px 0 var(--jp-shadow-ambient-color);
+  --jp-elevation-z4: 0 2px 4px -1px var(--jp-shadow-umbra-color),
+    0 4px 5px 0 var(--jp-shadow-penumbra-color),
+    0 1px 10px 0 var(--jp-shadow-ambient-color);
+  --jp-elevation-z6: 0 3px 5px -1px var(--jp-shadow-umbra-color),
+    0 6px 10px 0 var(--jp-shadow-penumbra-color),
+    0 1px 18px 0 var(--jp-shadow-ambient-color);
+  --jp-elevation-z8: 0 5px 5px -3px var(--jp-shadow-umbra-color),
+    0 8px 10px 1px var(--jp-shadow-penumbra-color),
+    0 3px 14px 2px var(--jp-shadow-ambient-color);
+  --jp-elevation-z12: 0 7px 8px -4px var(--jp-shadow-umbra-color),
+    0 12px 17px 2px var(--jp-shadow-penumbra-color),
+    0 5px 22px 4px var(--jp-shadow-ambient-color);
+  --jp-elevation-z16: 0 8px 10px -5px var(--jp-shadow-umbra-color),
+    0 16px 24px 2px var(--jp-shadow-penumbra-color),
+    0 6px 30px 5px var(--jp-shadow-ambient-color);
+  --jp-elevation-z20: 0 10px 13px -6px var(--jp-shadow-umbra-color),
+    0 20px 31px 3px var(--jp-shadow-penumbra-color),
+    0 8px 38px 7px var(--jp-shadow-ambient-color);
+  --jp-elevation-z24: 0 11px 15px -7px var(--jp-shadow-umbra-color),
+    0 24px 38px 3px var(--jp-shadow-penumbra-color),
+    0 9px 46px 8px var(--jp-shadow-ambient-color);
 
   /* Borders
    *
    * The following variables, specify the visual styling of borders in JupyterLab.
    */
 
   --jp-border-width: 1px;
@@ -105,17 +105,17 @@
    */
 
   --jp-ui-font-scale-factor: 1.2;
   --jp-ui-font-size0: 0.83333em;
   --jp-ui-font-size1: 13px; /* Base font size */
   --jp-ui-font-size2: 1.2em;
   --jp-ui-font-size3: 1.44em;
-
-  --jp-ui-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica,
-    Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';
+  --jp-ui-font-family: system-ui, -apple-system, blinkmacsystemfont, 'Segoe UI',
+    helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
+    'Segoe UI Symbol';
 
   /*
    * Use these font colors against the corresponding main layout colors.
    * In a light theme, these go from dark to light.
    */
 
   /* Defaults use Material Design specification */
@@ -150,42 +150,39 @@
   --jp-content-font-size2: 1.2em;
   --jp-content-font-size3: 1.44em;
   --jp-content-font-size4: 1.728em;
   --jp-content-font-size5: 2.0736em;
 
   /* This gives a magnification of about 125% in presentation mode over normal. */
   --jp-content-presentation-font-size1: 17px;
-
   --jp-content-heading-line-height: 1;
   --jp-content-heading-margin-top: 1.2em;
   --jp-content-heading-margin-bottom: 0.8em;
   --jp-content-heading-font-weight: 500;
 
   /* Defaults use Material Design specification */
   --jp-content-font-color0: rgba(0, 0, 0, 1);
   --jp-content-font-color1: rgba(0, 0, 0, 0.87);
   --jp-content-font-color2: rgba(0, 0, 0, 0.54);
   --jp-content-font-color3: rgba(0, 0, 0, 0.38);
-
-  --jp-content-link-color: var(--md-blue-700);
-
-  --jp-content-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI',
-    Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
-    'Segoe UI Symbol';
+  --jp-content-link-color: var(--md-blue-900);
+  --jp-content-font-family: system-ui, -apple-system, blinkmacsystemfont,
+    'Segoe UI', helvetica, arial, sans-serif, 'Apple Color Emoji',
+    'Segoe UI Emoji', 'Segoe UI Symbol';
 
   /*
    * Code Fonts
    *
    * Code font variables are used for typography of code and other monospaces content.
    */
 
   --jp-code-font-size: 13px;
   --jp-code-line-height: 1.3077; /* 17px for 13px base */
   --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
-  --jp-code-font-family-default: Menlo, Consolas, 'DejaVu Sans Mono', monospace;
+  --jp-code-font-family-default: menlo, consolas, 'DejaVu Sans Mono', monospace;
   --jp-code-font-family: var(--jp-code-font-family-default);
 
   /* This gives a magnification of about 125% in presentation mode over normal. */
   --jp-code-presentation-font-size: 16px;
 
   /* may need to tweak cursor width if you change font size */
   --jp-code-cursor-width0: 1.4px;
@@ -206,78 +203,73 @@
 
   /* Inverse Layout
    *
    * The following are the inverse layout colors use in JupyterLab. In a light
    * theme these would go from dark to light.
    */
 
-  --jp-inverse-layout-color0: #111111;
+  --jp-inverse-layout-color0: #111;
   --jp-inverse-layout-color1: var(--md-grey-900);
   --jp-inverse-layout-color2: var(--md-grey-800);
   --jp-inverse-layout-color3: var(--md-grey-700);
   --jp-inverse-layout-color4: var(--md-grey-600);
 
   /* Brand/accent */
 
   --jp-brand-color0: var(--md-blue-900);
   --jp-brand-color1: var(--md-blue-700);
   --jp-brand-color2: var(--md-blue-300);
   --jp-brand-color3: var(--md-blue-100);
   --jp-brand-color4: var(--md-blue-50);
-
   --jp-accent-color0: var(--md-green-900);
   --jp-accent-color1: var(--md-green-700);
   --jp-accent-color2: var(--md-green-300);
   --jp-accent-color3: var(--md-green-100);
 
   /* State colors (warn, error, success, info) */
 
   --jp-warn-color0: var(--md-orange-900);
   --jp-warn-color1: var(--md-orange-700);
   --jp-warn-color2: var(--md-orange-300);
   --jp-warn-color3: var(--md-orange-100);
-
   --jp-error-color0: var(--md-red-900);
   --jp-error-color1: var(--md-red-700);
   --jp-error-color2: var(--md-red-300);
   --jp-error-color3: var(--md-red-100);
-
   --jp-success-color0: var(--md-green-900);
   --jp-success-color1: var(--md-green-700);
   --jp-success-color2: var(--md-green-300);
   --jp-success-color3: var(--md-green-100);
-
   --jp-info-color0: var(--md-cyan-900);
   --jp-info-color1: var(--md-cyan-700);
   --jp-info-color2: var(--md-cyan-300);
   --jp-info-color3: var(--md-cyan-100);
 
   /* Cell specific styles */
 
   --jp-cell-padding: 5px;
-
   --jp-cell-collapser-width: 8px;
   --jp-cell-collapser-min-height: 20px;
   --jp-cell-collapser-not-active-hover-opacity: 0.6;
-
   --jp-cell-editor-background: var(--md-grey-100);
   --jp-cell-editor-border-color: var(--md-grey-300);
   --jp-cell-editor-box-shadow: inset 0 0 2px var(--md-blue-300);
   --jp-cell-editor-active-background: var(--jp-layout-color0);
   --jp-cell-editor-active-border-color: var(--jp-brand-color1);
-
   --jp-cell-prompt-width: 64px;
   --jp-cell-prompt-font-family: var(--jp-code-font-family-default);
-  --jp-cell-prompt-letter-spacing: 0px;
+  --jp-cell-prompt-letter-spacing: 0;
   --jp-cell-prompt-opacity: 1;
   --jp-cell-prompt-not-active-opacity: 0.5;
   --jp-cell-prompt-not-active-font-color: var(--md-grey-700);
+
   /* A custom blend of MD grey and blue 600
    * See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex */
   --jp-cell-inprompt-font-color: #307fc1;
+
   /* A custom blend of MD grey and orange 600
    * https://meyerweb.com/eric/tools/color-blend/#546E7A:F4511E:5:hex */
   --jp-cell-outprompt-font-color: #bf5b3d;
 
   /* Notebook specific styles */
 
   --jp-notebook-padding: 10px;
@@ -310,16 +302,16 @@
   --jp-console-padding: 10px;
 
   /* Toolbar specific styles */
 
   --jp-toolbar-border-color: var(--jp-border-color1);
   --jp-toolbar-micro-height: 8px;
   --jp-toolbar-background: var(--jp-layout-color1);
-  --jp-toolbar-box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.24);
-  --jp-toolbar-header-margin: 4px 4px 0px 4px;
+  --jp-toolbar-box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.24);
+  --jp-toolbar-header-margin: 4px 4px 0 4px;
   --jp-toolbar-active-background: var(--md-grey-300);
 
   /* Statusbar specific styles */
 
   --jp-statusbar-height: 24px;
 
   /* Input field styles */
@@ -341,23 +333,23 @@
   /* Code mirror specific styles */
 
   --jp-mirror-editor-keyword-color: #008000;
   --jp-mirror-editor-atom-color: #88f;
   --jp-mirror-editor-number-color: #080;
   --jp-mirror-editor-def-color: #00f;
   --jp-mirror-editor-variable-color: var(--md-grey-900);
-  --jp-mirror-editor-variable-2-color: #05a;
+  --jp-mirror-editor-variable-2-color: rgb(0, 54, 109);
   --jp-mirror-editor-variable-3-color: #085;
   --jp-mirror-editor-punctuation-color: #05a;
   --jp-mirror-editor-property-color: #05a;
-  --jp-mirror-editor-operator-color: #aa22ff;
+  --jp-mirror-editor-operator-color: #a2f;
   --jp-mirror-editor-comment-color: #408080;
   --jp-mirror-editor-string-color: #ba2121;
   --jp-mirror-editor-string-2-color: #708;
-  --jp-mirror-editor-meta-color: #aa22ff;
+  --jp-mirror-editor-meta-color: #a2f;
   --jp-mirror-editor-qualifier-color: #555;
   --jp-mirror-editor-builtin-color: #008000;
   --jp-mirror-editor-bracket-color: #997;
   --jp-mirror-editor-tag-color: #170;
   --jp-mirror-editor-attribute-color: #00c;
   --jp-mirror-editor-header-color: blue;
   --jp-mirror-editor-quote-color: #090;
@@ -401,14 +393,25 @@
 
   /* Icon colors that work well with light or dark backgrounds */
   --jp-icon-contrast-color0: var(--md-purple-600);
   --jp-icon-contrast-color1: var(--md-green-600);
   --jp-icon-contrast-color2: var(--md-pink-600);
   --jp-icon-contrast-color3: var(--md-blue-600);
 
+  /* Button colors */
+  --jp-accept-color-normal: var(--md-blue-700);
+  --jp-accept-color-hover: var(--md-blue-800);
+  --jp-accept-color-active: var(--md-blue-900);
+  --jp-warn-color-normal: var(--md-red-700);
+  --jp-warn-color-hover: var(--md-red-800);
+  --jp-warn-color-active: var(--md-red-900);
+  --jp-reject-color-normal: var(--md-grey-600);
+  --jp-reject-color-hover: var(--md-grey-700);
+  --jp-reject-color-active: var(--md-grey-800);
+
   /* File or activity icons and switch semantic variables */
   --jp-jupyter-icon-color: #f37626;
   --jp-notebook-icon-color: #f37626;
   --jp-json-icon-color: var(--md-orange-700);
   --jp-console-icon-background-color: var(--md-blue-700);
   --jp-console-icon-color: white;
   --jp-terminal-icon-background-color: var(--md-grey-800);
```

### Comparing `nbconvert-7.6.0/share/templates/latex/base.tex.j2` & `nbconvert-7.7.0/share/templates/latex/base.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/latex/display_priority.j2` & `nbconvert-7.7.0/share/templates/latex/display_priority.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/latex/document_contents.tex.j2` & `nbconvert-7.7.0/share/templates/latex/document_contents.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/latex/null.j2` & `nbconvert-7.7.0/share/templates/latex/null.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/latex/report.tex.j2` & `nbconvert-7.7.0/share/templates/latex/report.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/latex/style_bw_ipython.tex.j2` & `nbconvert-7.7.0/share/templates/latex/style_bw_ipython.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/latex/style_ipython.tex.j2` & `nbconvert-7.7.0/share/templates/latex/style_ipython.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/latex/style_jupyter.tex.j2` & `nbconvert-7.7.0/share/templates/latex/style_jupyter.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/latex/style_python.tex.j2` & `nbconvert-7.7.0/share/templates/latex/style_python.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/markdown/index.md.j2` & `nbconvert-7.7.0/share/templates/markdown/index.md.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/reveal/base.html.j2` & `nbconvert-7.7.0/share/templates/reveal/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/reveal/index.html.j2` & `nbconvert-7.7.0/share/templates/reveal/index.html.j2`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 {% set reveal_theme = resources.reveal.theme | default('white', true) %}
 {% set reveal_transition = resources.reveal.transition | default('slide', true) %}
 {% set reveal_number = resources.reveal.number | default('', true) %}
 {% set reveal_scroll = resources.reveal.scroll | default(false, true) | json_dumps %}
 
 {%- block header -%}
 <!DOCTYPE html>
-<html>
+<html lang="{{ resources.language_code }}">
 <head>
 
 {%- block html_head -%}
 <meta charset="utf-8" />
 <meta http-equiv="X-UA-Compatible" content="chrome=1" />
 
 <meta name="apple-mobile-web-app-capable" content="yes" />
@@ -114,21 +114,23 @@
 
 {%- block body_header -%}
 {% if resources.theme == 'dark' %}
 <body class="jp-Notebook" data-jp-theme-light="false" data-jp-theme-name="JupyterLab Dark">
 {% else %}
 <body class="jp-Notebook" data-jp-theme-light="true" data-jp-theme-name="JupyterLab Light">
 {% endif %}
+<main>
 <div class="reveal">
 <div class="slides">
 {%- endblock body_header -%}
 
 {% block body_footer %}
 </div>
 </div>
+</main>
 </body>
 {% endblock body_footer %}
 
 {% block footer %}
 {{ super() }}
 
 {% block footer_js %}
```

### Comparing `nbconvert-7.6.0/share/templates/reveal/static/custom_reveal.css` & `nbconvert-7.7.0/share/templates/reveal/static/custom_reveal.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/share/templates/rst/index.rst.j2` & `nbconvert-7.7.0/share/templates/rst/index.rst.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/.gitignore` & `nbconvert-7.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/LICENSE` & `nbconvert-7.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/README.md` & `nbconvert-7.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.6.0/hatch_build.py` & `nbconvert-7.7.0/hatch_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from urllib.request import urlopen
 
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 
 notebook_css_version = "5.4.0"
 notebook_css_url = "https://cdn.jupyter.org/notebook/%s/style/style.min.css" % notebook_css_version
 
-jupyterlab_css_version = "3.6.1"
+jupyterlab_css_version = "4.0.2"
 jupyterlab_css_url = (
     "https://unpkg.com/@jupyterlab/nbconvert-css@%s/style/index.css" % jupyterlab_css_version
 )
 
-jupyterlab_theme_light_version = "3.6.1"
+jupyterlab_theme_light_version = "4.0.2"
 jupyterlab_theme_light_url = (
     "https://unpkg.com/@jupyterlab/theme-light-extension@%s/style/variables.css"
     % jupyterlab_theme_light_version
 )
 
-jupyterlab_theme_dark_version = "3.6.1"
+jupyterlab_theme_dark_version = "4.0.2"
 jupyterlab_theme_dark_url = (
     "https://unpkg.com/@jupyterlab/theme-dark-extension@%s/style/variables.css"
     % jupyterlab_theme_dark_version
 )
 
 template_css_urls = {
     "lab": [
```

### Comparing `nbconvert-7.6.0/pyproject.toml` & `nbconvert-7.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling >=0.25"]
+requires = ["hatchling >=1.5"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nbconvert"
 authors = [{name = "Jupyter Development Team", email = "jupyter@googlegroups.com"}]
 license = {file = "LICENSE"}
 description = "Converting Jupyter Notebooks"
@@ -14,15 +14,15 @@
     "Intended Audience :: System Administrators",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 urls = {Homepage = "https://jupyter.org"}
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "beautifulsoup4",
     "bleach!=5.0.0",
     "defusedxml",
     "importlib_metadata>=3.6;python_version<\"3.10\"",
     "jinja2>=3.0",
     "jupyter_core>=4.7",
@@ -54,21 +54,22 @@
 notebook = "nbconvert.exporters:NotebookExporter"
 asciidoc = "nbconvert.exporters:ASCIIDocExporter"
 script = "nbconvert.exporters:ScriptExporter"
 
 [project.optional-dependencies]
 qtpng = ["pyqtwebengine>=5.15"]
 qtpdf = ["nbconvert[qtpng]"]
-webpdf = ["pyppeteer>=1,<1.1"]
+webpdf = ["playwright"]
 test = [
     "pytest",
     "pytest-dependency",
     "ipykernel",
     "ipywidgets>=7",
     "pre-commit",
+    "flaky"
 ]
 serve = ["tornado>=6.1"]
 docs = [
     "myst_parser",
     "sphinx==5.0.2",
     "pydata_sphinx_theme",
     "nbsphinx>=0.2.12",
@@ -125,15 +126,15 @@
 test = "mypy --install-types --non-interactive {args:nbconvert}"
 
 [tool.hatch.envs.lint]
 dependencies = [
   "black[jupyter]==23.3.0",
   "mdformat>0.7",
   "mdformat-gfm>=0.3.5",
-  "ruff==0.0.270"
+  "ruff==0.0.276"
 ]
 detached = true
 [tool.hatch.envs.lint.scripts]
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mdformat --check {args:docs *.md}"
@@ -159,14 +160,16 @@
     "ignore:getargs.*format is deprecated:DeprecationWarning",
     # From jupyter_client
     "ignore:unclosed <socket.socket:ResourceWarning",
     "ignore:There is no current event loop:DeprecationWarning",
     "ignore:unclosed event loop:ResourceWarning",
     # From jupyter_core
     "module:Jupyter is migrating its paths to use standard platformdirs:DeprecationWarning",
+    # From dateutil
+    "ignore:.*Use timezone-aware objects to represent datetimes in UTC:DeprecationWarning",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
   "pragma: no cover",
   "def __repr__",
   "if self.debug:",
@@ -222,14 +225,16 @@
   "E501",
   # SIM105 Use `contextlib.suppress(...)`
   "SIM105",
   # T201 `print` found
   "T201",
   # N802 Function name `CreateWellKnownSid` should be lowercase
   "N802", "N803",
+  # RUF012 Mutable class attributes should be annotated with `typing.ClassVar`
+  "RUF012",
 ]
 unfixable = [
   # Don't touch print statements
   "T201",
   # Don't touch noqa lines
   "RUF100",
 ]
```

### Comparing `nbconvert-7.6.0/PKG-INFO` & `nbconvert-7.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbconvert
-Version: 7.6.0
+Version: 7.7.0
 Summary: Converting Jupyter Notebooks
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
         - Copyright (c) 2001-2015, IPython Development Team
         - Copyright (c) 2015-, Jupyter Development Team
@@ -39,15 +39,15 @@
 Keywords: Interactive,Interpreter,Shell,Web
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: beautifulsoup4
 Requires-Dist: bleach!=5.0.0
 Requires-Dist: defusedxml
 Requires-Dist: importlib-metadata>=3.6; python_version < '3.10'
 Requires-Dist: jinja2>=3.0
 Requires-Dist: jupyter-core>=4.7
 Requires-Dist: jupyterlab-pygments
@@ -73,21 +73,22 @@
 Provides-Extra: qtpdf
 Requires-Dist: nbconvert[qtpng]; extra == 'qtpdf'
 Provides-Extra: qtpng
 Requires-Dist: pyqtwebengine>=5.15; extra == 'qtpng'
 Provides-Extra: serve
 Requires-Dist: tornado>=6.1; extra == 'serve'
 Provides-Extra: test
+Requires-Dist: flaky; extra == 'test'
 Requires-Dist: ipykernel; extra == 'test'
 Requires-Dist: ipywidgets>=7; extra == 'test'
 Requires-Dist: pre-commit; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-dependency; extra == 'test'
 Provides-Extra: webpdf
-Requires-Dist: pyppeteer<1.1,>=1; extra == 'webpdf'
+Requires-Dist: playwright; extra == 'webpdf'
 Description-Content-Type: text/markdown
 
 # nbconvert
 
 ### Jupyter Notebook Conversion
 
 [![Build Status](https://github.com/jupyter/nbconvert/actions/workflows/tests.yml/badge.svg?query=branch%3Amain++)](https://github.com/jupyter/nbconvert/actions/workflows/tests.yml/badge.svg?query=branch%3Amain++)
```

