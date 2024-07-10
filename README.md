# Required

- Installed Manjaro with i3
- Update your system `sudo pacman -Syu`

# Preparation

Create a `values.yaml`

```bash
cd $HOME && mkdir -p $HOME/.config/dotfiles && vim $HOME/.config/dotfiles/values.yaml
```

with the following content

```yaml
---
git_user_email: your-email@address.com
git_user_name: your name
```

# Installation

```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/MarbyRazor/dotfiles-i3-ansible/main/bin/dotfiles)"
```

# Post configurations

Make ZSH as default

```bash
chsh -s $(which zsh)
```

Logout and login

# Big Thanks

- https://github.com/ALT-F4-LLC/dotfiles
