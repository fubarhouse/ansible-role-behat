# Ansible Role: Behat

[![Build Status](https://travis-ci.org/fubarhouse/fubarhouse.behat.svg?branch=master)](https://travis-ci.org/fubarhouse/fubarhouse.behat)
[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/fubarhouse/fubarhouse.behat/master/LICENSE)

Installs Behat on Debian/Ubuntu servers.

## Requirements

* PHP
* Composer

## Role Variables

```
behat_version: "3.*@stable"
behat_package: "behat/behat"
behat_dir: "/opt/behat"
behat_exec: "/opt/behat/vendor/bin/behat"
behat_sym: "/usr/local/bin/behat"
behat_extensions:
  - name: "Mink"
    package: "behat/mink"
    version: "@stable"
  - name: "Mink Extension"
    package: "behat/mink-extension"
    version: "@stable"
```

Note: All version numbers use composer syntax.

## Dependencies

  none

## Example Playbook

```
  - { role: fubarhouse.behat }
```

## Installation

  * Add Behat role to playbook, as per the playbook example above.

## License

MIT / BSD

## Author Information

This role was created for Behat directly in 2015 but rewritten in 2016 by [Karl Hepworth](https://twitter.com/fubarhouse).
