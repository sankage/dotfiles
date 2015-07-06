Sankage Dotfiles
===============

I use [thoughtbot/dotfiles](https://github.com/thoughtbot/dotfiles) and
sankage/dotfiles-local together using [the `*.local` convention][dot-local].

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

    git clone https://github.com/thoughtbot/dotfiles
    git clone https://github.com/sankage/dotfiles-local.git ~/dotfiles-local

Install:

    env RCRC=$HOME/dotfiles/rcrc rcup

This will create symlinks for config files in my home directory.

I can safely run `rcup` multiple times to update.

What's in it?
-------------

[git](http://git-scm.com/) configuration:

* `l` alias for tight, colored, log output.
* My name and email.
