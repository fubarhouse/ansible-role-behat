# Ansible Role: Drupal Extension (Behat)

[![Build Status](https://travis-ci.org/fubarhouse/fubarhouse.drupal-extension.svg?branch=master)](https://travis-ci.org/fubarhouse/fubarhouse.drupal-extension)
[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/fubarhouse/fubarhouse.drupal-extension/master/LICENSE)

Installs Drupal Extension (Behat) on Debian/Ubuntu servers.

## Requirements

* PHP
* Composer

## Role Variables

In order to change the values below, rewrite the object using the example below:

```
fubarhouse_behat:
  extension_version: "~3.0"
  extension_dir: "/opt/drupalextension"
  extension_exec: "/opt/drupalextension/bin/behat"
  extension_sym: "/usr/local/bin/behat"
```

Note: The version number uses composer syntax.

## Dependencies

  none

## Example Playbook

```
  - { role: fubarhouse.drupal-extension }
```

## Installation

  * Add the Drupal Extension to playbook, as per the playbook example above.

## License

MIT / BSD

## Author Information

This role was created for Behat directly in 2015 but rewritten for Drupal Extension in 2016 by [Karl Hepworth](https://twitter.com/fubarhouse).
