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
