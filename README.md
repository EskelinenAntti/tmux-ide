# tmux-ide

A script to manage tmux sessions for your projects.

## Overview

`tmux-ide` is a simple shell script for creating and managing tmux sessions for your projects.

Run `ide [path_to_your_project_or_file]`, and the command either attaches you to an existing session or creates a new one if one didn't exist for the given path.

## Features

- **Automatic Session Management:** Creates a new tmux session if one doesn't exist for the specified path, or attaches to an existing session.
- **Git Integration:**
  - If the given path is inside git repository, the tmux session is created automatically in the root of the project directory.
  - If the project is a git repository and `lazygit` is installed, a new window with `lazygit` is automatically opened.

## Dependencies

Psst: If configuring and installing all of these sounds scary, you can find preconfigured versions from [boringconfigs](https://github.com/boringconfigs/).

### Required
- [tmux](https://github.com/tmux/tmux)
- [git](https://git-scm.com/)

### Optional but recommended
- [lazygit](https://github.com/jesseduffield/lazygit) for easier and quicker git actions.
- [Helix](https://helix-editor.com/) to be used as your text editor, aka `$EDITOR`.
- [fzf](https://github.com/junegunn/fzf) for fuzzy finding folders.

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
