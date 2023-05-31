## Setup QIB VMs for running Nextflow pipelines via Tower.nf

Ansible script to install dependencies on QIB Cloud VMs for using with tower.nf 

## Requirements

ansible >= `2.10.17`

Prepare a hosts file with the VM information including: IP, username, location to your private ssh key

```toml
[servers]
my-vm ansible_host=192.168.10.122 ansible_user=ubuntu
```

## Usage

```
ansible-playbook setup.yml
```