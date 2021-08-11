---
title: python virtual environment
date: 2021-08-11 13:51:48
tags:
---

sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt update
sudo apt install python3.8

mkdir test_pyenv
cd test_pyenv

/usr/bin/python3.8 -m venv .venv3.8
. .venv3.8/bin/activate

(.venv3.8) charlie@CHAB350M:~/test_pyenv$ python -V
Python 3.8.6
