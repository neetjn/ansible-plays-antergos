# ansible-plays-antergos

This playbook will install prepare my development workspace on Antergos, independent of my given desktop environment.

These tasks use the pacman package manager `pacman`, as well as `pacaur` for the AUR repository. This repository includes the [ansible-pacaur](https://github.com/sanderboom/ansible-pacaur) ansible module by @[sanderboom](https://github.com/sanderboom) in the `./library` directory to simplify installation.

The playbook has been broken up into four individual role groups:

### Common

* Install jshon for the pacaur package manager.
* Install pacaur package manager.
* Install synerg.
* Install redshift.
* Install mono (.NET).

### Aesthetics

* Install Oranchelo icon theme.
* Copy wallpaper to local pictures directory.

### Social

* Install Hipchat.
* Install Keybase.
* Install Teamviewer.
* Install Hamachi VPN.

### Development

* Create ssh key for git using `git_ssh_key_user` variable.
* Install npm.
* Install `n` nodejs manager.
* Install nodejs 6.11.3.
* Install coffeescript (global).
* Install webpack 2.2.0 (global).
* Install pip.
* Installed httpie.
* Install pylint.
* Install virtualenv.
* Install docker.
* Install py-docker module.
* Install docker-compose.
* Install awscli.
* Install vscode (with extensions).
* Install fiddler web debugger.

## Prerequisites

* git
* ansible 2+

## Use

```sh
git clone https://github.com/neetVeritas/ansible-plays-antergos.git

cd ansible-plays-antergos

ansible-playbook playbook.yml -i localhost
```

---
Copyright (c) 2017 John Nolette Licensed under the MIT license.