# #ROLE_NAME#

Master: [![Build Status](https://travis-ci.org/sansible/#ROLE_NAME#.svg?branch=master)](https://travis-ci.org/sansible/#ROLE_NAME#)  
Develop: [![Build Status](https://travis-ci.org/sansible/#ROLE_NAME#.svg?branch=develop)](https://travis-ci.org/sansible/#ROLE_NAME#)

* [ansible.cfg](#ansible-cfg)
* [Installation and Dependencies](#installation-and-dependencies)
* [Tags](#tags)
* [Examples](#examples)

This roles ...




## ansible.cfg

This role is designed to work with merge "hash_behaviour". Make sure your
ansible.cfg contains these settings

```INI
[defaults]
hash_behaviour = merge
```




## Installation and Dependencies

To install run `ansible-galaxy install sansible.#ROLE_NAME#` or add this to your
`roles.yml`.

```YAML
- name: sansible.#ROLE_NAME#
  version: v1.0
```

and run `ansible-galaxy install -p ./roles -r roles.yml`




## Tags

This role uses tags: **build** and **configure**

* `build` - Installs ...
* `configure` - Configures ...




## Examples

Simply include role in your playbook

```YAML
- name: Install and configure #ROLE_NAME#
  hosts: "somehost"

  roles:
    - role: sansible.#ROLE_NAME#
```
