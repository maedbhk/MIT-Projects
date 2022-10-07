---
title: Notes on Openmind
---

## Cloning a github repo onto openmind
* follow instructions set out on this [webpage](https://jhooq.com/github-permission-denied-publickey/#1-github---how-to-fix-this-issue) to set up SSH for github repo
* then run command `git clone git@github.com:maedbhk/healthy_brain_network.git`

## Navigating openmind
* `ssh <username>@openmind.mit.edu`
* `ssh <username>@openmind-dtn.mit.edu` ## to access data transfer node
* code for `healthy_brain_network` is stored at `/om2/user/maedbh/healthy_brain_network` but you can clone the github repo in your own path `/om2/user/<username>`
* phenotypic data for `healthy_brain_network` is stored at `/nese/mit/group/sig/projects/hbn/phenotype`

## Setting Paths
Set path in `.bash_profile` in your home directory.
For example, my `.bash_profile` is saved at `/home/maedbh` (see below). 

To activate ```source .bash_profile```

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