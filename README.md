# Ansible Role: Behat

Installs Behat on Debian/Ubuntu servers.

## Requirements

Requires `curl` to be installed on the server.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
vagrant_user: "vagrant"
```

```
behat_dir: "~/.behat"
behat_location: "{{ behat_dir }}/bin/behat"
```

## Dependencies

  none

## Example Playbook

```
  - { role: fubarhouse.behat, when: '"behat" in installed_extras' }
```

## Installation

  * Add "behat" to the installed_extras variable in your config.yml file to use this role with the playbook example above.
  * Add behat to playbook, as per the playbook example above.

## License

MIT / BSD

## Author Information

This role was created in 2015 by [Karl Hepworth](https://twitter.com/fubarhouse).
