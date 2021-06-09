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
- `intellij_package_checksum`: the checksum related to the intellij binary.
The value can be retrieved by appending `.sha256` to the package's url:
https://download.jetbrains.com/idea/ideaIC-2020.1.2.tar.gz.sha256

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

EUPL-1.2

Author Information
------------------

ECGALAXY team.
