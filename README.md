# Dotfiles

This is a shared dotfiles setup, it sets up a lot of useful defaults and
configuration for a bunch of things.

Clone this repo to anywhere, for example to `~/Projects/dotfiles` and then
run:

```
./setup
```

This will symlink dotfiles from your homedirectory to your checkout of this
repo, allowing you to modify and commit to these files easily.

## Vim

We're using [vim-plug](https://github.com/junegunn/vim-plug) for plugin
management. All plugins are listed in [vimrc](link/vimrc). Start vim and
run:

```
:PlugInstall
```

This should pop open a window and install all plugins.

## PS and bash completion

Install git and bash its bash completion:

```
brew install git bash_completion
```

## Project navigation

Assuming you have your projects in `~/Projects` you can easily jump to them
like this from anywhere:

``` sh
cd /anywhere/on/my/machine
p my_project # jumps to ~/Projects/my_project
p my_p<tab> # autocompletes "my_project"
```
