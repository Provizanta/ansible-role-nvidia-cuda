Ansible role: Nvidia + CUDA drivers
=========

![Build & Deploy](https://github.com/Provizanta/ansible-role-nvidia-cuda/workflows/molecule/badge.svg?branch=master)

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
