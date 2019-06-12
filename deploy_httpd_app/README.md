Role Name
=========

This role will install httpd (apache) web server using yum module (rpm file will not be pushed from central location but installed using yum command).
Also, this role can push httpd config file(s).

Requirements
------------

No pre-requisites needed.

Role Variables
--------------

This role has 2 optional variables:
- rpm_version
- roolback

"rollback" variable is added to support rpm downgrade (rollback). If variable is not passed, default is no which means downgrade is not allowed.

"rpm_version" variable is added to support installation of specific httpd version. If variable is not passed, then latest available httpd version will be installed. If we want to install specific httpd version we should pass, for example:
rpm_version=-2.4.6-88.el7.centos.x86_64

Both variables can be passed when ansible playbook is started, for example:              
--extra-vars "rpm_version=-2.4.6-88.el7.centos.x86_64" --extra-vars "roolback=yes"

Dependencies
------------

No dependencies.

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
