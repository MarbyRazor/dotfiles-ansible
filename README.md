# Required

- Installed MacOS
- Update your system

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

Afterwards create the following file:

```bash
touch $HOME/.config/dotfiles/vault-password.txt
```

and copy the required password from your keepass file :wink:

Furthermore add your github ssh public and private key to `$HOME/.ssh/`.

# Installation

> Maybe he is asking for your sudo password. This is needed for install the developer tools for your cli.

```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/MarbyRazor/dotfiles-ansible/main/bin/dotfiles)"
```

# Executing the playbook

Just type the following into your terminal

```bash
dotfiles
```

> This will execute the shell script `dotfiles`, which is automatically copied from the repo `bin/dotfiles` to your `$HOME/.local/bin/dotfiles`.

Logout and login

# Big Thanks

- https://github.com/ALT-F4-LLC/dotfiles
- https://www.josean.com/posts/7-amazing-cli-tools
