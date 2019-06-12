Role Name
=========

This role will install httpd (apache) web server using yum module (rpm file will not be pushed from central location but installed using yum command).
Also, this role can push httpd config file(s).

Requirements
------------

No pre-requisites needed.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use this role:

    - hosts: servers
      roles:
         - /ansible/deploy_httpd_app/

License
-------

GPL

Author Information
------------------

Vlad U
