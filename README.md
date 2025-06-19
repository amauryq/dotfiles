# Development Environment Configuration Setup (dotfiles)

## Homebrew Installation

```sh
export HOMEBREW_NO_INSTALL_FROM_API=1
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Use `stow` to create required symlinks

### neovim

```sh
mkdir ~/.config/nvim
stow -v2 -d ~/repos/amauryq/dotfiles/.config -t ~/.config/nvim nvim
```
