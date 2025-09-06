# GEMINI_cn.md

本文档提供了基于Astro的博客项目的全面概述，包括其结构、如何开发、自定义和部署它。

## 项目概述

这是一个使用[Astro](https://astro.build/)（现代静态网站生成器）构建的个人博客项目。该博客设计为快速、易于访问和可自定义。它使用[Svelte](https://svelte.dev/)创建交互式组件，使用[Tailwind CSS](https://tailwindcss.com/)进行样式设计。内容以Markdown格式编写，并位于`src/content/posts`目录中。

### 核心技术

*   **Astro:** 构建静态网站的核心框架。
*   **Svelte:** 用于创建交互式UI组件。
*   **Tailwind CSS:** 一个实用优先的CSS框架，用于样式设计。
*   **Markdown:** 编写博客文章的格式。
*   **Pagefind:** 构建后运行的静态搜索库。
*   **Swup:** 用于平滑页面转换的库。
*   **Expressive Code:** 一个用于美观且功能强大的代码块的库。

## 关键配置文件

*   **`astro.config.mjs`:** Astro的主配置文件。它定义了集成、Markdown设置和其他项目范围的配置。
*   **`package.json`:** 列出了项目的依赖项以及用于开发、构建和其他任务的脚本。
*   **`src/config.ts`:** 包含站点的配置，包括标题、作者、导航链接和社交媒体资料。
*   **`tailwind.config.cjs`:** Tailwind CSS的配置文件。它定义了调色板、字体和其他设计令牌。

## 开发

### 运行开发服务器

要启动开发服务器，请运行以下命令：

```bash
pnpm dev
```

这将在`http://localhost:4321`启动一个本地开发服务器。当代码发生更改时，服务器将自动重新加载。

### 创建新文章

要创建新的博客文章，请运行以下命令：

```bash
pnpm new-post
```

这将在`src/content/posts`目录中创建一个带有预定义前置内容（frontmatter）的新Markdown文件。

### 构建项目

要为生产构建项目，请运行以下命令：

```bash
pnpm build
```

这将创建一个包含博客静态文件的`dist`目录。

## 自定义

### 站点配置

要自定义站点的标题、作者、导航链接和社交媒体资料，请编辑`src/config.ts`文件。

### 样式设计

要自定义博客的外观，您可以修改`tailwind.config.cjs`中的Tailwind CSS配置以及`src/styles`目录中的全局样式表。

### 组件

博客的组件位于`src/components`目录中。您可以修改这些组件来更改博客的布局和功能。

## 部署

项目部署到GitHub Pages。`.github/workflows/deploy.yml`文件定义了用于构建和部署项目的GitHub Actions工作流。当新提交推送到`main`分支时，将触发此工作流。
