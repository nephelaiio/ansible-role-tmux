nephelaiio.tmux
=========

[![Build Status](https://travis-ci.org/nephelaiio/ansible-role-tmux.svg?branch=master)](https://travis-ci.org/nephelaiio/ansible-role-tmux)

An [ansible role](https://galaxy.ansible.com/nephelaiio/tmux) to install and configure tmux

Requirements
------------

Please make sure your environment has [docker](https://www.docker.com) installed in order to run role validation tests. Additional python dependencies are listed in the [requirements file](/requirements.txt)

Role Variables
--------------

Please refer to the [defaults file](/defaults/main.yml) for an up to date list of input parameters.

Dependencies
------------

This role depends on git being installed; currently this is achieved through dependency [nephelaiio.git](https://galaxy.ansible.com/nephelaiio/git/). Refer to the [depenencies file](/dependencies.yml) for up-to-date information

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: tmux tmux_packages: tmux }


Testing
-------

Role is tested against the following distributions (docker images):
  * Ubuntu Xenial
  * CentOS 7
  * Debian Jessie
  * Arch Linux

You can test the role from sources using the command line using molecule directly
```
molecule test
```
Please review the [documentation](http://docs.ansible.com/ansible/galaxy.html#setup-travis-integrations) in order to add continuous integration for the role using [Travis CI](https://travis-ci.org). Role configuration is provided in the [Travis-CI configuration file](/travis.yml)

License
-------

This project is licensed under the terms of the [MIT License](/LICENSE)
