# ansible-proxmox
Ansible Proxmox Ceph using lae.proxmox Ansible Galaxy role, this playbook has been tested with Debian Buster 10
Uses Zero Tier one for Ceph node communication.

## Install Ansible galaxy roles ##

ansible-galaxy install lae.proxmox geerlingguy.ntp
ansible-galaxy install m4rcu5nl.zerotier-one

## Edit Ansible inventory
Add the SSH hosts to the inventory file ./inventory ansible_host=1.2.3.4

## Run the playbook
ansible-playbook -i inventory -u root install_proxmox.yml

