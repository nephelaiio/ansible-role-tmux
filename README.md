# nephelaiio.tmux

[![Build Status](https://github.com/nephelaiio/ansible-role-tmux/workflows/molecule/badge.svg)](https://github.com/nephelaiio/ansible-role-tmux/actions)
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-nephelaiio.tmux-blue.svg)](https://galaxy.ansible.com/nephelaiio/tmux/)

An [ansible role](https://galaxy.ansible.com/nephelaiio/tmux) to install and configure [tmux](https://tmux.github.io)

## Local install

Execute the following from the command line shell

```
curl -s https://raw.githubusercontent.com/nephelaiio/ansible-role-tmux/master/install.sh | bash
```

## Role Variables

Please refer to the [defaults file](/defaults/main.yml) for an up to date list of input parameters.

## Example Playbooks

With default configuration:

```
    - hosts: all
      roles:
         - role: tmux
```

With literal configuration

```
    - hosts: all
      vars:
        tmux_conf_literal: |
          // tmux config content
      roles:
         - role: tmux
```

## Testing

Please make sure your environment has [docker](https://www.docker.com) installed in order to run role validation tests. Additional python dependencies are listed in the [requirements file](https://github.com/nephelaiio/ansible-role-requirements/blob/master/requirements.txt)

This role is tested against the following distributions:

  * Ubuntu 22.04
  * Ubuntu 20.04
  * Ubuntu 18.04
  * Debian 11
  * Debian 10

You can test the role directly from sources using command ` molecule test `

## License

This project is licensed under the terms of the [MIT License](/LICENSE)
