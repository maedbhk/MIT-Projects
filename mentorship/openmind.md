---
title: Getting Started on Openmind
---

> Example repo here is **healthy_brain_network** but can be applied to any github repo that uses a Pipfile or Conda environment

## First Steps
* `ssh <username>@openmind.mit.edu` ## to log in to OpenMind        
    * `ssh <username>@openmind-dtn.mit.edu` ## to access data transfer node
    * fyi: use `rsync` if you need to transfer data from your local network to openmind (and vice versa)
* code for **healthy_brain_network** is stored at **/om2/user/maedbh/healthy_brain_network** but you should clone the github repo in your own path 
```
    cd om2/user/"username"
    git clone git@github.com:maedbhk/healthy_brain_network.git
```
* Follow instructions set out on this [webpage](https://jhooq.com/github-permission-denied-publickey/#1-github---how-to-fix-this-issue) to set up SSH for github repo
* Also useful is this step-by-step [guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key) on setting up ssh keys
* phenotypic data for **healthy_brain_network** is stored at **/om2/user/maedbh/hbn_data/**
    * fyi: I/O operations to **om** and **om2** are fast, which is why I store code here. **om4** and **nese** are slower but have large storage space, which is why raw data are stored on **nese**.

## Installing and activating virtual environments
* To install the virtual environment, you need to make sure the Python module is loaded (OpenMind uses anaconda for running Python)
```
    module load openmind/anaconda/3-2022.05`
```
* You can use either **pipenv** or **conda** to activate the virtual environment for the project

> If you want to use **pipenv**
```
    # navigate to top-level directory of project
    cd om2/user/"username"/healthy_brain_network

    # make sure **pipenv** library is installed
    pip install pipenv

    # install virtual environment
    pipenv install ## if you're getting an error, it's probably because you have not set PATH to be **/home/"username"/.local/bin** in your **.bash_profile**. See **Setting Paths** below for more details)

    # activate the virtual environment
    pipenv shell
```

> If you want to use **conda**
```
    # navigate to top-level directory of project (example here is **healthy_brain_network** but can be any folder that contains an **environment.yml** file)
    $ cd om2/user/"username"/healthy_brain_network

    # load your own version of miniconda
    # see section below: `Download miniconda on OpenMind`

    # in this repo, install a conda environment from environment.yml
    $ conda env create -f environment.yml

    # activate the conda virtual environment
    $ conda activate healthy-brain-network # each **environment.yml** has its own unique name (look inside the file `$ vim environment.yml`)
```

## Download miniconda on OpenMind and add to PATH
```

    # create bin folder in your om2 directory - this is where you will store your distribution of miniconda
    $ cd /om2/user/"username"
    $ mkdir bin
    $ cd bin

    wget https://repo.anaconda.com/miniconda/Miniconda3-py310_22.11.1-1-Linux-x86_64.sh
    $ bash Miniconda3-latest-Linux-x86_64.sh

    # save the distrubtion (when prompted) to **/om2/user/"username"/bin/miniconda**

    # to permanently enable the conda command from your distribution of miniconda:
    $ echo ". /om2/user/"username"/miniconda3/etc/profile.d/conda.sh" >> ~/.bash_profile

    # to put conda's bse (root) environment on PATH:
    $ echo "conda activate" >> ~/.bash_profile

```

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
alias cddata="cd /om2/user/maedbh"/hbn_data/"
alias cdhome="cd /home/maedbh""
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