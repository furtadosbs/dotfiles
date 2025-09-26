# 🛠️ Dotfiles Managed with GNU Stow

Welcome to my personal dotfiles repository! This setup helps me keep my development environment consistent across machines using [GNU Stow](https://www.gnu.org/software/stow/), a symlink farm manager that makes managing dotfiles elegant and modular.

## 📦 Structure

Each directory in this repo corresponds to a specific application or tool (e.g., `zsh`, `nvim`, `git`). Inside each folder are the configuration files that would normally live in your home directory.

Example:
```
dotfiles/
├── zsh/
│   └── .zshrc
├── nvim/
│   └── .config/nvim/init.lua
├── git/
│   └── .gitconfig
```

## 🚀 Installation

Clone the repository into your home directory (or wherever you prefer):

```bash
git clone https://github.com/furtadosbs/dotfiles.git ~/dotfiles
cd ~/dotfiles
```

Use GNU Stow to symlink the desired configurations:

```bash
stow zsh
stow nvim
stow git
```

This will symlink the files into your `$HOME` directory, preserving the structure and avoiding clutter.

## 🧼 Uninstalling

To remove symlinks created by Stow:

```bash
stow -D zsh
```

## 🛠 Requirements

- [GNU Stow](https://www.gnu.org/software/stow/)
- Unix-like OS (Linux, macOS, WSL)

## 🧪 Tips

- Keep each app's config in its own folder.
- Use `.config/appname/` structure when needed.
- Test on a fresh machine or VM to ensure portability.

## 📜 License

Feel free to fork and adapt! Licensed under [MIT](LICENSE).
