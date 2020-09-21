# User
Ansible role to configures a user on a Windows 10 machine.

## Requirements
None.

## Role Variables
Available variables are listed below, along with default values `(see defaults/main.yml)`:
```yaml
user_name: null
user_password: null
```
Required variables (role will fail if the variables are not set):
```yaml
user_name: null
user_password: null
```

## Dependencies
* [check-required-variables](https://github.com/artcom/ansible-role-check-required-variables)

# Example Playbook
```yaml
- name: configure user
  hosts: all
  roles:
    - role: win-user
      vars:
        user_name: "user"
        user_password: "sup3rseKret"
```

## License
MIT
