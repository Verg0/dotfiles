# My ~

![Screenshot](https://i.imgur.com/HhjEfA3.png)

## Table of contents

<!-- vim-markdown-toc GFM -->

* [Getting Started](#getting-started)
    * [Prerequisites](#prerequisites)
    * [Installation](#installation)
    * [Quick usage instruction](#quick-usage-instruction)
* [Features](#features)
    * [Key bindings](#key-bindings)
    * [zsh](#zsh)
    * [st](#st)
    * [dmenu](#dmenu)
    * [slock](#slock)
    * [polybar](#polybar)
    * [compton](#compton)
    * [Neovim](#neovim)
    * [tmux](#tmux)
    * [Multi monitor support](#multi-monitor-support)
    * [GTK theme](#gtk-theme)
    * [Version control](#version-control)
    * [mpv](#mpv)
    * [Wallpapers](#wallpapers)
* [Acknowledgements](#acknowledgements)

<!-- vim-markdown-toc -->

## Getting Started

### Prerequisites

You can skip this step if you're using Arch Linux, use the install script below to install these packages automatically.

Install the following packages:

- `git`
- `xorg-server`
- `xorg-xinit`
- `bspwm`
- `sxhkd`
- [`polybar`](https://aur.archlinux.org/packages/polybar/)
- [`dmenu`](https://github.com/khuedoan/dmenu)
- [`st`](https://github.com/khuedoan/st)
- [`slock`](https://github.com/khuedoan/slock)
- [`compton-tryone-git`](https://aur.archlinux.org/packages/compton-tryone-git/)
- [`nerd-fonts-source-code-pro`](https://aur.archlinux.org/packages/nerd-fonts-source-code-pro/)

### Installation

Using the method bellow, you can update new features from my repo using `dotfiles pull`, but you can't push your own customization to GitHub.

If you want to push your customization to GitHub, you need to fork this repo, change the `REPO` variable in `install-dotfiles.sh`, then continue running the script with the instruction below. You can't update new features from me automatically with `dotfiles pull`, but you can [do that manually](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork).

Get the install script:

`curl -O https://raw.githubusercontent.com/khuedoan/linux-setup/master/misc/install-dotfiles.sh`

`chmod +x install-dotfiles.sh`

Run the TUI installer:

`./install-dotfiles.sh`

The install dotfiles option will work with any distro, but the install packages options only works with Arch Linux (PR for other distros are welcome).

![Screenshot](https://i.imgur.com/EBTG8mx.jpg)

### Quick usage instruction

Some key mapping are changed, you can change this in `.xinitrc`:

- Capslock is now Ctrl when held and Esc when tapped using `xcape`
- Left Alt and Left Super is swapped

Some basic key bindings:

- `super + /`         for key bindings help
- `super + enter`     for terminal
- `super + space`     for app launcher
- `super + shift + q` to quit app

## Features

### Key bindings

I use `sxhkd` for key bindings. You can check out the dynamically generated list of available key bindings via `super + /` (I choose this because of the `?` symbol)

The general "grammar" of my key bindings are:

- `super + ...`: regularly used or non-destructive actions, launch apps.
- `super + shift + ...`: moving windows, destructive actions, launch apps.
- `super + control + ...`: moving floating windows

### zsh

| Plugin | Details | Screenshot |
| :-- | :-- | :-- |
| powerlevel10k | Using powerlevel10k we have a future rich but still insanely fast prompt, no compromise | |
| zsh-autosuggestion| If we used a command before, it will suggest it the next time you type | |
| zsh-syntax-highlighting | Highlight shell command, no more plain white commands | |

### st

### dmenu

### slock

### polybar

### compton

### Neovim

### tmux

### Multi monitor support

### GTK theme

### Version control

### mpv

The following `dotfiles` command is an alias to [manage dotfiles using git bare](https://news.ycombinator.com/item?id=11070797).

Make change to the config files to suit your needs, then use `dotfiles` command instead of `git` for version control. For example:

`dotfiles add .config/foo`

`dotfiles commit`

`dotfiles push`

`dotfiles pull`

Check out `.aliases` for more

### Wallpapers

| Original | Blured|
| :-- | :-- |
| ![Original](https://i.imgur.com/ZlvUiIZ.jpg) | ![Blured](https://i.imgur.com/C3tCYsp.jpg) |

## Acknowledgements

- **StreakyCobra** for [manage dotfiles using git bare](https://news.ycombinator.com/item?id=11070797)
- **thugcee** for [show sxhkd key bindings with fuzzy search script](https://www.reddit.com/r/bspwm/comments/aejyze/tip_show_sxhkd_keybindings_with_fuzzy_search/)
