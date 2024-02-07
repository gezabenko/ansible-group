Ansible - Group
=========

Manage groups with Ansible.

Requirements
------------

NA

Role Variables
--------------

Only one variable needed for use (name), but implemented all [module's](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/group_module.html#ansible-collections-ansible-builtin-group-module) parameters. Example:

```yaml
group:
  - name: backup
    gid: 999
    local: 'true'
    non_unique: 'true'
    state: 'absent'
    system: 'true'
```

Dependencies
------------

- [ansible.builtin.group](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/group_module.html#ansible-collections-ansible-builtin-group-module)

Example Playbook
----------------

```yaml
    - hosts: servers
      roles:
         - { role: group, tags: [ group ] }
```

License
-------

GPLv3

