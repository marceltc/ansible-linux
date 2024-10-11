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
- `cloudflare-nginx`: Deployment of an Nginx web server configured for [Cloudflare Authenticated Origin Pulls](https://developers.cloudflare.com/ssl/origin-configuration/authenticated-origin-pull/)
    - Installation of latest nginx
    - Copy public/private keys, Cloudflare cert
    - Deployment of Nginx site configuration
- `simple-pki`: Deployment of a PKI with a root and intermediate signing CA
    - Creation of root and intermediate CAs
    - Deployment of server certificates to an Ansible inventory group
    - Private keys never leave their respective servers