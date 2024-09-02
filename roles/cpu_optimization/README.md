# Display CPU info

This role optimizes CPU for high-performance mode and disable C-state for all cores.

## Running role

To run this role, you don't need additional installation or variables. Use it in playbook like this:

    ```
    ---
    - name: Server preparation playbook
      hosts: all
      become: true

      roles:
        - cpu_optimization
    ```

## Note

It is impossible to run "Switch CPU governor to performance mode" in virtual machine, because it does not have acces to hardware and does not have needed directories. Task is working only on bare metal.
