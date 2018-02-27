# ansible-plays-antergos

This playbook will install prepare my development workspace on Antergos, independent of my given desktop environment.

These tasks use the pacman package manager `pacman`, as well as `pacaur` for the AUR repository. This repository includes the [ansible-pacaur](https://github.com/sanderboom/ansible-pacaur) ansible module by @[sanderboom](https://github.com/sanderboom) in the `./library` directory to simplify installation.

The playbook has been broken up into four individual role groups:

#### Common

* Install jshon for the pacaur package manager.
* Install pacaur package manager.
* Install synergy.
* Install redshift.
* Install deepin-screenshot.

#### Aesthetics

* Install Oranchelo icon theme.
* Copy wallpaper to local pictures directory.

#### Social

* Install Hipchat.
* Install Keybase.
* Install Teamviewer.
* Install Hamachi VPN.
* Install Gitter.
* Install Slack.

#### Development

* Create ssh key for git using `git_ssh_key_user` variable.
* Install npm.
* Install `n` nodejs manager.
* Install nodejs 8 lts.
* Install coffeescript (global).
* Install webpack 2.2.0 (global).
* Install angular-cli.
* Install vue-cli.
* Install pip.
* Installed httpie.
* Install pylint.
* Install twine (pypi package manager).
* Install sphinx (docs generator).
* Install virtualenv.
* Install docker.
* Install py-docker module.
* Install docker-compose.
* Install awscli.
* Install mongodb-compass.
* Install vscode (with extensions).
* Install fiddler web debugger.

## Variables

Playbook inventory variables can be found in `group_vars/all.yml`.

    git_ssh_key_user: Label of ssh key generated for git.

## Use

```sh
git clone https://github.com/neetjn/ansible-plays-antergos.git

cd ansible-plays-antergos

ansible-playbook playbook.yml
```

---
Copyright (c) 2017 John Nolette Licensed under the MIT license.
