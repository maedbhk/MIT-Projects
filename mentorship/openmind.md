---
title: Getting Started on Openmind
---

## First Steps
* `ssh <username>@openmind.mit.edu`
    * `ssh <username>@openmind-dtn.mit.edu` ## to access data transfer node
* use `rsync` if you need to transfer data from your local network to openmind (and vice versa)
* code for **healthy_brain_network** is stored at **/om2/user/maedbh/healthy_brain_network** but you should clone the github repo in your own path **om2/user/"username"**
    * follow instructions set out on this [webpage](https://jhooq.com/github-permission-denied-publickey/#1-github---how-to-fix-this-issue) to set up SSH for github repo
    * then run command `git clone git@github.com:maedbhk/healthy_brain_network.git` to clone the repo
    * to install the virtual environment, you need to make sure the python module is loaded (openmind uses anaconda for running Python)
    * run command `module load openmind/anaconda/3-2022.05` (if pipenv is not installed with anaconda, then run `pip install pipenv`)
    * then run `pipenv install` in top-level directory of **healthy_brain_network** (if you're getting an error, it's probably becuase you have not set PATH to be **/home/"username"/.local/bin** in your **.bash_profile**. See **Setting Paths** below for more details)
    * to activate the virtual environment, run `pipenv shell`
* phenotypic data for **healthy_brain_network** is stored at **/om2/user/maedbh/hbn_data/**
    * fyi: I/O operations to **om** and **om2** are fast, which is why I store code here. **om4** and **nese** are slower but have large storage space, which is why raw data are stored on **nese**.

## Setting Paths
* Create **.bash_profile** in your home directory (`cd /home/<username>` and `touch .bash_profile` if file doesn't exist)
* For example, my **.bash_profile** is saved at **/home/maedbh** (see below)
* You can see that I have set aliases (for easier navigation around openmind), you don't have to do this but it can make things easier when you're working on openmind.
* Make sure you set your PATH so that your scripts can find software saved to your .local/bin directory.

To activate ``source .bash_profile``

```
# .bash_profile

# Get the aliases and functions
if [ -f ~/.bashrc ]; then
        . ~/.bashrc
fi

# User specific environment and startup programs
LANG=en_US.UTF-8
PATH=$PATH:$HOME/bin:$HOME/.local/bin:/home/maedbh/.local/bin/

alias cdcode="cd /om2/user/maedbh/healthy_brain_network"
alias cddata="cd /nese/mit/group/sig/projects/hbn/phenotype"
alias cdhome="cd /home/maedbh"
alias cdenv="cd /home/maedbh/.local/share/virtualenvs"
alias diskspace="du -hs $PWD/.[!.]* $PWD/* | sort -h"
alias l="ls -alh"

module load openmind/anaconda/3-2022.05
if command -v pyenv 1>/dev/null 2>&1; then
  eval "$(pyenv init -)"
fi
```

## Using VS Code on OpenMind
* Open VS Code and add the extensions on the sidebar: **Remote - SSH** and **Remote - SSH: Editing Configuration Files**
* Go to **View** and open **Command Palette** 
    * Click **Remote-SSH: Add New SSH Host**
    * You'll be prompted to log in to OpenMind `ssh "username"@openmind.mit.edu`
    * You'll get a notification saying host added and an option to **connect** 
* Once you connect for the first time you'll be able to connect easily via **Remote Explorer** on the sidebar. You'll be prompted for your password every time you ssh in. 