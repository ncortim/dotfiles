# My dotfiles

This directory contains the dotfiles for setup the workstation

# Dependencies

Ensure you have the following installed on your system

# Git

```bash
sudo apt install git
```

# Stow

```bash
sudo apt install stow
```

# Installation

First, check out the dotfiles repo in your $HOME directory using git

```bash
$ git clone git@github.com/dreamsofautonomy/dotfiles.git
$ cd dotfiles
```

Use file `.stow-local-ignore` if you want to override the default ignored files

Then use GNU stow to create symlinks
```bash
$ stow .
```

In case of conflicts use
```bash
$ stow --adopt .
```

> [NOTE] This moves local files into dotfiles directory and then be allowed
to create the symbolic links


