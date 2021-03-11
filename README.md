osx-provisioning
================

Inspired by [Craig Marvelley](https://github.com/craigmarvelley/macbook-provisioning) & [Ben Davies](https://github.com/bendavies/osx-provisioning)

## Pre-requisites

* Homebrew `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
* Ansible `brew install ansible`
* Rosetta (if on M1 Silicon) `softwareupdate --install-rosetta`

Provision:

```ansible-playbook osx.yml```

Provisioning work computer?

`ansible-playbook osx.yml --extra-vars "email=ian@work.com" --ask-become-pass`

Want to update all brews?

`ansible-playbook osx.yml --extra-vars "homebrew_update=true" --ask-become-pass`
