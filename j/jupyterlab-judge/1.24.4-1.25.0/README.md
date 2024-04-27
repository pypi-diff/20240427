# Comparing `tmp/jupyterlab_judge-1.24.4.tar.gz` & `tmp/jupyterlab_judge-1.25.0.tar.gz`

## Comparing `jupyterlab_judge-1.24.4.tar` & `jupyterlab_judge-1.25.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/.copier-answers.yml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/.yarnrc.yml
--rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/CHANGELOG.md
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/babel.config.js
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/conftest.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jest.config.js
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/setup.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/tsconfig.test.json
--rw-r--r--   0        0        0   435917 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/yarn.lock
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyter-config/nb-config/jupyterlab_judge.json
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyter-config/server-config/jupyterlab_judge.json
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/_version.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/handlers.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/yjudge.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/package.json
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/schemas/jupyterlab-judge/plugin.json
--rw-r--r--   0        0        0    14975 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js.LICENSE.txt
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js
--rw-r--r--   0        0        0     6939 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js
--rw-r--r--   0        0        0    54375 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js
--rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js
--rw-r--r--   0        0        0  4279528 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js.LICENSE.txt
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js
--rw-r--r--   0        0        0    33296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/960.376cb311c5431702de57.js
--rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/remoteEntry.b81a0f7c77284e957c86.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/style.js
--rw-r--r--   0        0        0    38387 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json
--rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/tests/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/tests/test_handlers.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/schema/plugin.json
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/commands.ts
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/constants.ts
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/handler.ts
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/index.ts
--rw-r--r--   0        0        0    16041 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/model.ts
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/tokens.ts
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/toolbar.tsx
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/__tests__/jupyterlab_judge.spec.ts
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionArea.tsx
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionControl.tsx
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionItem.tsx
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionItemStatus.tsx
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionItemWait.tsx
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionItemWaitStatus.tsx
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionList.tsx
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/index.ts
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/problemProvider/HardCodedProblemProvider.ts
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/problemProvider/index.ts
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/problemProvider/problemProvider.ts
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/widgets/JudgeOutputArea.ts
--rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/widgets/JudgePanel.ts
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/widgets/JudgeProblemPanel.ts
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/widgets/JudgeSubmissionArea.tsx
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/widgets/JudgeTerminal.ts
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/widgets/index.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/style/index.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/style/judgeOutputArea.css
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/style/judgePanel.css
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/style/judgeTerminal.css
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/ui-tests/yarn.lock
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/ui-tests/tests/jupyterlab_judge.spec.ts
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/LICENSE
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/README.md
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/pyproject.toml
--rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/PKG-INFO
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/.copier-answers.yml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/.yarnrc.yml
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/babel.config.js
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/conftest.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jest.config.js
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/setup.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/tsconfig.test.json
+-rw-r--r--   0        0        0   435917 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/yarn.lock
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyter-config/nb-config/jupyterlab_judge.json
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyter-config/server-config/jupyterlab_judge.json
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/_version.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/handlers.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/yjudge.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/package.json
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/schemas/jupyterlab-judge/plugin.json
+-rw-r--r--   0        0        0    14975 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js.LICENSE.txt
+-rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js
+-rw-r--r--   0        0        0     6939 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js
+-rw-r--r--   0        0        0    54375 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js
+-rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js
+-rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js
+-rw-r--r--   0        0        0  4279528 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js.LICENSE.txt
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js
+-rw-r--r--   0        0        0    33915 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/960.560036ddbfd0e33374bc.js
+-rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/remoteEntry.933113d1b8fc3f476592.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/style.js
+-rw-r--r--   0        0        0    38387 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/tests/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/jupyterlab_judge/tests/test_handlers.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/schema/plugin.json
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/commands.ts
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/constants.ts
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/handler.ts
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/index.ts
+-rw-r--r--   0        0        0    16056 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/model.ts
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/tokens.ts
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/toolbar.tsx
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/__tests__/jupyterlab_judge.spec.ts
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/components/SubmissionArea.tsx
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/components/SubmissionControl.tsx
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/components/SubmissionItem.tsx
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/components/SubmissionItemStatus.tsx
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/components/SubmissionItemWait.tsx
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/components/SubmissionItemWaitStatus.tsx
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/components/SubmissionList.tsx
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/components/index.ts
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/problemProvider/HardCodedProblemProvider.ts
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/problemProvider/index.ts
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/problemProvider/problemProvider.ts
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/widgets/JudgeOutputArea.ts
+-rw-r--r--   0        0        0    23847 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/widgets/JudgePanel.ts
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/widgets/JudgeProblemPanel.ts
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/widgets/JudgeSubmissionArea.tsx
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/widgets/JudgeTerminal.ts
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/src/widgets/index.ts
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/style/index.js
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/style/judgeOutputArea.css
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/style/judgePanel.css
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/style/judgeTerminal.css
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/ui-tests/tests/jupyterlab_judge.spec.ts
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/LICENSE
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/README.md
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/pyproject.toml
+-rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.25.0/PKG-INFO
```

### Comparing `jupyterlab_judge-1.24.4/.copier-answers.yml` & `jupyterlab_judge-1.25.0/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/CHANGELOG.md` & `jupyterlab_judge-1.25.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.25.0
+
+([Full Changelog](https://github.com/team-monolith-product/jupyterlab-judge/compare/v1.24.4...a3a41129d26ebdb55328d0b60762e47e0d50cb1c))
+
+### Merged PRs
+
+- Expand submissions to have details [#59](https://github.com/team-monolith-product/jupyterlab-judge/pull/59) ([@a3626a](https://github.com/a3626a))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/team-monolith-product/jupyterlab-judge/graphs/contributors?from=2024-04-13&to=2024-04-27&type=c))
+
+[@a3626a](https://github.com/search?q=repo%3Ateam-monolith-product%2Fjupyterlab-judge+involves%3Aa3626a+updated%3A2024-04-13..2024-04-27&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.24.4
 
 ([Full Changelog](https://github.com/team-monolith-product/jupyterlab-judge/compare/v1.24.3...5364c40d9549fb4817110ffe9c841f46209c18ee))
 
 ### Merged PRs
 
 - fix: rstrip new line [#58](https://github.com/team-monolith-product/jupyterlab-judge/pull/58) ([@a3626a](https://github.com/a3626a))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/team-monolith-product/jupyterlab-judge/graphs/contributors?from=2024-04-08&to=2024-04-13&type=c))
 
 [@a3626a](https://github.com/search?q=repo%3Ateam-monolith-product%2Fjupyterlab-judge+involves%3Aa3626a+updated%3A2024-04-08..2024-04-13&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.24.3
 
 ([Full Changelog](https://github.com/team-monolith-product/jupyterlab-judge/compare/v1.24.2...668b1d002a29e4df3e7d9edf181841088dd27f09))
 
 ### Merged PRs
 
 - fix: make prompt argument optional [#57](https://github.com/team-monolith-product/jupyterlab-judge/pull/57) ([@a3626a](https://github.com/a3626a))
```

### Comparing `jupyterlab_judge-1.24.4/RELEASE.md` & `jupyterlab_judge-1.25.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jest.config.js` & `jupyterlab_judge-1.25.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/package.json` & `jupyterlab_judge-1.25.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'1.25.0'"}*

```diff
@@ -231,9 +231,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.24.4"
+    "version": "1.25.0"
 }
```

### Comparing `jupyterlab_judge-1.24.4/tsconfig.json` & `jupyterlab_judge-1.25.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/yarn.lock` & `jupyterlab_judge-1.25.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/__init__.py` & `jupyterlab_judge-1.25.0/jupyterlab_judge/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/handlers.py` & `jupyterlab_judge-1.25.0/jupyterlab_judge/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/yjudge.py` & `jupyterlab_judge-1.25.0/jupyterlab_judge/yjudge.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/package.json` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9796666666666667%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.933113d1b8fc3f476592.js'}}",*

 * * "'version'": "'1.25.0'"}*

```diff
@@ -135,15 +135,15 @@
         "schema/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/team-monolith-product/jupyterlab-judge",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b81a0f7c77284e957c86.js",
+            "load": "static/remoteEntry.933113d1b8fc3f476592.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_judge"
                 },
@@ -236,9 +236,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.24.4"
+    "version": "1.25.0"
 }
```

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'1.25.0'"}*

```diff
@@ -231,9 +231,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.24.4"
+    "version": "1.25.0"
 }
```

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/960.376cb311c5431702de57.js` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/960.560036ddbfd0e33374bc.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,50 +1,51 @@
 "use strict";
 (self.webpackChunkjupyterlab_judge = self.webpackChunkjupyterlab_judge || []).push([
     [960], {
         960: (e, t, s) => {
             s.r(t), s.d(t, {
-                HardCodedProblemProvider: () => q,
-                IJudgePanelFactory: () => R,
-                IJudgeSignal: () => z,
-                IJudgeSubmissionAreaFactory: () => K,
-                IJudgeTerminalFactory: () => B,
+                HardCodedProblemProvider: () => H,
+                IJudgePanelFactory: () => K,
+                IJudgeSignal: () => q,
+                IJudgeSubmissionAreaFactory: () => B,
+                IJudgeTerminalFactory: () => U,
                 IProblemProvider: () => $,
-                ISubmissionListFactory: () => U,
-                JudgeDocument: () => E,
+                ISubmissionListFactory: () => z,
+                JudgeDocument: () => T,
                 JudgeDocumentFactory: () => k,
                 JudgeError: () => w,
                 JudgeKernelImplementationError: () => S,
                 JudgeKernelNotConnectedError: () => v,
-                JudgeKernelReconnectingFailedError: () => j,
+                JudgeKernelReconnectingFailedError: () => E,
                 JudgeModel: () => M,
                 JudgeOutputArea: () => Ie,
                 JudgePanel: () => I,
                 JudgeProblemPanel: () => C,
-                JudgeSubmissionArea: () => Se,
+                JudgeSubmissionArea: () => Ee,
                 JudgeTerminal: () => ke,
-                SubmissionArea: () => ye,
-                SubmissionControl: () => V,
-                SubmissionItem: () => se,
-                SubmissionItemStatus: () => ee,
-                SubmissionItemWait: () => de,
-                SubmissionListImpl: () => me,
-                SubmissionListSignalWrapper: () => ce,
-                default: () => Ne,
-                factoryContext: () => ve,
-                openOrCreateFromId: () => A,
-                transContext: () => we
+                SubmissionArea: () => Ce,
+                SubmissionControl: () => Y,
+                SubmissionItem: () => ne,
+                SubmissionItemStatus: () => te,
+                SubmissionItemWait: () => le,
+                SubmissionListImpl: () => he,
+                SubmissionListSignalWrapper: () => me,
+                ValidationFailedError: () => j,
+                default: () => Ae,
+                factoryContext: () => Se,
+                openOrCreateFromId: () => O,
+                transContext: () => ve
             });
-            var n = s(4072),
-                o = s(1464),
-                i = s(8937),
-                r = s(6805),
-                a = s(7594),
-                d = s(2294),
-                l = s(3195),
+            var n = s(2677),
+                o = s(7756),
+                i = s(7560),
+                r = s(1731),
+                a = s(5114),
+                d = s(5048),
+                l = s(802),
                 u = s(6029),
                 c = s.n(u);
             const m = "jupyterlab-judge",
                 h = ".jce-judge",
                 p = "jupyterlab-judge";
             var g;
             ! function(e) {
@@ -77,15 +78,15 @@
                         name: "save",
                         widget: t(e, s)
                     }]
                 }
             }(g || (g = {}));
             var _ = s(4882),
                 b = s(5536),
-                y = s(3413);
+                y = s(2682);
             class C extends _.Panel {
                 constructor(e, t) {
                     super(), this._model = e.model, this._trans = e.translator.load(m), this._markdownRenderer = t.createRenderer("text/markdown"), this._markdownRenderer.addClass("jp-JudgePanel-problem"), this.addWidget(this._markdownRenderer)
                 }
                 renderProblem() {
                     var e, t;
                     this._markdownRenderer.renderModel(new y.MimeModel({
@@ -115,14 +116,19 @@
                 }
             }
             class S extends w {
                 constructor(e) {
                     super(e), this.name = this.constructor.name
                 }
             }
+            class E extends w {
+                constructor(e) {
+                    super(e), this.name = this.constructor.name
+                }
+            }
             class j extends w {
                 constructor(e) {
                     super(e), this.name = this.constructor.name
                 }
             }
             class I extends _.BoxPanel {
                 constructor(e) {
@@ -261,46 +267,68 @@
                     };
                     for (let e = 0; e < 20 && "idle" !== a.kernelDisplayStatus; e++) await new Promise((e => setTimeout(e, 1e3)));
                     if ("idle" !== a.kernelDisplayStatus) {
                         if ("connecting" !== a.kernelDisplayStatus) throw console.warn(`Kernel is still ${a.kernelDisplayStatus} after 20s`), new w(this._trans.__("Kernel is not responding. Please try again."));
                         {
                             const e = d._reconnectAttempt;
                             if (void 0 === e) throw new S(this._trans.__("Kernel is still connecting. Please check your network."));
-                            if (e > 0) throw new j(this._trans.__("Kernel is still connecting. Please check your network."));
+                            if (e > 0) throw new E(this._trans.__("Kernel is still connecting. Please check your network."));
                             if (0 === e) throw new v(this._trans.__("Kernel is still connecting. Please check your network."))
                         }
                     }
                     const l = [];
                     for (const e of i) {
                         const t = await this.runWithInput(d, n, s, e);
                         l.push(t), this.model.submissionStatus = {
                             type: "progress",
                             runCount: l.length,
                             totalCount: i.length
                         }
                     }
-                    let u = null;
-                    const c = await this.model.validate(l.map((e => e.output)));
-                    u = c.acceptedCount === c.totalCount ? "AC" : l.some((e => "RE" === e.status)) ? "RE" : l.some((e => "OLE" === e.status)) ? "OLE" : l.some((e => "TLE" === e.status)) ? "TLE" : "WA", await d.shutdown(), d.dispose();
-                    const m = await this.model.submit({
+                    const u = await this.model.validate(l.map((e => e.output)));
+                    if (null === u) throw new j(this._trans.__("Validation failed. Please try again"));
+                    await d.shutdown(), d.dispose();
+                    const c = await this.model.submit({
                         problemId: s.id,
-                        status: u,
                         code: n,
-                        cpuTime: l.map((e => e.cpuTime)).reduce(((e, t) => e + t), 0) / l.length,
-                        acceptedCount: c.acceptedCount,
-                        totalCount: c.totalCount,
-                        token: c.token,
+                        token: u.token,
                         language: "python",
-                        memory: 0
+                        details: l.map(((e, t) => {
+                            switch (e.status) {
+                                case "OK":
+                                    return u.results[t] ? {
+                                        status: "AC",
+                                        cpuTime: e.cpuTime,
+                                        memory: 0
+                                    } : {
+                                        status: "WA",
+                                        answer: e.output,
+                                        cpuTime: e.cpuTime,
+                                        memory: 0
+                                    };
+                                case "TLE":
+                                    return {
+                                        status: "TLE", cpuTime: e.cpuTime, memory: 0
+                                    };
+                                case "OLE":
+                                    return {
+                                        status: "OLE", cpuTime: e.cpuTime, memory: 0
+                                    };
+                                case "RE":
+                                    return {
+                                        status: "RE", memory: 0, cpuTime: e.cpuTime, errorName: e.errorName, errorValue: e.errorValue
+                                    }
+                            }
+                        }))
                     }, this);
                     this.model.submissionStatus = {
                         type: "idle"
                     }, this._submitted.emit({
                         widget: this,
-                        submission: m,
+                        submission: c,
                         problem: s
                     })
                 }
                 async runWithInput(e, t, s, n) {
                     const o = `\nimport io\nimport base64\n\ndef input(prompt=None):  \t\n    r = JUDGE_INPUT_STRING_IO.${"one_line"===s.inputTransferType?"readline":"read"}().rstrip('\\n')\n    if not r:  \t\t\n        return ''\n    return r\n\nJUDGE_INPUT_STRING_IO = io.StringIO()\n`;
                     await e.requestExecute({
                         code: o,
@@ -317,46 +345,63 @@
                     }
                     const r = {
                             code: "\nJUDGE_INPUT_STRING_IO.seek(0)\n" + t,
                             stop_on_error: !0,
                             allow_stdin: !0
                         },
                         a = Date.now(),
-                        d = e.requestExecute(r, !0, {}),
-                        l = {
-                            output: "",
-                            status: "OK",
-                            cpuTime: 0
-                        };
+                        d = e.requestExecute(r, !0, {});
+                    let l = {
+                        output: "",
+                        status: "OK",
+                        cpuTime: 0
+                    };
                     d.onIOPub = e => {
                         switch (e.header.msg_type) {
                             case "stream": {
                                 const t = e;
                                 "stdout" === t.content.name && (l.output = l.output.concat(t.content.text));
                                 break
                             }
-                            case "error":
-                                l.status = "RE"
+                            case "error": {
+                                const t = e;
+                                l = {
+                                    status: "RE",
+                                    errorName: t.content.ename,
+                                    errorValue: t.content.evalue,
+                                    output: l.output,
+                                    cpuTime: 0
+                                };
+                                break
+                            }
                         }
                     };
                     const u = 1e3 * s.timeout,
                         c = new Promise((e => {
                             setTimeout((() => {
                                 e(0)
                             }), 1.2 * u)
                         }));
-                    if (0 === await Promise.race([d.done, c])) d.dispose(), await e.interrupt(), l.status = "TLE";
+                    if (0 === await Promise.race([d.done, c])) d.dispose(), await e.interrupt(), l = {
+                        status: "TLE",
+                        output: l.output,
+                        cpuTime: null
+                    };
                     else {
                         const e = Date.now() - a;
-                        e > u ? l.status = "TLE" : l.cpuTime = e
+                        l.cpuTime = e, e > u && (l = {
+                            status: "TLE",
+                            output: l.output,
+                            cpuTime: e
+                        })
                     }
                     return l
                 }
             }
-            class E extends d.DocumentWidget {
+            class T extends d.DocumentWidget {
                 constructor(e) {
                     super(e), g.getDefaultItems(this.content, e.translator).forEach((e => {
                         this.toolbar.addItem(e.name, e.widget)
                     }))
                 }
             }
             class k extends d.ABCWidgetFactory {
@@ -373,31 +418,31 @@
                         sessionContextDialogs: this._sessionContextDialogs,
                         submitted: this._submitted,
                         executed: this._executed,
                         judgeSubmissionAreaFactory: this._judgeSubmissionAreaFactory,
                         judgeTerminalFactory: this._judgeTerminalFactory,
                         submissionListFactory: this._submissionListFactory
                     });
-                    return t.title.icon = x, new E({
+                    return t.title.icon = x, new T({
                         content: t,
                         context: e,
                         commands: this._commands,
                         translator: this.translator
                     })
                 }
             }
-            var T, P = s(2818),
-                F = s(8093),
-                N = s(4901),
-                J = s(7263);
+            var P, F = s(7520),
+                N = s(8093),
+                A = s(4901),
+                J = s(5421);
             class M {
                 constructor(e, t) {
-                    this._contentChanged = new N.Signal(this), this._stateChanged = new N.Signal(this), this._isDisposed = !1, this._dirty = !1, this._problemChanged = new N.Signal(this), this._submissionsChanged = new N.Signal(this), this._submissionStatus = {
+                    this._contentChanged = new A.Signal(this), this._stateChanged = new A.Signal(this), this._isDisposed = !1, this._dirty = !1, this._problemChanged = new A.Signal(this), this._submissionsChanged = new A.Signal(this), this._submissionStatus = {
                         type: "idle"
-                    }, this._submissionStatusChanged = new N.Signal(this), this.sharedModel = new M.YJudge, this.sharedModel.changed.connect((async (e, t) => {
+                    }, this._submissionStatusChanged = new A.Signal(this), this.sharedModel = new M.YJudge, this.sharedModel.changed.connect((async (e, t) => {
                         t.problemIdChange && (this._problem = await this._problemProvider.getProblem(t.problemIdChange), this._problemChanged.emit(this._problem)), t.stateChange && t.stateChange.forEach((e => {
                             "dirty" === e.name && (this.dirty = e.newValue)
                         })), t.sourceChange && (this._contentChanged.emit(), this.dirty = !0)
                     })), this._codeModel = new J.CodeCellModel({
                         sharedModel: this.sharedModel.yCodeCell
                     }), this._codeModel.mimeType = "text/x-python", this._problem = null, this._problemProvider = e, this._collaborationEnabled = !!(null == t ? void 0 : t.collaborationEnabled)
                 }
@@ -425,15 +470,15 @@
                     return !1
                 }
                 set readOnly(e) {}
                 get isDisposed() {
                     return this._isDisposed
                 }
                 dispose() {
-                    this.isDisposed || (this._isDisposed = !0, N.Signal.clearData(this))
+                    this.isDisposed || (this._isDisposed = !0, A.Signal.clearData(this))
                 }
                 initialize() {}
                 get defaultKernelName() {
                     return `Judge: Problem ${this.sharedModel.problemId}`
                 }
                 get defaultKernelLanguage() {
                     return "python"
@@ -510,15 +555,15 @@
                     return await this._problemProvider.validate(this.sharedModel.problemId, e)
                 }
                 async submit(e, t) {
                     const s = await this._problemProvider.submit(e, t);
                     return this._submissionsChanged.emit(await this._problemProvider.getSubmissions(this.sharedModel.problemId)), s
                 }
             }
-            async function A(e, t, s) {
+            async function O(e, t, s) {
                     const n = await e.getProblem(s);
                     if (n) {
                         const o = n.title,
                             i = `${h}/${s}/${o}.judge`,
                             r = `${h}`;
                         await t.services.contents.save(r, {
                             name: r,
@@ -528,15 +573,15 @@
                         return await t.services.contents.save(a, {
                             name: a,
                             type: "directory"
                         }), await async function(e, t, s, n) {
                             try {
                                 await t.services.contents.get(s)
                             } catch (o) {
-                                throw o instanceof P.ServerConnection.ResponseError && 404 === o.response.status && await t.services.contents.save(s, {
+                                throw o instanceof F.ServerConnection.ResponseError && 404 === o.response.status && await t.services.contents.save(s, {
                                     name: s,
                                     type: "file",
                                     format: "text",
                                     content: await M.newFileContent(e, n)
                                 }), o
                             } finally {
                                 return t.openOrReveal(s)
@@ -560,15 +605,15 @@
                         preferredLanguage(e) {
                             return "python"
                         }
                         createNew(t) {
                             return new e(this._problemProviderFactory(), t)
                         }
                     };
-                    class t extends F.YDocument {
+                    class t extends N.YDocument {
                         constructor() {
                             super(), this._version = "1.0.0", this._problemId = this.ydoc.getText("problem_id"), this._source = this.ydoc.getText("source"), this._outputs = this.ydoc.getArray("outputs"), this._metadata = this.ydoc.getMap("metadata"), this._ycodeCell = new s(this, this._source, this._outputs), this._problemId.observe((e => {
                                 this._changed.emit({
                                     problemIdChange: this.problemId
                                 })
                             })), this._ycodeCell.changed.connect(((e, t) => {
                                 this._changed.emit(t)
@@ -603,23 +648,23 @@
                         get version() {
                             return this._version
                         }
                     }
                     e.YJudge = t;
                     class s {
                         constructor(e, t, s) {
-                            this.id = "", this.cell_type = "code", this.execution_count = 0, this.isStandalone = !0, this.notebook = null, this.metadata = {}, this.metadataChanged = new N.Signal(this), this._sourceObserver = e => {
+                            this.id = "", this.cell_type = "code", this.execution_count = 0, this.isStandalone = !0, this.notebook = null, this.metadata = {}, this.metadataChanged = new A.Signal(this), this._sourceObserver = e => {
                                 this._changed.emit({
                                     sourceChange: e.changes.delta
                                 })
                             }, this._outputsObserver = e => {
                                 this._changed.emit({
                                     outputsChange: e.changes.delta
                                 })
-                            }, this._changed = new N.Signal(this), this._isDisposed = !1, this._disposed = new N.Signal(this), this._yjudge = e, this._source = t, this._outputs = s, this._source.observe(this._sourceObserver), this._outputs.observe(this._outputsObserver)
+                            }, this._changed = new A.Signal(this), this._isDisposed = !1, this._disposed = new A.Signal(this), this._yjudge = e, this._source = t, this._outputs = s, this._source.observe(this._sourceObserver), this._outputs.observe(this._outputsObserver)
                         }
                         get changed() {
                             return this._changed
                         }
                         get outputs() {
                             return this.getOutputs()
                         }
@@ -687,15 +732,15 @@
                         get disposed() {
                             return this._disposed
                         }
                         get isDisposed() {
                             return this._isDisposed
                         }
                         dispose() {
-                            this._isDisposed || (this._isDisposed = !0, this._source.unobserve(this._sourceObserver), this._outputs.unobserve(this._outputsObserver), this._disposed.emit(), N.Signal.clearData(this))
+                            this._isDisposed || (this._isDisposed = !0, this._source.unobserve(this._sourceObserver), this._outputs.unobserve(this._outputsObserver), this._disposed.emit(), A.Signal.clearData(this))
                         }
                         get ysource() {
                             return this._source
                         }
                         get awareness() {
                             return this._yjudge.awareness
                         }
@@ -711,26 +756,26 @@
                             judge_format: 1
                         };
                         return JSON.stringify(o)
                     }
                 }(M || (M = {})),
                 function(e) {
                     e.open = `${p}:plugin:open`, e.openOrCreateFromId = `${p}:plugin:open-or-create-from-id`, e.execute = `${p}:plugin:execute`, e.undo = `${p}:plugin:undo`, e.redo = `${p}:plugin:redo`, e.run = `${p}:plugin:run`, e.runAll = `${p}:plugin:run-all`
-                }(T || (T = {}));
-            var O = s(2232),
-                D = s(797),
-                L = s(5099),
-                W = s(7930);
-            const $ = new W.Token(`${p}:IProblemProvider`),
-                R = new W.Token(`${p}:IJudgePanelFactory`),
-                K = new W.Token(`${p}:IJudgeSubmissionAreaFactory`),
-                B = new W.Token(`${p}:IJudgeTerminalFactory`),
-                U = new W.Token(`${p}:ISubmissionListFactory`),
-                z = new W.Token(`${p}:IJudgeSignal`);
-            class q {
+                }(P || (P = {}));
+            var D = s(2377),
+                L = s(9874),
+                W = s(2832),
+                R = s(7930);
+            const $ = new R.Token(`${p}:IProblemProvider`),
+                K = new R.Token(`${p}:IJudgePanelFactory`),
+                B = new R.Token(`${p}:IJudgeSubmissionAreaFactory`),
+                U = new R.Token(`${p}:IJudgeTerminalFactory`),
+                z = new R.Token(`${p}:ISubmissionListFactory`),
+                q = new R.Token(`${p}:IJudgeSignal`);
+            class H {
                 constructor() {
                     this.problems = {
                         1: {
                             id: "1",
                             title: "덧셈",
                             timeout: 1,
                             inputTransferType: "one_line",
@@ -754,56 +799,52 @@
                     }, this._idToSubmissions = {}
                 }
                 async getTestCases(e) {
                     return this.problems[e].testCases
                 }
                 async validate(e, t) {
                     const s = this.problems[e].outputs;
-                    if (s.length !== t.length) return {
-                        token: null,
-                        totalCount: s.length,
-                        acceptedCount: 0
-                    };
-                    let n = 0;
-                    for (let e = 0; e < s.length; e++) s[e].trim() === t[e].trim() && (n += 1);
-                    return {
+                    return s.length !== t.length ? null : {
                         token: null,
-                        totalCount: s.length,
-                        acceptedCount: n
+                        results: s.map(((e, s) => e.trim() === t[s].trim()))
                     }
                 }
                 async getProblem(e) {
                     return this.problems[e]
                 }
                 async getSubmissions(e) {
                     var t;
                     return null !== (t = this._idToSubmissions[e]) && void 0 !== t ? t : []
                 }
                 async submit(e) {
-                    void 0 === this._idToSubmissions[e.problemId] && (this._idToSubmissions[e.problemId] = []);
-                    const t = {
+                    let t;
+                    void 0 === this._idToSubmissions[e.problemId] && (this._idToSubmissions[e.problemId] = []), t = e.details.every((e => "AC" === e.status)) ? "AC" : e.details.some((e => "RE" === e.status)) ? "RE" : e.details.some((e => "OLE" === e.status)) ? "OLE" : e.details.some((e => "TLE" === e.status)) ? "TLE" : "WA";
+                    const s = {
                         ...e,
+                        status: t,
                         id: this._idToSubmissions[e.problemId].length.toString(),
                         image: "",
                         userId: "",
-                        createdAt: (new Date).toISOString()
+                        createdAt: (new Date).toISOString(),
+                        acceptedCount: e.details.filter((e => "AC" === e.status)).length,
+                        totalCount: e.details.length
                     };
-                    return this._idToSubmissions[e.problemId].push(t), t
+                    return this._idToSubmissions[e.problemId].push(s), s
                 }
             }
-            var H = s(3848),
-                G = s(8149),
-                Q = s.n(G);
+            var G = s(3848),
+                V = s(8149),
+                Q = s.n(V);
 
-            function V(e) {
-                const t = (0, u.useContext)(we),
+            function Y(e) {
+                const t = (0, u.useContext)(ve),
                     [s, n] = (0, u.useState)(!1);
-                return c().createElement(Y, {
+                return c().createElement(X, {
                     className: e.className
-                }, c().createElement(X, {
+                }, c().createElement(Z, {
                     onClick: async () => {
                         n(!0);
                         try {
                             await e.panel.judge()
                         } catch (s) {
                             let o = "";
                             if (o = s instanceof w ? s.message : t.__("An error occurred during submission."), e.panel.model.submissionStatus = {
@@ -812,18 +853,18 @@
                                 }, n(!1), !(s instanceof v)) throw s
                         }
                         n(!1)
                     },
                     disabled: s
                 }, t.__("Submit")))
             }
-            const Y = Q().div`
+            const X = Q().div`
   background: var(--jp-layout-color2);
 `,
-                X = Q().button`
+                Z = Q().button`
   display: block;
   margin-top: 12px;
   margin-left: 20px;
   margin-right: 20px;
   padding: 11px 17px;
 
   cursor: pointer;
@@ -852,18 +893,18 @@
     cursor: not-allowed;
   }
 
   :not(:disabled):hover {
     background: var(--jp-brand-color0);
   }
 `;
-            var Z = s(8671);
+            var ee = s(1363);
 
-            function ee(e) {
-                const t = (0, u.useContext)(we);
+            function te(e) {
+                const t = (0, u.useContext)(ve);
                 let s = "",
                     n = "";
                 switch (e.status) {
                     case "AC":
                         s = `👍 ${t.__("Accepted")}`;
                         break;
                     case "WA":
@@ -877,129 +918,129 @@
                         break;
                     case "OLE":
                         s = `👀 ${t.__("Output Limit")}`;
                         break;
                     case "IE":
                         s = `☠ ${t.__("Please Try Again")}`
                 }
-                return c().createElement(te, {
+                return c().createElement(se, {
                     className: e.className,
                     title: n
                 }, s)
             }
-            const te = Q().span``;
+            const se = Q().span``;
 
-            function se(e) {
-                const t = (0, u.useContext)(we),
-                    s = Z.Time.formatHuman(new Date(e.submission.createdAt)),
-                    n = Z.Time.format(new Date(e.submission.createdAt));
-                return c().createElement(ne, {
+            function ne(e) {
+                const t = (0, u.useContext)(ve),
+                    s = ee.Time.formatHuman(new Date(e.submission.createdAt)),
+                    n = ee.Time.format(new Date(e.submission.createdAt));
+                return c().createElement(oe, {
                     className: e.className
-                }, c().createElement(oe, {
+                }, c().createElement(ie, {
                     status: e.submission.status,
                     acceptedCount: e.submission.acceptedCount,
                     totalCount: e.submission.totalCount
-                }), c().createElement(ie, {
+                }), c().createElement(re, {
                     onClick: () => {
                         e.setCode(e.submission.code)
                     },
                     title: e.submission.code.substring(0, 1e3)
-                }, t.__("Load this submission")), c().createElement(re, {
+                }, t.__("Load this submission")), c().createElement(ae, {
                     title: n
                 }, s))
             }
-            const ne = Q().li`
+            const oe = Q().li`
   display: flex;
   padding: 5px 12px;
   height: 16px;
 
   font-family: var(--jp-ui-font-family);
   font-style: normal;
   font-size: 12px;
   line-height: 16px;
 `,
-                oe = Q()(ee)`
+                ie = Q()(te)`
   height: 16px;
   flex-grow: 0;
   flex-shrink: 0;
 
   width: 101px;
   margin-right: 8px;
 `,
-                ie = Q().button`
+                re = Q().button`
   height: 16px;
   flex-grow: 0;
   flex-shrink: 0;
 
   all: unset;
   cursor: pointer;
 
   font-family: var(--jp-ui-font-family);
   font-style: normal;
   font-weight: 700;
   font-size: 12px;
   line-height: 16px;
   color: var(--jp-brand-color1);
 `,
-                re = Q().span`
+                ae = Q().span`
   height: 16px;
   flex-grow: 1;
   flex-shrink: 1;
 
   text-align: right;
 
   font-family: var(--jp-ui-font-family);
   font-style: normal;
   font-weight: 400;
   font-size: 12px;
   line-height: 16px;
 
   color: var(--jp-ui-font-color3);
 `,
-                ae = Q().span``;
+                de = Q().span``;
 
-            function de(e) {
-                return c().createElement(le, {
+            function le(e) {
+                return c().createElement(ue, {
                     className: e.className
-                }, c().createElement(ue, {
+                }, c().createElement(ce, {
                     status: e.status
                 }))
             }
-            const le = Q().li`
+            const ue = Q().li`
   display: flex;
   padding: 5px 12px;
   height: 16px;
 
   font-family: var(--jp-ui-font-family);
   font-style: normal;
   font-size: 12px;
   line-height: 16px;
 `,
-                ue = Q()((function(e) {
+                ce = Q()((function(e) {
                     const {
                         status: t
-                    } = e, s = (0, u.useContext)(we);
-                    return "idle" === t.type ? c().createElement(c().Fragment, null) : "error" === t.type ? c().createElement(ae, {
+                    } = e, s = (0, u.useContext)(ve);
+                    return "idle" === t.type ? c().createElement(c().Fragment, null) : "error" === t.type ? c().createElement(de, {
                         className: e.className
-                    }, `🚫 ${t.errorDetails}`) : c().createElement(ae, {
+                    }, `🚫 ${t.errorDetails}`) : c().createElement(de, {
                         className: e.className
                     }, 0 === t.totalCount ? `⌛ ${s.__("In Progress")}` : `⌛ ${s.__("In Progress")} (${t.runCount}/${t.totalCount})`)
                 }))`
   height: 16px;
   flex-grow: 0;
   flex-shrink: 0;
 
   margin-right: 8px;
 `;
 
-            function ce(e) {
-                const t = (0, H.useQueryClient)(),
+            function me(e) {
+                const t = (0, G.useQueryClient)(),
                     {
                         submissionListFactory: s
-                    } = (0, u.useContext)(ve);
+                    } = (0, u.useContext)(Se);
                 return c().createElement(o.UseSignal, {
                     signal: e.model.problemChanged,
                     initialSender: e.model,
                     initialArgs: e.model.problem
                 }, ((n, i) => c().createElement(o.UseSignal, {
                     signal: e.model.submissionsChanged,
                     initialSender: e.model
@@ -1021,43 +1062,43 @@
                             e.model.source = t
                         },
                         submissionStatus: null != n ? n : null
                     })))
                 }))))
             }
 
-            function me(e) {
-                const t = (0, u.useContext)(we);
-                if (null === e.problemId) return c().createElement(_e, {
+            function he(e) {
+                const t = (0, u.useContext)(ve);
+                if (null === e.problemId) return c().createElement(be, {
                     className: e.className
                 }, "⌛ ", t.__("Loading History"));
                 const {
                     data: s,
                     isLoading: n
-                } = (0, H.useQuery)(["submissions", e.problemId], e.getSubmissions);
-                if (n) return c().createElement(_e, {
+                } = (0, G.useQuery)(["submissions", e.problemId], e.getSubmissions);
+                if (n) return c().createElement(be, {
                     className: e.className
                 }, "⌛ ", t.__("Loading History"));
-                if (void 0 === s) return c().createElement(_e, {
+                if (void 0 === s) return c().createElement(be, {
                     className: e.className
                 }, "🚫 ", t.__("History Not Available"));
                 const o = e.submissionStatus && "idle" === e.submissionStatus.type;
-                return 0 === s.length && o ? c().createElement(be, {
+                return 0 === s.length && o ? c().createElement(ye, {
                     className: e.className
-                }, t.__("Submit your code to get results here.")) : c().createElement(he, {
+                }, t.__("Submit your code to get results here.")) : c().createElement(pe, {
                     className: e.className
-                }, e.submissionStatus && "idle" !== e.submissionStatus.type && c().createElement(ge, {
+                }, e.submissionStatus && "idle" !== e.submissionStatus.type && c().createElement(_e, {
                     status: e.submissionStatus
-                }), s.map((t => c().createElement(pe, {
+                }), s.map((t => c().createElement(ge, {
                     submission: t,
                     key: t.id,
                     setCode: e.setCode
                 }))))
             }
-            const he = Q().ul`
+            const pe = Q().ul`
   padding: 7px 0px 0px 0px;
   margin: 0px;
 
   overflow-y: auto;
 
   /* width */
   ::-webkit-scrollbar {
@@ -1066,73 +1107,73 @@
 
   /* Handle */
   ::-webkit-scrollbar-thumb {
     background: var(--jp-border-color0);
     border-radius: 12px;
   }
 `,
-                pe = Q()(se)``,
-                ge = Q()(de)``,
-                _e = Q().div`
+                ge = Q()(ne)``,
+                _e = Q()(le)``,
+                be = Q().div`
   text-align: center;
   padding: 5px;
   font-size: var(--jp-ui-font-size2);
 `,
-                be = Q().div`
+                ye = Q().div`
   padding: 12px;
   font-weight: 700;
   font-size: 12px;
   line-height: 16px;
   color: var(--jp-ui-font-color3);
 `;
 
-            function ye(e) {
-                const t = (0, u.useContext)(we);
-                return null === e.model ? c().createElement("div", null, t.__("No Submission History Found.")) : c().createElement(Ce, null, c().createElement(fe, {
+            function Ce(e) {
+                const t = (0, u.useContext)(ve);
+                return null === e.model ? c().createElement("div", null, t.__("No Submission History Found.")) : c().createElement(fe, null, c().createElement(xe, {
                     model: e.model
-                }), c().createElement(xe, {
+                }), c().createElement(we, {
                     panel: e.panel
                 }))
             }
-            const Ce = Q().div`
+            const fe = Q().div`
   display: flex;
   border-top: 4px solid var(--jp-border-color0);
   font-size: var(--jp-ui-font-size1);
 
   height: 100%;
 `,
-                fe = Q()(ce)`
+                xe = Q()(me)`
   flex-grow: 1;
   flex-shrink: 1;
 
   margin-right: 2px;
 `,
-                xe = Q()(V)`
+                we = Q()(Y)`
   flex-grow: 0;
   flex-shrink: 0;
 `,
-                we = c().createContext(i.nullTranslator.load(m)),
-                ve = c().createContext({
-                    submissionListFactory: me
+                ve = c().createContext(i.nullTranslator.load(m)),
+                Se = c().createContext({
+                    submissionListFactory: he
                 });
-            class Se extends o.ReactWidget {
+            class Ee extends o.ReactWidget {
                 constructor(e) {
-                    super(), this.queryClient = new H.QueryClient, this._panel = e.panel, this._model = e.model, this._trans = e.translator.load(m), this._submissionListFactory = e.submissionListFactory
+                    super(), this.queryClient = new G.QueryClient, this._panel = e.panel, this._model = e.model, this._trans = e.translator.load(m), this._submissionListFactory = e.submissionListFactory
                 }
                 render() {
                     var e, t;
-                    return c().createElement(ve.Provider, {
+                    return c().createElement(Se.Provider, {
                         value: {
                             submissionListFactory: this._submissionListFactory
                         }
-                    }, c().createElement(we.Provider, {
+                    }, c().createElement(ve.Provider, {
                         value: this._trans
-                    }, c().createElement(H.QueryClientProvider, {
+                    }, c().createElement(G.QueryClientProvider, {
                         client: this.queryClient
-                    }, c().createElement(ye, {
+                    }, c().createElement(Ce, {
                         key: null !== (t = null === (e = this._model.problem) || void 0 === e ? void 0 : e.id) && void 0 !== t ? t : "",
                         panel: this._panel,
                         model: this._model
                     }))))
                 }
             }
             const je = "jp-OutputArea-output";
@@ -1164,25 +1205,25 @@
                             output_type: "stream",
                             name: "stdin",
                             text: e + "\n"
                         }), i.dispose()
                     }))
                 }
             }
-            const Ee = new r.LabIcon({
+            const Te = new r.LabIcon({
                 name: "judge-icon:reset",
                 svgstr: b.cornerUpLeftDoubleFillSvg
             });
             class ke extends _.Panel {
                 constructor(e) {
                     super(), this.addClass("jp-JudgeTerminal");
                     const t = e.translator.load(m),
                         s = new _.Widget,
                         n = document.createElement("button");
-                    n.className = "jp-JudgeTerminal-resetButton", Ee.element({
+                    n.className = "jp-JudgeTerminal-resetButton", Te.element({
                         container: n
                     });
                     const o = n.children.item(0);
                     o && (o.classList.add("jp-icon3"), o.setAttribute("fill", "FFFFFF"));
                     const i = document.createElement("span");
                     i.className = "jp-JudgeTerminal-resetButtonLabel", i.textContent = t.__("Reset to skeleton code"), n.addEventListener("click", (() => {
                         var t;
@@ -1215,34 +1256,34 @@
                         await e.panel.session.shutdown()
                     })), c.appendChild(h), s.node.appendChild(n), s.node.appendChild(a), s.node.appendChild(d), s.node.appendChild(u), s.node.appendChild(c), this.addWidget(s), this._outputArea = new Ie(e), this.addWidget(this._outputArea)
                 }
                 get outputArea() {
                     return this._outputArea
                 }
             }
-            const Te = new N.Signal({}),
-                Pe = new N.Signal({}),
-                Fe = {
+            const Pe = new A.Signal({}),
+                Fe = new A.Signal({}),
+                Ne = {
                     id: `${p}:IJudgeSignal`,
-                    provides: z,
+                    provides: q,
                     activate: e => ({
                         get submitted() {
-                            return Te
+                            return Pe
                         },
                         get executed() {
-                            return Pe
+                            return Fe
                         }
                     }),
                     autoStart: !0
                 },
-                Ne = [{
+                Ae = [{
                     id: `${p}:plugin`,
                     autoStart: !0,
-                    requires: [i.ITranslator, a.IEditorServices, y.IRenderMimeRegistry, O.IDocumentManager, D.IMainMenu, o.ICommandPalette, o.ISessionContextDialogs],
-                    optional: [R, K, B, U, $, L.ISettingRegistry, n.ILayoutRestorer],
+                    requires: [i.ITranslator, a.IEditorServices, y.IRenderMimeRegistry, D.IDocumentManager, L.IMainMenu, o.ICommandPalette, o.ISessionContextDialogs],
+                    optional: [K, B, U, z, $, W.ISettingRegistry, n.ILayoutRestorer],
                     activate: async (e, t, s, n, i, r, a, d, l, u, c, h, p, g, _) => {
                         const b = t.load(m),
                             y = new o.WidgetTracker({
                                 namespace: "judge"
                             }),
                             C = b.__("Judge");
                         let f;
@@ -1250,19 +1291,19 @@
                         const x = new k({
                             editorServices: s,
                             rendermime: n,
                             commands: e.commands,
                             editorConfig: f,
                             sessionContextDialogs: d,
                             judgePanelFactory: null != l ? l : e => new I(e),
-                            judgeSubmissionAreaFactory: null != u ? u : e => new Se(e),
+                            judgeSubmissionAreaFactory: null != u ? u : e => new Ee(e),
                             judgeTerminalFactory: null != c ? c : e => new ke(e),
-                            submissionListFactory: null != h ? h : me,
-                            submitted: Te,
-                            executed: Pe,
+                            submissionListFactory: null != h ? h : he,
+                            submitted: Pe,
+                            executed: Fe,
                             factoryOptions: {
                                 name: C,
                                 modelName: "judge-model",
                                 fileTypes: ["judge"],
                                 defaultFor: ["judge"],
                                 preferKernel: !0,
                                 canStartKernel: !0,
@@ -1271,93 +1312,93 @@
                             }
                         });
                         x.widgetCreated.connect(((e, t) => {
                             t.context.pathChanged.connect((() => {
                                 y.save(t)
                             })), y.add(t)
                         })), e.docRegistry.addWidgetFactory(x);
-                        const w = null != p ? p : new q;
+                        const w = null != p ? p : new H;
                         e.docRegistry.addModelFactory(new M.JudgeModelFactory({
                                 problemProviderFactory: () => w
                             })), e.docRegistry.addFileType({
                                 name: "judge",
                                 contentType: "file",
                                 fileFormat: "text",
                                 displayName: b.__("Judge File"),
                                 extensions: [".judge"],
                                 mimeTypes: ["text/json", "application/json"]
                             }),
                             function(e, t, s, n, o) {
-                                e.addCommand(T.open, {
+                                e.addCommand(P.open, {
                                     execute: async e => {
                                         s.openOrReveal(e.path)
                                     },
                                     label: t.__("Open Judge")
-                                }), e.addCommand(T.openOrCreateFromId, {
+                                }), e.addCommand(P.openOrCreateFromId, {
                                     execute: async e => {
-                                        e.problemId && await A(o, s, e.problemId)
+                                        e.problemId && await O(o, s, e.problemId)
                                     },
                                     label: t.__("Open or Create Judge From Id")
-                                }), e.addCommand(T.execute, {
+                                }), e.addCommand(P.execute, {
                                     execute: async e => {
                                         n.currentWidget && n.currentWidget.content.execute()
                                     },
                                     label: t.__("Execute")
-                                }), e.addCommand(T.redo, {
+                                }), e.addCommand(P.redo, {
                                     execute: async () => {
                                         n.currentWidget && n.currentWidget.content.editor.redo()
                                     },
                                     label: t.__("Redo")
-                                }), e.addCommand(T.undo, {
+                                }), e.addCommand(P.undo, {
                                     execute: async () => {
                                         n.currentWidget && n.currentWidget.content.editor.undo()
                                     },
                                     label: t.__("Undo")
-                                }), e.addCommand(T.run, {
+                                }), e.addCommand(P.run, {
                                     execute: async () => {
                                         n.currentWidget && n.currentWidget.content.execute()
                                     },
                                     label: t.__("Run")
-                                }), e.addCommand(T.runAll, {
+                                }), e.addCommand(P.runAll, {
                                     execute: async () => {
                                         n.currentWidget && n.currentWidget.content.execute()
                                     },
                                     label: t.__("Run All")
                                 })
                             }(e.commands, b, i, y, w),
                             function(e, t, s) {
                                 ! function(e) {
                                     e.editMenu.undoers.undo.add({
-                                        id: T.undo,
-                                        isEnabled: e => e instanceof E
+                                        id: P.undo,
+                                        isEnabled: e => e instanceof T
                                     }), e.editMenu.undoers.redo.add({
-                                        id: T.redo,
-                                        isEnabled: e => e instanceof E
+                                        id: P.redo,
+                                        isEnabled: e => e instanceof T
                                     })
                                 }(e),
                                 function(e) {
                                     e.runMenu.codeRunners.run.add({
-                                        id: T.run,
-                                        isEnabled: e => e instanceof E
+                                        id: P.run,
+                                        isEnabled: e => e instanceof T
                                     }), e.runMenu.codeRunners.runAll.add({
-                                        id: T.runAll,
-                                        isEnabled: e => e instanceof E
+                                        id: P.runAll,
+                                        isEnabled: e => e instanceof T
                                     })
                                 }(e)
                             }(r), a.addItem({
-                                command: T.openOrCreateFromId,
+                                command: P.openOrCreateFromId,
                                 category: "Judge",
                                 args: {
                                     problemId: "1"
                                 }
                             }), _ && _.restore(y, {
-                                command: T.open,
+                                command: P.open,
                                 args: e => ({
                                     path: e.context.path
                                 }),
                                 name: e => e.context.path
                             })
                     }
-                }, Fe]
+                }, Ne]
         }
     }
 ]);
```

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/remoteEntry.b81a0f7c77284e957c86.js` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/remoteEntry.933113d1b8fc3f476592.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -57,15 +57,15 @@
         732: "d368cf762f465d394900",
         747: "2841a40cba671c554a8c",
         767: "69c7e698f115ea487665",
         860: "fee57e15b3a40a2d65fa",
         893: "389b596eee368876402a",
         901: "b84e014859b58a1fa86a",
         917: "ab3207654a9c812bc979",
-        960: "376cb311c5431702de57"
+        960: "560036ddbfd0e33374bc"
     } [e] + ".js?v=" + {
         29: "d2153138b471f40c1c27",
         146: "ffbfc6be3b1d44378330",
         316: "18d9e632074f3acc892c",
         378: "2c7a4a82fbc8f09f2463",
         505: "fe5d2436cfe6faec3918",
         599: "7e6937b28ad247ccde7c",
@@ -73,15 +73,15 @@
         732: "d368cf762f465d394900",
         747: "2841a40cba671c554a8c",
         767: "69c7e698f115ea487665",
         860: "fee57e15b3a40a2d65fa",
         893: "389b596eee368876402a",
         901: "b84e014859b58a1fa86a",
         917: "ab3207654a9c812bc979",
-        960: "376cb311c5431702de57"
+        960: "560036ddbfd0e33374bc"
     } [e], T.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -133,15 +133,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (o[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (i("@emotion/react", "11.11.1", (() => Promise.all([T.e(146), T.e(29), T.e(599)]).then((() => () => T(917))))), i("@emotion/styled", "11.11.0", (() => Promise.all([T.e(29), T.e(505), T.e(378)]).then((() => () => T(4378))))), i("@team-monolith/cds", "1.0.1", (() => Promise.all([T.e(146), T.e(901), T.e(29), T.e(704), T.e(316)]).then((() => () => T(7210))))), i("jupyterlab-judge", "1.24.4", (() => Promise.all([T.e(29), T.e(960)]).then((() => () => T(960))))), i("react-query", "3.39.3", (() => Promise.all([T.e(767), T.e(29), T.e(704)]).then((() => () => T(8767)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@emotion/react", "11.11.1", (() => Promise.all([T.e(146), T.e(29), T.e(599)]).then((() => () => T(917))))), i("@emotion/styled", "11.11.0", (() => Promise.all([T.e(29), T.e(505), T.e(378)]).then((() => () => T(4378))))), i("@team-monolith/cds", "1.0.1", (() => Promise.all([T.e(146), T.e(901), T.e(29), T.e(704), T.e(316)]).then((() => () => T(7210))))), i("jupyterlab-judge", "1.25.0", (() => Promise.all([T.e(29), T.e(960)]).then((() => () => T(960))))), i("react-query", "3.39.3", (() => Promise.all([T.e(767), T.e(29), T.e(704)]).then((() => () => T(8767)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         T.g.importScripts && (e = T.g.location + "");
         var r = T.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -250,48 +250,48 @@
         var n = T.I(r);
         return n && n.then ? n.then(e.bind(e, r, T.S[r], t, a, o)) : e(r, T.S[r], t, a, o)
     })(((e, r, t, a) => r && T.o(r, t) ? h(i(r, t)) : a())), y = m(((e, r, t, a) => (l(e, t), h(s(r, t, a) || b(r, e, t, a) || i(r, t))))), g = m(((e, r, t, a) => (l(e, t), f(r, 0, t, a)))), j = m(((e, r, t, a, o) => {
         var n = r && T.o(r, t) && s(r, t, a);
         return n ? h(n) : o()
     })), P = {}, w = {
         6029: () => g("default", "react", [1, 18, 2, 0]),
-        797: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 6]),
-        1464: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
-        2232: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 6]),
-        2294: () => y("default", "@jupyterlab/docregistry", [1, 4, 1, 6]),
-        2818: () => g("default", "@jupyterlab/services", [1, 7, 1, 6]),
-        3195: () => y("default", "@jupyterlab/outputarea", [1, 4, 1, 6]),
-        3413: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 6]),
+        802: () => y("default", "@jupyterlab/outputarea", [1, 4, 1, 8]),
+        1363: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 8]),
+        1731: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 8]),
+        2377: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 8]),
+        2677: () => g("default", "@jupyterlab/application", [1, 4, 1, 8]),
+        2682: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 8]),
+        2832: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 8]),
         3848: () => j("default", "react-query", [2, 3, 39, 0], (() => Promise.all([T.e(767), T.e(704)]).then((() => () => T(8767))))),
-        4072: () => g("default", "@jupyterlab/application", [1, 4, 1, 6]),
         4882: () => g("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         4901: () => g("default", "@lumino/signaling", [1, 2, 0, 0]),
-        5099: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 6]),
+        5048: () => y("default", "@jupyterlab/docregistry", [1, 4, 1, 8]),
+        5114: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 8]),
+        5421: () => y("default", "@jupyterlab/cells", [1, 4, 1, 8]),
         5536: () => j("default", "@team-monolith/cds", [1, 1, 0, 1], (() => Promise.all([T.e(146), T.e(901), T.e(704), T.e(316)]).then((() => () => T(7210))))),
-        6805: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
-        7263: () => y("default", "@jupyterlab/cells", [1, 4, 1, 6]),
-        7594: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 6]),
+        7520: () => g("default", "@jupyterlab/services", [1, 7, 1, 8]),
+        7560: () => g("default", "@jupyterlab/translation", [1, 4, 1, 8]),
+        7756: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 8]),
         7930: () => g("default", "@lumino/coreutils", [1, 2, 0, 0]),
         8093: () => g("default", "@jupyter/ydoc", [1, 1, 1, 1]),
         8149: () => j("default", "@emotion/styled", [1, 11, 6, 0], (() => Promise.all([T.e(505), T.e(860)]).then((() => () => T(4378))))),
-        8671: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
-        8937: () => g("default", "@jupyterlab/translation", [1, 4, 1, 6]),
+        9874: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 8]),
         799: () => j("default", "@emotion/react", [1, 11, 0, 0, , "rc", 0], (() => Promise.all([T.e(146), T.e(917)]).then((() => () => T(917))))),
         5211: () => v("default", "@emotion/react", (() => Promise.all([T.e(146), T.e(917)]).then((() => () => T(917))))),
         7704: () => g("default", "react-dom", [1, 18, 2, 0]),
         718: () => j("default", "@emotion/styled", [1, 11, 8, 1], (() => Promise.all([T.e(505), T.e(893)]).then((() => () => T(4378))))),
         2148: () => j("default", "@emotion/react", [1, 11, 4, 1], (() => T.e(732).then((() => () => T(917))))),
         8800: () => j("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([T.e(505), T.e(893)]).then((() => () => T(4378))))),
         9558: () => j("default", "@emotion/react", [1, 11, 8, 2], (() => T.e(732).then((() => () => T(917)))))
     }, S = {
         29: [6029],
         316: [718, 2148, 8800, 9558],
         505: [799, 5211],
         704: [7704],
-        960: [797, 1464, 2232, 2294, 2818, 3195, 3413, 3848, 4072, 4882, 4901, 5099, 5536, 6805, 7263, 7594, 7930, 8093, 8149, 8671, 8937]
+        960: [802, 1363, 1731, 2377, 2677, 2682, 2832, 3848, 4882, 4901, 5048, 5114, 5421, 5536, 7520, 7560, 7756, 7930, 8093, 8149, 9874]
     }, T.f.consumes = (e, r) => {
         T.o(S, e) && S[e].forEach((e => {
             if (T.o(P, e)) return r.push(P[e]);
             var t = r => {
                     P[e] = 0, T.m[e] = t => {
                         delete T.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/third-party-licenses.json` & `jupyterlab_judge-1.25.0/jupyterlab_judge/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json` & `jupyterlab_judge-1.25.0/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.89875%*

 * *Differences: {"''": "{'version': '1.24.4'}",*

 * * "'Redo'": "['다시실행']",*

 * * "'Run All'": "['모두 실행']",*

 * * "'Run'": "['실행']",*

 * * "'Undo'": "['실행취소']",*

 * * "'Validation failed. Please try again'": "['답안 평가에 실패했습니다. 다시 시도해주세요.']"}*

```diff
@@ -1,13 +1,13 @@
 {
     "": {
         "domain": "jupyterlab_judge",
         "language": "ko-KR",
         "plural_forms": "nplurals=1; plural=0;",
-        "version": "0.18.3"
+        "version": "1.24.4"
     },
     "Accepted": [
         "\uc815\ub2f5\uc785\ub2c8\ub2e4."
     ],
     "An error occurred during submission.": [
         "\uc81c\ucd9c \uc911 \uc624\ub958\uac00 \ubc1c\uc0dd\ud588\uc2b5\ub2c8\ub2e4."
     ],
@@ -91,17 +91,26 @@
     ],
     "Problem Not Available.": [
         "\ubb38\uc81c\ub97c \ubd88\ub7ec\uc624\uc9c0 \ubabb\ud588\uc2b5\ub2c8\ub2e4."
     ],
     "Problem has no test cases.": [
         "\ud14c\uc2a4\ud2b8 \ucf00\uc774\uc2a4\uac00 \ub4f1\ub85d\ub418\uc9c0 \uc54a\uc740 \ubb38\uc81c\uc785\ub2c8\ub2e4."
     ],
+    "Redo": [
+        "\ub2e4\uc2dc\uc2e4\ud589"
+    ],
     "Reset to skeleton code": [
         "\uc2a4\ucf08\ub808\ud1a4 \ucf54\ub4dc \ub418\ub3cc\ub9ac\uae30"
     ],
+    "Run": [
+        "\uc2e4\ud589"
+    ],
+    "Run All": [
+        "\ubaa8\ub450 \uc2e4\ud589"
+    ],
     "Run All Code": [
         "\uc2e4\ud589"
     ],
     "Run Code": [
         "\uc2e4\ud589"
     ],
     "Run the code": [
@@ -124,14 +133,20 @@
     ],
     "The cell has not been executed to avoid kernel deadlock as there is another pending input! Submit your pending input and try again.": [
         "\uc785\ub825\uc744 \uae30\ub2e4\ub9ac\uace0 \uc788\uc5b4 \uad50\ucc29 \uc0c1\ud0dc\ub97c \ubc29\uc9c0\ud558\uae30 \uc704\ud574 \ucf54\ub4dc\ub97c \uc2e4\ud589\ud558\uc9c0 \uc54a\uc558\uc2b5\ub2c8\ub2e4. \uc785\ub825\uc744 \uc644\ub8cc\ud558\uace0 \ub2e4\uc2dc \uc2dc\ub3c4\ud574\uc8fc\uc138\uc694."
     ],
     "Time Limit": [
         "\uc2dc\uac04 \ucd08\uacfc"
     ],
+    "Undo": [
+        "\uc2e4\ud589\ucde8\uc18c"
+    ],
+    "Validation failed. Please try again": [
+        "\ub2f5\uc548 \ud3c9\uac00\uc5d0 \uc2e4\ud328\ud588\uc2b5\ub2c8\ub2e4. \ub2e4\uc2dc \uc2dc\ub3c4\ud574\uc8fc\uc138\uc694."
+    ],
     "Wrong": [
         "\ud2c0\ub838\uc2b5\ub2c8\ub2e4."
     ],
     "schema\u0004jupyterlab-judge": [
         "jupyterlab_judge"
     ],
     "schema\u0004jupyterlab-judge settings.": [
```

### Comparing `jupyterlab_judge-1.24.4/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po` & `jupyterlab_judge-1.25.0/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: jupyterlab_judge 0.18.3\n"
+"Project-Id-Version: jupyterlab_judge 1.24.4\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-10-10 13:03+0900\n"
+"POT-Creation-Date: 2024-04-27 18:44+0900\n"
 "PO-Revision-Date: 2023-04-05 15:40+0900\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: ko_KR <LL@li.org>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -18,47 +18,64 @@
 msgid "jupyterlab-judge settings."
 msgstr "jupyterlab_judge 설정"
 
 msgctxt "schema"
 msgid "jupyterlab-judge"
 msgstr "jupyterlab_judge"
 
+#: src/commands.ts:100
+msgid "Run All"
+msgstr "모두 실행"
+
 #: src/commands.ts:158
 msgid "Run Code"
 msgstr "실행"
 
 #: src/commands.ts:162
 msgid "Run All Code"
 msgstr "실행"
 
-#: src/commands.ts:38
+#: src/commands.ts:38 src/commands.ts:43
 msgid "Open Judge"
 msgstr "문제 열기"
 
-#: src/commands.ts:51
+#: src/commands.ts:51 src/commands.ts:56
 msgid "Open or Create Judge From Id"
 msgstr "ID로부터 문제 열기"
 
-#: src/commands.ts:60 src/widgets/JudgeTerminal.ts:60
+#: src/commands.ts:60 src/commands.ts:65 src/widgets/JudgeTerminal.ts:60
+#: src/widgets/JudgeTerminal.ts:71 src/widgets/JudgeTerminal.ts:75
 msgid "Execute"
 msgstr "실행"
 
+#: src/commands.ts:74
+msgid "Redo"
+msgstr "다시실행"
+
+#: src/commands.ts:83
+msgid "Undo"
+msgstr "실행취소"
+
+#: src/commands.ts:92
+msgid "Run"
+msgstr "실행"
+
 #: src/components/SubmissionArea.tsx:16
 msgid "No Submission History Found."
 msgstr "제출 기록을 확인할 수 없습니다."
 
 #: src/components/SubmissionControl.tsx:29
 msgid "An error occurred during submission."
 msgstr "제출 중 오류가 발생했습니다."
 
 #: src/components/SubmissionControl.tsx:46
 msgid "Submit"
 msgstr "제출하기"
 
-#: src/components/SubmissionItem.tsx:34
+#: src/components/SubmissionItem.tsx:31 src/components/SubmissionItem.tsx:34
 msgid "Load this submission"
 msgstr "이 답안 불러오기"
 
 #: src/components/SubmissionItemStatus.tsx:19
 msgid "Accepted"
 msgstr "정답입니다."
 
@@ -95,85 +112,92 @@
 msgid "Submit your code to get results here."
 msgstr "답안을 제출하면 채점 결과가 여기 나타납니다."
 
 #: src/components/SubmissionList.tsx:86 src/components/SubmissionList.tsx:98
 msgid "Loading History"
 msgstr "불러오는 중입니다."
 
-#: src/index.ts:108
+#: src/index.ts:108 src/index.ts:114
 msgid "Judge"
 msgstr "문제"
 
-#: src/index.ts:172
+#: src/index.ts:172 src/index.ts:180
 msgid "Judge File"
 msgstr "문제 파일"
 
 #: src/toolbar.tsx:36
 msgid "Cannot Save"
 msgstr "저장할 수 없습니다"
 
 #: src/toolbar.tsx:37
 msgid "Document is read-only"
 msgstr "읽기 전용 문서입니다"
 
 #: src/toolbar.tsx:38 src/widgets/JudgePanel.ts:268
-#: src/widgets/JudgePanel.ts:280
+#: src/widgets/JudgePanel.ts:280 src/widgets/JudgePanel.ts:294
+#: src/widgets/JudgePanel.ts:312
 msgid "Ok"
 msgstr "확인"
 
 #: src/toolbar.tsx:54
 msgid "Save the judge contents and create checkpoint"
 msgstr "문제 풀이 저장"
 
 #: src/widgets/JudgeOutputArea.ts:43
 msgid "Execution result will be shown here"
 msgstr "여기에 실행 결과가 나타납니다."
 
-#: src/widgets/JudgePanel.ts:193
+#. 문제를 불러오지 못했습니다.
+#: src/widgets/JudgePanel.ts:193 src/widgets/JudgeProblemPanel.ts:30
 msgid "Problem Not Available."
 msgstr "문제를 불러오지 못했습니다."
 
-#: src/widgets/JudgePanel.ts:264
+#: src/widgets/JudgePanel.ts:264 src/widgets/JudgePanel.ts:308
 msgid "Cell not executed due to missing kernel"
 msgstr "커널이 선택되지 않아 실행하지 못했습니다"
 
-#: src/widgets/JudgePanel.ts:265
+#: src/widgets/JudgePanel.ts:265 src/widgets/JudgePanel.ts:309
 msgid ""
 "The cell has not been executed because no kernel selected. Please select a"
 " kernel to execute the cell."
 msgstr "커널이 선택되지 않아 코드를 실행할 수 없습니다. 커널을 선택하고 다시 시도해주세요."
 
-#: src/widgets/JudgePanel.ts:276
+#: src/widgets/JudgePanel.ts:276 src/widgets/JudgePanel.ts:290
 msgid "Cell not executed due to pending input"
 msgstr "입력을 기다리고 있어 실행하지 못했습니다"
 
-#: src/widgets/JudgePanel.ts:277
+#: src/widgets/JudgePanel.ts:277 src/widgets/JudgePanel.ts:291
 msgid ""
 "The cell has not been executed to avoid kernel deadlock as there is "
 "another pending input! Submit your pending input and try again."
 msgstr "입력을 기다리고 있어 교착 상태를 방지하기 위해 코드를 실행하지 않았습니다. 입력을 완료하고 다시 시도해주세요."
 
-#: src/widgets/JudgePanel.ts:342
+#: src/widgets/JudgePanel.ts:342 src/widgets/JudgePanel.ts:374
 msgid "Problem has no test cases."
 msgstr "테스트 케이스가 등록되지 않은 문제입니다."
 
 #: src/widgets/JudgePanel.ts:397 src/widgets/JudgePanel.ts:404
-#: src/widgets/JudgePanel.ts:411
+#: src/widgets/JudgePanel.ts:411 src/widgets/JudgePanel.ts:429
+#: src/widgets/JudgePanel.ts:436 src/widgets/JudgePanel.ts:443
 msgid "Kernel is still connecting. Please check your network."
 msgstr "커널에 연결하지 못했습니다. 네트워크를 확인하시고 다시 시도해주세요."
 
-#: src/widgets/JudgePanel.ts:422
+#: src/widgets/JudgePanel.ts:422 src/widgets/JudgePanel.ts:454
 msgid "Kernel is not responding. Please try again."
 msgstr "커널이 응답하지 않습니다. 다시 시도해주세요."
 
-#: src/widgets/JudgeTerminal.ts:37
+#: src/widgets/JudgePanel.ts:477
+msgid "Validation failed. Please try again"
+msgstr "답안 평가에 실패했습니다. 다시 시도해주세요."
+
+#: src/widgets/JudgeTerminal.ts:37 src/widgets/JudgeTerminal.ts:51
 msgid "Reset to skeleton code"
 msgstr "스켈레톤 코드 되돌리기"
 
-#: src/widgets/JudgeTerminal.ts:83
+#: src/widgets/JudgeTerminal.ts:83 src/widgets/JudgeTerminal.ts:98
 msgid "Stop"
 msgstr "중지"
 
 #~ msgid "Load"
 #~ msgstr "불러오기"
 
 #~ msgid "No History"
```

### Comparing `jupyterlab_judge-1.24.4/src/commands.ts` & `jupyterlab_judge-1.25.0/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/handler.ts` & `jupyterlab_judge-1.25.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/index.ts` & `jupyterlab_judge-1.25.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/model.ts` & `jupyterlab_judge-1.25.0/src/model.ts`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,17 @@
     this.dirty = true;
   }
 
   async getTestCases(): Promise<string[]> {
     return await this._problemProvider.getTestCases(this.sharedModel.problemId);
   }
 
-  async validate(outputs: string[]): Promise<ProblemProvider.IValidateResult> {
+  async validate(
+    outputs: string[]
+  ): Promise<ProblemProvider.IValidateResult | null> {
     return await this._problemProvider.validate(
       this.sharedModel.problemId,
       outputs
     );
   }
 
   async submit(
```

### Comparing `jupyterlab_judge-1.24.4/src/tokens.ts` & `jupyterlab_judge-1.25.0/src/tokens.ts`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 export interface IProblemProvider {
   getProblem(id: string): Promise<ProblemProvider.IProblem | null>;
   getTestCases(id: string): Promise<string[]>;
   validate(
     id: string,
     outputs: string[]
-  ): Promise<ProblemProvider.IValidateResult>;
+  ): Promise<ProblemProvider.IValidateResult | null>;
   getSubmissions(id: string): Promise<ProblemProvider.ISubmission[]>;
   submit(
     request: ProblemProvider.ISubmissionRequest,
     panel: JudgePanel
   ): Promise<ProblemProvider.ISubmission>;
 }
```

### Comparing `jupyterlab_judge-1.24.4/src/toolbar.tsx` & `jupyterlab_judge-1.25.0/src/toolbar.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/components/SubmissionArea.tsx` & `jupyterlab_judge-1.25.0/src/components/SubmissionArea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/components/SubmissionControl.tsx` & `jupyterlab_judge-1.25.0/src/components/SubmissionControl.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/components/SubmissionItem.tsx` & `jupyterlab_judge-1.25.0/src/components/SubmissionItem.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/components/SubmissionItemStatus.tsx` & `jupyterlab_judge-1.25.0/src/components/SubmissionItemStatus.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/components/SubmissionItemWait.tsx` & `jupyterlab_judge-1.25.0/src/components/SubmissionItemWait.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/components/SubmissionItemWaitStatus.tsx` & `jupyterlab_judge-1.25.0/src/components/SubmissionItemWaitStatus.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/components/SubmissionList.tsx` & `jupyterlab_judge-1.25.0/src/components/SubmissionList.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/problemProvider/HardCodedProblemProvider.ts` & `jupyterlab_judge-1.25.0/src/problemProvider/HardCodedProblemProvider.ts`

 * *Files 26% similar despite different names*

```diff
@@ -54,35 +54,25 @@
   };
   async getTestCases(id: string): Promise<string[]> {
     return this.problems[id].testCases;
   }
   async validate(
     id: string,
     outputs: string[]
-  ): Promise<ProblemProvider.IValidateResult> {
+  ): Promise<ProblemProvider.IValidateResult | null> {
     const solutions = this.problems[id].outputs;
     if (solutions.length !== outputs.length) {
-      return {
-        token: null,
-        totalCount: solutions.length,
-        acceptedCount: 0
-      };
-    }
-
-    let accepted = 0;
-    for (let i = 0; i < solutions.length; i++) {
-      if (solutions[i].trim() === outputs[i].trim()) {
-        accepted += 1;
-      }
+      return null;
     }
 
     return {
       token: null,
-      totalCount: solutions.length,
-      acceptedCount: accepted
+      results: solutions.map(
+        (solution, i) => solution.trim() === outputs[i].trim()
+      )
     };
   }
   async getProblem(id: string): Promise<ProblemProvider.IProblem | null> {
     return this.problems[id];
   }
 
   async getSubmissions(id: string): Promise<ProblemProvider.ISubmission[]> {
@@ -92,20 +82,37 @@
   async submit(
     request: ProblemProvider.ISubmissionRequest
   ): Promise<ProblemProvider.ISubmission> {
     if (this._idToSubmissions[request.problemId] === undefined) {
       this._idToSubmissions[request.problemId] = [];
     }
 
+    let status: ProblemProvider.SubmissionStatus;
+    if (request.details.every(detail => detail.status === 'AC')) {
+      status = 'AC';
+    } else if (request.details.some(detail => detail.status === 'RE')) {
+      status = 'RE';
+    } else if (request.details.some(detail => detail.status === 'OLE')) {
+      status = 'OLE';
+    } else if (request.details.some(detail => detail.status === 'TLE')) {
+      status = 'TLE';
+    } else {
+      status = 'WA';
+    }
+
     const submission: ProblemProvider.ISubmission = {
       ...request,
+      status,
       id: this._idToSubmissions[request.problemId].length.toString(),
       image: '',
       userId: '',
-      createdAt: new Date().toISOString()
+      createdAt: new Date().toISOString(),
+      acceptedCount: request.details.filter(detail => detail.status === 'AC')
+        .length,
+      totalCount: request.details.length
     };
 
     this._idToSubmissions[request.problemId].push(submission);
     return submission;
   }
 
   private _idToSubmissions: { [key: string]: ProblemProvider.ISubmission[] } =
```

### Comparing `jupyterlab_judge-1.24.4/src/widgets/JudgeOutputArea.ts` & `jupyterlab_judge-1.25.0/src/widgets/JudgeOutputArea.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/widgets/JudgePanel.ts` & `jupyterlab_judge-1.25.0/src/widgets/JudgePanel.ts`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,18 @@
   DocumentWidget,
   IDocumentWidget
 } from '@jupyterlab/docregistry';
 import { IRenderMimeRegistry } from '@jupyterlab/rendermime';
 import { CommandRegistry } from '@lumino/commands';
 import { OutputArea } from '@jupyterlab/outputarea';
 import { KernelMessage } from '@jupyterlab/services';
-import { IStreamMsg } from '@jupyterlab/services/lib/kernel/messages';
+import {
+  IErrorMsg,
+  IStreamMsg
+} from '@jupyterlab/services/lib/kernel/messages';
 import { JudgeModel } from '../model';
 import { ProblemProvider } from '../problemProvider/problemProvider';
 import { ToolbarItems } from '../toolbar';
 import { TRANSLATOR_DOMAIN } from '../constants';
 import { Signal } from '@lumino/signaling';
 import { BoxPanel, SplitPanel, Widget } from '@lumino/widgets';
 import { JudgeTerminal } from './JudgeTerminal';
@@ -46,19 +49,32 @@
 }
 
 const JudgeColorLabIcon = new LabIcon({
   name: 'jupyterlab-judge:problem-icon',
   svgstr: customJudgeColorSvg
 });
 
-interface IRunResult {
-  status: 'OK' | 'TLE' | 'OLE' | 'RE';
-  output: string;
-  cpuTime: number;
-}
+type IRunResult =
+  | {
+      status: 'OK' | 'OLE';
+      output: string;
+      cpuTime: number;
+    }
+  | {
+      status: 'RE';
+      output: string;
+      cpuTime: number;
+      errorValue: string;
+      errorName: string;
+    }
+  | {
+      status: 'TLE';
+      output: string;
+      cpuTime: number | null; // null if killed
+    };
 
 export class JudgeError extends Error {
   constructor(message?: string) {
     super(message);
     this.name = this.constructor.name;
   }
 }
@@ -80,14 +96,21 @@
 export class JudgeKernelReconnectingFailedError extends JudgeError {
   constructor(message?: string) {
     super(message);
     this.name = this.constructor.name;
   }
 }
 
+export class ValidationFailedError extends JudgeError {
+  constructor(message?: string) {
+    super(message);
+    this.name = this.constructor.name;
+  }
+}
+
 export namespace JudgePanel {
   export interface IOptions {
     editorServices: IEditorServices;
     editorConfig: Pick<CodeEditor.IOptions, 'config'>;
     rendermime: IRenderMimeRegistry;
     context: DocumentRegistry.IContext<JudgeModel>;
     translator: ITranslator;
@@ -440,46 +463,72 @@
       this.model.submissionStatus = {
         type: 'progress',
         runCount: results.length,
         totalCount: testCases.length
       };
     }
 
-    let status: ProblemProvider.SubmissionStatus | null = null;
     const validateResult = await this.model.validate(
       results.map(result => result.output)
     );
-    if (validateResult.acceptedCount === validateResult.totalCount) {
-      status = 'AC';
-    } else if (results.some(result => result.status === 'RE')) {
-      status = 'RE';
-    } else if (results.some(result => result.status === 'OLE')) {
-      status = 'OLE';
-    } else if (results.some(result => result.status === 'TLE')) {
-      status = 'TLE';
-    } else {
-      status = 'WA';
+
+    if (validateResult === null) {
+      throw new ValidationFailedError(
+        this._trans.__('Validation failed. Please try again')
+      );
     }
 
     await kernel.shutdown();
     kernel.dispose();
 
     const submission = await this.model.submit(
       {
         problemId: problem.id,
-        status: status,
         code,
-        cpuTime:
-          results.map(result => result.cpuTime).reduce((a, b) => a + b, 0) /
-          results.length,
-        acceptedCount: validateResult.acceptedCount,
-        totalCount: validateResult.totalCount,
         token: validateResult.token,
         language: 'python',
-        memory: 0
+        details: results.map((result, index) => {
+          switch (result.status) {
+            case 'OK':
+              if (validateResult.results[index]) {
+                return {
+                  status: 'AC',
+                  cpuTime: result.cpuTime,
+                  memory: 0
+                };
+              } else {
+                return {
+                  status: 'WA',
+                  answer: result.output,
+                  cpuTime: result.cpuTime,
+                  memory: 0
+                };
+              }
+            case 'TLE':
+              return {
+                status: 'TLE',
+                cpuTime: result.cpuTime,
+                memory: 0
+              };
+            case 'OLE':
+              return {
+                status: 'OLE',
+                cpuTime: result.cpuTime,
+                memory: 0
+              };
+            case 'RE':
+              return {
+                status: 'RE',
+                memory: 0,
+                cpuTime: result.cpuTime,
+                errorName: result.errorName,
+                errorValue: result.errorValue
+              };
+          }
+        })
       },
       this
     );
 
     this.model.submissionStatus = { type: 'idle' };
 
     this._submitted.emit({
@@ -555,29 +604,37 @@
       stop_on_error: true,
       allow_stdin: true
     };
 
     const startTime = Date.now();
     const future = kernel.requestExecute(content, true, {});
 
-    const result: IRunResult = { output: '', status: 'OK', cpuTime: 0 };
+    let result: IRunResult = { output: '', status: 'OK', cpuTime: 0 };
     future.onIOPub = (msg: KernelMessage.IIOPubMessage) => {
       const msgType = msg.header.msg_type;
 
       switch (msgType) {
         case 'stream': {
           const msgStream = msg as IStreamMsg;
           if (msgStream.content.name === 'stdout') {
             result.output = result.output.concat(msgStream.content.text);
           }
           break;
         }
-        case 'error':
-          result.status = 'RE';
+        case 'error': {
+          const msgError = msg as IErrorMsg;
+          result = {
+            status: 'RE',
+            errorName: msgError.content.ename,
+            errorValue: msgError.content.evalue,
+            output: result.output,
+            cpuTime: 0
+          };
           break;
+        }
         case 'execute_result':
         case 'display_data':
         case 'clear_output':
         case 'update_display_data':
         default:
           break;
       }
@@ -593,25 +650,33 @@
     });
     const a = await Promise.race([future.done, timeout]);
     if (a === 0) {
       future.dispose();
       await kernel.interrupt();
 
       // 강제 종료는 당연히 TLE
-      result.status = 'TLE';
+      // result.status = 'TLE';
+      result = {
+        status: 'TLE',
+        output: result.output,
+        cpuTime: null
+      };
     } else {
       // 강제 종료가 아니더라도 TLE 일 수 있습니다.
       // 우리가 시간을 산정하고, TLE를 부여하는 것은 이 cpuTime 기준입니다.
       // 위에서 setTimeout을 하는 것은 다만 커널을 강제종료하기 위한 기준입니다.
       // cpuTime 언제나 0보다 크고 timelimit 이하인 값입니다.
       const cpuTime = Date.now() - startTime;
+      result.cpuTime = cpuTime;
       if (cpuTime > timelimit) {
-        result.status = 'TLE';
-      } else {
-        result.cpuTime = cpuTime;
+        result = {
+          status: 'TLE',
+          output: result.output,
+          cpuTime: cpuTime
+        };
       }
     }
 
     return result;
   }
 
   private _context: DocumentRegistry.IContext<JudgeModel>;
```

### Comparing `jupyterlab_judge-1.24.4/src/widgets/JudgeProblemPanel.ts` & `jupyterlab_judge-1.25.0/src/widgets/JudgeProblemPanel.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/widgets/JudgeSubmissionArea.tsx` & `jupyterlab_judge-1.25.0/src/widgets/JudgeSubmissionArea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/src/widgets/JudgeTerminal.ts` & `jupyterlab_judge-1.25.0/src/widgets/JudgeTerminal.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/style/judgePanel.css` & `jupyterlab_judge-1.25.0/style/judgePanel.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/style/judgeTerminal.css` & `jupyterlab_judge-1.25.0/style/judgeTerminal.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/ui-tests/README.md` & `jupyterlab_judge-1.25.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/ui-tests/tests/jupyterlab_judge.spec.ts` & `jupyterlab_judge-1.25.0/ui-tests/tests/jupyterlab_judge.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/.gitignore` & `jupyterlab_judge-1.25.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/LICENSE` & `jupyterlab_judge-1.25.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/README.md` & `jupyterlab_judge-1.25.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/pyproject.toml` & `jupyterlab_judge-1.25.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.4/PKG-INFO` & `jupyterlab_judge-1.25.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab_judge
-Version: 1.24.4
+Version: 1.25.0
 Dynamic: Keywords
 Summary: A simple online judge for Jupyter Lab.
 Project-URL: Homepage, https://github.com/team-monolith-product/jupyterlab-judge
 Project-URL: Bug Tracker, https://github.com/team-monolith-product/jupyterlab-judge/issues
 Project-URL: Repository, https://github.com/team-monolith-product/jupyterlab-judge.git
 Author-email: ChangHwan Lee <lch@team-mono.com>
 License: BSD 3-Clause License
```

