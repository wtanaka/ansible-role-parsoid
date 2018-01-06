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

    - hosts: all
      roles:
        - role: wtanaka.parsoid


Author Information
------------------

https://wtanaka.com/
