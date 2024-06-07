# Required

- Installed Manjaro with i3

# Preparation

Create a `values.yaml`

```bash
cd $HOME && mkdir -p .config/dotfiles && vim .config/dotfiles/values.yaml
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

# Big Thanks

- https://github.com/ALT-F4-LLC/dotfiles
