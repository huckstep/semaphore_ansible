# semaphore_ansible
Ansible Playbooks and Roles for Semaphore

This repository contains Ansible playbooks and roles used by Semaphore. Inventories are handled by Semaphore.

## Structure

```
.
├── ansible.cfg          # Ansible configuration
├── .gitignore           # Git ignore file
├── requirements.yml     # Collection dependencies
├── playbooks/           # Playbooks
└── roles/               # Ansible roles
    └── example_role/
        ├── defaults/    # Default variables
        ├── vars/        # Variables
        ├── tasks/       # Tasks
        ├── handlers/    # Handlers
        ├── templates/   # Templates
        ├── files/       # Static files
        └── meta/        # Role metadata
```

`host_vars` and `group_vars` live in the separate inventories repository.

## 1Password Connect Integration

Secrets are read with the `onepassword.connect` collection (see `playbooks/test-1password.yml`). Provide the connection via `OP_CONNECT_HOST` / `OP_CONNECT_TOKEN` environment variables, or the `runtime_secret_endpoint` / `runtime_secret_token` variables.

## License

MIT
