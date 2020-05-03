## Chrome

Download, login. Get the order of accounts right.

## 1Password

Download, configure. Phone required.

## Homebrew

Firstly, we need Homebrew to manage dependencies. 

In the dotfiles we have a Brewfile. We need to install brew, install git, clone the dotfiles repo, then run the brewfile.

- Install homebrew: https://brew.sh/
- `brew install git`
- `git clone https://github.com/iHiD/dotfiles.git ~/.dotfiles`
- `ln -s ~/.dotfiles/files/Brewfile ~/Brewfile`
-  `cd ~ && brew bundle`

## Terminal

Load iHiD terminal from dotfiles:/files

## Fish

Fish will be installed via Homebrew. Run these to make it default:
- `echo /usr/local/bin/fish | sudo tee -a /etc/shells `
- `chsh -s /usr/local/bin/fish`
- `ln ~/.dotfiles/files/config.fish ~/.config/fish/config.fish`

Install fisher:
- `curl https://git.io/fisher --create-dirs -sLo ~/.config/fish/functions/fisher.fish`
- `ln -s ~/.dotfiles/files/fishfile ~/.config/fish/fishfile`
- `fish -c fisher`

Set correct colours for ls:
`set -Ux LSCOLORS gxfxbEaEBxxEhEhBaDaCaD`

## Alfred

Download: https://www.alfredapp.com/

## Visual Studio Code

Install from https://code.visualstudio.com/

Copy settings:W
`ln -s  ~/.dotfiles/files/code-settings.json ~/Library/Application\ Support/Code/User/settings.json`