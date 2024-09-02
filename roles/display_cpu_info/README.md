# Display CPU info

This role checks, how many CPU cores system has and checks for Intel Hyper-Threading or AMD multithreading. Then show all this debug information.

## Running role

To run this role, you don't need additional installation or variables. Use it in playbook like this:

    ```
    ---
    - name: Server preparation playbook
      hosts: all
      become: true

      roles:
        - display_cpu_info
    ```
