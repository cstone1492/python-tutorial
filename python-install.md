# Introduction

This document contains a guide to installing Python, Git, and VsCode on your work computer. If you have any questions or problems contact Caroline Stone at cs831k@att.com.

This guide assumes you already have administrator priveleges on your computer. Follow the guide linked in the TDP Teams page if you do not. 

# Git

Git is a version control management language, it allows you track changes to files over multiple file location and users. 

## Installation

1. go to https://git-scm.com/ > Downloads > choose your operating system
2. follow the installer
    - default settings are fine unless you have knowledge/personal preferences to change something

If you are interested in jumping into learning git, I recomend this interactive tutorial https://learngitbranching.js.org/

## Configure Git

We need to change some configuration settings in git so that it works with the AT&T proxy.
Note that in GitBash, to copy use CTRL+SHIFT+C, to paste, right-click>Paste or SHIFT+INSERT

1. Open GitBash (this is a git specific command line interface (CLI) that allows you to use Git command line in a Windows)
2. Enter 'git config --global http.proxy http://sub.proxy.att.com:8080' (without quotations)
3. Enter 'git config --global https.proxy http://sub.proxy.att.com:8080'
4. Enter 'git config --global https.sslVerify "false"' (include quotations around false)
5. check your configuration with the command 'git config --list'. the http.proxy, https.proxy, and https.sslVerify values should match what you entered above.

## Set up GitHub account

AT&T git repos exist mostly on Azure, but this requires granting and managing access permissions in order to download specific project repos. For our purposes we will be using GitHub instead. Please create an account if you don't have one

1. go to https://github.com/
2. Click Sign-Up and create a new account

# VSCode 

VSCode is an open-source code editor with a lot of fun extensions.

## Instalation 

1. got to https://code.visualstudio.com/ > Download for Windows
2. use intaller with standard installation recomendations

# Python 

## Installation 

1. go to https://www.python.org/downloads/
2. Select Python 3.11.5 (or any version of 3)
3. download Windows installer (64-bit)
4. use installer, follow standard install settings. Be sure to select 'Add Python to PATH', this will ensure that python commands are recognized in whatever terminal you're using.
5. Check installation by entering 'python -V' in gitBash. It should return 'Python 3.11.5'
   - if this returns 'command not found', you need to set the Python Path variable on your system. Here's a guide: https://www.educative.io/answers/how-to-add-python-to-path-variable-in-windows


That's it! You will know be able to write and run python scripts. 