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

These variables are defined in [defaults/main.yml](./defaults/main.yml):

    nvidia_cuda_driver_version: 430

    nvidia_cuda_install_cuda: false

    nvidia_cuda_install_container_runtime: false

Dependencies
------------

None

Example Playbook
----------------

    - hosts: localhost
      roles:
        - role: nvidia-cuda
          vars:
            nvidia_cuda_install_cuda: true

License
-------

MIT

Author Information
------------------

Tibor Csóka
