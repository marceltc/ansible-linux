# CCDC Linux Hardening

This is an Ansible role that is specific to hardening Linux for CCDC and CCDC-style competitions. The main goal here is to create a secure base configuration for Linux without breaking anything or messing up any pre-existing service configurations. 

The tasks it performs are the following:
- Install `sudo`
- Create new admin user
- Harden crontab permissions
- Remove SUID/SGID bit from LOLbins
- Import `auditd` ruleset and set up the Linux Audit Daemon
- Use SHA256 hashes in shadow file
- Log privilege escalation events and user logins
- Common SSHD hardening

View the `defaults` directory to customize the role's behaviors.
