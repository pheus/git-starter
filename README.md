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

- Global gitignore file ([gitignore](config/gitignore))
- Commit message template ([gitmessage](config/gitmessage))
- Default branch changed to `main` (from 'master') (requires Git 2.28+)
- Simple push (only push current branch)
- Recursive submodule init

The basic and recommended settings are provided in the file
[gitconfig-recommendations](config/gitconfig-recommendations).
Please change the user settings if the content is copied.

### Optional settings

Some additional settings are included in the [gitconfig-complete](config/gitconfig-complete) configuration template (like aliases and color settings).

### Usage of provided configurations

The global configurations are a user-specific settings found in the user home directory (`~/`) (or in the User folder for Windows, e.g. `C:\Users\<YourName>`)

1. Copy either [gitconfig-recommendations](config/gitconfig-recommendations) or [gitconfig-complete](config/gitconfig-complete) to `~/.gitconfig` (or `~/.config/git/config`)
2. Replace username and commit email address in `~/.gitconfig` (or `~/.config/git/config`) directly or [via git config commands](#basic-settings)
3. Copy [gitignore](config/gitignore) to `~/.gitignore`
4. Copy [gitmessage](config/gitmessage) to `~/.gitmessage`

## Useful resources

Git basics:

- Git cheat sheet: [Git Cheat Sheet (from GitHub)](https://education.github.com/git-cheat-sheet-education.pdf)
- Git Introduction: [Git: The Beginner's Guide to Understanding Core Version Control Concepts](https://www.freecodecamp.org/news/git-the-laymans-guide-to-understanding-the-core-concepts/)
- Git Basics: [Free Git book](https://git-scm.com/book/)

Best practices:

- Git ignore: [Git ignore recommendations](https://github.com/github/gitignore)
- Commit Messages: [Git commit message best practices](https://chris.beams.io/posts/git-commit/)
