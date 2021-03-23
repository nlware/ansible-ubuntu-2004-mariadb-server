## ubuntu-2004-mariadb-server

Ansible role to set up a MariaDB server on Ubuntu 20.04.

#### Variables

* `ubuntu_2004_mariadb_server_root_password`: [required]: Root password

* `ubuntu_2004_mariadb_server_certificates_present`: [default: `{}`]: SSL certificates to create
* `ubuntu_2004_mariadb_server_certificates_absent`: [default: `[]`]: SSL certificates to remove

* `ubuntu_2004_mariadb_server_configuration_files_present`: [default: `{}`]: Configuration files to create
* `ubuntu_2004_mariadb_server_configuration_files_absent`: [default: `[]`]: Configuration files to remove

#### Examples

##### Minimal (set root password only)

```yaml
---
- hosts: all
  roles:
    - ubuntu-2004-mariadb-server
  vars:
    ubuntu_2004_mariadb_server_root_password: 'this-is-a-test-password'
```
