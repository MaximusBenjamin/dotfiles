# Neovim Keybindings Reference

Leader key: `<Space>`

## Navigation & Editing

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>h` | n | Clear search highlights |
| `K` | v | Move selected block up |
| `J` | v | Move selected block down |
| `<C-u>` | n | Scroll up half page + center |
| `<C-d>` | n | Scroll down half page + center |
| `n` | n | Next search result + center |
| `N` | n | Previous search result + center |
| `<Down>` | n | Move 5 lines down + center |
| `<Up>` | n | Move 5 lines up + center |
| `<C-c>` | i | Escape (insert mode) |
| `<C-b>` | n | Increment number (remapped from `<C-a>`) |
| `<leader>-` | n, v | Jump to next underscore |
| `<leader>l` | n, v | Jump to previous underscore |

## Yank, Paste & Delete

| Keybind | Mode | Action |
|---------|------|--------|
| `p` | x | Paste without yanking replaced text |
| `<leader>y` | n, v | Yank to system clipboard |
| `<leader>Y` | n | Yank line to system clipboard |
| `<leader>d` | n, v | Delete without yanking |

## Search & Replace

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>sr` | n | Search and replace word under cursor |

## Code Helpers

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>ig` | n | Append `# noqa` to line (ruff ignore) |
| `<leader>jc` | n, v | Comment line with `//` (JS/Vue) |
| `<leader>jd` | n, v | Uncomment `//` (JS/Vue) |
| `<leader>dh` | n | Insert date header (`# YYYY-MM-DD`) |

## Checkboxes

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>ti` | n | Toggle checkbox `[ ]` / `[x]` |
| `<leader>ty` | n | Check checkbox `[ ]` -> `[x]` |
| `<leader>tu` | n | Uncheck checkbox `[x]` -> `[ ]` |

---

## Telescope (plugins/keymaps.lua)

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>fs` | n | Find files in project |
| `<leader>fp` | n | Find git files |
| `<leader>fo` | n | Recently opened files |
| `<leader>fb` | n | Search buffers |
| `<leader>fz` | n | Live grep whole project |
| `<leader>fg` | n | Live grep open files only |
| `<leader>fh` | n | Search help tags |
| `<leader>se` | n | Search emoji (telescope) |
| `<C-j>` | i, n | Telescope: next item |
| `<C-k>` | i, n | Telescope: previous item |

## File Explorer (nvim-tree)

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>e` | n | Toggle file tree (find current file) |

## Comments (nvim-comment)

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>/` | n, v | Toggle comment |

## Icon Picker

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>ic` | n | Open icon picker |

## Twilight & Zen Mode

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>il` | n | Toggle Twilight (dim inactive code) |
| `<leader>zm` | n | Toggle Zen Mode |

## Markdown Preview

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>mp` | n | Toggle markdown preview in browser |

---

## LSP (plugins/lsp.lua)

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>rn` | n | Rename symbol |
| `gd` | n | Go to definition |
| `gr` | n | Go to references (telescope) |
| `gt` | n | Go to type definition |
| `K` | n | Hover documentation |
| `<C-k>` | n | Signature help |
| `:Format` | cmd | Format buffer with LSP |

## Diagnostics

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>dp` | n | Previous diagnostic |
| `<leader>dn` | n | Next diagnostic |
| `<leader>dd` | n | Open diagnostic float |
| `<leader>ds` | n | Diagnostics to location list |

## Goto Preview

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>gd` | n | Preview definition (floating) |
| `<leader>gt` | n | Preview type definition (floating) |
| `<leader>gi` | n | Preview implementation (floating) |
| `<leader>gp` | n | Close all preview windows |

---

## Autocomplete (nvim-cmp)

| Keybind | Mode | Action |
|---------|------|--------|
| `<Tab>` | i, s | Next completion item / expand snippet |
| `<S-Tab>` | i, s | Previous completion item |
| `<CR>` | i | Confirm completion |
| `<C-Space>` | i | Trigger completion |
| `<C-d>` | i | Scroll docs up |
| `<C-f>` | i | Scroll docs down |

---

## Git (gitsigns)

| Keybind | Mode | Action |
|---------|------|--------|
| `]c` | n | Next hunk |
| `[c` | n | Previous hunk |
| `<leader>hp` | n | Preview hunk |
| `<leader>hi` | n | Preview hunk inline |
| `<leader>hD` | n | Diff against uncommitted changes |
| `<leader>hd` | n | Diff against HEAD~{count} |
| `<leader>hQ` | n | All hunks to quickfix |
| `<leader>hq` | n | Buffer hunks to quickfix |
| `<leader>hw` | n | Toggle word diff |
| `<leader>hb` | n | Blame current line |
| `<leader>hB` | n | Blame whole buffer |

---

## Obsidian Workflows (workflows.lua)

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>on` | n | Apply note template |
| `<leader>of` | n | Format note title |
| `<leader>os` | n | Search vault files |
| `<leader>oz` | n | Grep vault files |
| `<leader>ok` | n | Move file to zettelkasten |
| `<leader>odd` | n | Delete current file |
| `gf` | n | Follow wiki link (in vault) |

---

## AI / LLM

### Ollama

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>oo` | n, v | Ollama prompt menu |
| `<leader>oG` | n, v | Ollama generate code |

### OpenCode

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>ae` | n, x | Ask opencode about current context |
| `<leader>at` | n, t | Toggle opencode terminal |
| `<leader>ad` | n, x | Add range to opencode |

### CodeCompanion (currently commented out)

| Keybind | Mode | Action |
|---------|------|--------|
| `<leader>oa` | n, v | CodeCompanion actions |
| `<leader>oe` | n, v | Toggle CodeCompanion chat |
| `ga` | v | Add selection to CodeCompanion chat |
| `:cc` | cmd | Expands to `:CodeCompanion` |

---

## Flash / Jump (flash.nvim)

| Keybind | Mode | Action |
|---------|------|--------|
| `s` | n, x, o | Flash jump |
| `S` | n, x, o | Flash Treesitter |
| `r` | o | Remote Flash |
| `R` | o, x | Treesitter Search |
| `<C-s>` | c | Toggle Flash Search |

## Vim Surround (plugin)

| Keybind | Mode | Action |
|---------|------|--------|
| `cs"'` | n | Change surrounding `"` to `'` |
| `ds"` | n | Delete surrounding `"` |
| `ysiw"` | n | Surround word with `"` |
| `S"` | v | Surround selection with `"` |

## JSON Folding

| Keybind | Mode | Action |
|---------|------|--------|
| `zc` | n | Close fold |
| `zo` | n | Open fold |
| `za` | n | Toggle fold |
| `zR` | n | Open all folds |
| `zM` | n | Close all folds |

---

## Terminal Aliases (.zshrc)

### Neovim

| Alias | Command |
|-------|---------|
| `v` | `nvim` |
| `vim` | `nvim` |

### File Listing (eza)

| Alias | Command |
|-------|---------|
| `ls` | `eza --long --icons=always` |
| `lr` | `eza --long --icons=always --sort=newest` |
| `lt` | `eza --long --icons=always -T` |
| `lt2` | `eza --long --icons=always -T -L=2` |
| `lt3` | `eza --long --icons=always -T -L=3` |

### Tmux

| Alias | Command |
|-------|---------|
| `t` | `tmux` |

### Python

| Alias | Command |
|-------|---------|
| `python3` | `/opt/homebrew/bin/python3.12` |
| `pip3` | `/opt/homebrew/bin/pip3.12` |
| `pyv` | `~/virtualenvs/adhoc/bin/python` |
| `piv` | `~/virtualenvs/adhoc/bin/pip` |
| `jn` | `~/virtualenvs/adhoc/bin/jupyter notebook` |
| `jc` | `~/virtualenvs/adhoc/bin/jupyter console` |

### Git

| Alias | Command |
|-------|---------|
| `gits` | `git status` |
| `gita` | `git add -u` |
| `gitm "msg"` | `git commit -m "msg"` (function) |
| `gitp` | `git push` |
| `gitu` | `git commit -m "Update YYYY-MM-DD"` |
| `gitq` | `git add -u && commit date && push` |
| `gitc` | `aicommits` (AI commit messages) |
| `lg` | `lazygit` |

### Obsidian

| Alias | Command |
|-------|---------|
| `oo` | `cd` to Obsidian vault |
| `or` | Open inbox notes in nvim |
| `ou` | Run notion-obsidian sync (last 5 days) |

### Path Shortcuts

| Alias | Command |
|-------|---------|
| `nvc` | `cd ~/.config/nvim && vim` |
| `zc` | `cd ~/pro/zazencodes-season-2/src` |
| `cmcp` | Edit Claude MCP config |
| `gmcp` | Edit Gemini settings |
| `devlogs` | `vim ~/pro/devlogs` |
| `keybinds` | `nvim ~/dotfiles/nvim/keybinds.md` |

### Navigation

| Alias | Command |
|-------|---------|
| `cl` | `clear` |
| `z` | `cd` |
| `..` | `cd ..` |
| `...` | `cd ../..` |
| `....` | `cd ../../..` |
| `.....` | `cd ../../../..` |
| `......` | `cd ../../../../..` |
| `zr` | `cd` to newest subdirectory (function) |

### Apps & Tools

| Alias | Command |
|-------|---------|
| `cat` | `bat -pp` |
| `fuck` | thefuck (auto-correct previous command) |

### LLM / AI

| Alias | Command |
|-------|---------|
| `llm_gs` | `llm -m gemma3:4b` |
| `llm_gm` | `llm -m gemma3:12b` |
| `llm_gl` | `llm -m gemma3:27b` |
| `llm_cat_dir` | Cat all files in current dir |
| `zc2git` | mcphost with claude-sonnet for zc season 2 |
| `fgemini` | Gemini with flash model |
| `ayima_claude_code` | Claude Code with Ayima API key (function) |

### Scripts

| Alias | Command |
|-------|---------|
| `ayima_search_volumes` | SEMrush keyword overview script |

### FZF Keybindings

| Keybind | Action |
|---------|--------|
| `Ctrl+R` | Fuzzy search command history |
| `Ctrl+T` | Fuzzy file search (fd) |
| `Ctrl+G` | Fuzzy cd into directory (fd) |
| `**<tab>` | Fuzzy directory completion |
