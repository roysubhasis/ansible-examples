## Explain : Below command along with project structure

```
ansible-playboook -i environments/dev application-deployment.yml -l executesql --extra-vars "env=dev, dbname=sampledb" --tags execute-query
```

### Project Structure
ansible/
├── application-deployment.yml
├── environments/
│   └── dev
│       └── hosts
├── group_vars/
│   └── all.yml
├── host_vars/
├── roles/
│   └── executesql/
│       ├── tasks/
│       │   └── main.yml
│       ├── files/
│       ├── templates/
│       └── vars/
│           └── main.yml
└── README.md


### Explanation:

- application-deployment.yml: Main playbook.
- environments/dev/hosts: Inventory file for the dev environment.
- group_vars/ and host_vars/: Variable files for groups/hosts.
- roles/executesql/: Role for executing SQL queries.
- roles/executesql/tasks/main.yml: Tasks for the executesql role.
- roles/executesql/vars/main.yml: Role-specific variables.