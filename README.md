ansible-role-motd
=================

An ansible role for configuring Message Of The Day (motd) file.

Requirements
------------

Tested on:

-	Ubuntu 20.04 LTS

Should work with:

-	All Ubuntu
-	All Debian
-	All RHEL
-	All Centos

Role Variables
--------------

```yaml
# Name of motd file placed in /etc/update-mot.d. The leading digits determine
position in the motd
motd_file: 99-motd
# Plaintext content to be added to motd
motd_content:
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
    - hosts: servers
      roles:
         - { role: andbanman.motd }
```

License
-------

GPLv3 License.

Author Information
------------------

Andrew Banman

Inspiration
-----------

[adriagalin/ansible.motd] (https://github.com/adriagalin/ansible.motd)
