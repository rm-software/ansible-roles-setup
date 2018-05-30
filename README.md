Role Name
=========

Standard setup for fresh-built Ubuntu servers

Requirements
------------

None

Role Variables
--------------

Reboot server after setup tasks complete:

    setup_reboot: no

Server timezone and locale

    setup_timezone: America/Los_Angeles
    setup_locale: en_US.UTF-8

Dependencies
------------


Example Playbook
----------------

    - hosts: servers
      - import_role:
          name: setup
        vars:
          setup_reboot: yes
