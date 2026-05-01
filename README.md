# dev workflow

tmux session manager for my development workflow. Spins up a pre-configured session with windows for the editor, two pi agent instances, and a general 3-pane split window for scripts, gitflow, general-use.

## Windows

- `editor` — launches `$EDITOR` (defaults to Neovim)
- `pi` — two side-by-side panes running `pi`
- `extra` — three panes for git, scripts, and otherwise general-use panes

## Usage

```bash
dev              # Launch session for current directory
dev -p <path>    # Launch session for a directory
dev -h           # Show help
```

Session names are derived from the working directory name (e.g., `dev-myproject`), so multiple sessions can exist simultaneously.

## Installation

```bash
./install.sh
```

Helper to install the `dev` script to `~/.local/bin` and make it executable. Ensure `~/.local/bin` is in `$PATH`.
