# Contributing to Gemini CLI Git Extension

Thank you for your interest in contributing! We love pull requests from everyone. By participating in this project, you agree to uphold a safe and welcoming environment.

## 🚀 Getting Started

1.  **Fork** the repository on GitHub.
2.  **Clone** your fork locally:
    ```bash
    git clone https://github.com/your-username/gemini-cli-git.git
    cd gemini-cli-git
    ```
3.  **Create a Branch** for your changes. We follow **Git Flow**:
    *   For features: `git checkout -b feature/my-new-feature`
    *   For bug fixes: `git checkout -b fix/my-bug-fix`

## 🛠️ Development Workflow

This extension is configuration-driven using `gemini-extension.json` and TOML files.

1.  **Modify** the command definitions in the `commands/` directory.
2.  **Test** your changes by installing the extension from the local source:
    ```bash
    gemini install .
    ```
3.  **Verify** the commands work as expected in your terminal.

## 📝 Commit Guidelines

We strictly follow **Conventional Commits**. This is crucial for our automated release process.

**Format:** `<type>(<scope>): <subject>`

**Allowed Types:**
*   `feat`: A new feature
*   `fix`: A bug fix
*   `docs`: Documentation only changes
*   `style`: Formatting, missing semi-colons, etc; no code change
*   `refactor`: Refactoring production code
*   `perf`: A code change that improves performance
*   `test`: Adding missing tests, refactoring tests
*   `chore`: Updating build tasks, package manager configs, etc

**Example:**
```text
feat(pr): add support for gitlab merge requests
```

## 📬 Pull Requests

1.  Push your branch to your fork (`git push origin feature/my-new-feature`).
2.  Open a Pull Request against the **`develop`** branch of the main repository.
3.  Describe your changes clearly and link to any relevant issues.
