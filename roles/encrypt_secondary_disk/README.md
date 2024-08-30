# Encrypt secondary disk

This role installs cryptsetup package, then encrypt disk, partition of what is specified in inventory file. Then open it.
For example, /dev/sdb

## Possible upgrade

After encrypting, creating filesystem and mounting it.
