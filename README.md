# tmux-ide

A script to manage tmux sessions for your projects.

## Overview

`tmux-ide` is a simple shell script that streamlines your development workflow by creating and managing tmux sessions for your projects. It automatically creates a new tmux session for a given directory or attaches to an existing one, providing a consistent and efficient development environment.

## Features

- **Automatic Session Management:** Creates a new tmux session if one doesn't exist for the specified directory, or attaches to an existing session.
- **Git Integration:** If the project is a git repository, it automatically opens a new window with `lazygit`.
- **Workspace Awareness:** The tmux session is created in the root of the project directory, providing a clean and organized workspace.
- **Helix Integration:** Opens the selected file or directory in Helix editor.

## Dependencies

- [tmux](https://github.com/tmux/tmux)
- [git](https://git-scm.com/)
- [lazygit](https://github.com/jesseduffield/lazygit)
- [Helix](https://helix-editor.com/)

## Usage

```bash
ide [path]
```

### Arguments

- `path` (optional) - Path to the project root directory or a file. If not provided, the current directory is used.

## Installation

```bash
brew install EskelinenAntti/cli/tmux-ide
```
