# Encrypt secondary disk

This role installs cryptsetup package, then encrypt disk, partition of what is specified in inventory file. Then open it.
For example, /dev/sdb

## Possible upgrade

After encrypting, creating filesystem and mounting it.

## Running role

To run this role, you need to install `community.crypto` ansible galaxy collection and use `disk_to_encrypt` and `luks_passphrase` variables in your inventory.

After installation Use it in playbook like this:

    ```
    ---
    - name: Server preparation playbook
      hosts: all
      become: true

      roles:
        - encrypt_secondary_disk
    ```
