# tmux-ide

A command for managing tmux sessions for your projects.

## What does it do?

Run `ide path/to/my/project`, and you'll find yourself within a nicely named tmux session with your favourite editor and lazygit ready to go.

The session will be tied to the folder/file location itself. You can detach it, do other work, and return back right where you were by running `ide path/to/my/project` again.

Additional niceties:
- You can freely use both relative and absolute paths as argument, as under the hood the session is always tied to the *absolute path* of the file/folder you provided.
- If the file or folder you opened is within a git repository and `lazygit` is installed, a secondary window with `lazygit` is opened in the repository root.

## Dependencies

Psst: If configuring and installing all of these sounds like too much work, you can find preconfigured versions from [boringconfigs](https://github.com/boringconfigs/).

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
or, even better, if you have [fzf](https://github.com/junegunn/fzf) installed, you can do

```bash
ide **<tab>
```

and fuzzy find your way to whereever you want to go.

### Arguments

- `path` (optional) - Path to the project root directory or a file. If not provided, the current directory is used.

## Installation

```bash
brew install EskelinenAntti/cli/tmux-ide
```
