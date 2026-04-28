# Personal Website — Jekyll + GitHub Pages

這是一個履歷型個人網站，適合放履歷、作品集、專案與文章。

## 如何部署到 GitHub Pages

1. 建立一個 GitHub repository，名稱建議：`your-github-username.github.io`
2. 將本資料夾所有檔案上傳到 repository 根目錄。
3. 到 repository 的 Settings → Pages。
4. Source 選擇 `Deploy from a branch`。
5. Branch 選擇 `main`，資料夾選擇 `/root`。
6. 儲存後等待 GitHub Pages 部署。

## 如何新增文章

在 `_posts` 資料夾新增 markdown 檔案，命名格式：

`YYYY-MM-DD-title.md`

檔案開頭需包含：

```yaml
---
layout: post
title: "文章標題"
---
```

## 如何新增專案

在 `projects` 資料夾新增 markdown 檔案，開頭格式：

```yaml
---
layout: project
title: "專案標題"
category: "分類"
summary: "一句話摘要"
---
```

## 本地預覽

```bash
bundle install
bundle exec jekyll serve
```

然後打開 `http://localhost:4000`。
