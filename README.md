# Project description
Coding practice for Ansible

## Installation 
[Ansible Installation on Ubuntu](https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html)

### Prerequisite
- Ubuntu 20+

### _Run ansible playbook without tags_
```
ansible-playbook <yaml file name>
```

### _Run ansible playbook with tags_
```
ansible-playbook sample_tasks.yaml --tags print-msg;
ansible-playbook sample_tasks.yaml --tags copy-files;
```
