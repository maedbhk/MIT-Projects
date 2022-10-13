---
title: Getting Started on Openmind
---

## First Steps
* `ssh <username>@openmind.mit.edu`
    * `ssh <username>@openmind-dtn.mit.edu` ## to access data transfer node
* use `rsync` if you need to transfer data from your local network to openmind (and vice versa)
* code for `healthy_brain_network` is stored at `/om2/user/maedbh/healthy_brain_network` but you should clone the github repo in your own path `/om2/user/<username>`
    * follow instructions set out on this [webpage](https://jhooq.com/github-permission-denied-publickey/#1-github---how-to-fix-this-issue) to set up SSH for github repo
    * then run command `git clone git@github.com:maedbhk/healthy_brain_network.git` to clone the repo
    * to install the virtual environment, you need to make sure the python module is loaded (openmind uses anaconda for running Python)
    * run command `module load openmind/anaconda/3-2022.05` (if pipenv is not installed with anaconda, then run `pip install pipenv`)
    * then run `pipenv install` in top-level directory of `healthy_brain_network` (if you're getting an error, it's probably becuase you have not set your paths to /home/<username>/.local/bin. See ## Setting Paths below for more details)
    * to activate the virtual environment, run `pipenv shell`
* phenotypic data for `healthy_brain_network` is stored at `/nese/mit/group/sig/projects/hbn/phenotype`
    * fyi: I/O operations to `om` and `om2` are fast, which is why I store code here. `om4` and `nese` are slower but have large storage space, which is why data are stored on `nese`.

## Setting Paths
* Create `.bash_profile` in your home directory (`cd /home/<username>` and `touch .bash_profile` if file doesn't exist)
* For example, my `.bash_profile` is saved at `/home/maedbh` (see below)
* You can see that I have set aliases (for easier navigation around openmind), you don't have to do this but it can make things easier when you're working on openmind.
* Make sure you set your PATH so that your scripts can find software saved to your .local/bin directory.

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