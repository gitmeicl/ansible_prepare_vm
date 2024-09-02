# ansible_prepare_vm

This is ansible project for preparation virtual machine or hardware on Linux.

## This project has this roles

- encrypt_secondary_disk
- encrypt_adjacent_partition
- cpu_optimization
- rename_network_interface
- display_cpu_info

All of them are needed to prepare vm for working in high-performance and low latency mode.

## Installation

<https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#pip-install>

ansible-galaxy collection install -r requirements.yml  --collections-path=./

## Run

To run you need to fill inventory, like inventory.example.yml, then run with command like this:

    ```bash
    ansible-playbook playbook.yml -i inventory.yml
    ```

## Note

On virtual machine ot is impossible to run `cpu_optimization` role. Read note on

- [cpu_optimization role](roles/cpu_optimization/README.md)
