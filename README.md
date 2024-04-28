# Git Starter

This Git repository contains basic and recommended Git configurations in addition to useful web URLs.

## Git configuration

### Basic settings

At least every user should configure her/his name and a commit email address. These settings can be configured globally with the `--global` parameter and will be saved in the user's root directory (`~/.gitconfig`):

```shell
git config --global user.name "firstname lastname"
git config --global user.email firstname.lastname@example.org
```

### Recommended settings

The recommendation for an additional configuration includes:

- global gitignore file ([gitignore](config/gitignore))
- commit message template ([gitmessage](config/gitmessage))
- default branch changed to `main` (from 'master') (requires Git 2.28+)
- simple push (only push current branch)
- recursive submodule init

The basic and recommended settings are provided in the file
[gitconfig-recommendations](config/gitconfig-recommendations).
Please change the user settings, if the content is copied.

### Usage of provided configurations

The global configurations are a user specific settings found in the user home directory (`~/`) (or in the User folder for Windows, e.g. `C:\Users\<YourName>`)

1. copy [gitconfig-recommendations](config/gitconfig-recommendations) to `~/.gitconfig` (or `~/.config/git/config`)
2. replace user name and commit email address in `~/.gitconfig` (or `~/.config/git/config`) directly or [via git config commands](#basic-settings)
3. copy [gitignore](config/gitignore) to `~/.gitignore`
4. copy [gitmessage](config/gitmessage) to `~/.gitmessage`
