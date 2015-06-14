Provision Your Mac with Ansible
===

Setup a new mac as dev machine is tedious. This repo is to make it easy and fast. 

Prerequisite
===

0. The current user needs to be Admin so that the playbook can run `sudo` 
1. Command Line Tools. To install, run `xcode-select --install`
2. [Homebrew](http://brew.sh). To install, run `ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
3. [Ansible](http://www.ansible.com). To install, run `brew install ansible` 
4. Install dependencies. `ansible-galaxy install -r requirements --force`

Usage
===

By default, this playbook will run for local machine. You can change that in `hosts`.
Run the playbook: `ansible-playbook provision_osx.yml -K`

The playbook will do the following:

1. Install and config vim using [ChengLong.vim](https://github.com/ChengLong/ansible-vim)
2. Install and config zsh using [ChengLong.zsh](https://github.com/ChengLong/ansible-zsh)
3. Install these Homebrew formulae
4. Install these Homebrew Cask packages 

Author
===
[Cheng Long](https://twitter.com/ChengLong_)

License
===
MIT
