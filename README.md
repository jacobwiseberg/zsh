# Zsh

This repository houses my Zsh configuration, organized according to XDG standards to keep the home directory clean. It uses **Oh My Zsh** for plugin management and theme support.

## 📂 Structure

- `~/.zshenv`: The entry point that redirects Zsh to this folder.
- `~/.config/zsh/.zshrc`: The main configuration and customization file.
- `~/.config/zsh/.oh-my-zsh/`: The framework files (managed with git submodule).
- New plugins and themes can be added in the `custom` folder inside the Oh My Zsh directory.

## 🚀 Installation

To set up this configuration on a new machine:

### 1. Redirect Zsh (Critical Step)
Zsh looks in `~` by default. You must tell it to look in `~/.config/zsh` by creating a `.zshenv` file in your **home** directory:

```bash
echo 'export ZDOTDIR=$HOME/.config/zsh' > ~/.zshenv
```