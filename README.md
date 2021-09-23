Ansible Role: Deadline
=========

Install Thinkbox Deadline Server on RHEL/CentOs/RockyLinux 8 servers.

Requirements
------------

No special requirements; note that this role requires root access, so either run it in a playbook with a global `become: yes`, or invoke the role in your playbook like:

    - hosts: database
      roles:
        - role: dg.deadline
          become: yes


Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: deadline
      become: yes
      vars_files:
        - vars/main.yml
      roles:
        - dg.deadline

License
-------

MIT/BSD

Author Information
------------------

This role was created in 2021 by Jonathan Hansen
