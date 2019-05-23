Role Name
=========

Execute sequelize seeders

Requirements
------------

Role Variables
--------------

userdba: OS User responsible for seeding, must have the proper permissions in the target database
appdir: Your application directory, in there sequelize-cli expects to find directories created by sequelize-cli init.

Dependencies
------------

Example Playbook
----------------

    - hosts: servers
      roles:
        - {
            role: oscbco.sequelize_migrate,
            userdba: "{{ global_userdba }}",
            appdir: "{{ global_appdir }}"
          }

License
-------

MIT

Author Information
------------------

oscbco.me
