# Ansible Role: requirements

An Ansible Role that installs some requirements to use Ansible:

- python packages
- `ansible` user

[![Actions Status](https://github.com/tristan-weil/ansible-role-requirements/workflows/molecule/badge.svg?branch=master)](https://github.com/tristan-weil/ansible-role-requirements/actions)

## Role Variables

Available variables are listed below, (see also `defaults/main.yml`).

Mandatory variables:

| Variable      | Description |
| :------------ | :---------- |

Optional variables:

| Variable      | Default | Description |
| :------------ | :------ | :---------- |
| requirements_ansible_ssh_authorized_keys | [] | a list of SSH public keys allowed to connect as `ansible` |
| requirements_packages | [] | a dictionary of packages to install (the key is the distribution) |
| requirements_ansible_home | /home/ansible | the home directory of the ansible user |

## Example Playbook

    - hosts: 'webservers'
      roles:
        - role: 'ansible-role-requirements'
        
## Todo

None.

## Dependencies

See [requirements_galaxy.yml](https://github.com/tristan-weil/ansible-role-requirements/blob/master/requirements_galaxy.yml)

## Supported platforms

See [meta/main.yml](https://github.com/tristan-weil/ansible-role-requirements/blob/master/meta/main.yml)

## License

See [LICENSE.md](LICENSE.md)
