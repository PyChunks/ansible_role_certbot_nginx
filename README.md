Role Name
=========

Creates a SSL certificate for a given domain via certbot

Requirements
------------

None.

Role Variables
--------------

Variables that need to be set:
```yaml
domain: 
validate_email: 
```

Where: 
`domain` is the domain you wish to create a certificate for.

`validate_email` is the email you wish to register the certificate with. 

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: servers
  vars:
    domain: example.com 
    validate_email: yourEmail@example.com 
  roles:
     - ansible_role_certbot_nginx
```

License
-------

BSD

Author Information
------------------

Created by Vincent D-Gauthier
