# Rename network interface

This role finds active network interface and renames it to net0

## Running role

To run this role, you don't need additional installation or variables. Use it in playbook like this:

    ```
    ---
    - name: Server preparation playbook
      hosts: all
      become: true

      roles:
        - rename_network_interface
    ```
