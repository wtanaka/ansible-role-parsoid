[![Build
Status](https://travis-ci.org/wtanaka/ansible-role-parsoid.svg?branch=master)](https://travis-ci.org/wtanaka/ansible-role-parsoid)
[![CircleCI](https://circleci.com/gh/wtanaka/ansible-role-parsoid.svg?style=svg)](https://circleci.com/gh/wtanaka/ansible-role-parsoid)

wtanaka.parsoid
===============

Ansible role to install Parsoid.  Parsoid is an application which can
translate back and forth, at runtime, between MediaWiki's wikitext
syntax and an equivalent HTML/RDFa document model with enhanced
support for automated processing and rich editing. It has been under
development by a team at the Wikimedia Foundation since 2012. It is
currently used extensively by VisualEditor, Flow, Content Translation
and other applications.

Example Playbook
----------------

Simple default install

    - hosts: all
      roles:
        - role: wtanaka.parsoid

You can configure the role in the playbook:

    - hosts: servers
      roles:
        - role: wtanaka.parsoid
          parsoid_conf:
            loadWMF: true

Or using variables in an appropriate `host_vars` or `group_vars` file.

The full set of configuration options available are visible in
[defaults/main.yml](defaults/main.yml)

### `parsoid_mw_apis`

Configures the `mwApis` configuration setting

Default:

```
parsoid_mw_apis:
- uri: 'http://localhost/w/api.php'
  domain: 'localhost'
```

License
-------

GPLv2

Author Information
------------------

https://wtanaka.com/
