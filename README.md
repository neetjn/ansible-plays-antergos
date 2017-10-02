# ansible-plays-antergos

This playbook will install prepare my development workspace on Antergos, independent of my given desktop environment.

These tasks use the pacman package manager `pacman`, as well as `pacaur` for the AUR repository. This repository includes the [ansible-pacaur](https://github.com/sanderboom/ansible-pacaur) ansible module by @[sanderboom](https://github.com/sanderboom) in the `./library` directory to simplify installation.

The playbook has been broken up into four individual role groups:

---
Copyright (c) 2017 John Nolette Licensed under the MIT license.