# A Stable IDE config for Neovim

## Get healthy

Open `nvim` and enter the following:

```
:checkhealth
```

## Configuration

### Use NerdFont monofur

### LSP

To add a new LSP

First Enter:

```
:LspInstallInfo
```

and press `i` on the Language Server you wish to install

Next you will need to add the server to this list: [servers](https://github.com/LunarVim/nvim-basic-ide/blob/8b9ec3bffe8c8577042baf07c75408532a733fea/lua/user/lsp/lsp-installer.lua#L6)

### Formatters and linters

Make sure the formatter or linter is installed and add it to this setup function: [null-ls](https://github.com/LunarVim/nvim-basic-ide/blob/8b9ec3bffe8c8577042baf07c75408532a733fea/lua/user/lsp/null-ls.lua#L13)

**NOTE** Some are already setup as examples, remove them if you want

## Usage

### Navigation

Switch buffers
Move between windows
Inside the buffer window,
  - highlight file location in the Tree
  - quick search file and content, open searched files in splitted windows
Inside tree window,
  - create, rename, delete files
  - open file in splitted windows

### LSP
Formatting code on save
Display linting reports

### Github Copilot

## Keymaps

⌥ Option or Alt
⌘ Command or Cmd
⇧ Shift
⌃ Control or Ctrl
⇪ Caps Lock

the leader key can be <cmd> or <space>

- t Show problem/trouble view
- o Find files
- f Find in files
- s Save file
- w close file
- +/- expand/collapse code block
- [/] Navigate back/forward
- p move to project/navigation window

Control

- k/j Select previous/next item
- r Show variable/function usages/references in all places
- d Go to declaration/definitions
- a Show actions
- f quick fix problem(eslint)
- s find and replace
- i quick documentation
- e view error description
- p show parameter info
- u go to next usage in the current file

Cmd + Shift

- r reload all
- +/- expand/collapse all code blocks
- [/] Select previous/next tab/buffer
- k/j Select previous/next highlighted error
