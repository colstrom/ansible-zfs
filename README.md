Description
===========

The native ZFS filesystem for Linux.

Ubuntu 16.04 includes ZFS support out of the box. This role adds ZFS to the other LTS releases still within support. The goal is not to promote continued use of older releases, but to make it easier to migrate by minimizing the differences between the old and new.

Tunables
========

-   None

Dependencies
============

-   colstrom.apt-repository

Example Playbook
================

``` yaml
  - hosts: servers
    roles:
      - role: colstrom.zfs
```

License
=======

This role is distributed under the terms of the [MIT License](https://tldrlegal.com/license/mit-license), see LICENSE.txt for the full text. Software installed by this role may have its own terms.

Contributors
============

-   [Chris Olstrom](https://colstrom.github.io/) | [e-mail](mailto:chris@olstrom.com) | [Twitter](https://twitter.com/ChrisOlstrom)

