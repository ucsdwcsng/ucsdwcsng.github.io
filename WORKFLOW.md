# 添加论文网页 + 本地预览 + 合并到主分支

## 一、在**自己的分支**上工作

```bash
cd /path/to/ucsdwcsng.github.io
git checkout pearson_dev   # 或你的分支名
git pull origin pearson_dev
```

之后所有修改都在这个分支上做，**不要**在 `main`/`master` 上直接改。

---

## 二、在 `_posts` 里添加新论文页面

1. **参考已有文章**  
   打开 [\_posts 目录](https://github.com/ucsdwcsng/ucsdwcsng.github.io/tree/master/_posts)，参考同类型论文的 `.md` 文件（如 `2025-12-12-prism.md`）。  
   格式说明见：`_posts/README.md`。

2. **新建一篇帖子**  
   在 `_posts/` 下新建文件，**文件名**格式：`YYYY-MM-DD-简短英文名.md`  
   例如：`2025-12-12-phoenix.md`。

3. **写 front matter 和正文**  
   复制一篇类似文章（如 `2025-12-12-prism.md`）的头部 YAML，按 README 和示例改：
   - `title`, `short_title`, `tags`, `authors`, `conference`, `paper` 等必填项
   - `author_list`、`description`、`citation` 等按需填写
   - 图片放到 `assets/images/你的项目名/`，PDF 放到 `files/`，在 YAML 里用 `/assets/images/...`、`/files/xxx.pdf` 引用。

---

## 三、本地用 Jekyll 编译并预览

任选一种方式，在项目根目录执行。

### 方式 A：Docker（推荐，不依赖本机 Ruby）

```bash
docker compose up
```

浏览器打开：**http://localhost:4000**。

### 方式 B：本机 Ruby + bundle exec

```bash
bundle install --path vendor/bundle
bundle exec jekyll serve
```

浏览器打开：**http://localhost:4000**。

确认你的新论文页面显示正常、链接和图片都没问题。

---

## 四、验证通过后：推分支 + 用 PR 合并到主分支

1. **提交并推送你的分支**

   ```bash
   git add .
   git status   # 确认要提交的文件
   git commit -m "Add Phoenix paper page"
   git push origin pearson_dev
   ```

2. **在 GitHub 上开 Pull Request**
   - 打开：https://github.com/ucsdwcsng/ucsdwcsng.github.io
   - **左边 Base**：选主分支（`master` 或 `main`，以仓库默认分支为准）
   - **右边 Compare**：选你的分支（如 `pearson_dev`）
   - 填写 PR 标题和说明，点 **Create pull request**。

3. **合并**
   - 审阅通过后点 **Merge pull request**，把你的分支合并进主分支。

---

## 小结

| 步骤 | 做什么 |
|------|--------|
| 1 | 在自己分支工作：`git checkout pearson_dev` |
| 2 | 在 `_posts` 按示例添加 `YYYY-MM-DD-xxx.md`，资源放 `assets/images/`、`files/` |
| 3 | 本地预览：`docker compose up` 或 `bundle exec jekyll serve` → 打开 http://localhost:4000 |
| 4 | 验证无误后：`git push origin pearson_dev` |
| 5 | GitHub：New PR，**Base=主分支**，**Compare=你的分支** → Merge |

**不要**直接 `git push origin main`：主分支受保护，必须通过 PR 合并。
