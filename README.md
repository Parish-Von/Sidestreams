diff --git a/README.md b/README.md
index 448a2af39d42d8c1b5765d30e80f55432f02590c..711594534298b7d825169ca6c76c76cf5486e7a2 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,40 @@
-# Sidestreams
\ No newline at end of file
+# Sidestreams
+
+此仓库用于维护 sidestreams.wiki 的可自由编辑 Wiki 内容，并通过 GitHub Actions 自动部署。
+
+## 使用方式
+
+1. 在 `docs/` 中新增或编辑 Markdown 文件。
+2. 提交到 `main` 分支或合并 Pull Request。
+3. Workflow 将自动构建并发布到 GitHub Pages。
+
+## 本地预览
+
+```bash
+pip install mkdocs-material
+mkdocs serve
+```
+
+## 复制即用（Copy-paste ready）
+
+将下列命令复制到终端即可初始化并推送：
+
+```bash
+git clone <your-repo-url>
+cd <your-repo-name>
+python -m venv .venv
+source .venv/bin/activate
+pip install mkdocs-material
+mkdocs serve
+```
+
+提交内容并触发部署：
+
+```bash
+git add docs mkdocs.yml
+
+git commit -m "Update wiki content"
+
+git push origin main
+```
+

