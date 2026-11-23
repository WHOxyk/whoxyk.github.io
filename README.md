# WHOxyk 的文章与笔记

网站地址：https://whoxyk.github.io

仓库地址：https://github.com/WHOxyk/whoxyk.github.io

## 发布新文章（只需要浏览器）

1. 登录 GitHub，打开上面的仓库。
2. 点击 `_posts` 文件夹。
3. 点击 **Add file → Create new file**。
4. 输入文件名，例如 `2026-11-23-reading-notes.md`。日期用实际发布日期，不要使用未来日期；同一天的文章使用不同的英文短名。
5. 复制以下模板，修改标题、日期和正文。标题可以使用中文；标点和开头两行 `---` 请保留。

```markdown
---
layout: post
title: "我的读书笔记"
date: 2026-11-23 00:00:00 +0800
categories: notes
---

这里写文章的第一段。

## 一个小标题

这里继续写正文。

- 第一个要点
- 第二个要点
```

6. 点击 **Commit changes…**，选择 **Commit directly to the main branch**，再点击 **Commit changes**。
7. 等待 GitHub 自动发布，通常几分钟，可能需要约 10 分钟。刷新网站即可看到新文章。

## 修改内容

- 修改文章：打开 `_posts` 中对应文件，点击铅笔图标编辑，保存提交。
- 修改首页简介：编辑 `index.md` 中两行 `---` 后的文字。
- 修改网站名字：编辑 `_config.yml` 中的 `title`。
- 修改个人介绍：编辑 `about.md` 中两行 `---` 后的文字。
- 文章与 note 都可以放在 `_posts` 中。当前首页统一按日期显示所有内容。
- 示例文章可以直接替换内容；文章标题、日期和文件名请相应调整。

## 首次部署或重新部署

仓库 **Settings → Pages → Build and deployment**：

- Source：**Deploy from a branch**
- Branch：**main**
- Folder：**/ (root)**
- 点击 **Save**。

文件必须在仓库根目录；`_posts` 保留为文件夹。不要将 ZIP 文件直接作为网站上传，也不要创建 `.nojekyll`。

## 图片

在仓库新建 `assets/images` 目录并上传图片后，文章中可写：

```markdown
![图片说明](/assets/images/example.png)
```

文件名区分大小写。上传与 Markdown 引用的文件名要一致。

## 常见问题

- 页面暂时显示 404：先检查 Pages 的分支和目录，再到 **Actions** 查看发布是否成功。
- 文章没出现在首页：检查文件是否放在 `_posts`、文件名是否有日期、扩展名是否为 `.md`，以及开头的 `---` 是否完整。未来日期文章默认不会发布。
- 网站仍显示旧内容：等待发布完成，再按 Ctrl+F5 刷新。

此方案的网站和源码公开可见，请只上传准备公开的内容。

参考：https://docs.github.com/en/pages/quickstart
