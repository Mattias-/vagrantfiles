#!/usr/bin/env bash

date > /tmp/time_provisioned
apt-get --yes --quiet update
apt-get --yes --quiet upgrade
apt-get --yes --quiet install curl git vim screen build-essential
apt-get --yes --quiet install python-dev python-pip ipython
pip install pep8 pylint virtualenv virtualenvwrapper
#apt-get --yes --quiet install haskell-platform hlint
su --command "git clone https://github.com/Mattias-/dotfilez.git" vagrant
su --command "python ./dotfilez/setup_dotfiles.py" vagrant
