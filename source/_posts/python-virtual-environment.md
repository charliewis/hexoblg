---
title: python virtual environment
date: 2021-08-11 13:51:48
tags:
---

## Install pyenv
``` bash
sudo apt install linuxbrew-wrapper

brew install  pyenv
brew install  pyenv-virtualenv
```
---

## e.g. Create project with python version 3.8 venv
### Install version3.8 python
``` bash
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt update
sudo apt install python3.8
```

### Create project and venv
``` bash
mkdir proj_test_pyenv
cd proj_test_pyenv
/usr/bin/python3.8 -m venv .venv3.8
. .venv3.8/bin/activate
(.venv3.8) charlie@CHAB350M:~/proj_test_pyenv$ python -V
Python 3.8.6
```

## cf. python2
```
virtualenv -p /usr/bin/python2.7 .venv2.7
```
