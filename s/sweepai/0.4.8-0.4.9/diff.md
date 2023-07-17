# Comparing `tmp/sweepai-0.4.8.tar.gz` & `tmp/sweepai-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.4.8.tar", max compression
+gzip compressed data, was "sweepai-0.4.9.tar", max compression
```

## Comparing `sweepai-0.4.8.tar` & `sweepai-0.4.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.4.8/LICENSE
--rw-r--r--   0        0        0     7019 2023-07-13 23:38:51.881474 sweepai-0.4.8/README.md
--rw-r--r--   0        0        0     1411 2023-07-14 17:55:12.308118 sweepai-0.4.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.8/sweepai/__init__.py
--rw-r--r--   0        0        0    12345 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/api.py
--rw-r--r--   0        0        0     6977 2023-07-14 04:12:55.561425 sweepai-0.4.8/sweepai/app/api_client.py
--rw-r--r--   0        0        0    12755 2023-07-14 03:56:57.223048 sweepai-0.4.8/sweepai/app/backend.py
--rw-r--r--   0        0        0     1167 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/app/cli.py
--rw-r--r--   0        0        0     3615 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/app/config.py
--rw-r--r--   0        0        0    16697 2023-07-14 04:26:38.459296 sweepai-0.4.8/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.8/sweepai/core/__init__.py
--rw-r--r--   0        0        0    18015 2023-07-13 23:57:23.352400 sweepai-0.4.8/sweepai/core/chat.py
--rw-r--r--   0        0        0     2880 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     8273 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/core/entities.py
--rw-r--r--   0        0        0      535 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/core/gha_extraction.py
--rw-r--r--   0        0        0    16873 2023-07-13 22:20:26.747256 sweepai-0.4.8/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3489 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/core/react.py
--rw-r--r--   0        0        0    20835 2023-07-13 07:06:00.213068 sweepai-0.4.8/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    13594 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     3191 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.8/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     7146 2023-07-13 23:57:23.352400 sweepai-0.4.8/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     2613 2023-07-13 22:20:26.750590 sweepai-0.4.8/sweepai/handlers/on_check_suite.py
--rw-r--r--   0        0        0     9748 2023-07-13 22:20:26.750590 sweepai-0.4.8/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     4042 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    19991 2023-07-13 23:38:31.094765 sweepai-0.4.8/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.8/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     3822 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.8/sweepai/utils/config/__init__.py
--rw-r--r--   0        0        0     2761 2023-07-14 17:53:38.131398 sweepai-0.4.8/sweepai/utils/config/client.py
--rw-r--r--   0        0        0     3460 2023-07-14 04:49:15.051252 sweepai-0.4.8/sweepai/utils/config/server.py
--rw-r--r--   0        0        0     6524 2023-07-13 22:20:26.750590 sweepai-0.4.8/sweepai/utils/diff.py
--rw-r--r--   0        0        0      675 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5256 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8431 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0      100 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/hash.py
--rw-r--r--   0        0        0     5585 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      849 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1528 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11648 2023-07-13 01:02:13.147504 sweepai-0.4.8/sweepai/utils/utils.py
--rw-r--r--   0        0        0     8239 2023-07-14 17:55:15.414130 sweepai-0.4.8/setup.py
--rw-r--r--   0        0        0     7998 2023-07-14 17:55:15.414584 sweepai-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.4.9/LICENSE
+-rw-r--r--   0        0        0     7813 2023-07-14 18:26:12.305858 sweepai-0.4.9/README.md
+-rw-r--r--   0        0        0     1411 2023-07-14 19:14:56.280803 sweepai-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.9/sweepai/__init__.py
+-rw-r--r--   0        0        0    12345 2023-07-13 01:02:13.144171 sweepai-0.4.9/sweepai/api.py
+-rw-r--r--   0        0        0     7139 2023-07-14 19:11:55.424037 sweepai-0.4.9/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    13088 2023-07-14 19:11:07.497344 sweepai-0.4.9/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1167 2023-07-13 01:02:13.144171 sweepai-0.4.9/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3615 2023-07-13 01:02:13.144171 sweepai-0.4.9/sweepai/app/config.py
+-rw-r--r--   0        0        0    16856 2023-07-14 19:02:40.713731 sweepai-0.4.9/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.9/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    18015 2023-07-13 23:57:23.352400 sweepai-0.4.9/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2880 2023-07-13 01:02:13.144171 sweepai-0.4.9/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     8273 2023-07-13 01:02:13.144171 sweepai-0.4.9/sweepai/core/entities.py
+-rw-r--r--   0        0        0      535 2023-07-13 01:02:13.144171 sweepai-0.4.9/sweepai/core/gha_extraction.py
+-rw-r--r--   0        0        0    16873 2023-07-13 22:20:26.747256 sweepai-0.4.9/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3489 2023-07-13 01:02:13.144171 sweepai-0.4.9/sweepai/core/react.py
+-rw-r--r--   0        0        0    20835 2023-07-13 07:06:00.213068 sweepai-0.4.9/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    13594 2023-07-13 01:02:13.144171 sweepai-0.4.9/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     3191 2023-07-13 01:02:13.144171 sweepai-0.4.9/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.9/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     7146 2023-07-13 23:57:23.352400 sweepai-0.4.9/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     2613 2023-07-13 22:20:26.750590 sweepai-0.4.9/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0        0        0     9748 2023-07-13 22:20:26.750590 sweepai-0.4.9/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     4042 2023-07-13 01:02:13.144171 sweepai-0.4.9/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    19991 2023-07-14 18:26:12.305858 sweepai-0.4.9/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.9/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.9/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     3822 2023-07-14 18:26:12.305858 sweepai-0.4.9/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0        0 2023-07-13 01:02:13.144171 sweepai-0.4.9/sweepai/utils/config/__init__.py
+-rw-r--r--   0        0        0     2761 2023-07-14 17:53:38.131398 sweepai-0.4.9/sweepai/utils/config/client.py
+-rw-r--r--   0        0        0     3460 2023-07-14 19:13:57.390771 sweepai-0.4.9/sweepai/utils/config/server.py
+-rw-r--r--   0        0        0     6524 2023-07-13 22:20:26.750590 sweepai-0.4.9/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      675 2023-07-13 01:02:13.147504 sweepai-0.4.9/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5256 2023-07-13 01:02:13.147504 sweepai-0.4.9/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8449 2023-07-14 18:26:12.305858 sweepai-0.4.9/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0      100 2023-07-13 01:02:13.147504 sweepai-0.4.9/sweepai/utils/hash.py
+-rw-r--r--   0        0        0     5585 2023-07-13 01:02:13.147504 sweepai-0.4.9/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      849 2023-07-13 01:02:13.147504 sweepai-0.4.9/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1528 2023-07-13 01:02:13.147504 sweepai-0.4.9/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11648 2023-07-13 01:02:13.147504 sweepai-0.4.9/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     9038 2023-07-14 19:15:03.535174 sweepai-0.4.9/setup.py
+-rw-r--r--   0        0        0     8792 2023-07-14 19:15:03.535655 sweepai-0.4.9/PKG-INFO
```

### Comparing `sweepai-0.4.8/LICENSE` & `sweepai-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/README.md` & `sweepai-0.4.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 </a>
 <a href="https://github.com/sweepai/sweep">
     <img src="https://img.shields.io/github/stars/sweepai/sweep" />
 </a>
 <a href="https://twitter.com/sweep__ai">
     <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />
 </a>
+<br>
+<a href="https://www.producthunt.com/posts/sweep-5?utm_source=badge-featured&utm_medium=badge&utm_souce=badge-sweep&#0045;5" target="_blank"><img src="https://api.producthunt.com/widgets/embed-image/v1/featured.svg?post_id=404410&theme=neutral" alt="Sweep - Sweep&#0032;is&#0032;an&#0032;AI&#0045;powered&#0032;junior&#0032;dev&#0032;on&#0032;your&#0032;team&#0046; | Product Hunt" style="width: 175px; height: 36px;" width="175" height="36" /></a>
 </p>
 
 <b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.
 
 Describe bugs, small features, and refactors like you would to a junior developer, and Sweep:
 1. 🔍 reads your codebase
 2. 📝 plans the changes
@@ -37,15 +39,15 @@
 See highlights at https://docs.sweep.dev/examples.
 
 [Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)
 
 ## 🌠 Sweep
 * 🔧 Turns issues directly into pull requests (without an IDE)
 * 👀 Addresses developer replies & comments on its PRs
-* 🕵️‍♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))
+* 🕵️‍♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/blogs/building-code-search))
 * 🎊 New: Fixes PRs based on Github Actions feedback
 * 🎊 New: Sweep Chat, a local interface for Sweep (see below)
 
 ## 🚀 Getting Started
 
 ### 🍲 Recipes
 #### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. 
@@ -64,22 +66,24 @@
 #### Limitations:
 Sweep is unlikely to complete complex issues on the first try, similar to the average junior developer. Here are Sweep's limitations(for now):
 - Try to change less than 200 lines of code
 - Try to modify less than 3 files
 - Do not include files with more than 1500 lines of code
 
 ### ✨ Sweep Github App
-Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.
-We support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.
+Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address. Here are the steps to get started:
+
+1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to your desired repos
+2. Create a new issue in your repo. The issue should describe the problem or feature you want Sweep to address. For example, you could write "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"
+3. Respond with a message like "Sweep: use a different package instead" to have Sweep retry the issue or pull request. You can also comment on the code for minor changes!
 
-1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
-2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"
+We support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.
 
 ### 🖥️ Sweep Chat
-Sweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. 
+Sweep Chat allows you to interact with Sweep and GitHub locally. You can collaborate on the plan with Sweep, and then have it create the pull request for you. Here's how to use Sweep Chat:
 
 **Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository
 
 1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**
     - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.
     - This runs GitHub authentication in your browser.
 
@@ -101,15 +105,15 @@
 If you want the nightly build and or if the latest build has issues.
 
 1. `git clone https://github.com/sweepai/sweep && poetry install`
 2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.
 
 ## 💰 Pricing
 * We charge $120/month for 60 GPT4 tickets per month.
-* For unpaid users, we offer 3 free GPT4 tickets per month.
+* For unpaid users, we offer 5 free GPT4 tickets per month.
 * We also offer unlimited GPT3.5 tickets.
 ## 🤝 Contributing
 
 Contributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 For more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).
 
 ## 📘 Story
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
   [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                  3e61f57ad233]
                Bug Reports & Feature Requests â¶  Code Changes
       [Landing_Page] [Docs] [https://dcbadge.vercel.app/api/server/sweep-
 ai?style=flat] [PyPI] [https://static.pepy.tech/badge/sweepai/month] [https://
   img.shields.io/github/stars/sweepai/sweep] [https://img.shields.io/twitter/
                 url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]
+   [Sweep_-_Sweep_is_an_AI-powered_junior_dev_on_your_team._|_Product_Hunt]
 Sweep is an AI junior developer that transforms bug reports & feature requests
 into code changes. Describe bugs, small features, and refactors like you would
 to a junior developer, and Sweep: 1. ð reads your codebase 2. ð plans the
 changes 3. â¡**writes a pull request with code**â¡ See highlights at https://
 docs.sweep.dev/examples. [Demo](https://github.com/sweepai/sweep/assets/
 44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47) ## ð  Sweep * ð§ Turns
 issues directly into pull requests (without an IDE) * ð Addresses developer
 replies & comments on its PRs * ðµï¸ââï¸ Uses embedding-based code
 search, with popularity reranking for repository-level code understanding (
-[ð Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-
-rebuilt-our-code-search-engine-in-a-day)) * ð New: Fixes PRs based on Github
-Actions feedback * ð New: Sweep Chat, a local interface for Sweep (see
-below) ## ð Getting Started ### ð² Recipes #### To get the best
-performance from Sweep, we recommend the following approach to writing github
-issues/chats. For harder problems, try to provide the same information a human
-would need. For simpler problems, providing a single line and a file name
-should suffice. A good issue might include: | Where to look
+[ð Rebuilding our Search Engine in a Day](https://docs.sweep.dev/blogs/
+building-code-search)) * ð New: Fixes PRs based on Github Actions feedback *
+ð New: Sweep Chat, a local interface for Sweep (see below) ## ð Getting
+Started ### ð² Recipes #### To get the best performance from Sweep, we
+recommend the following approach to writing github issues/chats. For harder
+problems, try to provide the same information a human would need. For simpler
+problems, providing a single line and a file name should suffice. A good issue
+might include: | Where to look
 **[file name or function name]**| What to do
 **[change the logic to do this]** | Additional Context (optional)
 **[there's a bug/we need this feature/there's this dependency]** | |-----------
 |------------|----------------------| |In `sweepai/app/ui.py`|use an os-
 agnostic temp directory|N/A| |In `on_comment.py`|we should not fire an
 event|because it's possible that the comment is on a closed PR| |In the config
 loader in `packages/server/src/config.ts`|add a third option called "env" to
@@ -34,38 +35,43 @@
 full path. Similarly, to have Sweep use a function, try to mention the class
 method or what it does. Also see [â¨ Tips and tricks for Sweep](https://
 docs.sweep.dev/tricks). #### Limitations: Sweep is unlikely to complete complex
 issues on the first try, similar to the average junior developer. Here are
 Sweep's limitations(for now): - Try to change less than 200 lines of code - Try
 to modify less than 3 files - Do not include files with more than 1500 lines of
 code ### â¨ Sweep Github App Setting up Sweep is as simple as adding the
-GitHub bot to a repo, then creating an issue for the bot to address. We support
-all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C#
-and C++. 1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to
-desired repos 2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py
-use an os-agnostic temp directory" ### ð¥ï¸ Sweep Chat Sweep Chat allows you
-to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep,
-then have it create the pull request for you. **Prerequisites:** Install [Sweep
-GitHub app](https://github.com/apps/sweep-ai) to your repository 1. Run `pip3
-install sweepai && sweep`. Note that you need **python 3.10+.** - Alternatively
-run `pip3 install --force-reinstall sweepai && sweep` if the previous command
+GitHub bot to a repo, then creating an issue for the bot to address. Here are
+the steps to get started: 1. Add the [Sweep GitHub app](https://github.com/
+apps/sweep-ai) to your desired repos 2. Create a new issue in your repo. The
+issue should describe the problem or feature you want Sweep to address. For
+example, you could write "Sweep: In sweepai/app/ui.py use an os-agnostic temp
+directory" 3. Respond with a message like "Sweep: use a different package
+instead" to have Sweep retry the issue or pull request. You can also comment on
+the code for minor changes! We support all languages GPT4 supports, including
+Python, Typescript, Rust, Go, Java, C# and C++. ### ð¥ï¸ Sweep Chat Sweep
+Chat allows you to interact with Sweep and GitHub locally. You can collaborate
+on the plan with Sweep, and then have it create the pull request for you.
+Here's how to use Sweep Chat: **Prerequisites:** Install [Sweep GitHub app]
+(https://github.com/apps/sweep-ai) to your repository 1. Run `pip3 install
+sweepai && sweep`. Note that you need **python 3.10+.** - Alternatively run
+`pip3 install --force-reinstall sweepai && sweep` if the previous command
 fails. - This runs GitHub authentication in your browser. 2. Copy the ðµ blue
 8-digit code from your terminal into the page. You should only need to do the
 authentication once. - Wait a few seconds and Sweep Chat will start. 3. Choose
 a repository from the dropdown at the top (the Github app must be installed to
 this repository). - â¡ Start chatting with Sweep Chat! â¡ [https://
 github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/
 gradio-screenshot.png] Tips: * ð Relevant searched files will show up on the
 right. * ð Sweep Chat creates PRs when the "Create PR" button is clicked. *
 ð¡ You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
 #### From Source If you want the nightly build and or if the latest build has
 issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
 `python sweepai/app/cli.py`. Note that you need **python 3.10+**. ## ð°
 Pricing * We charge $120/month for 60 GPT4 tickets per month. * For unpaid
-users, we offer 3 free GPT4 tickets per month. * We also offer unlimited GPT3.5
+users, we offer 5 free GPT4 tickets per month. * We also offer unlimited GPT3.5
 tickets. ## ð¤ Contributing Contributions are welcome and greatly
 appreciated! For detailed guidelines on how to contribute, please see the
 [CONTRIBUTING.md](CONTRIBUTING.md) file. For more detailed docs, see [ð
 Quickstart](https://docs.sweep.dev/). ## ð Story We were frustrated by small
 tickets, like simple bug fixes, annoying refactors, and small features. Each
 task required us to open our IDE to fix simple bugs. So we decided to leverage
 the capabilities of ChatGPT to address this directly in GitHub. Unlike existing
```

### Comparing `sweepai-0.4.8/pyproject.toml` & `sweepai-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.4.8"
+version = "0.4.9"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
```

### Comparing `sweepai-0.4.8/sweepai/api.py` & `sweepai-0.4.9/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/app/api_client.py` & `sweepai-0.4.9/sweepai/app/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,11 +189,14 @@
                     }
             ) as response:
                 for delta_chunk in response.iter_text():
                     if not delta_chunk:
                         break
                     try:
                         for item in break_json(delta_chunk):
+                            if "error" in item:
+                                logger.error(item)
+                                raise Exception(item["error"])
                             yield item
                     except json.decoder.JSONDecodeError as e:
                         logger.error(delta_chunk)
                         raise e
```

### Comparing `sweepai-0.4.8/sweepai/app/backend.py` & `sweepai-0.4.9/sweepai/app/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Proxy for the UI.
 """
 
 from datetime import datetime
+from http.client import HTTPException
 import json
 from typing import Any
 
 import fastapi
 import modal
 from fastapi import FastAPI
 from fastapi.responses import StreamingResponse
@@ -318,17 +319,23 @@
             if request.do_add_plan:
                 chatgpt.messages[-1].content += gradio_user_prompt
         except Exception as e:
             posthog.capture(request.config.github_username, "failed", properties={"error": str(e), **metadata})
             raise e
 
         def stream_chat():
-            for chunk in chatgpt.chat_stream(messages[-1].content, model="gpt-4-0613", functions=request.functions,
-                                             function_call=request.function_call):
-                yield json.dumps(chunk)
+            try:
+                stream = chatgpt.chat_stream(messages[-1].content, model="gpt-4-0613", functions=request.functions,
+                                                function_call=request.function_call)
+                for chunk in stream:
+                    yield json.dumps(chunk)
+            except Exception as e:
+                logger.error(e)
+                posthog.capture(request.config.github_username, "failed", properties={"error": str(e), **metadata})
+                yield json.dumps({"error": str(e)})
             posthog.capture(request.config.github_username, "success", properties=metadata)
 
         return StreamingResponse(
             stream_chat(),
             media_type="text/event-stream"
         )
```

### Comparing `sweepai-0.4.8/sweepai/app/cli.py` & `sweepai-0.4.9/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/app/config.py` & `sweepai-0.4.9/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/app/ui.py` & `sweepai-0.4.9/sweepai/app/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,27 +325,31 @@
                 raise gr.Error(str(e))
         else:
             stream = api_client.stream_chat(chat_history, selected_snippets)
         function_name = ""
         raw_arguments = ""
         raw_response = ""
         parsed_response = ""
-        for chunk in stream:
-            if chunk.get("content"):
-                token = chunk["content"]
-                raw_response += token
-                parsed_response, plan = parse_response(raw_response)
-                chat_history[-1][1] = parsed_response
-                yield chat_history, snippets_text, file_names, plan
-            if chunk.get("function_call"):
-                function_call = chunk["function_call"]
-                function_name = function_name or function_call.get("name")
-                raw_arguments += function_call.get("arguments")
-                chat_history[-1][1] = f"Calling function: `{function_name}`\n```json\n{raw_arguments}\n```"
-                yield chat_history, snippets_text, file_names, plan
+        try:
+            for chunk in stream:
+                if chunk.get("content"):
+                    token = chunk["content"]
+                    raw_response += token
+                    parsed_response, plan = parse_response(raw_response)
+                    chat_history[-1][1] = parsed_response
+                    yield chat_history, snippets_text, file_names, plan
+                if chunk.get("function_call"):
+                    function_call = chunk["function_call"]
+                    function_name = function_name or function_call.get("name")
+                    raw_arguments += function_call.get("arguments")
+                    chat_history[-1][1] = f"Calling function: `{function_name}`\n```json\n{raw_arguments}\n```"
+                    yield chat_history, snippets_text, file_names, plan
+        except Exception as e:
+            logger.error(e)
+            raise gr.Error(str(e))
         if function_name:
             arguments = json.loads(raw_arguments)
             if function_name == "create_pr":
                 assert "title" in arguments
                 assert "summary" in arguments
                 assert "plan" in arguments
                 if "branch" not in arguments:
```

### Comparing `sweepai-0.4.8/sweepai/core/chat.py` & `sweepai-0.4.9/sweepai/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/core/code_repair.py` & `sweepai-0.4.9/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/core/entities.py` & `sweepai-0.4.9/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/core/gha_extraction.py` & `sweepai-0.4.9/sweepai/core/gha_extraction.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/core/prompts.py` & `sweepai-0.4.9/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/core/react.py` & `sweepai-0.4.9/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/core/sweep_bot.py` & `sweepai-0.4.9/sweepai/core/sweep_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/core/vector_db.py` & `sweepai-0.4.9/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/events.py` & `sweepai-0.4.9/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/handlers/create_pr.py` & `sweepai-0.4.9/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/handlers/on_check_suite.py` & `sweepai-0.4.9/sweepai/handlers/on_check_suite.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/handlers/on_comment.py` & `sweepai-0.4.9/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/handlers/on_review.py` & `sweepai-0.4.9/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/handlers/on_ticket.py` & `sweepai-0.4.9/sweepai/handlers/on_ticket.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
             return f"![{index}%](https://progress-bar.dev/{index}/?&title=Errored&width=600)"
         return f"![{index}%](https://progress-bar.dev/{index}/?&title=Progress&width=600)" + (
             "\n" + stars_suffix + config_pr_message if index != -1 else "")
 
     # Find the first comment made by the bot
     issue_comment = None
     is_paying_user = chat_logger.is_paying_user()
-    tickets_allocated = 60 if is_paying_user else 3
+    tickets_allocated = 60 if is_paying_user else 5
     ticket_count = max(tickets_allocated - chat_logger.get_ticket_count(), 0)
     use_faster_model = chat_logger.use_faster_model()
     payment_message = f"To create this ticket, I used {'gpt-3.5. ' if use_faster_model else 'gpt-4. '}You have {ticket_count} gpt-4 tickets left." + (" For more gpt-4 tickets, visit [our payment portal.](https://buy.stripe.com/fZe03512h99u0AE6os)" if not is_paying_user else "")
     first_comment = f"{get_comment_header(0)}\n{sep}I am currently looking into this ticket!. I will update the progress of the ticket in this comment. I am currently searching through your code, looking for relevant snippets.\n{sep}## {progress_headers[1]}\nWorking on it...{bot_suffix}{discord_suffix}"
     for comment in comments:
         if comment.user.login == GITHUB_BOT_USERNAME:
             issue_comment = comment
```

### Comparing `sweepai-0.4.8/sweepai/utils/chat_logger.py` & `sweepai-0.4.9/sweepai/utils/chat_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     def use_faster_model(self):
         if self.ticket_collection is None:
             logger.error('Ticket Collection Does Not Exist')
             return True
         if self.is_paying_user():
             return self.get_ticket_count() >= 60
-        return self.get_ticket_count() >= 3
+        return self.get_ticket_count() >= 5
 
 
 def discord_log_error(content):
     try:
         url = DISCORD_WEBHOOK_URL
         data = {'content': content}
         headers = {'Content-Type': 'application/json'}
```

### Comparing `sweepai-0.4.8/sweepai/utils/config/client.py` & `sweepai-0.4.9/sweepai/utils/config/client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/utils/config/server.py` & `sweepai-0.4.9/sweepai/utils/config/server.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/utils/diff.py` & `sweepai-0.4.9/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/utils/event_logger.py` & `sweepai-0.4.9/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/utils/file_change_functions.py` & `sweepai-0.4.9/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/utils/github_utils.py` & `sweepai-0.4.9/sweepai/utils/github_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     return tree, file_list
 
 
 def get_file_contents(repo: Repository, file_path, ref=None):
     if ref is None:
         ref = repo.default_branch
     file = repo.get_contents(file_path, ref=ref)
-    contents = file.decoded_content.decode("utf-8")
+    contents = file.decoded_content.decode("utf-8", errors='replace')
     return contents
 
 
 def search_snippets(
         repo: Repository,
         query: str,
         installation_id: int,
```

### Comparing `sweepai-0.4.8/sweepai/utils/prompt_constructor.py` & `sweepai-0.4.9/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/utils/scorer.py` & `sweepai-0.4.9/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/utils/snippets.py` & `sweepai-0.4.9/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/sweepai/utils/utils.py` & `sweepai-0.4.9/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.8/setup.py` & `sweepai-0.4.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'Sweep software chores',
-    'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/month" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.\n\nDescribe bugs, small features, and refactors like you would to a junior developer, and Sweep:\n1. 🔍 reads your codebase\n2. 📝 plans the changes\n3. ⚡**writes a pull request with code**⚡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Sweep\n* 🔧 Turns issues directly into pull requests (without an IDE)\n* 👀 Addresses developer replies & comments on its PRs\n* 🕵️\u200d♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))\n* 🎊 New: Fixes PRs based on Github Actions feedback\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🍲 Recipes\n#### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. \nFor harder problems, try to provide the same information a human would need. For simpler problems, providing a single line and a file name should suffice.\n\nA good issue might include:\n\n| Where to look <br> **[file name or function name]**| What to do <br> **[change the logic to do this]** | Additional Context (optional) <br> **[there\'s a bug/we need this feature/there\'s this dependency]** |\n|-----------|------------|----------------------|\n|In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an event|because it\'s possible that the comment is on a closed PR|\n|In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).\n\n#### Limitations:\nSweep is unlikely to complete complex issues on the first try, similar to the average junior developer. Here are Sweep\'s limitations(for now):\n- Try to change less than 200 lines of code\n- Try to modify less than 3 files\n- Do not include files with more than 1500 lines of code\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\nWe support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. \n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**\n    - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.\n    - This runs GitHub authentication in your browser.\n\n2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  \n    - Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).\n\n    - ⚡ Start chatting with Sweep Chat! ⚡\n\n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\nTips:\n* 🔍 Relevant searched files will show up on the right. \n* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. \n* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.\n\n## 💰 Pricing\n* We charge $120/month for 60 GPT4 tickets per month.\n* For unpaid users, we offer 3 free GPT4 tickets per month.\n* We also offer unlimited GPT3.5 tickets.\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nSee [🗺️ Roadmap](https://docs.sweep.dev/roadmap)\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
+    'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/month" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n<br>\n<a href="https://www.producthunt.com/posts/sweep-5?utm_source=badge-featured&utm_medium=badge&utm_souce=badge-sweep&#0045;5" target="_blank"><img src="https://api.producthunt.com/widgets/embed-image/v1/featured.svg?post_id=404410&theme=neutral" alt="Sweep - Sweep&#0032;is&#0032;an&#0032;AI&#0045;powered&#0032;junior&#0032;dev&#0032;on&#0032;your&#0032;team&#0046; | Product Hunt" style="width: 175px; height: 36px;" width="175" height="36" /></a>\n</p>\n\n<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.\n\nDescribe bugs, small features, and refactors like you would to a junior developer, and Sweep:\n1. 🔍 reads your codebase\n2. 📝 plans the changes\n3. ⚡**writes a pull request with code**⚡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Sweep\n* 🔧 Turns issues directly into pull requests (without an IDE)\n* 👀 Addresses developer replies & comments on its PRs\n* 🕵️\u200d♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/blogs/building-code-search))\n* 🎊 New: Fixes PRs based on Github Actions feedback\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🍲 Recipes\n#### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. \nFor harder problems, try to provide the same information a human would need. For simpler problems, providing a single line and a file name should suffice.\n\nA good issue might include:\n\n| Where to look <br> **[file name or function name]**| What to do <br> **[change the logic to do this]** | Additional Context (optional) <br> **[there\'s a bug/we need this feature/there\'s this dependency]** |\n|-----------|------------|----------------------|\n|In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an event|because it\'s possible that the comment is on a closed PR|\n|In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).\n\n#### Limitations:\nSweep is unlikely to complete complex issues on the first try, similar to the average junior developer. Here are Sweep\'s limitations(for now):\n- Try to change less than 200 lines of code\n- Try to modify less than 3 files\n- Do not include files with more than 1500 lines of code\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address. Here are the steps to get started:\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to your desired repos\n2. Create a new issue in your repo. The issue should describe the problem or feature you want Sweep to address. For example, you could write "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"\n3. Respond with a message like "Sweep: use a different package instead" to have Sweep retry the issue or pull request. You can also comment on the code for minor changes!\n\nWe support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally. You can collaborate on the plan with Sweep, and then have it create the pull request for you. Here\'s how to use Sweep Chat:\n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**\n    - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.\n    - This runs GitHub authentication in your browser.\n\n2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  \n    - Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).\n\n    - ⚡ Start chatting with Sweep Chat! ⚡\n\n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\nTips:\n* 🔍 Relevant searched files will show up on the right. \n* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. \n* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.\n\n## 💰 Pricing\n* We charge $120/month for 60 GPT4 tickets per month.\n* For unpaid users, we offer 5 free GPT4 tickets per month.\n* We also offer unlimited GPT3.5 tickets.\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nSee [🗺️ Roadmap](https://docs.sweep.dev/roadmap)\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -2,43 +2,44 @@
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils',
 'sweepai.utils.config'] package_data = \ {'': ['*']} install_requires = \
 ['GitPython>=3.1.31,<4.0.0', 'PyGithub==1.58.2', 'config-path>=1.0.3,<2.0.0',
 'gradio>=3.35.2,<4.0.0', 'loguru>=0.6.0,<0.7.0', 'pyyaml>=6.0,<7.0',
 'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0', 'typer>=0.9.0,<0.10.0',
 'urllib3<2.0.0'] entry_points = \ {'console_scripts': ['sweep =
 sweepai.app.cli:app', 'sweepai = sweepai.app.cli:app']} setup_kwargs =
-{ 'name': 'sweepai', 'version': '0.4.8', 'description': 'Sweep software
+{ 'name': 'sweepai', 'version': '0.4.9', 'description': 'Sweep software
 chores', 'long_description': '
  \n [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                 3e61f57ad233]\n
 \n
              \n Bug Reports & Feature Requests â¶  Code Changes\n
 \n\n
 \n\n_[Landing_Page]\n\n\n_[Docs]\n \n\n_[https://dcbadge.vercel.app/api/server/
   sweep-ai?style=flat]\n\n[PyPI]\n\n_[https://static.pepy.tech/badge/sweepai/
 month]\n\n\n_[https://img.shields.io/github/stars/sweepai/sweep]\n\n\n_[https:/
   /img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]\n\n
+ \n[Sweep_-_Sweep_is_an_AI-powered_junior_dev_on_your_team._|_Product_Hunt]\n
 \n\nSweep is an AI junior developer that transforms bug reports & feature
 requests into code changes.\n\nDescribe bugs, small features, and refactors
 like you would to a junior developer, and Sweep:\n1. ð reads your
 codebase\n2. ð plans the changes\n3. â¡**writes a pull request with
 code**â¡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n[Demo]
 (https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
 0af02f2b0e47)\n\n## ð  Sweep\n* ð§ Turns issues directly into pull requests
 (without an IDE)\n* ð Addresses developer replies & comments on its PRs\n*
 ðµï¸\u200dâï¸ Uses embedding-based code search, with popularity reranking
 for repository-level code understanding ([ð Rebuilding our Search Engine in
-a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-
-day))\n* ð New: Fixes PRs based on Github Actions feedback\n* ð New:
-Sweep Chat, a local interface for Sweep (see below)\n\n## ð Getting
-Started\n\n### ð² Recipes\n#### To get the best performance from Sweep, we
-recommend the following approach to writing github issues/chats. \nFor harder
-problems, try to provide the same information a human would need. For simpler
-problems, providing a single line and a file name should suffice.\n\nA good
-issue might include:\n\n| Where to look
+a Day](https://docs.sweep.dev/blogs/building-code-search))\n* ð New: Fixes
+PRs based on Github Actions feedback\n* ð New: Sweep Chat, a local interface
+for Sweep (see below)\n\n## ð Getting Started\n\n### ð² Recipes\n#### To
+get the best performance from Sweep, we recommend the following approach to
+writing github issues/chats. \nFor harder problems, try to provide the same
+information a human would need. For simpler problems, providing a single line
+and a file name should suffice.\n\nA good issue might include:\n\n| Where to
+look
 **[file name or function name]**| What to do
 **[change the logic to do this]** | Additional Context (optional)
 **[there\'s a bug/we need this feature/there\'s this dependency]** |\n|--------
 ---|------------|----------------------|\n|In `sweepai/app/ui.py`|use an os-
 agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an
 event|because it\'s possible that the comment is on a closed PR|\n|In the
 config loader in `packages/server/src/config.ts`|add a third option called
@@ -48,38 +49,43 @@
 the class method or what it does. Also see [â¨ Tips and tricks for Sweep]
 (https://docs.sweep.dev/tricks).\n\n#### Limitations:\nSweep is unlikely to
 complete complex issues on the first try, similar to the average junior
 developer. Here are Sweep\'s limitations(for now):\n- Try to change less than
 200 lines of code\n- Try to modify less than 3 files\n- Do not include files
 with more than 1500 lines of code\n\n### â¨ Sweep Github App\nSetting up Sweep
 is as simple as adding the GitHub bot to a repo, then creating an issue for the
-bot to address.\nWe support all languages GPT4 supports, including Python,
-Typescript, Rust, Go, Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https:
-//github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like
-"Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"\n\n### ð¥ï¸
-Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally.
-Collaborate on the plan with Sweep, then have it create the pull request for
-you. \n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/
-sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note
-that you need **python 3.10+.**\n - Alternatively run `pip3 install --force-
-reinstall sweepai && sweep` if the previous command fails.\n - This runs GitHub
-authentication in your browser.\n\n2. Copy the ðµ blue 8-digit code from your
-terminal into the page. You should only need to do the authentication once. \n
-- Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from
-the dropdown at the top (the Github app must be installed to this
-repository).\n\n - â¡ Start chatting with Sweep Chat! â¡\n\n[https://
-github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/
-gradio-screenshot.png]\n\nTips:\n* ð Relevant searched files will show up on
-the right. \n* ð Sweep Chat creates PRs when the "Create PR" button is
-clicked. \n* ð¡ You can force dark mode by going to http://127.0.0.1:7861/
+bot to address. Here are the steps to get started:\n\n1. Add the [Sweep GitHub
+app](https://github.com/apps/sweep-ai) to your desired repos\n2. Create a new
+issue in your repo. The issue should describe the problem or feature you want
+Sweep to address. For example, you could write "Sweep: In sweepai/app/ui.py use
+an os-agnostic temp directory"\n3. Respond with a message like "Sweep: use a
+different package instead" to have Sweep retry the issue or pull request. You
+can also comment on the code for minor changes!\n\nWe support all languages
+GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.\n\n###
+ð¥ï¸ Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub
+locally. You can collaborate on the plan with Sweep, and then have it create
+the pull request for you. Here\'s how to use Sweep Chat:\n\n**Prerequisites:**
+Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your
+repository\n\n1. Run `pip3 install sweepai && sweep`. Note that you need
+**python 3.10+.**\n - Alternatively run `pip3 install --force-reinstall sweepai
+&& sweep` if the previous command fails.\n - This runs GitHub authentication in
+your browser.\n\n2. Copy the ðµ blue 8-digit code from your terminal into the
+page. You should only need to do the authentication once. \n - Wait a few
+seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown
+at the top (the Github app must be installed to this repository).\n\n - â¡
+Start chatting with Sweep Chat! â¡\n\n[https://github.com/sweepai/sweep/blob/
+856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-
+screenshot.png]\n\nTips:\n* ð Relevant searched files will show up on the
+right. \n* ð Sweep Chat creates PRs when the "Create PR" button is clicked.
+\n* ð¡ You can force dark mode by going to http://127.0.0.1:7861/
 ?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the
 latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep &&
 poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python
 3.10+**.\n\n## ð° Pricing\n* We charge $120/month for 60 GPT4 tickets per
-month.\n* For unpaid users, we offer 3 free GPT4 tickets per month.\n* We also
+month.\n* For unpaid users, we offer 5 free GPT4 tickets per month.\n* We also
 offer unlimited GPT3.5 tickets.\n## ð¤ Contributing\n\nContributions are
 welcome and greatly appreciated! For detailed guidelines on how to contribute,
 please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed
 docs, see [ð Quickstart](https://docs.sweep.dev/).\n\n## ð Story\n\nWe
 were frustrated by small tickets, like simple bug fixes, annoying refactors,
 and small features. Each task required us to open our IDE to fix simple bugs.
 So we decided to leverage the capabilities of ChatGPT to address this directly
```

### Comparing `sweepai-0.4.8/PKG-INFO` & `sweepai-0.4.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.4.8
+Version: 0.4.9
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
@@ -47,14 +47,16 @@
 </a>
 <a href="https://github.com/sweepai/sweep">
     <img src="https://img.shields.io/github/stars/sweepai/sweep" />
 </a>
 <a href="https://twitter.com/sweep__ai">
     <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />
 </a>
+<br>
+<a href="https://www.producthunt.com/posts/sweep-5?utm_source=badge-featured&utm_medium=badge&utm_souce=badge-sweep&#0045;5" target="_blank"><img src="https://api.producthunt.com/widgets/embed-image/v1/featured.svg?post_id=404410&theme=neutral" alt="Sweep - Sweep&#0032;is&#0032;an&#0032;AI&#0045;powered&#0032;junior&#0032;dev&#0032;on&#0032;your&#0032;team&#0046; | Product Hunt" style="width: 175px; height: 36px;" width="175" height="36" /></a>
 </p>
 
 <b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.
 
 Describe bugs, small features, and refactors like you would to a junior developer, and Sweep:
 1. 🔍 reads your codebase
 2. 📝 plans the changes
@@ -63,15 +65,15 @@
 See highlights at https://docs.sweep.dev/examples.
 
 [Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)
 
 ## 🌠 Sweep
 * 🔧 Turns issues directly into pull requests (without an IDE)
 * 👀 Addresses developer replies & comments on its PRs
-* 🕵️‍♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))
+* 🕵️‍♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/blogs/building-code-search))
 * 🎊 New: Fixes PRs based on Github Actions feedback
 * 🎊 New: Sweep Chat, a local interface for Sweep (see below)
 
 ## 🚀 Getting Started
 
 ### 🍲 Recipes
 #### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. 
@@ -90,22 +92,24 @@
 #### Limitations:
 Sweep is unlikely to complete complex issues on the first try, similar to the average junior developer. Here are Sweep's limitations(for now):
 - Try to change less than 200 lines of code
 - Try to modify less than 3 files
 - Do not include files with more than 1500 lines of code
 
 ### ✨ Sweep Github App
-Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.
-We support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.
+Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address. Here are the steps to get started:
+
+1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to your desired repos
+2. Create a new issue in your repo. The issue should describe the problem or feature you want Sweep to address. For example, you could write "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"
+3. Respond with a message like "Sweep: use a different package instead" to have Sweep retry the issue or pull request. You can also comment on the code for minor changes!
 
-1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
-2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py use an os-agnostic temp directory"
+We support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.
 
 ### 🖥️ Sweep Chat
-Sweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. 
+Sweep Chat allows you to interact with Sweep and GitHub locally. You can collaborate on the plan with Sweep, and then have it create the pull request for you. Here's how to use Sweep Chat:
 
 **Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository
 
 1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**
     - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.
     - This runs GitHub authentication in your browser.
 
@@ -127,15 +131,15 @@
 If you want the nightly build and or if the latest build has issues.
 
 1. `git clone https://github.com/sweepai/sweep && poetry install`
 2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.
 
 ## 💰 Pricing
 * We charge $120/month for 60 GPT4 tickets per month.
-* For unpaid users, we offer 3 free GPT4 tickets per month.
+* For unpaid users, we offer 5 free GPT4 tickets per month.
 * We also offer unlimited GPT3.5 tickets.
 ## 🤝 Contributing
 
 Contributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 For more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/).
 
 ## 📘 Story
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.4.8 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.4.9 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: GitPython
 (>=3.1.31,<4.0.0) Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path
 (>=1.0.3,<2.0.0) Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru
 (>=0.6.0,<0.7.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests
 (>=2.28.2,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist:
@@ -14,31 +14,32 @@
   [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                  3e61f57ad233]
                Bug Reports & Feature Requests â¶  Code Changes
       [Landing_Page] [Docs] [https://dcbadge.vercel.app/api/server/sweep-
 ai?style=flat] [PyPI] [https://static.pepy.tech/badge/sweepai/month] [https://
   img.shields.io/github/stars/sweepai/sweep] [https://img.shields.io/twitter/
                 url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]
+   [Sweep_-_Sweep_is_an_AI-powered_junior_dev_on_your_team._|_Product_Hunt]
 Sweep is an AI junior developer that transforms bug reports & feature requests
 into code changes. Describe bugs, small features, and refactors like you would
 to a junior developer, and Sweep: 1. ð reads your codebase 2. ð plans the
 changes 3. â¡**writes a pull request with code**â¡ See highlights at https://
 docs.sweep.dev/examples. [Demo](https://github.com/sweepai/sweep/assets/
 44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47) ## ð  Sweep * ð§ Turns
 issues directly into pull requests (without an IDE) * ð Addresses developer
 replies & comments on its PRs * ðµï¸ââï¸ Uses embedding-based code
 search, with popularity reranking for repository-level code understanding (
-[ð Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-
-rebuilt-our-code-search-engine-in-a-day)) * ð New: Fixes PRs based on Github
-Actions feedback * ð New: Sweep Chat, a local interface for Sweep (see
-below) ## ð Getting Started ### ð² Recipes #### To get the best
-performance from Sweep, we recommend the following approach to writing github
-issues/chats. For harder problems, try to provide the same information a human
-would need. For simpler problems, providing a single line and a file name
-should suffice. A good issue might include: | Where to look
+[ð Rebuilding our Search Engine in a Day](https://docs.sweep.dev/blogs/
+building-code-search)) * ð New: Fixes PRs based on Github Actions feedback *
+ð New: Sweep Chat, a local interface for Sweep (see below) ## ð Getting
+Started ### ð² Recipes #### To get the best performance from Sweep, we
+recommend the following approach to writing github issues/chats. For harder
+problems, try to provide the same information a human would need. For simpler
+problems, providing a single line and a file name should suffice. A good issue
+might include: | Where to look
 **[file name or function name]**| What to do
 **[change the logic to do this]** | Additional Context (optional)
 **[there's a bug/we need this feature/there's this dependency]** | |-----------
 |------------|----------------------| |In `sweepai/app/ui.py`|use an os-
 agnostic temp directory|N/A| |In `on_comment.py`|we should not fire an
 event|because it's possible that the comment is on a closed PR| |In the config
 loader in `packages/server/src/config.ts`|add a third option called "env" to
@@ -47,38 +48,43 @@
 full path. Similarly, to have Sweep use a function, try to mention the class
 method or what it does. Also see [â¨ Tips and tricks for Sweep](https://
 docs.sweep.dev/tricks). #### Limitations: Sweep is unlikely to complete complex
 issues on the first try, similar to the average junior developer. Here are
 Sweep's limitations(for now): - Try to change less than 200 lines of code - Try
 to modify less than 3 files - Do not include files with more than 1500 lines of
 code ### â¨ Sweep Github App Setting up Sweep is as simple as adding the
-GitHub bot to a repo, then creating an issue for the bot to address. We support
-all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C#
-and C++. 1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to
-desired repos 2. Create new issue in repo, like "Sweep: In sweepai/app/ui.py
-use an os-agnostic temp directory" ### ð¥ï¸ Sweep Chat Sweep Chat allows you
-to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep,
-then have it create the pull request for you. **Prerequisites:** Install [Sweep
-GitHub app](https://github.com/apps/sweep-ai) to your repository 1. Run `pip3
-install sweepai && sweep`. Note that you need **python 3.10+.** - Alternatively
-run `pip3 install --force-reinstall sweepai && sweep` if the previous command
+GitHub bot to a repo, then creating an issue for the bot to address. Here are
+the steps to get started: 1. Add the [Sweep GitHub app](https://github.com/
+apps/sweep-ai) to your desired repos 2. Create a new issue in your repo. The
+issue should describe the problem or feature you want Sweep to address. For
+example, you could write "Sweep: In sweepai/app/ui.py use an os-agnostic temp
+directory" 3. Respond with a message like "Sweep: use a different package
+instead" to have Sweep retry the issue or pull request. You can also comment on
+the code for minor changes! We support all languages GPT4 supports, including
+Python, Typescript, Rust, Go, Java, C# and C++. ### ð¥ï¸ Sweep Chat Sweep
+Chat allows you to interact with Sweep and GitHub locally. You can collaborate
+on the plan with Sweep, and then have it create the pull request for you.
+Here's how to use Sweep Chat: **Prerequisites:** Install [Sweep GitHub app]
+(https://github.com/apps/sweep-ai) to your repository 1. Run `pip3 install
+sweepai && sweep`. Note that you need **python 3.10+.** - Alternatively run
+`pip3 install --force-reinstall sweepai && sweep` if the previous command
 fails. - This runs GitHub authentication in your browser. 2. Copy the ðµ blue
 8-digit code from your terminal into the page. You should only need to do the
 authentication once. - Wait a few seconds and Sweep Chat will start. 3. Choose
 a repository from the dropdown at the top (the Github app must be installed to
 this repository). - â¡ Start chatting with Sweep Chat! â¡ [https://
 github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/
 gradio-screenshot.png] Tips: * ð Relevant searched files will show up on the
 right. * ð Sweep Chat creates PRs when the "Create PR" button is clicked. *
 ð¡ You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
 #### From Source If you want the nightly build and or if the latest build has
 issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
 `python sweepai/app/cli.py`. Note that you need **python 3.10+**. ## ð°
 Pricing * We charge $120/month for 60 GPT4 tickets per month. * For unpaid
-users, we offer 3 free GPT4 tickets per month. * We also offer unlimited GPT3.5
+users, we offer 5 free GPT4 tickets per month. * We also offer unlimited GPT3.5
 tickets. ## ð¤ Contributing Contributions are welcome and greatly
 appreciated! For detailed guidelines on how to contribute, please see the
 [CONTRIBUTING.md](CONTRIBUTING.md) file. For more detailed docs, see [ð
 Quickstart](https://docs.sweep.dev/). ## ð Story We were frustrated by small
 tickets, like simple bug fixes, annoying refactors, and small features. Each
 task required us to open our IDE to fix simple bugs. So we decided to leverage
 the capabilities of ChatGPT to address this directly in GitHub. Unlike existing
```

