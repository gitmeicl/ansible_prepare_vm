# Encrypt adjacent disk

This role defines partition next to root (for example: /dev/sda2), encrypts it and open it.

## Possible upgrade

After encrypting, creating filesystem and mounting it.

## Running role

To run this role, you need to install `community.crypto` ansible galaxy collection and use `luks_passphrase` variable in your inventory.

After installation Use it in playbook like this:

    ```
    ---
    - name: Server preparation playbook
      hosts: all
      become: true

      roles:
        - encrypt_adjacent_partition
    ```
