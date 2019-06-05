Nvidia + CUDA drivers
=========

[![Build Status](https://travis-ci.com/Teebor-Choka/Provisioning---Ansible-role-nvidia-cuda.svg?branch=master)](https://travis-ci.com/Teebor-Choka/Provisioning---Ansible-role-nvidia-cuda)

Install Nvidia drivers with optionally installing the latest CUDA drivers.

Highly inspired by:
- [CSCfi](https://github.com/CSCfi/ansible-role-cuda.git)
- [slothai](https://github.com/slothai/ansible-cuda.git)

Requirements
------------

None

Role Variables
--------------

    version: <int, nvidia driver version to be installed>
    cuda_compatible: <bool, use a cuda comptabile driver>

Dependencies
------------

None

Example Playbook
----------------

    - hosts: localhost
      roles:
        - role: nvidia-cuda
          vars:
            cuda_compatible: true

License
-------

MIT

Author Information
------------------

Tibor Csoka
