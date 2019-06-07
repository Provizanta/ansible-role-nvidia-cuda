Nvidia + CUDA drivers
=========

[![Build Status](https://travis-ci.com/Teebor-Choka/Provisioning---Ansible-role-nvidia-cuda.svg?branch=master)](https://travis-ci.com/Teebor-Choka/Provisioning---Ansible-role-nvidia-cuda)

Install Nvidia drivers with optionally installing the latest CUDA drivers.

Highly inspired by:
- [CSCfi](https://github.com/CSCfi/ansible-role-cuda.git)

Requirements
------------

None

Role Variables
--------------

    driver:
      version: <int, nvidia driver version to be installed>
      cuda_compatible: <bool, use cuda compatible driver>
    install_cuda: <bool, establish cuda along with its drivers>

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
