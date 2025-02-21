# Git Pullmaster

![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)

A simple GitHub CLI extension that pulls updates for all git repositories located in subfolders of the current directory. This is particularly useful in the context of microservices.

## 📜 Description

This extension iterates over each directory in the current folder, checks if it is a Git repository, and if so, pulls the latest changes from the respective remote branch. It provides clear output indicating which repositories are being pulled and skips directories that are not Git repositories.

## 🛠️ Installation

To install this extension, you need to have the GitHub CLI installed. If you don't have it yet, you can find installation instructions [here](https://docs.github.com/en/github-cli/github-cli/installation).

1. **Install the extension**:
    ```bash
    gh extension install tkachenko0/gh-pullmaster
    ```

## 🚀 Usage

1. Navigate to the directory containing your subdirectories with Git repositories.
    ```bash
    cd path/to/your/directory
    ```

2. Run the extension:
    ```bash
    gh pullmaster
    ```

## 💻 Example Output

When you run the extension, you should see output similar to the following:

```plaintext
Pulling in ProjectA on branch main
Already up to date.
Skipping directory non-git-folder/ - not a git repository
Pulling in ProjectB on branch develop
Updating a1b2c3d..d4e5f6
```
## Updates

To istall new updates run the following

```bash
gh extension upgrade tkachenko0/gh-pullmaster
```

## 📚 More Information

For more information on using GitHub CLI extensions, refer to the [GitHub CLI documentation](https://docs.github.com/en/github-cli/github-cli/using-github-cli-extensions).
