---
title: 简单的Fuwari博客模板指南
published: 2025-07-01
description: "Fuwari博客模板的使用方法。"
image: ""
tags: ["Example"]
category: Examples
draft: false
---

## Front-matter of Posts

![](https://cdn.jsdelivr.net/gh/YAO-JIAYE/my_imgs_repo@main/imgs/cover.jpeg)

```yaml
---
title: My First Blog Post
published: 2023-09-09
description: This is the first post of my new Astro blog.
image: ./cover.jpg
tags: [Foo, Bar]
category: Front-end
draft: false
---
```
| 属性         | 描述                                                                                                                                                                                                 |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `title`       | 文章的标题。                                                                                                                                                                                      |
| `published`   | 文章的发布日期。                                                                                                                                                                            |
| `description` | 文章的简短描述。显示在索引页上。                                                                                                                                                   |
| `image`       | 文章的封面图片路径。<br/>1. 以 `http://` 或 `https://` 开头：使用网络图片<br/>2. 以 `/` 开头：表示图片位于 `public` 目录<br/>3. 无上述前缀：相对于 Markdown 文件的路径 |
| `tags`        | 文章的标签。                                                                                                                                                                                       |
| `category`    | 文章的分类。                                                                                                                                                                                   |
| `draft`       | 是否为草稿（草稿不会显示）。                                                                                                                                                    |
## Where to Place the Post Files



帖子文件应该放在 `src/content/posts/` 目录中。您也可以创建子目录，以便更好地组织您的帖子和资源。

```
src/content/posts/
├── post-1.md
└── post-2/
    ├── cover.png
    └── index.md
```
