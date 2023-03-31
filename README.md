# Darwin Dotfiles

Too lazy to automate this yet... these are the steps I took when setting up a new M2 Pro MBP.

## System

- Setup correct hostname
- Removed all items from dock
- Make menu and dock always autohide
- Create new SSH keys

#### Keybinds

- Mission Control use ALT + N to move between workspaces
- Spotlight use CMD + D to open

## Brews

Packages are installed with [brew](https://brew.sh/):

- git
- wezterm
- neovim
- slack
- amethyst
- nvm
- jq
- shellcheck
- grip
- firefox
- htop
- flameshot

## Software Configurations

### node.js

Node is managed via [nvm](https://github.com/nvm-sh/nvm):

`nvm install node`

### neovim

_note: Make sure node is installed before running nvim since the plugins require it._

1. Copy config from [20k-ultra/dotfiles/nvim](https://github.com/20k-ultra/dotfiles/tree/master/nvim)
2. Start nvim and run `Lazy :sync` and `MasonUpdateAll`

### Terminal

1. Copy config from [20k-ultra/dotfiles/wezterm](https://github.com/20k-ultra/dotfiles/tree/master/wezterm)

### Firefox

1. download extensions https://addons.mozilla.org/en-US/firefox/collections/16570358/My-add-ons/
2. in FF settings:

- set tab to cycle through tabs in recent order
- customize toolbar:
  - enable title
  - remove junk spaces
- add userChrome.css from [20k-ultra/dotfiles/firefox](https://github.com/20k-ultra/dotfiles/tree/master/firefox/chrome)
- customize toolbar and enable title bar
- verify tree style tab extension settings
- enable HTTPS everywhere
  - go to about:preferences#privacy and enable at the bottom of the page

### Amethyst

Apply the following keybinds:

- cycling between tiles: ALT + J or ALT + K
- focus to main: ALT + ENTER
- resize to tiles: ALT + H or ALT + L

### Flameshot

Add the following keybinds:

- capture screen: CTRL + SHIFT + S
