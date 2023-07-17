# Comparing `tmp/jupyterlab_nodeeditor-1.0.5.tar.gz` & `tmp/jupyterlab_nodeeditor-1.0.6.tar.gz`

## Comparing `jupyterlab_nodeeditor-1.0.5.tar` & `jupyterlab_nodeeditor-1.0.6.tar`

### file list

```diff
@@ -1,453 +1,444 @@
--rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/.copier-answers.yml
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/.gitmodules
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/.prettierignore
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/.yarnrc.yml
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/CHANGELOG.md
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/RELEASE.md
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/dev.sh
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/init.sh
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/install.json
--rwxr-xr-x   0        0        0     6269 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/package.json
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/setup.py
--rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/tsconfig.json
--rwxr-xr-x   0        0        0   215696 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/yarn.lock
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/.vscode/settings.json
--rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/.copier-answers.yml
--rwxr-xr-x   0        0        0     1587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/.gitignore
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/.prettierignore
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/.yarnrc.yml
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/CHANGELOG.md
--rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/LICENSE
--rwxr-xr-x   0        0        0     2571 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/README.md
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/RELEASE.md
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/install.json
--rwxr-xr-x   0        0        0     5198 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/package.json
--rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/pyproject.toml
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/setup.py
--rwxr-xr-x   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/tsconfig.json
--rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/jupyterlab_nodeeditor/__init__.py
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/schema/plugin.json
--rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/src/index.ts
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/style/base.css
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/style/index.css
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/_temp_extension/style/index.js
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/.babelrc
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/.editorconfig
--rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/.eslintrc
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/.git
--rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/.gitignore
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/.npmignore
--rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/.nvmrc
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/.travis.yml
--rwxr-xr-x   0        0        0     3369 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/CODE_OF_CONDUCT.md
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/LICENSE
--rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/README.md
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/cypress.json
--rwxr-xr-x   0        0        0   533606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/logo.ai
--rwxr-xr-x   0        0        0    15873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/logo.png
--rwxr-xr-x   0        0        0     3123 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/logo.svg
--rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/package.json
--rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/rollup.config.js
--rwxr-xr-x   0        0        0   675825 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/yarn.lock
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/cypress/fixtures/example.json
--rwxr-xr-x   0        0        0     4389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/cypress/integration/NodeEditorSpec.js
--rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/cypress/plugins/index.js
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/cypress/support/commands.js
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/cypress/support/index.js
--rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/.gitignore
--rwxr-xr-x   0        0        0      721 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/README.md
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/babel.config.js
--rwxr-xr-x   0        0        0     3301 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docusaurus.config.js
--rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/package.json
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/sidebars.js
--rwxr-xr-x   0        0        0   428509 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/yarn.lock
--rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/blog/2019-05-28-hola.md
--rwxr-xr-x   0        0        0      428 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/blog/2019-05-29-hello-world.md
--rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/blog/2019-05-30-welcome.md
--rwxr-xr-x   0        0        0     4098 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/components/AnatomyExample.js
--rwxr-xr-x   0        0        0     1446 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/components/Colors.js
--rwxr-xr-x   0        0        0     5622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/components/ControlExamples.js
--rwxr-xr-x   0        0        0     5735 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/components/DynamicNodesExamples.js
--rwxr-xr-x   0        0        0     2495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/components/DynamicThemingExample.js
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/components/FlexRow.js
--rwxr-xr-x   0        0        0    16960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/components/GettingStartedExample.js
--rwxr-xr-x   0        0        0     6137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/NodeEditor.mdx
--rwxr-xr-x   0        0        0     5303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/RootEngine.mdx
--rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/anatomy.mdx
--rwxr-xr-x   0        0        0     8565 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/basic-config.mdx
--rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/colors.mdx
--rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/comments.mdx
--rwxr-xr-x   0        0        0     8897 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/controls.mdx
--rwxr-xr-x   0        0        0      525 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/defining-nodes.mdx
--rwxr-xr-x   0        0        0     4129 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/doc1.md
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/doc2.md
--rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/doc3.md
--rwxr-xr-x   0        0        0     5038 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/dynamic-nodes.mdx
--rwxr-xr-x   0        0        0     7241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/faq.mdx
--rwxr-xr-x   0        0        0    10532 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/flume-config.mdx
--rwxr-xr-x   0        0        0     4261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/logic-nodes.mdx
--rwxr-xr-x   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/mdx.md
--rwxr-xr-x   0        0        0     2232 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/node-editor.mdx
--rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/overview.mdx
--rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/quick-start.mdx
--rwxr-xr-x   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/root-engine.mdx
--rwxr-xr-x   0        0        0     2978 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/root-node.mdx
--rwxr-xr-x   0        0        0     2981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/running-logic.mdx
--rwxr-xr-x   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/saving-nodes.mdx
--rwxr-xr-x   0        0        0     1929 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/theming.mdx
--rwxr-xr-x   0        0        0     2296 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/type-safety.mdx
--rwxr-xr-x   0        0        0     4178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/using-with-react.mdx
--rwxr-xr-x   0        0        0     1818 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/docs/using-without-react.mdx
--rwxr-xr-x   0        0        0     8877 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/src/exampleFlumeConfig.js
--rwxr-xr-x   0        0        0    49415 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/src/components/TypeSafe.js
--rwxr-xr-x   0        0        0     1304 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/src/css/custom.css
--rwxr-xr-x   0        0        0    15622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/src/pages/index.js
--rwxr-xr-x   0        0        0    11943 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/src/pages/styles.module.css
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/.nojekyll
--rwxr-xr-x   0        0        0     4297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/60fps.svg
--rwxr-xr-x   0        0        0     5914 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/android-chrome-192x192.png
--rwxr-xr-x   0        0        0    17474 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/android-chrome-512x512.png
--rwxr-xr-x   0        0        0     5337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/apple-touch-icon.png
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/arrow-right-blue.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/arrow-right-green.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/arrow-right-red.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/arrow-right-red_1.svg
--rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/arrow-right.svg
--rwxr-xr-x   0        0        0     3193 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/controls.svg
--rwxr-xr-x   0        0        0   539930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/example_editors.png
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/favicon-16x16.png
--rwxr-xr-x   0        0        0      765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/favicon-32x32.png
--rwxr-xr-x   0        0        0    15406 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/favicon.ico
--rwxr-xr-x   0        0        0   127864 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/fb-img.png
--rwxr-xr-x   0        0        0   737734 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/flume-short-web.mp4
--rwxr-xr-x   0        0        0     5893 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/friends-graph.svg
--rwxr-xr-x   0        0        0    48634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/hero-nodes.svg
--rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/logo-dark.svg
--rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/logo.svg
--rwxr-xr-x   0        0        0     5626 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/netlify.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/page-curve-blue.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/page-curve-dark.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/page-curve.svg
--rwxr-xr-x   0        0        0     1588 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/performance-tile.svg
--rwxr-xr-x   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/play-icon.svg
--rwxr-xr-x   0        0        0     2880 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/react-tile.svg
--rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/size-tile.svg
--rwxr-xr-x   0        0        0     2330 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/theme-tile.svg
--rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/theme.svg
--rwxr-xr-x   0        0        0    41674 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/type-safe-node.svg
--rwxr-xr-x   0        0        0    21728 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/type-safe-nodes.svg
--rwxr-xr-x   0        0        0    31457 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/undraw_docusaurus_mountain.svg
--rwxr-xr-x   0        0        0    35968 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/undraw_docusaurus_react.svg
--rwxr-xr-x   0        0        0    11784 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/undraw_docusaurus_tree.svg
--rwxr-xr-x   0        0        0   146113 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/valid_port_types.png
--rwxr-xr-x   0        0        0      499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/wordmark_white.svg
--rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/.eslintrc
--rwxr-xr-x   0        0        0   105919 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/README.md
--rwxr-xr-x   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/package.json
--rwxr-xr-x   0        0        0   913821 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/yarn.lock
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/public/index.html
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/public/manifest.json
--rwxr-xr-x   0        0        0    18960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/App.js
--rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/index.css
--rwxr-xr-x   0        0        0     1503 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/index.js
--rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/TestRoutes/TestEditor.js
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/TestRoutes/nodes.js
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/components/Checkbox.js
--rwxr-xr-x   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/components/FloatingNavigation.js
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/components/Header.js
--rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/components/LogicEditor.js
--rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/components/Modal.js
--rwxr-xr-x   0        0        0     2000 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/components/OptionsEditor.js
--rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/icons/BoxIcon.js
--rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/icons/FormIcon.js
--rwxr-xr-x   0        0        0     3783 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/icons/GearIcon.js
--rwxr-xr-x   0        0        0     6066 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/Attributes.js
--rwxr-xr-x   0        0        0     2886 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/Body.js
--rwxr-xr-x   0        0        0     2020 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/Field.js
--rwxr-xr-x   0        0        0    10739 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/Form.css
--rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/Form.js
--rwxr-xr-x   0        0        0     1834 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/InputTypes.js
--rwxr-xr-x   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/NodeTypes.js
--rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/PreviewField.js
--rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/Sidebar.js
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/defaultNodes.js
--rwxr-xr-x   0        0        0      815 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/designerReducer.js
--rwxr-xr-x   0        0        0     1261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/fieldTypes.js
--rwxr-xr-x   0        0        0     1560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/fieldsReducer.js
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/formHandler.js
--rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/previewFieldsReducer.js
--rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/resolveLogic.js
--rwxr-xr-x   0        0        0     8710 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/wizardLogic/logicTypes.js
--rwxr-xr-x   0        0        0     1910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Forms/Forms.css
--rwxr-xr-x   0        0        0     1854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Forms/Forms.js
--rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Records/Records.css
--rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Records/Records.js
--rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/.eslintrc
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/Cache.js
--rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/RootEngine.js
--rwxr-xr-x   0        0        0     2060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/commentsReducer.js
--rwxr-xr-x   0        0        0     6241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/connectionCalculator.js
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/constants.js
--rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/context.js
--rwxr-xr-x   0        0        0     9649 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/index.js
--rwxr-xr-x   0        0        0    14282 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/nodesReducer.js
--rwxr-xr-x   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/stageReducer.js
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/styles.css
--rwxr-xr-x   0        0        0     1191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/toastsReducer.js
--rwxr-xr-x   0        0        0     8905 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/typeBuilders.js
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/utilities.js
--rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Checkbox/Checkbox.css
--rwxr-xr-x   0        0        0      651 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Checkbox/Checkbox.js
--rwxr-xr-x   0        0        0     1134 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/ColorPicker/ColorPicker.css
--rwxr-xr-x   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/ColorPicker/ColorPicker.js
--rwxr-xr-x   0        0        0     2159 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Comment/Comment.css
--rwxr-xr-x   0        0        0     7028 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Comment/Comment.js
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Connection/Connection.css
--rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Connection/Connection.js
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Connections/Connections.css
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Connections/Connections.js
--rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/ContextMenu/ContextMenu.css
--rwxr-xr-x   0        0        0     7071 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/ContextMenu/ContextMenu.js
--rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Control/Control.css
--rwxr-xr-x   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Control/Control.js
--rwxr-xr-x   0        0        0     3751 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Draggable/Draggable.js
--rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/IoPorts/IoPorts.css
--rwxr-xr-x   0        0        0    12769 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/IoPorts/IoPorts.js
--rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Node/Node.css
--rwxr-xr-x   0        0        0     7392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Node/Node.js
--rwxr-xr-x   0        0        0     2001 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Select/Select.css
--rwxr-xr-x   0        0        0     3675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Select/Select.js
--rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Stage/Stage.css
--rwxr-xr-x   0        0        0     9421 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Stage/Stage.js
--rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/TextInput/TextInput.css
--rwxr-xr-x   0        0        0     3405 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/TextInput/TextInput.js
--rwxr-xr-x   0        0        0     2223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Toaster/Toaster.css
--rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/components/Toaster/Toaster.js
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/hooks/usePrevious.js
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/img/grid.png
--rwxr-xr-x   0        0        0     8912 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/tests/dynamic.test.js
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/tests/nodes.js
--rwxr-xr-x   0        0        0     1409 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/tests/ssr.test.js
--rwxr-xr-x   0        0        0     1397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/flume/src/tests/test.js
--rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/__init__.py
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/_version.py
--rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/select.py
--rwxr-xr-x   0        0        0     2578 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/utils.py
--rwxr-xr-x   0        0        0    20983 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/build_log.json
--rwxr-xr-x   0        0        0     5572 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/package.json
--rwxr-xr-x   0        0        0     6248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig
--rwxr-xr-x   0        0        0    11646 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json
--rwxr-xr-x   0        0        0    73464 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf
--rwxr-xr-x   0        0        0    17913 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/data_image_png_base64_iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5_AAAAAXNSR0IArs4c6QAAAARnQU1-5f4412.8573e56b3e457c1d826b.js
--rwxr-xr-x   0        0        0   540746 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/lib_index_js.fcc62e78977ee568769f.js
--rwxr-xr-x   0        0        0   853578 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/lib_index_js.fcc62e78977ee568769f.js.map
--rwxr-xr-x   0        0        0     6996 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_apex_apex_js.9982e0769f40abee234a.js
--rwxr-xr-x   0        0        0     9200 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_apex_apex_js.9982e0769f40abee234a.js.map
--rwxr-xr-x   0        0        0     2664 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_azcli_azcli_js.182cee8a9aa456f6febd.js
--rwxr-xr-x   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_azcli_azcli_js.182cee8a9aa456f6febd.js.map
--rwxr-xr-x   0        0        0     3696 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_bat_bat_js.55db1a421d24f3d884a7.js
--rwxr-xr-x   0        0        0     4079 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_bat_bat_js.55db1a421d24f3d884a7.js.map
--rwxr-xr-x   0        0        0     4786 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_bicep_bicep_js.1d144118bc30d3f19464.js
--rwxr-xr-x   0        0        0     5791 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_bicep_bicep_js.1d144118bc30d3f19464.js.map
--rwxr-xr-x   0        0        0     4505 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_cameligo_cameligo_js.1674e1b671d71f42a4c2.js
--rwxr-xr-x   0        0        0     5512 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_cameligo_cameligo_js.1674e1b671d71f42a4c2.js.map
--rwxr-xr-x   0        0        0     6584 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_coffee_coffee_js.5203585c44a43b4dd973.js
--rwxr-xr-x   0        0        0     8209 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_coffee_coffee_js.5203585c44a43b4dd973.js.map
--rwxr-xr-x   0        0        0     9106 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_cpp_cpp_js.0fa4bdcecb4b3a69eb94.js
--rwxr-xr-x   0        0        0    11989 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_cpp_cpp_js.0fa4bdcecb4b3a69eb94.js.map
--rwxr-xr-x   0        0        0     7946 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_csharp_csharp_js.d17276a727e138d62758.js
--rwxr-xr-x   0        0        0    10449 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_csharp_csharp_js.d17276a727e138d62758.js.map
--rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_csp_csp_js.7d0541c505bba64c05d9.js
--rwxr-xr-x   0        0        0     2761 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_csp_csp_js.7d0541c505bba64c05d9.js.map
--rwxr-xr-x   0        0        0     7137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_css_css_js.ee8ef84415cbaf78afb7.js
--rwxr-xr-x   0        0        0     9112 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_css_css_js.ee8ef84415cbaf78afb7.js.map
--rwxr-xr-x   0        0        0     6218 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_cypher_cypher_js.a0c83171cb974949a02c.js
--rwxr-xr-x   0        0        0     7949 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_cypher_cypher_js.a0c83171cb974949a02c.js.map
--rwxr-xr-x   0        0        0     7205 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_dart_dart_js.4420e06db9a150d9b45c.js
--rwxr-xr-x   0        0        0     9164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_dart_dart_js.4420e06db9a150d9b45c.js.map
--rwxr-xr-x   0        0        0     4248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_dockerfile_dockerfile_js.2f95d8158ea4f41996f4.js
--rwxr-xr-x   0        0        0     4888 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_dockerfile_dockerfile_js.2f95d8158ea4f41996f4.js.map
--rwxr-xr-x   0        0        0     9034 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_ecl_ecl_js.0f56bcbc2002bbee3a30.js
--rwxr-xr-x   0        0        0    12353 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_ecl_ecl_js.0f56bcbc2002bbee3a30.js.map
--rwxr-xr-x   0        0        0     3901 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_flow9_flow9_js.ee19c04e3556e2f3320e.js
--rwxr-xr-x   0        0        0     4596 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_flow9_flow9_js.ee19c04e3556e2f3320e.js.map
--rwxr-xr-x   0        0        0     5484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_fsharp_fsharp_js.7a7fd32fad2f13d0265b.js
--rwxr-xr-x   0        0        0     6809 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_fsharp_fsharp_js.7a7fd32fad2f13d0265b.js.map
--rwxr-xr-x   0        0        0     5105 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_go_go_js.5be77765d5a4b7ffa983.js
--rwxr-xr-x   0        0        0     6431 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_go_go_js.5be77765d5a4b7ffa983.js.map
--rwxr-xr-x   0        0        0     4459 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_graphql_graphql_js.4a586f64f410b2ee3f6a.js
--rwxr-xr-x   0        0        0     5215 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_graphql_graphql_js.4a586f64f410b2ee3f6a.js.map
--rwxr-xr-x   0        0        0     6040 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_hcl_hcl_js.230c7d363321015f2c60.js
--rwxr-xr-x   0        0        0     7144 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_hcl_hcl_js.230c7d363321015f2c60.js.map
--rwxr-xr-x   0        0        0     9137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_html_html_js.6d7d95bee6027181f0af.js
--rwxr-xr-x   0        0        0    11085 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_html_html_js.6d7d95bee6027181f0af.js.map
--rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_ini_ini_js.b4cd6fd84ced941317a1.js
--rwxr-xr-x   0        0        0     2854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_ini_ini_js.b4cd6fd84ced941317a1.js.map
--rwxr-xr-x   0        0        0     5758 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_java_java_js.b5a0555fb9f413aebaf1.js
--rwxr-xr-x   0        0        0     7187 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_java_java_js.b5a0555fb9f413aebaf1.js.map
--rwxr-xr-x   0        0        0     6132 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_kotlin_kotlin_js.84d331c6922c4b011779.js
--rwxr-xr-x   0        0        0     7750 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_kotlin_kotlin_js.84d331c6922c4b011779.js.map
--rwxr-xr-x   0        0        0     6347 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_less_less_js.0cefe82e77a5f720a3a8.js
--rwxr-xr-x   0        0        0     7847 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_less_less_js.0cefe82e77a5f720a3a8.js.map
--rwxr-xr-x   0        0        0     4730 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_lexon_lexon_js.5856d26bc8d67dadde9e.js
--rwxr-xr-x   0        0        0     5606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_lexon_lexon_js.5856d26bc8d67dadde9e.js.map
--rwxr-xr-x   0        0        0     7442 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_liquid_liquid_js.ccc8e1bb782d3bdb55c0.js
--rwxr-xr-x   0        0        0     9108 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_liquid_liquid_js.ccc8e1bb782d3bdb55c0.js.map
--rwxr-xr-x   0        0        0     4386 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_lua_lua_js.7bb5d5716d12f5c2174e.js
--rwxr-xr-x   0        0        0     5307 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_lua_lua_js.7bb5d5716d12f5c2174e.js.map
--rwxr-xr-x   0        0        0     5283 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_m3_m3_js.afda01e1b4bcc050d4f2.js
--rwxr-xr-x   0        0        0     6629 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_m3_m3_js.afda01e1b4bcc050d4f2.js.map
--rwxr-xr-x   0        0        0     6771 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_markdown_markdown_js.1fb78cdc3130ad3eaba3.js
--rwxr-xr-x   0        0        0     8213 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_markdown_markdown_js.1fb78cdc3130ad3eaba3.js.map
--rwxr-xr-x   0        0        0     5181 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_mips_mips_js.1bf6111c8b5601cd2b20.js
--rwxr-xr-x   0        0        0     6277 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_mips_mips_js.1bf6111c8b5601cd2b20.js.map
--rwxr-xr-x   0        0        0     8230 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_msdax_msdax_js.64aeebc1b0c103ab96af.js
--rwxr-xr-x   0        0        0    10919 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_msdax_msdax_js.64aeebc1b0c103ab96af.js.map
--rwxr-xr-x   0        0        0     4838 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_objective-c_objective-c_js.8c0d01235bc1d630adfa.js
--rwxr-xr-x   0        0        0     5873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_objective-c_objective-c_js.8c0d01235bc1d630adfa.js.map
--rwxr-xr-x   0        0        0     5648 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pascal_pascal_js.df74d1d4ca179e1b1afd.js
--rwxr-xr-x   0        0        0     7341 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pascal_pascal_js.df74d1d4ca179e1b1afd.js.map
--rwxr-xr-x   0        0        0     4257 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pascaligo_pascaligo_js.ff3af5a55838b031f360.js
--rwxr-xr-x   0        0        0     5106 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pascaligo_pascaligo_js.ff3af5a55838b031f360.js.map
--rwxr-xr-x   0        0        0     3938 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pla_pla_js.1932e28a5d8475c1ee52.js
--rwxr-xr-x   0        0        0     4566 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pla_pla_js.1932e28a5d8475c1ee52.js.map
--rwxr-xr-x   0        0        0     6473 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_powershell_powershell_js.e3c2ee7998ea24edb731.js
--rwxr-xr-x   0        0        0     8014 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_powershell_powershell_js.e3c2ee7998ea24edb731.js.map
--rwxr-xr-x   0        0        0     9200 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pug_pug_js.9926ff3fec177afe4c34.js
--rwxr-xr-x   0        0        0    12274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_pug_pug_js.9926ff3fec177afe4c34.js.map
--rwxr-xr-x   0        0        0     7044 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_python_python_js.f9cd61ae70cb69be71d9.js
--rwxr-xr-x   0        0        0     8652 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_python_python_js.f9cd61ae70cb69be71d9.js.map
--rwxr-xr-x   0        0        0     5760 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_qsharp_qsharp_js.3159e1b26ee42f37dc9e.js
--rwxr-xr-x   0        0        0     7569 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_qsharp_qsharp_js.3159e1b26ee42f37dc9e.js.map
--rwxr-xr-x   0        0        0     5896 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_r_r_js.08cb4e804cb3e9a28ace.js
--rwxr-xr-x   0        0        0     7493 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_r_r_js.08cb4e804cb3e9a28ace.js.map
--rwxr-xr-x   0        0        0     6486 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_redis_redis_js.8ae88e112ec72cfcf9f7.js
--rwxr-xr-x   0        0        0     8468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_redis_redis_js.8ae88e112ec72cfcf9f7.js.map
--rwxr-xr-x   0        0        0     6415 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_restructuredtext_restructuredtext_js.562d4848347010a99e0e.js
--rwxr-xr-x   0        0        0     7509 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_restructuredtext_restructuredtext_js.562d4848347010a99e0e.js.map
--rwxr-xr-x   0        0        0     7373 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_rust_rust_js.7c87889f44878696136b.js
--rwxr-xr-x   0        0        0     9872 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_rust_rust_js.7c87889f44878696136b.js.map
--rwxr-xr-x   0        0        0     3779 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_sb_sb_js.ae2f354ae4f12d7bd72b.js
--rwxr-xr-x   0        0        0     4229 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_sb_sb_js.ae2f354ae4f12d7bd72b.js.map
--rwxr-xr-x   0        0        0     3729 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_scheme_scheme_js.e36dc0d354f0f5b3fbf0.js
--rwxr-xr-x   0        0        0     4205 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_scheme_scheme_js.e36dc0d354f0f5b3fbf0.js.map
--rwxr-xr-x   0        0        0     9582 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_scss_scss_js.35f4327ac70035ac003a.js
--rwxr-xr-x   0        0        0    12633 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_scss_scss_js.35f4327ac70035ac003a.js.map
--rwxr-xr-x   0        0        0     5689 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_shell_shell_js.d8464c269c4488a6b1fe.js
--rwxr-xr-x   0        0        0     7135 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_shell_shell_js.d8464c269c4488a6b1fe.js.map
--rwxr-xr-x   0        0        0     5158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_sophia_sophia_js.e3f378c1653b0a1e984f.js
--rwxr-xr-x   0        0        0     6252 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_sophia_sophia_js.e3f378c1653b0a1e984f.js.map
--rwxr-xr-x   0        0        0     4895 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_sparql_sparql_js.d0d19d5b847835e9b1e3.js
--rwxr-xr-x   0        0        0     6025 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_sparql_sparql_js.d0d19d5b847835e9b1e3.js.map
--rwxr-xr-x   0        0        0     8323 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_swift_swift_js.47b7cefa925e9c066b7c.js
--rwxr-xr-x   0        0        0    10656 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_swift_swift_js.47b7cefa925e9c066b7c.js.map
--rwxr-xr-x   0        0        0     6239 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_tcl_tcl_js.d48ef01cf0e13cf29944.js
--rwxr-xr-x   0        0        0     8056 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_tcl_tcl_js.d48ef01cf0e13cf29944.js.map
--rwxr-xr-x   0        0        0     9704 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_twig_twig_js.d82831f1acc1c666fb3d.js
--rwxr-xr-x   0        0        0    12280 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_twig_twig_js.d82831f1acc1c666fb3d.js.map
--rwxr-xr-x   0        0        0     9551 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_typescript_typescript_js.0ae9761d4b0d1e6cfa16.js
--rwxr-xr-x   0        0        0    11825 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_typescript_typescript_js.0ae9761d4b0d1e6cfa16.js.map
--rwxr-xr-x   0        0        0     9174 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_vb_vb_js.a4905a4081d413b6d210.js
--rwxr-xr-x   0        0        0    12065 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_vb_vb_js.a4905a4081d413b6d210.js.map
--rwxr-xr-x   0        0        0     9782 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_wgsl_wgsl_js.645eabcb3aff15176c38.js
--rwxr-xr-x   0        0        0    12972 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_wgsl_wgsl_js.645eabcb3aff15176c38.js.map
--rwxr-xr-x   0        0        0     4982 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_xml_xml_js.aacaca7fd9d934e1d513.js
--rwxr-xr-x   0        0        0     5400 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_xml_xml_js.aacaca7fd9d934e1d513.js.map
--rwxr-xr-x   0        0        0     7285 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_yaml_yaml_js.f54c221e346beb62289c.js
--rwxr-xr-x   0        0        0     8643 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_monaco-editor_esm_vs_basic-languages_yaml_yaml_js.f54c221e346beb62289c.js.map
--rwxr-xr-x   0        0        0    23727 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_process_browser_js-data_image_png_base64_iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAAC-c7fe92.426b74ce6f751a6627be.js
--rwxr-xr-x   0        0        0     6843 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/node_modules_process_browser_js-data_image_png_base64_iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAAC-c7fe92.426b74ce6f751a6627be.js.map
--rwxr-xr-x   0        0        0    41803 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/remoteEntry.daeae06c6d772e670e7b.js
--rwxr-xr-x   0        0        0    41012 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/remoteEntry.daeae06c6d772e670e7b.js.map
--rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/style.js
--rwxr-xr-x   0        0        0    19500 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/style_index_js.81c2517e7d07af255c14.js
--rwxr-xr-x   0        0        0    15018 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/style_index_js.81c2517e7d07af255c14.js.map
--rwxr-xr-x   0        0        0    43753 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-flume_node_modules_prop-types_index_js-node_modules_process_browser_js.42651e68d03e160d6f50.js
--rwxr-xr-x   0        0        0    49836 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-flume_node_modules_prop-types_index_js-node_modules_process_browser_js.42651e68d03e160d6f50.js.map
--rwxr-xr-x   0        0        0    22154 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_abap_abap_js.b9acd748da7ff3350995.js
--rwxr-xr-x   0        0        0    32103 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_abap_abap_js.b9acd748da7ff3350995.js.map
--rwxr-xr-x   0        0        0    14810 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_clojure_clojure_js.a5f8283882d0bdb93925.js
--rwxr-xr-x   0        0        0    20622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_clojure_clojure_js.a5f8283882d0bdb93925.js.map
--rwxr-xr-x   0        0        0    15527 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_elixir_elixir_js.2979134714531778d948.js
--rwxr-xr-x   0        0        0    19907 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_elixir_elixir_js.2979134714531778d948.js.map
--rwxr-xr-x   0        0        0    26576 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_freemarker2_freemarker2_js.7d62e95fa6c125a74bf5.js
--rwxr-xr-x   0        0        0    33791 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_freemarker2_freemarker2_js.7d62e95fa6c125a74bf5.js.map
--rwxr-xr-x   0        0        0    11996 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_handlebars_handlebars_js.f2c604f0bc3f6423e8c7.js
--rwxr-xr-x   0        0        0    14936 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_handlebars_handlebars_js.f2c604f0bc3f6423e8c7.js.map
--rwxr-xr-x   0        0        0    12598 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_javascript_javascript_js.c3c5914a19d6e077645e.js
--rwxr-xr-x   0        0        0    14289 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_javascript_javascript_js.c3c5914a19d6e077645e.js.map
--rwxr-xr-x   0        0        0    11534 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_julia_julia_js.660cedb0abb2fe3e27a7.js
--rwxr-xr-x   0        0        0    15462 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_julia_julia_js.660cedb0abb2fe3e27a7.js.map
--rwxr-xr-x   0        0        0    17119 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_mysql_mysql_js.4dcbef8818f057aeaab3.js
--rwxr-xr-x   0        0        0    23804 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_mysql_mysql_js.4dcbef8818f057aeaab3.js.map
--rwxr-xr-x   0        0        0    13235 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_perl_perl_js.92abc34c6cf667e58d20.js
--rwxr-xr-x   0        0        0    18301 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_perl_perl_js.92abc34c6cf667e58d20.js.map
--rwxr-xr-x   0        0        0    19185 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_pgsql_pgsql_js.0964523139d4821964b6.js
--rwxr-xr-x   0        0        0    25614 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_pgsql_pgsql_js.0964523139d4821964b6.js.map
--rwxr-xr-x   0        0        0    12885 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_php_php_js.89c54b836095365cbd76.js
--rwxr-xr-x   0        0        0    16472 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_php_php_js.89c54b836095365cbd76.js.map
--rwxr-xr-x   0        0        0    12904 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_postiats_postiats_js.39e416b365187b825ab1.js
--rwxr-xr-x   0        0        0    17558 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_postiats_postiats_js.39e416b365187b825ab1.js.map
--rwxr-xr-x   0        0        0    22953 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_powerquery_powerquery_js.794f25521bfb793e2592.js
--rwxr-xr-x   0        0        0    29584 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_powerquery_powerquery_js.794f25521bfb793e2592.js.map
--rwxr-xr-x   0        0        0    13967 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_protobuf_protobuf_js.109b1979e218a3fccb2a.js
--rwxr-xr-x   0        0        0    18320 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_protobuf_protobuf_js.109b1979e218a3fccb2a.js.map
--rwxr-xr-x   0        0        0    14667 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_razor_razor_js.963081f3fb1d7074c622.js
--rwxr-xr-x   0        0        0    18604 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_razor_razor_js.963081f3fb1d7074c622.js.map
--rwxr-xr-x   0        0        0    17358 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_redshift_redshift_js.2bec585aca61add92a63.js
--rwxr-xr-x   0        0        0    23435 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_redshift_redshift_js.2bec585aca61add92a63.js.map
--rwxr-xr-x   0        0        0    13475 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_ruby_ruby_js.f1d2de0d3708113d1047.js
--rwxr-xr-x   0        0        0    17609 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_ruby_ruby_js.f1d2de0d3708113d1047.js.map
--rwxr-xr-x   0        0        0    11370 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_scala_scala_js.17d63d898fcd57883055.js
--rwxr-xr-x   0        0        0    14258 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_scala_scala_js.17d63d898fcd57883055.js.map
--rwxr-xr-x   0        0        0    26840 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_solidity_solidity_js.60c54c6dab98bc84fed9.js
--rwxr-xr-x   0        0        0    37198 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_solidity_solidity_js.60c54c6dab98bc84fed9.js.map
--rwxr-xr-x   0        0        0    15932 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_sql_sql_js.e41c82d9fa334693ad98.js
--rwxr-xr-x   0        0        0    22315 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_sql_sql_js.e41c82d9fa334693ad98.js.map
--rwxr-xr-x   0        0        0    11243 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_st_st_js.da9aa70576309f2d7607.js
--rwxr-xr-x   0        0        0    15184 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_st_st_js.da9aa70576309f2d7607.js.map
--rwxr-xr-x   0        0        0    12392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_systemverilog_systemverilog_js.d4906f14a72eeea290d0.js
--rwxr-xr-x   0        0        0    16673 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_basic-languages_systemverilog_systemverilog_js.d4906f14a72eeea290d0.js.map
--rwxr-xr-x   0        0        0 10725780 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_editor_editor_main_js.2f82887a25519ad5606c.js
--rwxr-xr-x   0        0        0  9781956 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_editor_editor_main_js.2f82887a25519ad5606c.js.map
--rwxr-xr-x   0        0        0    71400 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_css_cssMode_js.0e78e528ecf4b44f65e3.js
--rwxr-xr-x   0        0        0    83402 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_css_cssMode_js.0e78e528ecf4b44f65e3.js.map
--rwxr-xr-x   0        0        0    72566 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_html_htmlMode_js.4d082c3f023de51f874a.js
--rwxr-xr-x   0        0        0    84609 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_html_htmlMode_js.4d082c3f023de51f874a.js.map
--rwxr-xr-x   0        0        0    86490 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_json_jsonMode_js.3877344c5bc28d2c62f1.js
--rwxr-xr-x   0        0        0   102226 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_json_jsonMode_js.3877344c5bc28d2c62f1.js.map
--rwxr-xr-x   0        0        0    44884 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_typescript_tsMode_js.532242b4e273f33ae96d.js
--rwxr-xr-x   0        0        0    50468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_monaco-editor_esm_vs_language_typescript_tsMode_js.532242b4e273f33ae96d.js.map
--rwxr-xr-x   0        0        0    58952 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_react-portal_es_index_js.e0238c949efe3800e101.js
--rwxr-xr-x   0        0        0    59619 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_react-portal_es_index_js.e0238c949efe3800e101.js.map
--rwxr-xr-x   0        0        0    33766 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_uuid_dist_esm-browser_index_js.50ddbbbe16d9fbb8e598.js
--rwxr-xr-x   0        0        0    25722 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/vendors-node_modules_uuid_dist_esm-browser_index_js.50ddbbbe16d9fbb8e598.js.map
--rwxr-xr-x   0        0        0    11646 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/schema/plugin.json
--rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/ReRunIcon.tsx
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/arrownIcon.tsx
--rwxr-xr-x   0        0        0     1455 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/clearIcon.tsx
--rwxr-xr-x   0        0        0      954 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/deleteIcon.tsx
--rwxr-xr-x   0        0        0     1505 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/exportIcon.tsx
--rwxr-xr-x   0        0        0     1310 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/factory.ts
--rwxr-xr-x   0        0        0    37793 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/flumeConfig.tsx
--rwxr-xr-x   0        0        0     7454 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/imageViewer.tsx
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/index.ts
--rwxr-xr-x   0        0        0     2268 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/lockIcon.tsx
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/model.ts
--rwxr-xr-x   0        0        0      807 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/newIcon.tsx
--rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/runIcon.tsx
--rwxr-xr-x   0        0        0     2349 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/utils.tsx
--rwxr-xr-x   0        0        0   168993 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/widget.tsx
--rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/src/yesIcon.tsx
--rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/style/base.css
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/style/index.css
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/style/index.js
--rwxr-xr-x   0        0        0   254494 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/test_ext/1.jpeg
--rwxr-xr-x   0        0        0   153675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/test_ext/2.jpeg
--rwxr-xr-x   0        0        0     2162 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/test_ext/main.ipynb
--rwxr-xr-x   0        0        0   546797 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/test_ext/testlib.ipynb
--rwxr-xr-x   0        0        0     1586 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/.gitignore
--rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/LICENSE
--rwxr-xr-x   0        0        0     2557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/README.md
--rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/.copier-answers.yml
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/.gitmodules
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/.prettierignore
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/.yarnrc.yml
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/CHANGELOG.md
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/RELEASE.md
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/dev.sh
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/init.sh
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/install.json
+-rwxr-xr-x   0        0        0     6248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/package.json
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/setup.py
+-rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/tsconfig.json
+-rwxr-xr-x   0        0        0   215696 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/yarn.lock
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/.vscode/settings.json
+-rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/.copier-answers.yml
+-rwxr-xr-x   0        0        0     1587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/.gitignore
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/.prettierignore
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/.yarnrc.yml
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/LICENSE
+-rwxr-xr-x   0        0        0     2571 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/README.md
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/RELEASE.md
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/install.json
+-rwxr-xr-x   0        0        0     5198 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/package.json
+-rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/pyproject.toml
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/setup.py
+-rwxr-xr-x   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/tsconfig.json
+-rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/jupyterlab_nodeeditor/__init__.py
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/schema/plugin.json
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/src/index.ts
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/style/base.css
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/style/index.css
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/style/index.js
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.babelrc
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.editorconfig
+-rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.eslintrc
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.git
+-rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.gitignore
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.npmignore
+-rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.nvmrc
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.travis.yml
+-rwxr-xr-x   0        0        0     3369 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/LICENSE
+-rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/README.md
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/cypress.json
+-rwxr-xr-x   0        0        0   533606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/logo.ai
+-rwxr-xr-x   0        0        0    15873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/logo.png
+-rwxr-xr-x   0        0        0     3123 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/logo.svg
+-rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/package.json
+-rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/rollup.config.js
+-rwxr-xr-x   0        0        0   675825 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/yarn.lock
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/cypress/fixtures/example.json
+-rwxr-xr-x   0        0        0     4389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/cypress/integration/NodeEditorSpec.js
+-rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/cypress/plugins/index.js
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/cypress/support/commands.js
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/cypress/support/index.js
+-rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/.gitignore
+-rwxr-xr-x   0        0        0      721 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/README.md
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/babel.config.js
+-rwxr-xr-x   0        0        0     3301 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docusaurus.config.js
+-rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/package.json
+-rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/sidebars.js
+-rwxr-xr-x   0        0        0   428509 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/yarn.lock
+-rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/blog/2019-05-28-hola.md
+-rwxr-xr-x   0        0        0      428 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/blog/2019-05-29-hello-world.md
+-rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/blog/2019-05-30-welcome.md
+-rwxr-xr-x   0        0        0     4098 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/AnatomyExample.js
+-rwxr-xr-x   0        0        0     1446 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/Colors.js
+-rwxr-xr-x   0        0        0     5622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/ControlExamples.js
+-rwxr-xr-x   0        0        0     5735 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/DynamicNodesExamples.js
+-rwxr-xr-x   0        0        0     2495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/DynamicThemingExample.js
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/FlexRow.js
+-rwxr-xr-x   0        0        0    16960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/GettingStartedExample.js
+-rwxr-xr-x   0        0        0     6137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/NodeEditor.mdx
+-rwxr-xr-x   0        0        0     5303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/RootEngine.mdx
+-rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/anatomy.mdx
+-rwxr-xr-x   0        0        0     8565 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/basic-config.mdx
+-rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/colors.mdx
+-rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/comments.mdx
+-rwxr-xr-x   0        0        0     8897 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/controls.mdx
+-rwxr-xr-x   0        0        0      525 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/defining-nodes.mdx
+-rwxr-xr-x   0        0        0     4129 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/doc1.md
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/doc2.md
+-rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/doc3.md
+-rwxr-xr-x   0        0        0     5038 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/dynamic-nodes.mdx
+-rwxr-xr-x   0        0        0     7241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/faq.mdx
+-rwxr-xr-x   0        0        0    10532 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/flume-config.mdx
+-rwxr-xr-x   0        0        0     4261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/logic-nodes.mdx
+-rwxr-xr-x   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/mdx.md
+-rwxr-xr-x   0        0        0     2232 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/node-editor.mdx
+-rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/overview.mdx
+-rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/quick-start.mdx
+-rwxr-xr-x   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/root-engine.mdx
+-rwxr-xr-x   0        0        0     2978 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/root-node.mdx
+-rwxr-xr-x   0        0        0     2981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/running-logic.mdx
+-rwxr-xr-x   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/saving-nodes.mdx
+-rwxr-xr-x   0        0        0     1929 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/theming.mdx
+-rwxr-xr-x   0        0        0     2296 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/type-safety.mdx
+-rwxr-xr-x   0        0        0     4178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/using-with-react.mdx
+-rwxr-xr-x   0        0        0     1818 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/using-without-react.mdx
+-rwxr-xr-x   0        0        0     8877 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/src/exampleFlumeConfig.js
+-rwxr-xr-x   0        0        0    49415 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/src/components/TypeSafe.js
+-rwxr-xr-x   0        0        0     1304 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/src/css/custom.css
+-rwxr-xr-x   0        0        0    15622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/src/pages/index.js
+-rwxr-xr-x   0        0        0    11943 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/src/pages/styles.module.css
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/.nojekyll
+-rwxr-xr-x   0        0        0     4297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/60fps.svg
+-rwxr-xr-x   0        0        0     5914 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/android-chrome-192x192.png
+-rwxr-xr-x   0        0        0    17474 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/android-chrome-512x512.png
+-rwxr-xr-x   0        0        0     5337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/apple-touch-icon.png
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/arrow-right-blue.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/arrow-right-green.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/arrow-right-red.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/arrow-right-red_1.svg
+-rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/arrow-right.svg
+-rwxr-xr-x   0        0        0     3193 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/controls.svg
+-rwxr-xr-x   0        0        0   539930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/example_editors.png
+-rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/favicon-16x16.png
+-rwxr-xr-x   0        0        0      765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/favicon-32x32.png
+-rwxr-xr-x   0        0        0    15406 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/favicon.ico
+-rwxr-xr-x   0        0        0   127864 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/fb-img.png
+-rwxr-xr-x   0        0        0   737734 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/flume-short-web.mp4
+-rwxr-xr-x   0        0        0     5893 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/friends-graph.svg
+-rwxr-xr-x   0        0        0    48634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/hero-nodes.svg
+-rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/logo-dark.svg
+-rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/logo.svg
+-rwxr-xr-x   0        0        0     5626 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/netlify.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/page-curve-blue.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/page-curve-dark.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/page-curve.svg
+-rwxr-xr-x   0        0        0     1588 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/performance-tile.svg
+-rwxr-xr-x   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/play-icon.svg
+-rwxr-xr-x   0        0        0     2880 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/react-tile.svg
+-rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/size-tile.svg
+-rwxr-xr-x   0        0        0     2330 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/theme-tile.svg
+-rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/theme.svg
+-rwxr-xr-x   0        0        0    41674 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/type-safe-node.svg
+-rwxr-xr-x   0        0        0    21728 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/type-safe-nodes.svg
+-rwxr-xr-x   0        0        0    31457 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/undraw_docusaurus_mountain.svg
+-rwxr-xr-x   0        0        0    35968 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/undraw_docusaurus_react.svg
+-rwxr-xr-x   0        0        0    11784 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/undraw_docusaurus_tree.svg
+-rwxr-xr-x   0        0        0   146113 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/valid_port_types.png
+-rwxr-xr-x   0        0        0      499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/wordmark_white.svg
+-rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/.eslintrc
+-rwxr-xr-x   0        0        0   105919 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/README.md
+-rwxr-xr-x   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/package.json
+-rwxr-xr-x   0        0        0   913821 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/yarn.lock
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/public/index.html
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/public/manifest.json
+-rwxr-xr-x   0        0        0    18960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/App.js
+-rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/index.css
+-rwxr-xr-x   0        0        0     1503 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/index.js
+-rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/TestRoutes/TestEditor.js
+-rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/TestRoutes/nodes.js
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/components/Checkbox.js
+-rwxr-xr-x   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/components/FloatingNavigation.js
+-rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/components/Header.js
+-rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/components/LogicEditor.js
+-rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/components/Modal.js
+-rwxr-xr-x   0        0        0     2000 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/components/OptionsEditor.js
+-rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/icons/BoxIcon.js
+-rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/icons/FormIcon.js
+-rwxr-xr-x   0        0        0     3783 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/icons/GearIcon.js
+-rwxr-xr-x   0        0        0     6066 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Attributes.js
+-rwxr-xr-x   0        0        0     2886 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Body.js
+-rwxr-xr-x   0        0        0     2020 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Field.js
+-rwxr-xr-x   0        0        0    10739 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Form.css
+-rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Form.js
+-rwxr-xr-x   0        0        0     1834 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/InputTypes.js
+-rwxr-xr-x   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/NodeTypes.js
+-rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/PreviewField.js
+-rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Sidebar.js
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/defaultNodes.js
+-rwxr-xr-x   0        0        0      815 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/designerReducer.js
+-rwxr-xr-x   0        0        0     1261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/fieldTypes.js
+-rwxr-xr-x   0        0        0     1560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/fieldsReducer.js
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/formHandler.js
+-rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/previewFieldsReducer.js
+-rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/resolveLogic.js
+-rwxr-xr-x   0        0        0     8710 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/wizardLogic/logicTypes.js
+-rwxr-xr-x   0        0        0     1910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Forms/Forms.css
+-rwxr-xr-x   0        0        0     1854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Forms/Forms.js
+-rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Records/Records.css
+-rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Records/Records.js
+-rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/.eslintrc
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/Cache.js
+-rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/RootEngine.js
+-rwxr-xr-x   0        0        0     2060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/commentsReducer.js
+-rwxr-xr-x   0        0        0     6241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/connectionCalculator.js
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/constants.js
+-rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/context.js
+-rwxr-xr-x   0        0        0     9649 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/index.js
+-rwxr-xr-x   0        0        0    14282 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/nodesReducer.js
+-rwxr-xr-x   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/stageReducer.js
+-rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/styles.css
+-rwxr-xr-x   0        0        0     1191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/toastsReducer.js
+-rwxr-xr-x   0        0        0     8905 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/typeBuilders.js
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/utilities.js
+-rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Checkbox/Checkbox.css
+-rwxr-xr-x   0        0        0      651 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Checkbox/Checkbox.js
+-rwxr-xr-x   0        0        0     1134 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/ColorPicker/ColorPicker.css
+-rwxr-xr-x   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/ColorPicker/ColorPicker.js
+-rwxr-xr-x   0        0        0     2159 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Comment/Comment.css
+-rwxr-xr-x   0        0        0     7028 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Comment/Comment.js
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Connection/Connection.css
+-rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Connection/Connection.js
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Connections/Connections.css
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Connections/Connections.js
+-rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/ContextMenu/ContextMenu.css
+-rwxr-xr-x   0        0        0     7071 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/ContextMenu/ContextMenu.js
+-rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Control/Control.css
+-rwxr-xr-x   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Control/Control.js
+-rwxr-xr-x   0        0        0     3751 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Draggable/Draggable.js
+-rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/IoPorts/IoPorts.css
+-rwxr-xr-x   0        0        0    12769 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/IoPorts/IoPorts.js
+-rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Node/Node.css
+-rwxr-xr-x   0        0        0     7392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Node/Node.js
+-rwxr-xr-x   0        0        0     2001 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Select/Select.css
+-rwxr-xr-x   0        0        0     3675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Select/Select.js
+-rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Stage/Stage.css
+-rwxr-xr-x   0        0        0     9421 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Stage/Stage.js
+-rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/TextInput/TextInput.css
+-rwxr-xr-x   0        0        0     3405 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/TextInput/TextInput.js
+-rwxr-xr-x   0        0        0     2223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Toaster/Toaster.css
+-rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Toaster/Toaster.js
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/hooks/usePrevious.js
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/img/grid.png
+-rwxr-xr-x   0        0        0     8912 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/tests/dynamic.test.js
+-rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/tests/nodes.js
+-rwxr-xr-x   0        0        0     1409 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/tests/ssr.test.js
+-rwxr-xr-x   0        0        0     1397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/tests/test.js
+-rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/__init__.py
+-rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/_version.py
+-rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/select.py
+-rwxr-xr-x   0        0        0     3962 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/utils.py
+-rwxr-xr-x   0        0        0     5572 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/package.json
+-rwxr-xr-x   0        0        0     6248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig
+-rwxr-xr-x   0        0        0     7391 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json
+-rwxr-xr-x   0        0        0     3987 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     6292 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    18679 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3638 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7685 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    11356 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1849 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4595 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    10308 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5078 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1183 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5424 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js
+-rwxr-xr-x   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     9725 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4055 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     9126 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js.LICENSE.txt
+-rwxr-xr-x   0        0        0  3246909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js
+-rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2846 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4006 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1927 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1892 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4030 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    17021 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2459 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2519 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7231 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1911 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     6491 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    32283 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    32835 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7177 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5600.cb8c4c5c969d7f385fe8.js
+-rwxr-xr-x   0        0        0     6820 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7177 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5794.4a7528c68458a721936d.js
+-rwxr-xr-x   0        0        0     1951 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    16144 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3065 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3470 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    11882 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2342 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    38168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5447 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2567 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3657 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3351 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3653 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    10379 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8109 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    73464 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf
+-rwxr-xr-x   0        0        0     3654 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js
+-rwxr-xr-x   0        0        0     8337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7938 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    22618 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js
+-rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    14242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2658 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3155 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0   216372 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8863.82c89f078a753cb91d3d.js
+-rwxr-xr-x   0        0        0     2899 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1501 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4332 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3017 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js
+-rwxr-xr-x   0        0        0     4099 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js
+-rwxr-xr-x   0        0        0     5873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    13543 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    13292 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/remoteEntry.80729a1327f495afa265.js
+-rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/style.js
+-rwxr-xr-x   0        0        0     9868 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json
+-rwxr-xr-x   0        0        0     7391 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/schema/plugin.json
+-rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/ReRunIcon.tsx
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/arrownIcon.tsx
+-rwxr-xr-x   0        0        0     1455 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/clearIcon.tsx
+-rwxr-xr-x   0        0        0      954 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/deleteIcon.tsx
+-rwxr-xr-x   0        0        0     1505 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/exportIcon.tsx
+-rwxr-xr-x   0        0        0     1310 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/factory.ts
+-rwxr-xr-x   0        0        0    41954 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/flumeConfig.tsx
+-rwxr-xr-x   0        0        0     7454 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/imageViewer.tsx
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/index.ts
+-rwxr-xr-x   0        0        0     2268 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/lockIcon.tsx
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/model.ts
+-rwxr-xr-x   0        0        0      807 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/newIcon.tsx
+-rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/runIcon.tsx
+-rwxr-xr-x   0        0        0     2544 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/utils.tsx
+-rwxr-xr-x   0        0        0   176897 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/widget.tsx
+-rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/yesIcon.tsx
+-rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/style/base.css
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/style/index.css
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/style/index.js
+-rwxr-xr-x   0        0        0   254494 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/test_ext/1.jpeg
+-rwxr-xr-x   0        0        0   153675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/test_ext/2.jpeg
+-rwxr-xr-x   0        0        0     2162 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/test_ext/main.ipynb
+-rwxr-xr-x   0        0        0   546624 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/test_ext/testlib.ipynb
+-rwxr-xr-x   0        0        0     1586 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/.gitignore
+-rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/LICENSE
+-rwxr-xr-x   0        0        0     2557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/README.md
+-rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/PKG-INFO
```

### Comparing `jupyterlab_nodeeditor-1.0.5/RELEASE.md` & `jupyterlab_nodeeditor-1.0.6/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/package.json` & `jupyterlab_nodeeditor-1.0.6/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.0.6'"}*

```diff
@@ -175,9 +175,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.5"
+    "version": "1.0.6"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.5/tsconfig.json` & `jupyterlab_nodeeditor-1.0.6/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/yarn.lock` & `jupyterlab_nodeeditor-1.0.6/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/_temp_extension/.gitignore` & `jupyterlab_nodeeditor-1.0.6/_temp_extension/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/_temp_extension/LICENSE` & `jupyterlab_nodeeditor-1.0.6/_temp_extension/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/_temp_extension/README.md` & `jupyterlab_nodeeditor-1.0.6/_temp_extension/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/_temp_extension/RELEASE.md` & `jupyterlab_nodeeditor-1.0.6/_temp_extension/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/_temp_extension/package.json` & `jupyterlab_nodeeditor-1.0.6/_temp_extension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/_temp_extension/pyproject.toml` & `jupyterlab_nodeeditor-1.0.6/_temp_extension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/_temp_extension/tsconfig.json` & `jupyterlab_nodeeditor-1.0.6/_temp_extension/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/_temp_extension/jupyterlab_nodeeditor/__init__.py` & `jupyterlab_nodeeditor-1.0.6/_temp_extension/jupyterlab_nodeeditor/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/_temp_extension/src/index.ts` & `jupyterlab_nodeeditor-1.0.6/_temp_extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/CODE_OF_CONDUCT.md` & `jupyterlab_nodeeditor-1.0.6/flume/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/LICENSE` & `jupyterlab_nodeeditor-1.0.6/flume/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/README.md` & `jupyterlab_nodeeditor-1.0.6/flume/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/logo.ai` & `jupyterlab_nodeeditor-1.0.6/flume/logo.ai`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/logo.png` & `jupyterlab_nodeeditor-1.0.6/flume/logo.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/logo.svg` & `jupyterlab_nodeeditor-1.0.6/flume/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/package.json` & `jupyterlab_nodeeditor-1.0.6/flume/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/rollup.config.js` & `jupyterlab_nodeeditor-1.0.6/flume/rollup.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/yarn.lock` & `jupyterlab_nodeeditor-1.0.6/flume/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/cypress/integration/NodeEditorSpec.js` & `jupyterlab_nodeeditor-1.0.6/flume/cypress/integration/NodeEditorSpec.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/cypress/plugins/index.js` & `jupyterlab_nodeeditor-1.0.6/flume/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/cypress/support/commands.js` & `jupyterlab_nodeeditor-1.0.6/flume/cypress/support/commands.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/cypress/support/index.js` & `jupyterlab_nodeeditor-1.0.6/flume/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/README.md` & `jupyterlab_nodeeditor-1.0.6/flume/docs/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docusaurus.config.js` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/package.json` & `jupyterlab_nodeeditor-1.0.6/flume/docs/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/yarn.lock` & `jupyterlab_nodeeditor-1.0.6/flume/docs/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/components/AnatomyExample.js` & `jupyterlab_nodeeditor-1.0.6/flume/docs/components/AnatomyExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/components/Colors.js` & `jupyterlab_nodeeditor-1.0.6/flume/docs/components/Colors.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/components/ControlExamples.js` & `jupyterlab_nodeeditor-1.0.6/flume/docs/components/ControlExamples.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/components/DynamicNodesExamples.js` & `jupyterlab_nodeeditor-1.0.6/flume/docs/components/DynamicNodesExamples.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/components/DynamicThemingExample.js` & `jupyterlab_nodeeditor-1.0.6/flume/docs/components/DynamicThemingExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/components/GettingStartedExample.js` & `jupyterlab_nodeeditor-1.0.6/flume/docs/components/GettingStartedExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/NodeEditor.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/NodeEditor.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/RootEngine.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/RootEngine.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/anatomy.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/anatomy.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/basic-config.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/basic-config.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/colors.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/colors.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/comments.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/comments.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/controls.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/controls.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/defining-nodes.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/defining-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/doc1.md` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/doc1.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/doc3.md` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/doc3.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/dynamic-nodes.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/dynamic-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/faq.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/faq.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/flume-config.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/flume-config.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/logic-nodes.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/logic-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/mdx.md` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/mdx.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/node-editor.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/node-editor.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/overview.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/overview.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/quick-start.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/quick-start.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/root-engine.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/root-engine.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/root-node.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/root-node.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/running-logic.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/running-logic.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/saving-nodes.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/saving-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/theming.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/theming.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/type-safety.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/type-safety.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/using-with-react.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/using-with-react.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/docs/using-without-react.mdx` & `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/using-without-react.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/src/exampleFlumeConfig.js` & `jupyterlab_nodeeditor-1.0.6/flume/docs/src/exampleFlumeConfig.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/src/components/TypeSafe.js` & `jupyterlab_nodeeditor-1.0.6/flume/docs/src/components/TypeSafe.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/src/css/custom.css` & `jupyterlab_nodeeditor-1.0.6/flume/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/src/pages/index.js` & `jupyterlab_nodeeditor-1.0.6/flume/docs/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/src/pages/styles.module.css` & `jupyterlab_nodeeditor-1.0.6/flume/docs/src/pages/styles.module.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/60fps.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/60fps.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/android-chrome-192x192.png` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/android-chrome-512x512.png` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/apple-touch-icon.png` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/controls.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/controls.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/example_editors.png` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/example_editors.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/favicon-32x32.png` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/favicon.ico` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/fb-img.png` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/fb-img.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/flume-short-web.mp4` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/flume-short-web.mp4`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/friends-graph.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/friends-graph.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/hero-nodes.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/hero-nodes.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/logo-dark.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/logo.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/netlify.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/netlify.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/performance-tile.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/performance-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/react-tile.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/react-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/size-tile.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/size-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/theme-tile.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/theme-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/theme.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/theme.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/type-safe-node.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/type-safe-node.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/type-safe-nodes.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/type-safe-nodes.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/undraw_docusaurus_mountain.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/undraw_docusaurus_react.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/undraw_docusaurus_tree.svg` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/docs/static/img/valid_port_types.png` & `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/valid_port_types.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/README.md` & `jupyterlab_nodeeditor-1.0.6/flume/example/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/package.json` & `jupyterlab_nodeeditor-1.0.6/flume/example/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/yarn.lock` & `jupyterlab_nodeeditor-1.0.6/flume/example/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/public/index.html` & `jupyterlab_nodeeditor-1.0.6/flume/example/public/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/App.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/App.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/index.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/TestRoutes/TestEditor.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/TestRoutes/TestEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/TestRoutes/nodes.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/TestRoutes/nodes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/components/Checkbox.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/components/Checkbox.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/components/FloatingNavigation.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/components/FloatingNavigation.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/components/LogicEditor.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/components/LogicEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/components/OptionsEditor.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/components/OptionsEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/icons/BoxIcon.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/icons/BoxIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/icons/FormIcon.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/icons/FormIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/icons/GearIcon.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/icons/GearIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/Attributes.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Attributes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/Body.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Body.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/Field.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Field.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/Form.css` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Form.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/Form.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Form.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/InputTypes.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/InputTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/NodeTypes.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/NodeTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/PreviewField.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/PreviewField.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/Sidebar.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Sidebar.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/designerReducer.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/designerReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/fieldTypes.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/fieldTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/fieldsReducer.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/fieldsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/previewFieldsReducer.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/previewFieldsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/resolveLogic.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/resolveLogic.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Form/wizardLogic/logicTypes.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/wizardLogic/logicTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Forms/Forms.css` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Forms/Forms.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Forms/Forms.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Forms/Forms.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Records/Records.css` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Records/Records.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/example/src/pages/Records/Records.js` & `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Records/Records.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/RootEngine.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/RootEngine.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/commentsReducer.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/commentsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/connectionCalculator.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/connectionCalculator.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/context.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/context.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/index.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/nodesReducer.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/nodesReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/toastsReducer.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/toastsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/typeBuilders.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/typeBuilders.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/utilities.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/utilities.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/Checkbox/Checkbox.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/Checkbox/Checkbox.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/ColorPicker/ColorPicker.css` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/ColorPicker/ColorPicker.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/ColorPicker/ColorPicker.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/ColorPicker/ColorPicker.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/Comment/Comment.css` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/Comment/Comment.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/Comment/Comment.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/Comment/Comment.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/Connection/Connection.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/Connection/Connection.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/ContextMenu/ContextMenu.css` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/ContextMenu/ContextMenu.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/ContextMenu/ContextMenu.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/ContextMenu/ContextMenu.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/Control/Control.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/Control/Control.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/Draggable/Draggable.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/Draggable/Draggable.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/IoPorts/IoPorts.css` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/IoPorts/IoPorts.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/IoPorts/IoPorts.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/IoPorts/IoPorts.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/Node/Node.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/Node/Node.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/Select/Select.css` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/Select/Select.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/Select/Select.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/Select/Select.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/Stage/Stage.css` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/Stage/Stage.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/Stage/Stage.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/Stage/Stage.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/TextInput/TextInput.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/TextInput/TextInput.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/Toaster/Toaster.css` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/Toaster/Toaster.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/components/Toaster/Toaster.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/components/Toaster/Toaster.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/tests/dynamic.test.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/tests/dynamic.test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/tests/nodes.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/tests/nodes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/tests/ssr.test.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/tests/ssr.test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/flume/src/tests/test.js` & `jupyterlab_nodeeditor-1.0.6/flume/src/tests/test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/select.py` & `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/select.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/utils.py` & `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import json
-# import re
-# import import_ipynb
-# import sys
-# import os
-
+import io
+import base64
 
 def get_instance_info(v):
     from .select import select, mselect
     t = type(v)
     d = None
     if isinstance(v, int) \
             or isinstance(v, float) \
@@ -18,30 +15,77 @@
             or isinstance(v, mselect):
         d = v.get_show_options()
 
     return json.dumps({"type": str(t), "value": d})
 
 
 def get_urls(urls):
+    # 如果urls是字符串
     if isinstance(urls, str):
         try:
             ret = json.loads(urls)
             if not isinstance(ret, list):
                 raise TypeError('Expecting a list')
             return json.dumps(ret)
         except ValueError as e:
             return json.dumps([urls])
         except TypeError as e:
             raise TypeError('Invalid input type')
-    elif isinstance(urls, list):
+    
+    # 如果urls是列表
+    if isinstance(urls, list):
         return json.dumps(urls)
-    elif isinstance(urls, dict):
+    
+    # 如果urls是字典
+    if isinstance(urls, dict):
         return json.dumps(list(urls.values()))
-    else:
-        raise TypeError('Invalid input type')
+    
+    # 如果urls是cv2的numpy.ndarry
+    try:
+        import cv2
+        from numpy import ndarray
+        if isinstance(urls, ndarray):
+            img_bytes = cv2.imencode('.png', urls)[1].tobytes()
+            img_b64 = base64.b64encode(img_bytes).decode()
+            img_url = "data:image/png;base64," + img_b64
+            return json.dumps([img_url])
+    except:
+        pass
+    
+    # 如果urls是matplotlib的画布
+    try:
+        from matplotlib.figure import Figure
+        from matplotlib.image import AxesImage
+        import matplotlib.pyplot as plt
+        if urls == plt:
+            fig = urls
+        if isinstance(urls, Figure):
+            fig = urls
+        if isinstance(urls, AxesImage) :
+            fig = urls.get_figure()
+        buffer = io.BytesIO()
+        fig.savefig(buffer, format='png')
+        url = 'data:image/png;base64,' + \
+            base64.b64encode(buffer.getvalue()).decode()
+        return json.dumps([url])
+    except:
+        pass
+
+    # 如果urls是PILLOW的Image
+    try:
+        from PIL import Image
+        if isinstance(urls, Image):
+            buffer = io.BytesIO()
+            urls.save(buffer, format="PNG")
+            url = 'data:image/png;base64,' + \
+                base64.b64encode(buffer.getvalue()).decode()
+            return json.dumps([url])
+    except:
+        pass
+    raise TypeError('Invalid input type')
 
 
 def get_boolean_value(v):
     if v:
         return True
     else:
         return False
@@ -98,8 +142,8 @@
 # def loadNotebook(path):
 #     importNotebook(path)
 #     nodeTypes = importNodeTypesFromNotebook(path)
 
 
 # if __name__ == "__main__":
 #     path = "test_ext/testlib.ipynb"
-#     loadNotebook(path)
+#     loadNotebook(path)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/package.json` & `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.80729a1327f495afa265.js'}}",*

 * * "'version'": "'1.0.6'"}*

```diff
@@ -107,15 +107,15 @@
         "schema/**/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/github_username/jupyterlab_nodeeditor",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.daeae06c6d772e670e7b.js",
+            "load": "static/remoteEntry.80729a1327f495afa265.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_nodeeditor/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -180,9 +180,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.4"
+    "version": "1.0.6"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig` & `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.0.6'"}*

```diff
@@ -175,9 +175,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.4"
+    "version": "1.0.6"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json` & `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9640858426704014%*

 * *Differences: {"'jupyter.lab.menus'": "{'main': {0: {'items': {21: {'command': 'nd-run-start-node'}, delete: "*

 * *                        '[33, 30, 29, 28, 27, 26, 25, 24, 23, 22, 12, 11, 10]}}}}',*

 * * "'jupyter.lab.shortcuts'": "{5: {'selector': "*

 * *                            "'[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]'}, "*

 * *                            "6: {'selector': "*

 * *                            "'[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]'}, "*

 * *     […]*

```diff
@@ -33,23 +33,14 @@
                     {
                         "command": "nd-redo"
                     },
                     {
                         "command": "nd-reset-viewport"
                     },
                     {
-                        "command": "nd-toggle-output-area"
-                    },
-                    {
-                        "command": "nd-clear-output-area"
-                    },
-                    {
-                        "command": "nd-open-code-editor"
-                    },
-                    {
                         "command": "nd-kernel-interrupt"
                     },
                     {
                         "command": "nd-kernel-restart"
                     },
                     {
                         "command": "nd-kernel-change"
@@ -69,51 +60,21 @@
                     {
                         "command": "nd-focus-to-selected-nodes"
                     },
                     {
                         "command": "nd-close-image-viewer"
                     },
                     {
-                        "command": "nd-run-cucrrent-cell"
-                    },
-                    {
-                        "command": "nd-insert-cell"
-                    },
-                    {
-                        "command": "nd-delete-cell"
-                    },
-                    {
-                        "command": "nd-cell-undo"
-                    },
-                    {
-                        "command": "nd-cell-redo"
-                    },
-                    {
-                        "command": "nd-edit-pre-cell"
-                    },
-                    {
-                        "command": "nd-edit-next-cell"
-                    },
-                    {
-                        "command": "nd-cell-up"
-                    },
-                    {
-                        "command": "nd-cell-down"
-                    },
-                    {
                         "command": "nd-set-as-default"
                     },
                     {
                         "command": "nd-open-comment-color-picker"
                     },
                     {
-                        "command": "nd-combine-selected-nodes"
-                    },
-                    {
-                        "command": "nd-separate-selected-node"
+                        "command": "nd-run-start-node"
                     }
                 ],
                 "label": "\u8282\u70b9\u7f16\u8f91\u5668",
                 "rank": 100
             }
         ]
     },
@@ -154,22 +115,22 @@
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-run-all-cells",
             "keys": [
                 "Shift R"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-clear-run-cache",
             "keys": [
                 "Shift C"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-undo",
             "keys": [
                 "Accel Z"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
@@ -185,35 +146,14 @@
             "command": "nd-reset-viewport",
             "keys": [
                 "G"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
-            "command": "nd-toggle-output-area",
-            "keys": [
-                "Accel E"
-            ],
-            "selector": "[data-show-image-viewer=false]"
-        },
-        {
-            "command": "nd-clear-output-area",
-            "keys": [
-                "Accel L"
-            ],
-            "selector": "[data-show-image-viewer=false]"
-        },
-        {
-            "command": "nd-open-code-editor",
-            "keys": [
-                "E"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
-        },
-        {
             "command": "nd-kernel-interrupt",
             "keys": [
                 "Accel I"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
         },
         {
@@ -262,101 +202,31 @@
             "command": "nd-close-image-viewer",
             "keys": [
                 "Escape"
             ],
             "selector": "[data-show-image-viewer=true][data-show-code-editor=false]"
         },
         {
-            "command": "nd-run-cucrrent-cell",
-            "keys": [
-                "Accel Enter"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-insert-cell",
-            "keys": [
-                "Accel I"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-delete-cell",
-            "keys": [
-                "Accel Delete"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-cell-undo",
-            "keys": [
-                "Alt Shift Z"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-cell-redo",
-            "keys": [
-                "Alt Shift Y"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-edit-pre-cell",
-            "keys": [
-                "Alt ArrowUp"
-            ],
-            "selector": "[data-show-image-viewer=false][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-edit-next-cell",
-            "keys": [
-                "Alt ArrowDown"
-            ],
-            "selector": "[data-show-image-viewer=false][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-cell-up",
-            "keys": [
-                "Shift ArrowUp"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-cell-down",
-            "keys": [
-                "Shift ArrowDown"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
             "command": "nd-set-as-default",
             "keys": [
                 "Alt Shift D"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-open-comment-color-picker",
             "keys": [
                 "C"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
-            "command": "nd-combine-selected-nodes",
+            "command": "nd-run-start-node",
             "keys": [
-                "B"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
-        },
-        {
-            "command": "nd-separate-selected-node",
-            "keys": [
-                "Shift B"
+                "Accel Enter"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
         }
     ],
     "title": "\u8282\u70b9\u7f16\u8f91\u5668",
     "type": "object"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.5/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf` & `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/schema/plugin.json` & `jupyterlab_nodeeditor-1.0.6/schema/plugin.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9640858426704014%*

 * *Differences: {"'jupyter.lab.menus'": "{'main': {0: {'items': {21: {'command': 'nd-run-start-node'}, delete: "*

 * *                        '[33, 30, 29, 28, 27, 26, 25, 24, 23, 22, 12, 11, 10]}}}}',*

 * * "'jupyter.lab.shortcuts'": "{5: {'selector': "*

 * *                            "'[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]'}, "*

 * *                            "6: {'selector': "*

 * *                            "'[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]'}, "*

 * *     […]*

```diff
@@ -33,23 +33,14 @@
                     {
                         "command": "nd-redo"
                     },
                     {
                         "command": "nd-reset-viewport"
                     },
                     {
-                        "command": "nd-toggle-output-area"
-                    },
-                    {
-                        "command": "nd-clear-output-area"
-                    },
-                    {
-                        "command": "nd-open-code-editor"
-                    },
-                    {
                         "command": "nd-kernel-interrupt"
                     },
                     {
                         "command": "nd-kernel-restart"
                     },
                     {
                         "command": "nd-kernel-change"
@@ -69,51 +60,21 @@
                     {
                         "command": "nd-focus-to-selected-nodes"
                     },
                     {
                         "command": "nd-close-image-viewer"
                     },
                     {
-                        "command": "nd-run-cucrrent-cell"
-                    },
-                    {
-                        "command": "nd-insert-cell"
-                    },
-                    {
-                        "command": "nd-delete-cell"
-                    },
-                    {
-                        "command": "nd-cell-undo"
-                    },
-                    {
-                        "command": "nd-cell-redo"
-                    },
-                    {
-                        "command": "nd-edit-pre-cell"
-                    },
-                    {
-                        "command": "nd-edit-next-cell"
-                    },
-                    {
-                        "command": "nd-cell-up"
-                    },
-                    {
-                        "command": "nd-cell-down"
-                    },
-                    {
                         "command": "nd-set-as-default"
                     },
                     {
                         "command": "nd-open-comment-color-picker"
                     },
                     {
-                        "command": "nd-combine-selected-nodes"
-                    },
-                    {
-                        "command": "nd-separate-selected-node"
+                        "command": "nd-run-start-node"
                     }
                 ],
                 "label": "\u8282\u70b9\u7f16\u8f91\u5668",
                 "rank": 100
             }
         ]
     },
@@ -154,22 +115,22 @@
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-run-all-cells",
             "keys": [
                 "Shift R"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-clear-run-cache",
             "keys": [
                 "Shift C"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-undo",
             "keys": [
                 "Accel Z"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
@@ -185,35 +146,14 @@
             "command": "nd-reset-viewport",
             "keys": [
                 "G"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
-            "command": "nd-toggle-output-area",
-            "keys": [
-                "Accel E"
-            ],
-            "selector": "[data-show-image-viewer=false]"
-        },
-        {
-            "command": "nd-clear-output-area",
-            "keys": [
-                "Accel L"
-            ],
-            "selector": "[data-show-image-viewer=false]"
-        },
-        {
-            "command": "nd-open-code-editor",
-            "keys": [
-                "E"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
-        },
-        {
             "command": "nd-kernel-interrupt",
             "keys": [
                 "Accel I"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
         },
         {
@@ -262,101 +202,31 @@
             "command": "nd-close-image-viewer",
             "keys": [
                 "Escape"
             ],
             "selector": "[data-show-image-viewer=true][data-show-code-editor=false]"
         },
         {
-            "command": "nd-run-cucrrent-cell",
-            "keys": [
-                "Accel Enter"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-insert-cell",
-            "keys": [
-                "Accel I"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-delete-cell",
-            "keys": [
-                "Accel Delete"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-cell-undo",
-            "keys": [
-                "Alt Shift Z"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-cell-redo",
-            "keys": [
-                "Alt Shift Y"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-edit-pre-cell",
-            "keys": [
-                "Alt ArrowUp"
-            ],
-            "selector": "[data-show-image-viewer=false][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-edit-next-cell",
-            "keys": [
-                "Alt ArrowDown"
-            ],
-            "selector": "[data-show-image-viewer=false][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-cell-up",
-            "keys": [
-                "Shift ArrowUp"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
-            "command": "nd-cell-down",
-            "keys": [
-                "Shift ArrowDown"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=true][data-use-diff-editor=false]"
-        },
-        {
             "command": "nd-set-as-default",
             "keys": [
                 "Alt Shift D"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
             "command": "nd-open-comment-color-picker",
             "keys": [
                 "C"
             ],
             "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
         },
         {
-            "command": "nd-combine-selected-nodes",
+            "command": "nd-run-start-node",
             "keys": [
-                "B"
-            ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
-        },
-        {
-            "command": "nd-separate-selected-node",
-            "keys": [
-                "Shift B"
+                "Accel Enter"
             ],
-            "selector": "[data-show-image-viewer=false][data-show-code-editor=false][data-inputing=false]"
+            "selector": "[data-show-image-viewer=false][data-show-code-editor=false]"
         }
     ],
     "title": "\u8282\u70b9\u7f16\u8f91\u5668",
     "type": "object"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.5/src/ReRunIcon.tsx` & `jupyterlab_nodeeditor-1.0.6/src/ReRunIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/src/arrownIcon.tsx` & `jupyterlab_nodeeditor-1.0.6/src/arrownIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/src/clearIcon.tsx` & `jupyterlab_nodeeditor-1.0.6/src/clearIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/src/deleteIcon.tsx` & `jupyterlab_nodeeditor-1.0.6/src/deleteIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/src/exportIcon.tsx` & `jupyterlab_nodeeditor-1.0.6/src/exportIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/src/factory.ts` & `jupyterlab_nodeeditor-1.0.6/src/factory.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/src/flumeConfig.tsx` & `jupyterlab_nodeeditor-1.0.6/src/flumeConfig.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import { FlumeConfig, Colors, Controls, Node } from '../flume'
 import React, { useState, useCallback } from 'react'
 import { NodeEditorWidget } from './widget'
 import { buildNodeWidth } from './utils'
+import * as monaco from 'monaco-editor';
 
 export let headerFontsize = 16
 export let nodeMinWidth = 200
 export let nodeMaxWidth = 1000
 
 let image_urls_functions: any = {}
 export function setImageUrls(node_id, urls) {
@@ -302,15 +303,17 @@
             type: "any",
             name: "any",
             label: "任何类型",
             color: Colors.grey,
             acceptTypes: ["any",
                 "string", "number",
                 "boolean", "image",
-                "select", "mselect"],
+                "select", "mselect",
+                "video", "tuple", "dict"
+            ],
             controls: [
                 Controls.text({
                     name: "any",
                     label: "默认值",
                     defaultValue: "None"
                 })
             ]
@@ -824,19 +827,82 @@
                         {
                             "value": "is",
                             "label": "身份运算符(is)"
                         },
                         {
                             "value": "is not",
                             "label": "非身份运算符(is not)"
+                        },
+                        {
+                            "value": "[]",
+                            "label": "取值[key]"
                         }
                     ]
                 }),
             ]
         })
+        .addPortType({
+            type: "code_editor",
+            name: "code_editor",
+            label: "code_editor",
+            color: Colors.dict,
+            acceptTypes: [],
+            hidePort: true,
+            controls: [
+                Controls.custom({
+                    name: "code_editor",
+                    label: "",
+                    defaultValue: {},
+                    render: (data: {},
+                        onChange,
+                        executionContext: NodeEditorWidget,
+                        triggerRecalculation,
+                        portProps, allData) => {
+                        const editorContainerRef = React.useRef(null)
+                        const editorRef = React.useRef<null | monaco.editor.IStandaloneCodeEditor>(null)
+                        const [showEditor, setShowEditor] = React.useState(false)
+                        React.useEffect(() => {
+                            if (showEditor) {
+                                editorRef.current = monaco.editor.create(
+                                    editorContainerRef.current as unknown as HTMLElement, {
+                                    theme: "vs-dark",
+                                    language: "python",
+                                })
+                                let editor = editorRef.current as monaco.editor.IStandaloneCodeEditor
+                                editor.layout()
+                                editor.onDidFocusEditorWidget(e => {
+                                    executionContext.setInputing(true)
+                                })
+                                editor.onDidBlurEditorWidget(e => {
+                                    executionContext.setInputing(false)
+                                })
+                            }
+                        }, [showEditor])
+                        return (
+                            <div style={{
+                                width: "100%"
+                            }}>
+                                <button onClick={e => {
+                                    setShowEditor(!showEditor)
+                                }}>{showEditor ? '完成' : '编辑'}</button>
+                                {
+                                    showEditor && <div ref={editorContainerRef}
+                                        style={{
+                                            width: "100%",
+                                            height: "400px"
+                                        }}
+                                    ></div>
+                                }
+
+                            </div>
+                        )
+                    }
+                }),
+            ]
+        })
         .addNodeType({
             type: "image",
             label: "图片显示(show image)",
             description: "图片显示(show image)",
             initialWidth: 250,
             inputs: ports => [
                 get_port_func("control")(ports),
@@ -976,18 +1042,18 @@
             ],
             outputs: common_out,
         })
         .addNodeType({
             type: "string",
             label: "文本/字符串(string)",
             description: "文本/字符串(string)",
-            initialWidth: buildNodeWidth("string", headerFontsize, nodeMinWidth, nodeMaxWidth),
+            initialWidth: 500,
             inputs: ports => [
                 get_port_func("control")(ports),
-                get_port_func("string")(ports, "值1", "value", 0)
+                get_port_func("string")(ports, " ", "value", 0)
             ],
             outputs: common_out,
         })
         .addNodeType({
             type: "bool",
             label: "布尔(bool)(真/假)",
             description: "布尔(bool)(真/假)",
@@ -1033,10 +1099,44 @@
                 get_port_func("control")(ports),
                 ports.operator(),
                 get_port_func("any")(ports, "参数1", "value1", "None"),
                 get_port_func("any")(ports, "参数2", "value2", "None"),
             ],
             outputs: common_out,
         })
+        .addNodeType({
+            type: "setvar",
+            label: "设置变量(setvar)",
+            description: "设置变量(setvar)",
+            initialWidth: buildNodeWidth("设置变量(setvar)", headerFontsize, nodeMinWidth, nodeMaxWidth),
+            inputs: ports => [
+                get_port_func("control")(ports),
+                get_port_func("any")(ports, "变量名", "name", ""),
+                get_port_func("any")(ports, "值", "value", "None"),
+            ],
+            outputs: common_out,
+        })
+        .addNodeType({
+            type: "start",
+            label: "开始(start)",
+            description: "开始(start)",
+            initialWidth: buildNodeWidth("开始(start)", headerFontsize, nodeMinWidth, nodeMaxWidth),
+            inputs: ports => [
+                get_port_func("control")(ports),
+            ],
+            outputs: [],
+        })
+        // .addNodeType({
+        //     type: "function",
+        //     label: "函数(function)",
+        //     description: "函数(function)",
+        //     initialWidth: 500,
+        //     inputs: ports => [
+        //         get_port_func("control")(ports),
+        //         ports.code_editor()
+
+        //     ],
+        //     outputs: [],
+        // })
 
     return config
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.5/src/imageViewer.tsx` & `jupyterlab_nodeeditor-1.0.6/src/imageViewer.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/src/index.ts` & `jupyterlab_nodeeditor-1.0.6/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/src/lockIcon.tsx` & `jupyterlab_nodeeditor-1.0.6/src/lockIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/src/newIcon.tsx` & `jupyterlab_nodeeditor-1.0.6/src/newIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/src/runIcon.tsx` & `jupyterlab_nodeeditor-1.0.6/src/runIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/src/utils.tsx` & `jupyterlab_nodeeditor-1.0.6/src/utils.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -72,8 +72,13 @@
 export function rectsIntersect(rect1, rect2) {
     let duijiao1 = getDuiJiaoZuoBiao(rect1)
     let duijiao2 = getDuiJiaoZuoBiao(rect2)
     return duijiao1.x1 < duijiao2.x2
         && duijiao1.x2 > duijiao2.x1
         && duijiao1.y1 < duijiao2.y2
         && duijiao1.y2 > duijiao2.y1
+}
+
+export function removeAnsi(text: string): string {
+    const ansiRegex = /[\u001B\u009B][[()#;?]*(?:[0-9]{1,4}(?:;[0-9]{0,4})*)?[0-9A-ORZcf-nqry=><]/g;
+    return text.replace(ansiRegex, '');
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.5/src/widget.tsx` & `jupyterlab_nodeeditor-1.0.6/src/widget.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 } from "./flumeConfig"
 import { v4 as uuidv4 } from "uuid"
 import {
     buildNodeWidth,
     cloneDeep,
     nextFrame,
     findAll,
-    rectsIntersect
+    rectsIntersect,
+    removeAnsi
 } from './utils'
 import RunIcon from "./runIcon";
 import DeleteIcon from "./deleteIcon";
 import ImageViewer from "./imageViewer";
 import ReRunIcon from "./ReRunIcon";
 import LockIcon from "./lockIcon";
 import ArrownIcon from "./arrownIcon";
@@ -177,14 +178,20 @@
 
         let that = this
         this._context.model.sharedModel.changed.connect((sender, change) => {
             this.onContentChanged(sender, change)
         });
 
         this._context.sessionContext.ready.then(async (value) => { await that.onReady() })
+        this._context.sessionContext.session?.kernelChanged.connect(async slot => {
+            if (!await this._initPython()) {
+                return false
+            }
+        })
+
         this._context.saveState.connect(() => { that.onSaveState() })
         this.editorConfig = createConfig()
 
         // 创建输出框
         const rendermime = new RenderMimeRegistry({
             initialFactories: standardRendererFactories
         });
@@ -217,14 +224,27 @@
         this.node.addEventListener("command", async e => {
             await this._onCommand(e as CustomEvent)
         })
         this.node.addEventListener("resize", e => {
             this._onResize()
         })
 
+        this.node.addEventListener("wheel", e => {
+            if (!e.ctrlKey) {
+                return
+            }
+            e.preventDefault()
+            e.stopPropagation()
+            if (e.deltaY > 0) {
+                this._editNextCell()
+            } else {
+                this._editPreCell()
+            }
+        })
+
         // 注册size监测
         this._sizeCache = {
             width: this.node.clientWidth,
             height: this.node.clientHeight
         }
         setInterval(() => {
             this.onInterval()
@@ -927,14 +947,22 @@
 
     async onReady() {
         // this._checkSessionAndKernel(null)首先要检测，必须要有内核
         if (!await this._checkSessionAndKernel(null)) {
             return false
         }
 
+        this._context.sessionContext.session?.kernel?.statusChanged.connect((conn, status) => {
+            switch (status) {
+                case "restarting": {
+                    this._initPython()
+                } break
+            }
+        })
+
         // this._initPython() 必须在 this._loadNodesFromAllCell()之前
         if (!await this._initPython()) {
             return false
         }
 
         // 加载所有的保存的类型
         let options = this._loadNodesAsList()
@@ -986,35 +1014,30 @@
         this._needSaveNodes = false
         this.setCurNodeName("未命名")
         this._clearNodes()
         this._needSaveNodes = true
     }
 
     async onConnectToSpace(e, nodeId, portName) {
-        // let node = this._getNode(nodeId)
-        // if (!node) {
-        //     return
-        // }
-
-        // let outVarName = this._get_out_var_name(nodeId)
-        // switch (node.type) {
-        //     case "image":
-        //         if (portName == "curUrl") {
-        //             outVarName = `${outVarName}_cur`
-        //         }
-        //         break
-        //     default:
-        //         let ret = /instance@(get|set)@(.*)/g.exec(node.type)
-        //         if (ret) {
-        //             outVarName = ret[2]
-        //         }
-        //         break
-        // }
+        let node = this._getNode(nodeId)
+        if (!node) {
+            return
+        }
 
-        // this._setMenuOpen(`${outVarName}`)
+        let outVarName = this._getOutVarName(nodeId)
+        switch (node.type) {
+            default:
+                let ret = /instance@(get|set)@(.*)/g.exec(node.type)
+                if (ret) {
+                    outVarName = ret[2]
+                }
+                break
+        }
+
+        this._setMenuOpen(`${outVarName}`)
     }
 
     async runNode(id, clearCache = false) {
         this._interruptingKernel = false
         this._stopCreateNodeType = true
         let removeList = [id]
         let exceptIds: any = []
@@ -1187,17 +1210,17 @@
         }
 
         this._draggingSelectedNodes = false
     }
 
 
     async onStageDraggableMouseDown(e: MouseEvent) {
+        this.setInputing(false)
     }
 
-
     async onStageDraggableMouseUp(e: MouseEvent) {
         if (!this._stageDragging) {
             this.selectedNodes.clear()
             this.refreshNodeBoxShadow()
         }
         this._stageDragging = false
     }
@@ -1665,14 +1688,23 @@
 
     setNodes(id, data) {
         let allNodes = this.getAllNodes()
         allNodes[id] = data
         this.setAllNodes(allNodes)
     }
 
+    getDefaultNodesId() {
+        return this._context.model.getMetadata("default_nodes_id")
+    }
+
+    setDefaultNodesId(id) {
+        return this._context.model.setMetadata("default_nodes_id", id)
+    }
+
+
     async onContextMenuFilter(
         filter: string,
         options: any[] = [],
         setOptions,
         filterOptions,
         from
     ) {
@@ -1690,14 +1722,22 @@
         if (option.label.charAt(0) == ".") {
             this._loadNodes(option.data)
             return
         }
 
         let addNode = this.editorOptions["addNode"]
         if (addNode) {
+            if (option.node.type == "start") {
+                for (const node of Object.values(this.editorNodes)) {
+                    if ((node as any).type == "start") {
+                        showErrorMessage("错误", "只能有一个[开始[(start)]节点")
+                        return
+                    }
+                }
+            }
             addNode(option)
         }
     }
 
     async onMenuStateChange(menuOpen, hideFilter, from) {
         this._stopCreateNodeType = !menuOpen
         this._stopFilterCell = !menuOpen
@@ -1722,32 +1762,28 @@
 
         let matches = reply.content.metadata._jupyter_types_experimental as []
         for (let index = 0; index < matches.length; index++) {
             if (!this._loadingNodes && this._stopCreateNodeType) {
                 return ret
             }
             let node_types = await this.buildNodeTypeByCompleteMatch(matches[index], filter)
+            this._addNodeTypes(node_types)
             for (const node_type of node_types) {
                 ret.push(node_type)
                 if (options && setOptions && filterOptions) {
                     let has_opt = false
                     for (const opt of options) {
                         if (opt.value == node_type.type) {
                             has_opt = true
                             break
                         }
                     }
                     if (!has_opt) {
                         options.push(generateMenuOption(node_type))
                     }
-                    try {
-                        if (this.editorConfig[node_type.type])
-                            this.editorConfig.removeNodeType(node_type.type)
-                        this.editorConfig.addNodeType(node_type)
-                    } catch (error) { }
                     options = filterOptions(filter, options) as any[]
                     setOptions(options)
                 }
             }
         }
         return ret
     }
@@ -1813,85 +1849,184 @@
                 this._nodeTypes[node_type_name] = {
                     type: "function",
                     node_type_name,
                     in_ports,
                 }
             } break;
             case "module": { } break;
-            case "class": { } break;
+            case "class": {
+                let ret = await this._context.sessionContext.session?.kernel?.requestInspect({
+                    code: node_type_name,
+                    cursor_pos: node_type_name.length,
+                    detail_level: 1
+                })
+                if (ret && ret.content.status == "ok") {
+                    let content = ret.content.data['text/plain'] as string
+                    content = removeAnsi(content)
+                    let execRet = /Init\ssignature:(.*?)(\(.*\))/g.exec(content)
+                    if (execRet) {
+                        let in_ports: any[] = this._buildInputPortsFromSignature(execRet[2])
+                        // 2.构建nodeType
+                        node_types = this._buildCommonNodeTypes(node_type_name, in_ports, "class")
+                        // 3.记录下来
+                        this._nodeTypes[node_type_name] = {
+                            type: "class",
+                            node_type_name,
+                            in_ports,
+                        }
+                    }
+                }
+            } break;
             case "keywork": { } break;
         }
         return node_types
     }
 
     private _buildInputPortsFromSignature(signature: String) {
+        signature = signature.replace(/->.*/g, "")
         signature = signature.trim()
         signature = signature.slice(1, signature.length - 1)
         // 2.用 ", "分割
         let segs = signature.split(",")
         // 3.解析参数和默认值
         let in_ports: any[] = []
+        let arg_in_type = "keyword"
+
+        // 4.检查签名是否同时出现了* 和 /（有时候获取的签名有错误，比如numpy.array的签名）
+        let starIndex = -1
+        let gangIndex = -1
+        let index = 0
         for (let seg of segs) {
+            if (seg.trim() == "*") {
+                starIndex = index
+            }
+            if (seg.trim() == "/") {
+                gangIndex = index
+            }
+            index++
+        }
+
+        if (starIndex != -1 && gangIndex != -1 && starIndex < gangIndex) {
+            // 如果/在最后面，以前面的*为主
+            if (gangIndex == segs.length - 1) {
+                segs.pop()
+            } else {
+
+            }
+            // 需要重新获取签名
+        }
+
+        index = 0
+        for (let seg of segs) {
+            index++
             seg = seg.trim()
             if (!seg) {
                 continue
             }
 
-            let arg_name: string = "/"
+            let arg_name: string = ""
             let arg_type: string = "any"
             let arg_default: any = "None"
-            if (seg.charAt(0) == "/") {
-                in_ports.push({
-                    arg_name,
-                    arg_type,
-                    arg_default
-                })
+            if (seg == "/") {
+                arg_in_type = "keyword"
+                for (let port of in_ports) {
+                    port.arg_in_type = "positional"
+                }
                 continue
             }
-            let ret = /\*{2}\s*([_\w]+)/g.exec(seg)
-            if (ret) {
-                try { arg_name = "**" + ret[1].trim() + "(dict)" } catch (error) { }
-                arg_type = "dict"
-            } else {
+
+            if (seg == "*") {
+                arg_in_type = "keyword"
+                continue
+            }
+
+            if (seg == "self" && index == 1) {
+                continue
+            }
+
+            while (true) {
+                // 判断是否是dict
+                let ret = /\*{2}\s*([_\w]+)/g.exec(seg)
+                if (ret) {
+                    try { arg_name = "**" + ret[1].trim() + "(dict)" } catch (error) { }
+                    arg_type = "dict"
+                    break
+                }
+                // 判断是否是tuple
                 ret = /\*\s*([_\w]+)/g.exec(seg)
                 if (ret) {
                     try { arg_name = "*" + ret[1].trim() + "(tuple)" } catch (error) { }
                     arg_type = "tuple"
-                } else {
-                    ret = /([_\w]+)\s*(:\s*([_\w]+)){0,1}\s*(=(.*)){0,1}/g.exec(seg)
-                    if (ret) {
-                        try { arg_name = ret[1].trim() } catch (error) { }
-                        try { arg_type = ret[3].trim() } catch (error) { }
-                        try {
+                    break
+                }
+
+                // 正常的类型参数
+                ret = /([_\w]+)\s*(:\s*([_\w]+)){0,1}\s*(=(.*)){0,1}/g.exec(seg)
+                if (ret) {
+                    try { arg_name = ret[1].trim() } catch (error) { }
+                    try { arg_type = ret[3].trim() } catch (error) { }
+                    try {
+                        while (ret[5]) {
                             let dvalue = ret[5].trim()
                             // 判断是什么类型
                             // 字符串
                             if ((dvalue.charAt(0) == "\"" && dvalue.charAt(dvalue.length - 1) == "\"")
                                 || (dvalue.charAt(0) == "\'" && dvalue.charAt(dvalue.length - 1) == "\'")) {
                                 arg_type = "str"
                                 arg_default = eval(dvalue)
-                            } else {
-                                let ret = /[\d\.]+/g.exec(dvalue)
-                                if (ret) {
-                                    arg_type = "int"
-                                    arg_default = Number(dvalue)
-                                } else {
-                                    arg_default = dvalue
-                                }
+                                break
                             }
-                        } catch (error) { }
-                    }
+                            // class类型 "<class 'matplotlib.figure.Figure'>"
+                            ret = /<class(.*)>/g.exec(dvalue)
+                            if (ret) {
+                                arg_type = "any"
+                                arg_default = dvalue
+                                break
+                            }
+
+                            // 普通函数类型
+                            ret = /<function(.*?)at/g.exec(dvalue)
+                            if (ret) {
+                                arg_type = "any"
+                                arg_default = dvalue
+                                break
+                            }
+
+                            // build-in函数： <built-in function imread>
+                            // 目前不知道如何处理
+                            ret = /<built-in function (.*)>/g.exec(dvalue)
+                            if (ret) {
+                                arg_type = "any"
+                                arg_default = dvalue
+                                break
+                            }
+
+                            // 数字类型
+                            ret = /[\d\.]+/g.exec(dvalue)
+                            if (ret) {
+                                arg_type = "int"
+                                arg_default = Number(dvalue)
+                                break
+                            }
+
+                            arg_default = dvalue
+                            break
+                        }
+
+                    } catch (error) { }
+                    break
                 }
+                break
             }
-
             if (arg_name.length > 0) {
                 in_ports.push({
                     arg_name,
                     arg_type,
-                    arg_default
+                    arg_default,
+                    arg_in_type
                 })
             }
         }
 
         return in_ports
     }
 
@@ -1903,18 +2038,21 @@
             label: node_type_name,
             description: node_type_name,
             initialWidth: buildNodeWidth(node_type_name, headerFontsize, nodeMinWidth, nodeMaxWidth),
             inputs: ports => (inputData, connections, executionContext: NodeEditorWidget, nodeId) => {
                 let ret: any[] = [
                     get_port_func("control")(ports),
                 ]
+
+                let node = executionContext._getNode(nodeId)
                 for (const in_port of in_ports) {
-                    if (in_port.arg_name == "/") {
+                    if (node && node.hidePorts && node.hidePorts[in_port.arg_name]) {
                         continue
                     }
+
                     let f = get_port_func(in_port.arg_type)
                     let port = f(
                         ports,
                         in_port.arg_label || in_port.arg_name,
                         in_port.arg_name,
                         in_port.arg_default
                     )
@@ -2197,43 +2335,58 @@
                             }
                         // 2.如果是get，直接返回该变量的名称
                         case "get":
                             return { out: match_ret[2] }
                     }
                     return inputValues
                 // 2.节点是函数
+                case "class":
                 case "function":
-                    let no_keyword_arguments = false
                     let type_cache = this._nodeTypes[match_ret[2]]
-                    if (type_cache) {
-                        for (const port of type_cache.in_ports) {
-                            no_keyword_arguments = port.arg_name == "/"
-                        }
-                    }
+
                     // 1.构建参数字符串
                     let args_string = ""
                     for (const input of inputs) {
                         let name = input.name as string
+                        let value = inputValues[name]
+                        if (input.type == "any") {
+                            if (/<function(.*?)at/g.exec(value)
+                                || /<built-in function (.*)>/g.exec(value)
+                                || /<class(.*)>/g.exec(value)
+                                || value == "") {
+                                continue
+                            }
+                        }
                         let first_xing = name.charAt(0) == "*"
                         let second_xing = name.charAt(1) == "*"
                         // 1.检测是否是**开头
                         if (first_xing && second_xing) {
-                            args_string += `, **${inputValues[name]}`
+                            args_string += `, **${value}`
                         }
                         // 2.检测是否是*开头
                         else if (first_xing) {
-                            args_string += `, *${inputValues[name]}`
+                            args_string += `, *${value}`
                         }
                         // 3.正常的参数
                         else if (input.type != "control") {
-                            if (!no_keyword_arguments) {
-                                args_string += `, ${name}=${inputValues[name]}`
+                            let in_type = "keyword"
+                            if (type_cache) {
+                                for (const port of type_cache.in_ports) {
+                                    if (port.arg_name == name) {
+                                        in_type = port.arg_in_type
+                                        break
+                                    }
+                                }
+                            }
+
+                            if (in_type == "keyword") {
+                                args_string += `, ${name}=${value}`
                             }
                             else {
-                                args_string += `, ${inputValues[name]}`
+                                args_string += `, ${value}`
                             }
                         }
                     }
                     // 2.去除开头的,
                     args_string = args_string.slice(1, args_string.length)
                     // 3.构建代码
                     let out_var_name = this._getOutVarName(id)
@@ -2413,27 +2566,46 @@
                 }
                 case "operator": {
                     let out_var_name = this._getOutVarName(id)
                     let yiyuan_operator = ["not", "~"]
                     let operator = inputValues["operator"]["operator"]
                     let code
                     if (!yiyuan_operator.includes(operator)) {
-                        code = `${out_var_name} = ${inputValues["value1"]} ${operator} ${inputValues["value2"]}`
+                        switch (operator) {
+                            case "[]": {
+                                code = `${out_var_name} = ${inputValues["value1"]}[${inputValues["value2"]}]`
+                            } break;
+                            default: {
+                                code = `${out_var_name} = ${inputValues["value1"]} ${operator} ${inputValues["value2"]}`
+                            } break;
+                        }
                     } else {
                         code = `${out_var_name} = ${operator} ${inputValues["value1"]}`
+
                     }
                     if (this._exportingCodeNodeId) {
                         this._exportCode(code)
                     } else {
                         await this._runCode(code)
                     }
                     return {
                         out: out_var_name
                     }
                 }
+                case "setvar": {
+                    let code = `${inputValues['name']} = ${inputValues["value"]}`
+                    if (this._exportingCodeNodeId) {
+                        this._exportCode(code)
+                    } else {
+                        await this._runCode(code)
+                    }
+                    return {
+                        out: inputValues['name']
+                    }
+                }
             }
         }
     }
 
     private async _runCell(
         cell: CodeCellModel,
         translator: ITranslator | null) {
@@ -2576,15 +2748,14 @@
             id: this._curNodesId,
             name: this.curNodeName,
             nodes,
             nodeTypes: {},
             locked: [...this._lockedNodes],
             runCache: this._runCache,
             comments: this.editorComments,
-            default: this._curNodesIsDefault,
         }
 
         const saveNodeType = (type_name) => {
             // 1.判断是instance 还是 function
             let ret = /instance.*?@(get|set)@(.*)/g.exec(type_name)
             if (ret) {
                 save_data.nodeTypes[ret[2]] = this._nodeTypes[ret[2]]
@@ -2595,14 +2766,20 @@
                     save_data.nodeTypes[ret[1]] = this._nodeTypes[ret[1]]
                 }
                 else {
                     ret = /combine@(.*)/g.exec(type_name)
                     if (ret) {
                         save_data.nodeTypes[ret[1]] = this._nodeTypes[ret[1]]
                     }
+                    else {
+                        ret = /class@(.*)/g.exec(type_name)
+                        if (ret) {
+                            save_data.nodeTypes[ret[1]] = this._nodeTypes[ret[1]]
+                        }
+                    }
                 }
             }
         }
 
         // 检查并保存所有用到的nodetypes
         for (const key in nodes) {
             saveNodeType(nodes[key].type)
@@ -2693,15 +2870,15 @@
             await this._readRunCache(data)
 
             // 5.读取node数据
             this._curNodesId = data.id
             this.editorNodes = data.nodes
             this.editorComments = data.comments || {}
             this.setCurNodeName(data.name)
-            this._curNodesIsDefault = data.default
+            this._curNodesIsDefault = data.id == this.getDefaultNodesId()
 
             // 6.清除当前数据
             this._refreshNodeEditorCache()
 
             // 7.将数据同步到节点编辑器
             this.dispatchNodes({ type: "RE_INIT", nodes: this.editorNodes })
             this.dispatchComments({ type: "RE_INIT", comments: this.editorComments })
@@ -2834,15 +3011,15 @@
             case "any":
                 for (const key in data) {
                     return data[key]
                 }
                 return "None"
             case 'string':
                 for (const key in data) {
-                    return `'${data[key]}'`
+                    return `${JSON.stringify(data[key])}`
                 }
                 return `''`
             case 'jsstring':
                 for (const key in data) {
                     return data[key]
                 }
                 return ""
@@ -2938,26 +3115,36 @@
             this._setRunningNode(this._runningNodeId, true)
             this.refreshNodeBoxShadow()
             outputMsg = {
                 output_type: "error",
                 ...msg.content
             }
         }
-        else if (KernelMessage.isExecuteResultMsg(msg)) {
+        else if (KernelMessage.isExecuteResultMsg(msg) || KernelMessage.isDisplayDataMsg(msg)) {
             console.log(msg.content.data)
             outputMsg = {
                 output_type: "execute_result",
                 ...msg.content
             }
         }
         else if (KernelMessage.isStatusMsg(msg)) {
             let state = kernelStateMap[msg.content.execution_state]
             if (state) {
                 this._setKernelState(state)
             }
+        } else if (KernelMessage.isUpdateDisplayDataMsg(msg)) {
+            const transient = ((msg.content as any).transient || {})
+            const displayId = transient['display_id'] as string;
+            let output = { ...msg.content, output_type: 'display_data' };
+            let targets = (this._outputArea as any)._displayIdMap.get(displayId);
+            if (targets) {
+                for (const index of targets) {
+                    this._outputArea.model.set(index, output);
+                }
+            }
         }
 
         if (outputMsg) {
             if (this._outputArea) {
                 this._outputArea.model.add(outputMsg)
             }
         }
@@ -3368,15 +3555,15 @@
         });
     }
 
     private _addNodeTypes(nodeTypes) {
         for (const nodeType of nodeTypes) {
             // 添加节点类型
             try {
-                if (this.editorConfig[nodeType.type])
+                if (this.editorConfig.nodeTypes[nodeType.type])
                     this.editorConfig.removeNodeType(nodeType.type)
                 this.editorConfig.addNodeType(nodeType)
             } catch (error) { }
         }
     }
 
     private async _combineSelectedNodes() {
@@ -3478,14 +3665,20 @@
                         connectionData[id] = connectionData[id] || []
                         connectionData[id].push(connection[0])
                         let cacheNode = nodesCache[id]
                         delete cacheNode.connections.inputs[input.name]
                     }
                     else {
                         arg_default = await this._getInputValue(input, node)
+                        switch (input.type) {
+                            case "str":
+                            case "string": {
+                                arg_default = eval(arg_default)
+                            } break;
+                        }
                     }
                     in_ports.push({
                         arg_name: `${id}@${input.name}`,
                         arg_label: input.label,
                         arg_type: input.type,
                         arg_default,
                     })
@@ -4256,14 +4449,22 @@
         var suggestions: monaco.languages.CompletionItem[] = [];
 
         if (reply?.content.status == "ok") {
             let matches: any[] = reply.content.metadata._jupyter_types_experimental as []
             for (const match of matches) {
                 let suggestion: any = null
                 switch (match.type) {
+                    case "statement": {
+                        suggestion = {
+                            label: match.text,
+                            kind: monaco.languages.CompletionItemKind.Constant,
+                            insertText: match.text,
+                            range: range,
+                        }
+                    } break;
                     case "instance": {
                         suggestion = {
                             label: match.text,
                             kind: monaco.languages.CompletionItemKind.Variable,
                             insertText: match.text,
                             range: range,
                         }
@@ -4597,35 +4798,35 @@
         }
         this._context.model.sharedModel.moveCell(this._curEditingCellIndex, targetIndex)
         this._editCell(targetIndex)
     }
 
     private _setCurrentNodesAsDefault() {
         this._curNodesIsDefault = true
+        this.setDefaultNodesId(this._curNodesId)
         this._updateNodesDefaultShow()
-        this._needSaveNodes = true
-        this._saveNodes()
     }
 
     private async _buildNodeCode(id) {
-        let preCheckCache = this._runCheckCache
+        let preCheckCache = this._runCache
         try {
             this._exportRet = []
             this._exportingCodeNodeId = id
-            this._runCheckCache = false
+            this._runCheckCache = true
+            this._runCache = {}
             this._exportIndent = ""
             await this.runNode(id)
             this._codeEditorValueCache = this._getExportedCodeText()
         } catch (e) {
             showErrorMessage("错误", "将节点生成为代码发生错误！")
             return false
         }
         finally {
             this._exportingCodeNodeId = null
-            this._runCheckCache = preCheckCache
+            this._runCache = preCheckCache
         }
 
         return true
     }
 
     private async _dispatchNodesAction(action) {
         switch (action.type) {
@@ -4661,14 +4862,15 @@
             switch (type_data.type) {
                 case "instance": {
                     node_types = this._buildInstanceNodeTypes(
                         type_data.node_type_name,
                         type_data.target_type,
                         type_data.target_value)
                 } break
+                case "class":
                 case "combine":
                 case "function": {
                     node_types = this._buildCommonNodeTypes(
                         type_data.node_type_name,
                         type_data.in_ports,
                         type_data.type)
 
@@ -4729,30 +4931,40 @@
         fn()
     }
 
 
     private async _tryLoadNodes() {
         let allNodes = this.getAllNodes()
         let targetNodes: any = null
+        let defaultNodesId = this.getDefaultNodesId()
         for (const nodes of Object.values<any>(allNodes)) {
             if (targetNodes == null) {
                 targetNodes = nodes
             }
-            if (nodes.default) {
+            if (defaultNodesId == nodes.id) {
                 targetNodes = nodes
             }
         }
 
         if (targetNodes == null) {
             return true
         }
 
         return await this._loadNodes(targetNodes, false)
     }
 
+    private async _runStartNode() {
+        for (const node of Object.values(this.editorNodes)) {
+            if ((node as any).type == "start") {
+                await this.runNode((node as any).id, true)
+                return
+            }
+        }
+    }
+
     private _createCommands() {
         try {
             this._createCommand("nd-load", "加载", () => { this._openLoadMenu() })
             this._createCommand("nd-create", "创建", () => this.createNewNodes())
             this._createCommand("nd-delete", "删除", () => this.deleteNodes())
             this._createCommand("nd-rename", "重命名", () => this._renameNodes())
             this._createCommand("nd-copy", "复制", () => this._copyNodes())
@@ -4780,16 +4992,17 @@
             this._createCommand("nd-cell-redo", "重做Cell", () => { this._redoCell() })
             this._createCommand("nd-edit-pre-cell", "编辑上一个Cell", () => { this._editPreCell() })
             this._createCommand("nd-edit-next-cell", "编辑下一个Cell", () => { this._editNextCell() })
             this._createCommand("nd-cell-up", "Cell上移", () => { this._CellMove(-1) })
             this._createCommand("nd-cell-down", "Cell下移", () => { this._CellMove(1) })
             this._createCommand("nd-set-as-default", "设置为默认", () => { this._setCurrentNodesAsDefault() })
             this._createCommand("nd-open-comment-color-picker", "打开注释颜色选择器", () => { this._openSelectedCommentsColorPicker() })
-            this._createCommand("nd-combine-selected-nodes", "组合节点", () => { this._combineSelectedNodes() })
-            this._createCommand("nd-separate-selected-node", "拆分节点", () => { this._separateSelectedNode() })
+            // this._createCommand("nd-combine-selected-nodes", "组合节点", () => { this._combineSelectedNodes() })
+            // this._createCommand("nd-separate-selected-node", "拆分节点", () => { this._separateSelectedNode() })
+            this._createCommand("nd-run-start-node", "运行开始节点", () => { this._runStartNode() })
         } catch (error) {
 
         }
     }
 }
 
 const NOTEBOOK_PANEL_TOOLBAR_CLASS = 'jp-NotebookPanel-toolbar';
```

### Comparing `jupyterlab_nodeeditor-1.0.5/src/yesIcon.tsx` & `jupyterlab_nodeeditor-1.0.6/src/yesIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/test_ext/1.jpeg` & `jupyterlab_nodeeditor-1.0.6/test_ext/1.jpeg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/test_ext/2.jpeg` & `jupyterlab_nodeeditor-1.0.6/test_ext/2.jpeg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/test_ext/main.ipynb` & `jupyterlab_nodeeditor-1.0.6/test_ext/main.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/test_ext/testlib.ipynb` & `jupyterlab_nodeeditor-1.0.6/test_ext/testlib.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996014030612245%*

 * *Differences: {"'metadata'": "{'nodes': {'23c5c583-f212-45ad-9add-fd05abd4f3d1': {'nodes': {'UIAx4IF1ga': {'x': "*

 * *               "-437.75, 'y': -684.5}, 'e3OuU2LPvU': {'x': -432.25, 'y': -347}, 'h8w053AX2P': "*

 * *               "{'x': -433.25, 'y': -527}, 'wSSpVc-eCL': {'x': -154.75, 'y': -511.5}}, 'runCache': "*

 * *               '{replace: OrderedDict()}}}}'}*

```diff
@@ -350,16 +350,16 @@
                             "90C3K9qUKs@index": {
                                 "90C3K9qUKs@index": "10"
                             },
                             "control": {}
                         },
                         "type": "combine@\u521d\u59cb\u5316index",
                         "width": 200,
-                        "x": -432.75,
-                        "y": -686.5
+                        "x": -437.75,
+                        "y": -684.5
                     },
                     "e3OuU2LPvU": {
                         "connections": {
                             "inputs": {},
                             "outputs": {
                                 "control": [
                                     {
@@ -374,16 +374,16 @@
                             "AQZcy7z-da@value2": {
                                 "AQZcy7z-da@value2": "1"
                             },
                             "control": {}
                         },
                         "type": "combine@index-=",
                         "width": 200,
-                        "x": -428.25,
-                        "y": -309
+                        "x": -432.25,
+                        "y": -347
                     },
                     "h8w053AX2P": {
                         "connections": {
                             "inputs": {},
                             "outputs": {
                                 "out": [
                                     {
@@ -398,16 +398,16 @@
                             "control": {},
                             "sS_rQnU2Vo@value2": {
                                 "sS_rQnU2Vo@value2": "0"
                             }
                         },
                         "type": "combine@index>0?",
                         "width": 200,
-                        "x": -435.25,
-                        "y": -507
+                        "x": -433.25,
+                        "y": -527
                     },
                     "wSSpVc-eCL": {
                         "connections": {
                             "inputs": {
                                 "control": [
                                     {
                                         "nodeId": "UIAx4IF1ga",
@@ -435,29 +435,19 @@
                             "loop": {},
                             "value": {
                                 "value": 0
                             }
                         },
                         "type": "loop",
                         "width": 200,
-                        "x": -121.75,
-                        "y": -500.5
+                        "x": -154.75,
+                        "y": -511.5
                     }
                 },
-                "runCache": {
-                    "UIAx4IF1ga": {
-                        "out": "_UIAx4IF1ga_out"
-                    },
-                    "h8w053AX2P": {
-                        "out": "_h8w053AX2P_out"
-                    },
-                    "wSSpVc-eCL": {
-                        "out": "None"
-                    }
-                }
+                "runCache": {}
             },
             "73b188df-39a6-43e6-8289-0d2169b4b0df": {
                 "comments": {},
                 "default": true,
                 "id": "73b188df-39a6-43e6-8289-0d2169b4b0df",
                 "locked": [],
                 "name": "\u6d4b\u8bd5\u56fe\u7247",
```

### Comparing `jupyterlab_nodeeditor-1.0.5/.gitignore` & `jupyterlab_nodeeditor-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/LICENSE` & `jupyterlab_nodeeditor-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/README.md` & `jupyterlab_nodeeditor-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/pyproject.toml` & `jupyterlab_nodeeditor-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.5/PKG-INFO` & `jupyterlab_nodeeditor-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nodeeditor
-Version: 1.0.5
+Version: 1.0.6
 Summary: 一个节点编辑器
 Project-URL: Homepage, https://github.com/github_username/jupyterlab_nodeeditor
 Project-URL: Bug Tracker, https://github.com/github_username/jupyterlab_nodeeditor/issues
 Project-URL: Repository, https://github.com/github_username/jupyterlab_nodeeditor.git
 Author-email: l0n0l <cenlan@hotmail.com>
 License: BSD 3-Clause License
```

