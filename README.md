ECGALAXY IntelliJ role
=======================

Installs IDEA IntelliJ (Community|Ultimate) - https://www.jetbrains.com/idea/

Requirements
------------

None.

Role Variables
--------------

- `intellij_version`: IntelliJ version to install
- `intellij_edition`: (community|ultimate)
- `intellij_package_checksum`: the checksum related to the IntelliJ archive.

The value can be retrieved by appending `.sha256` to the archive's URL:
https://download.jetbrains.com/idea/ideaIC-2021.3.2.tar.gz.sha256

Dependencies
------------

* ecgalaxy.common_packages

Example Playbook
----------------

    - hosts: all
      roles:
        - ecgalaxy.common_packages
        - ecgalaxy.intellij

License
-------

Copyright the European Union 2022.

Licensed under the EUPL-1.2 or later.

Author Information
------------------

ECGALAXY team.

NOTE: This role is based on [original work by John Freeman](https://github.com/gantsign/ansible-role-intellij).
