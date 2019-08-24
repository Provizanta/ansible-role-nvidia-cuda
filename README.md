Ansible role: Nvidia + CUDA drivers
=========

[![Build Status](https://travis-ci.com/Provizanta/ansible-role-nvidia-cuda.svg?branch=master)](https://travis-ci.com/Provizanta/ansible-role-nvidia-cuda)

Install Nvidia drivers with optionally installing the latest CUDA drivers.

Highly inspired by:
- [CSCfi](https://github.com/CSCfi/ansible-role-cuda.git)

Requirements
------------

None

Role Variables
--------------

These variables are defined in defaults/main.yml:

    driver:
      version: 418
      cuda_compatible: true

    install_cuda: false

    install_container_runtime: false

Dependencies
------------

None

Example Playbook
----------------

    - hosts: localhost
      roles:
        - role: nvidia-cuda
          vars:
            install_cuda: true

License
-------

MIT

Author Information
------------------

Tibor Csoka
