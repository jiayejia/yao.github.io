# GEMINI.md

This file provides a comprehensive overview of the Astro-based blog project, its structure, and how to develop, customize, and deploy it.

## Project Overview

This is a personal blog project built with [Astro](https://astro.build/), a modern static site generator. The blog is designed to be fast, accessible, and easily customizable. It uses [Svelte](https://svelte.dev/) for interactive components and [Tailwind CSS](https://tailwindcss.com/) for styling. The content is written in Markdown and is located in the `src/content/posts` directory.

### Key Technologies

*   **Astro:** The core framework for building the static site.
*   **Svelte:** Used for creating interactive UI components.
*   **Tailwind CSS:** A utility-first CSS framework for styling.
*   **Markdown:** The format for writing blog posts.
*   **Pagefind:** A static search library that runs after the build.
*   **Swup:** A library for smooth page transitions.
*   **Expressive Code:** A library for beautiful and functional code blocks.

## Key Configuration Files

*   **`astro.config.mjs`:** The main configuration file for Astro. It defines integrations, Markdown settings, and other project-wide configurations.
*   **`package.json`:** Lists the project's dependencies and scripts for development, building, and other tasks.
*   **`src/config.ts`:** Contains the site's configuration, including the title, author, navigation links, and social media profiles.
*   **`tailwind.config.cjs`:** The configuration file for Tailwind CSS. It defines the color palette, fonts, and other design tokens.

## Development

### Running the Development Server

To start the development server, run the following command:

```bash
pnpm dev
```

This will start a local development server at `http://localhost:4321`. The server will automatically reload when you make changes to the code.

### Creating a New Post

To create a new blog post, run the following command:

```bash
pnpm new-post
```

This will create a new Markdown file in the `src/content/posts` directory with a predefined frontmatter.

### Building the Project

To build the project for production, run the following command:

```bash
pnpm build
```

This will create a `dist` directory with the static files for the blog.

## Customization

### Site Configuration

To customize the site's title, author, navigation links, and social media profiles, edit the `src/config.ts` file.

### Styling

To customize the blog's appearance, you can modify the Tailwind CSS configuration in `tailwind.config.cjs` and the global stylesheets in the `src/styles` directory.

### Components

The blog's components are located in the `src/components` directory. You can modify these components to change the layout and functionality of the blog.

## Deployment

The project is deployed to GitHub Pages. The `.github/workflows/deploy.yml` file defines the GitHub Actions workflow for building and deploying the project. The workflow is triggered when a new commit is pushed to the `main` branch.
