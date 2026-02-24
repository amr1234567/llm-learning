# LLM Learning Project

## 🚀 Project Overview

This is a simple Astro project designed as an interactive learning resource for understanding the fundamentals of Large Language Models (LLMs) and effective prompting techniques. It aims to provide clear, practical examples and explanations for developers and enthusiasts looking to grasp LLM concepts.

### Key Features:

1.  **Basics of Prompting:** An interactive page explaining core prompting concepts, including prompt structure (System, User, Assistant roles) and techniques like zero-shot and few-shot prompting. Features a "Prompt Quality Checker" for real-time feedback.
2.  **LLM Settings Cheat Sheet:** An interactive guide to common LLM parameters (Temperature, Top P, Max Length, penalties), demonstrating how each setting influences model output.
3.  **Prompt Examples — Dissected:** A detailed breakdown of 7 real-world prompting examples, illustrating effective techniques, their impact on output, and pitfalls to avoid.

The project is built with vanilla JavaScript and CSS for client-side interactivity, leveraging Astro for a fast, modern static site experience.

## 🛠️ Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

*   Node.js (LTS version recommended)
*   npm or Yarn

### Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/amr1234567/llm-learning.git
    cd llm-learning
    ```
2.  Install NPM dependencies:
    ```bash
    npm install
    ```

### Running Locally

To start the development server:
```bash
npm run dev
```
This will start the local dev server at `localhost:4321`.

## 📂 Project Structure

The key directories and files in this project are:

```
├── public/                  # Static assets (favicons, images)
├── src/
│   ├── components/          # Reusable Astro components (Navbar, Sidebar)
│   ├── layouts/             # Astro layout components (e.g., Layout.astro)
│   └── pages/               # Astro pages, defining routes (e.g., /introduction/basics-of-prompting)
│       └── introduction/    # Pages related to LLM introductions
├── GEMINI.md                # Gemini CLI instructions and project-specific conventions for agents
└── README.md                # This file
```

## 📐 Development Conventions

*   **Styling:** Component-specific styling is typically handled using inline `<style>` tags within each `.astro` file. There is no global CSS file or framework in use beyond the base styles in `Layout.astro`.
*   **Routing:** Each `.astro` file within the `src/pages` directory automatically becomes a route.
*   **Interactivity:** Client-side interactivity is implemented using vanilla JavaScript within `<script>` tags embedded in the `.astro` files.
*   **Layout:** All content pages should utilize `src/layouts/Layout.astro` for consistent structure, navigation, and base styling.
*   **Page Content Wrapper:** Main page content within `<Layout>` should be enclosed in a `<div class="container">` for consistent padding, max-width, and centering.
*   **Page Titles:** Each page using `Layout.astro` must pass a `title` prop to the layout component, which will be used in the browser tab (e.g., `<Layout title="Basics of Prompting">`).

## 🤝 Contributing

We welcome contributions to improve this learning resource! To contribute:

1.  **Fork** the repository on GitHub.
2.  **Clone** your forked repository to your local machine.
3.  **Create a new branch** for your feature or bug fix:
    ```bash
    git checkout -b feature/your-feature-name
    ```
    or
    ```bash
    git checkout -b bugfix/issue-description
    ```
4.  **Make your changes**, adhering to the existing coding style and project conventions.
    *   **Refer to `GEMINI.md` for specific instructions on refactoring pages and other agent-assisted development guidelines.**
5.  **Test your changes** thoroughly to ensure everything works as expected.
6.  **Commit your changes** with a clear and descriptive commit message.
7.  **Push your branch** to your forked repository:
    ```bash
    git push origin feature/your-feature-name
    ```
8.  **Open a Pull Request** from your branch to the `main` branch of the original repository.
    *   Clearly describe the changes you've made and why they are necessary.
    *   Ensure your pull request passes all automated checks.

Your pull request will be reviewed, and feedback may be provided. Please be responsive to comments and be prepared to make further adjustments.