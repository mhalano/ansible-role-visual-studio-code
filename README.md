visual-studio-code
==================

This role download and install Microsoft Visual Studio Code in the latest available version. I wrote this role to be compatible with all systems based on DEB and RPM, but I just tested on Ubuntu. Please, report bugs.

Requirements
------------

No special requirements except Ansible 2.1. Need to be this version because the packages are downloaded by the apt module itself and this feature begun to be available on this release.

Role Variables
--------------

No variables for now. May be in the future.

Dependencies
------------

No dependencies.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
      roles:
         - visual-studio-code


License
-------

MIT

Author Information
------------------

My name is Marcos H. Alano. This is my first role published on Ansible Galaxy. I wrote a lots of roles and I will porting one by one. Is all roles related to desktop applications (may be a few server applications in the future) because my plan is automatize the post-installation of my computer.

To Do
-----

* Support macOS
* Do tests on RPM-based distributions
* Do tests on Debian distribution
* Support GenericLinux (use the .zip instead of a package)

Known Bugs
----------
* Sometimes the playbook fails because it has problems downloading the package. That's a Microsoft problem related with the shorten links.