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

### _Run ansible with extra params_
```
ansible-playbook sample_tasks.yaml --extra-vars "file_patterns=create_db.sql,alter_table.sql,payload.json" --tags copy-all-files
ansible-playbook test.yaml --extra-vars "file_patterns=create_db.sql,alter_table.sql,payload.json,select.sql cr_number=CR12345" --tags copy-only-crnumber-file
```