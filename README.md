# Gemini CLI Git Extension

This project provides a powerful extension for the Gemini CLI, offering advanced Git workflow automation. It streamlines common development tasks by integrating Conventional Commits, Git-Flow branching strategies, and automated Pull Request workflows directly into your command-line interface.

## ✨ Features

- **Conventional Commit Automation**: Automatically stages changes and generates high-quality commit messages following the Conventional Commits specification, ensuring a clean and consistent commit history.
- **Git-Flow Branching**: Enforces Git-Flow branching principles, automatically creating new feature branches from `develop` when using the commit command.
- **Pull Request Management**: Simplifies the Pull Request (PR) creation process by syncing local branches with remotes, generating descriptive PR titles and bodies from commit history, and opening the PR directly in your browser using `gh`, `glab`, or a direct URL.
- **Intelligent Push Synchronization**: Ensures local changes are synchronized with the remote repository, including automated commits with Conventional Commit messages and pushing to the correct upstream branches, with safeguards against direct pushes to `main`/`master` without explicit intent.

## 🚀 Installation

_Instructions on how to install the Gemini CLI Git Extension will go here. This typically involves using the Gemini CLI's own extension management command._

```bash
# Example: (Please replace with actual installation command)
gemini install gemini-cli-git
```

## 💡 Usage

Once installed, you can use the following commands:

### `/commit [project name (optional)]`

Automates the staging and committing process. It analyzes your repository, determines if a new branch is needed based on Git-Flow, and crafts a Conventional Commit message based on your actual code changes.

```bash
/commit
# Or with a project scope
/commit "my-feature"
```

### `/pr [project name (optional)]`

Facilitates the creation of Pull Requests. It helps identify feature branches, handles unsynced changes, and prepares the necessary commands to create and open the PR in your browser.

```bash
/pr
# Or with a project scope
/pr "api-refactor"
```

### `/push [project name (optional)]`

Synchronizes your local changes with the remote repository. This command ensures all pending work is committed according to Conventional Commits standards and pushed to the correct upstream branch following Git-Flow principles.

```bash
/push
# Or with a project scope
/push "docs-update"
```

## 🤝 Contributing

We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to get started, our commit standards, and the pull request process.
