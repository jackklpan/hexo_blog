---
title: Install python 3 in AWS linux by pyenv
tags: [python, aws]
date: 2017-03-19 22:51:00
---

## Install Pyenv and Python 3

curl -L https://raw.githubusercontent.com/pyenv/pyenv-installer/master/bin/pyenv-installer | bash

vim .bash_profile

add following lines to .bash_profile:
```
export PATH="/home/ec2-user/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
```

sudo yum install gcc

sudo yum install openssl-devel

sudo yum install bzip2-devel

sudo yum install sqlite-devel

sudo yum install readline-devel

pyenv install 3.4.3


## Install lxml lib

sudo yum install libxml2-dev libxslt-dev python34-dev
