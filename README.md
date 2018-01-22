sandyleo26 dotfiles
===============

I use [thoughtbot/dotfiles](https://github.com/thoughtbot/dotfiles) and
sandyleo26/dotfiles together using [the `*.local` convention][dot-local].

[dot-local]: http://robots.thoughtbot.com/manage-team-and-personal-dotfiles-together-with-rcm

Requirements
------------

Set zsh as my login shell.

    chsh -s /bin/zsh

Install [rcm](https://github.com/mike-burns/rcm).

    brew tap thoughtbot/formulae
    brew install rcm

Install
-------

Clone onto my laptop:

    git clone https://github.com/sandyleo26/dotfiles.git ~/dotfiles-local
    git clone https://github.com/thoughtbot/dotfiles.git ~/dotfiles

Install:

    env RCRC=$HOME/dotfiles-local/rcrc rcup

This will create symlinks for config files in my home directory.

I can safely run `rcup` multiple times to update.
