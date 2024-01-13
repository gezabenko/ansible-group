Group
=========

Manage groups

Requirements
------------

NA

Role Variables
--------------

Only one variable needed for use (name), but implemented all [module's](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/group_module.html#ansible-collections-ansible-builtin-group-module) parameters. Example:

```yaml
group:
  backup:
    force: 'true'
    gid: 999
    local: 'true'
    non_unique: 'true'
    state: 'absent'
    system: 'true'
```

Dependencies
------------

- ansible.builtin.group

Example Playbook
----------------

```yaml
    - hosts: servers
      roles:
         - { role: group, tags: [ group ] }
```

License
-------

BSD

