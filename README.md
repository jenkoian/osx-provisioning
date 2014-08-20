osx-provisioning
================

Inspired by [Craig Marvelley](https://github.com/craigmarvelley/macbook-provisioning) & [Ben Davies](https://github.com/bendavies/osx-provisioning)

Provision:

```ansible-playbook osx.yml```

Provisioning work computer?

```ansible-playbook osx.yml --extra-vars "email=ian@work.com"```

Want to update all brews?

```ansible-playbook osx.yml --extra-vars "homebrew_update=true"```
