# dev workflow

tmux session manager for my development workflow. Spins up a pre-configured session with windows for the editor, two pi agent instances, and a general dev terminal.

## Windows

- `editor` — launches `$EDITOR` (defaults to Neovim)
- `pi` — two side-by-side panes running `pi`
- `dev` — three panes for git, project scripts, and general use

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
