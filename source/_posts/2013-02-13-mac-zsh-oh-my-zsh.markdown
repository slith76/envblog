---
layout: post
title: "Mac ZSH oh-my-zsh"
date: 2013-02-13 12:21
comments: true
categories: 
---
## ZSH:

### Install:

        brew install zsh

### Change the Default Shell:

Mac: Systemeinstellungen - Benutzer - Erweiterte Optionen beim Nutzer (unlocked!)

### oh-my-zsh

[https://github.com/robbyrussell/oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)

        git clone git://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh
        cp ~/.zshrc ~/.zshrc.orig
        cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc
        #chsh -s /bin/zsh ##set the default shell

#### Usage:

Themes: https://github.com/robbyrussell/oh-my-zsh/wiki/themes
