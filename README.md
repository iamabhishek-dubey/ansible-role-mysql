# Ansible Role: MySQL
I am an ansible role for installing and configuring **[MySQL Server](https://www.mysql.com/)**.

## Requirments
No requirments for this role :-)

## Role Variables
### Mandatory Variables
**Here is the list of mandatory variables**

|**Variables**|**Default Value**|**Description**|
|-------------|-----------------|---------------|
|**mysql_root_password**|root|Password of root for MySQL|
|**mysql_user_name**|opstree|MySQL username|
|**mysql_user_password**|opstree|Password for MySQL username|
|**mysql_database_name**|opstree|Primary database for MySQL|

### Optional Variables
There is no optional variables.

## Dependencies
None :-)

## Example Playbook
Here is an example playbook:-
```yml
---
- hosts: exporter
  user: ubuntu
  become: yes
  roles:
    - iamabhishek-dubey.ansible-role-mysql
```

## Usage
This is an example of how to run this role

```shell
ansible-playbook -i hosts site.yml
```

## Author
**[Abhishek Dubey](https://github.com/iamabhishek-dubey)**