# Project Overview

This is a simple Astro project designed as a learning resource for understanding the fundamentals of Large Language Models (LLMs). It includes two main educational pages:

1.  **Basics of Prompting:** An interactive page that explains the core concepts of prompting, including the difference between vague and clear prompts, the roles in a prompt (System, User, Assistant), and techniques like zero-shot and few-shot prompting. It features a "Prompt Quality Checker" to provide real-time feedback on user-written prompts.

2.  **LLM Settings Cheat Sheet:** An interactive guide to common LLM parameters like Temperature, Top P, Max Length, and penalties. It uses sliders and detailed explanations to help users understand how each setting affects the model's output.

The project is built with vanilla JavaScript and CSS, with a focus on creating a clear and engaging user experience.

## Building and Running

The following commands are used to work with this project:

| Command | Action |
| :--- | :--- |
| `npm install` | Installs dependencies |
| `npm run dev` | Starts local dev server at `localhost:4321` |
| `npm run build` | Build your production site to `./dist/` |
| `npm run preview` | Preview your build locally, before deploying |

## Development Conventions

*   **Styling:** The project uses inline `<style>` tags within each `.astro` file for component-specific styling. There is no global CSS file or framework in use.
*   **Routing:** Each `.astro` file in the `src/pages` directory corresponds to a route. For example, `src/pages/basics-of-prompting.astro` is accessible at `/basics-of-prompting`.
*   **Interactivity:** Client-side interactivity is handled by vanilla JavaScript in `<script>` tags within the `.astro` files.

## Gemini CLI Instructions

*   Do not execute any `git` command without explicit confirmation.
*   Do not refactor a page into components without explicit confirmation.
*   When instructed to "refactor this page," it means to:
    *   **Integrate with `src/layouts/Layout.astro`:**
        *   Add `import Layout from '../../layouts/Layout.astro';` to the frontmatter of the page being refactored.
        *   Wrap the entire page's main content (everything that would normally be inside the `<body>` tag, excluding global CSS/JS which are handled by the layout) within a `<div class="container">` which itself is wrapped within `<Layout>...</Layout>`. This `div.container` is used for consistent padding, max-width, and horizontal centering across pages.
        *   **Remove redundant HTML structure:** Ensure the refactored page does *not* contain `<!doctype html>`, `<html>`, `<head>`, or `<body>` tags, as these are provided by `src/layouts/Layout.astro`.
    *   **Manage Styling:**
        *   Move all page-specific `<style>` tags to the bottom of the `.astro` file, *outside* the `<Layout>` component.
        *   Remove any global CSS rules (like `* { ... }` or `body { ... }` selectors) from the page's `<style>` block, as these are handled by `src/layouts/Layout.astro`.
    *   **Manage Scripting:**
        *   Move all page-specific `<script>` tags to the bottom of the `.astro` file, *outside* the `<Layout>` component.
    *   **Update Navigation:**
        *   Add a navigation link to the refactored page in `src/components/Navbar.astro`, ensuring it's placed logically based on its folder hierarchy (e.g., under 'Introduction' for pages in `src/pages/introduction`).
        *   Add a link (card, if applicable) to the refactored page on the main `src/pages/index.astro` page.
