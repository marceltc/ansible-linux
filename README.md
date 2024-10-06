# Linux Ansible Collection

>My personal Ansible playbooks and useful Ansible roles

**Note:**
Tested compatibility with Debian-based systems using `apt` and RPM-based systems using `dnf`, since that's mostly what I'm running. 

## Roles
- `common`: Configuration of initial Linux installs.
    - Installation of some basic packages
    - Creation of a new user with sudo privileges
    - Transfer of dotfiles and SSH public keys
    - Security hardening (SSH key auth, disable SSH root login, configuring automatic updates)
