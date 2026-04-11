# gamedev

tmux session manager for my game development workflow. Spins up a pre-configured session with windows for the editor, two opencode instances, and a general dev terminal.

## Windows

- `editor` — launches `$EDITOR` (defaults to Neovim)
- `opencode` — two side-by-side panes running `opencode`
- `dev` — three panes for git, project scripts, and general use

## Usage

```bash
gamedev -p <path>    # Launch session for a project
gamedev -h           # Show help
```

Session names are derived from the project directory name (e.g., `gamedev-myproject`), so multiple project sessions can exist simultaneously.

## Installation

```bash
./install.sh
```

Helper to install the `gamedev` script to `~/.local/bin` and make it executable. Ensure `~/.local/bin` is in `$PATH`.
