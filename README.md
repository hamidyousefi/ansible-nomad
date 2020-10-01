# Hashicorp Nomad Anisble Role
Hashicorp is one of the most brilliant companies focused on infrastructure services. I like them and using their
products on my personal or enterprise projects, so having solid defined Ansible roles for installing
and setting up them would make everything easier.

This role is of course a role for personal uses, but you are free to add it into your
playbooks. I will promise to keep backward compatibility and add the necessary
customizable options to keep this repository fresh and usable.

## How to Use It
You can simply install this role on your machine by using the below command:
```bash
ansible-galaxy install hamidyousefi.nomad
```
Also if you defined your playbook, you can simply add below lines to your `roles/requirements.yml`.
You can create this file if your playbook doesn't have it yet.
```yaml
- name: hamidyousefi.nomad
  version: master
```
Of course `master` is the most updated version of this role. You should prefer to 
define which version you are going to use just by replacing it with something like `v1.0.2`.
You can find the versions list and their changelogs from [releases page](https://github.com/hamidyousefi/ansible-nomad/releases).

## Default Variables
```yaml
nomad_version: 0.12.5
nomad_servers:
  - ip: 127.0.0.1
    port: 4647
nomad_network_interface: ens3
nomad_ip_version: ipv4
```
