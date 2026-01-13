# Sidestreams
 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
index 448a2af39d42d8c1b5765d30e80f55432f02590c..c89e24a382b0eab808183f3d1cc2952887faf8a1 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,17 @@
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
 
EOF
)
