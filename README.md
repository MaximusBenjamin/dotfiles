# dotfiles

Originally forked from [zazencodes/dotfiles](https://github.com/zazencodes/dotfiles), with my own additions and changes over time.

## Configs

```bash
git clone https://github.com/MaximusBenjamin/dotfiles.git ~/dotfiles

ln -s ~/dotfiles/alacritty ~/.config/alacritty
ln -s ~/dotfiles/nvim ~/.config/nvim
ln -s ~/dotfiles/.tmux.conf ~/.tmux.conf
ln -s ~/dotfiles/.zshrc ~/.zshrc
ln -s ~/dotfiles/.p10k.zsh ~/.p10k.zsh
ln -s ~/dotfiles/.gitconfig ~/.gitconfig

# llm cli tool templates
# Do not run this until after you have installed llm
rm -rf ~/Library/Application\ Support/io.datasette.llm/templates # delete if exists
ln -s ~/dotfiles/llm/templates ~/Library/Application\ Support/io.datasette.llm
```

## Secrets

`.zshrc` sources two untracked files — create them before opening a new shell:

```bash
touch ~/.secrets.sh   # exported credentials (API keys etc.)
touch ~/.zshrc.local  # machine-local env vars
```

## `/bin`

Scripts intended to be symlinked into `~/bin`:

```bash
mkdir -p ~/bin
./symlink_dotfiles.sh

# Runs symlink command for each file in ~/dotfiles/bin
# But ignores files that already exist
# e.g.
# ln -s ~/dotfiles/bin/on ~/bin/on
```
