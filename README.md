
# Regenerate SSH Host Keys Systemd Unit

This repository contains a systemd unit file that automates the regeneration of SSH host keys. This can be particularly useful for initializing new instances, ensuring unique SSH keys for security purposes.

## Purpose

The purpose of this unit is to:
- **Regenerate SSH host keys**: This ensures that each machine has unique SSH host keys, which is critical for security and preventing man-in-the-middle (MITM) attacks.
- **Automate this process**: The unit will run once, regenerate the SSH host keys, and then disable itself to prevent future executions.

Once the file is copied to your system
  
Change permissions such that root owns this file
```bash 
sudo chown root:root regenerate_ssh_host_keys.service
```
Move the file 
```bash 
sudo mv regenerate_ssh_host_keys.service
```
