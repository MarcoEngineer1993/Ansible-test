# My Ansible Project

This project is designed to automate tasks using Ansible. It includes a main playbook, roles, and an inventory file to manage the configuration of target hosts.

## Project Structure

```
my-ansible-project
├── playbooks
│   └── main.yml          # Main playbook that defines tasks and roles
├── roles
│   ├── common
│   │   ├── tasks
│   │   │   └── main.yml  # Tasks for the common role
│   │   ├── templates
│   │   │   └── example.j2 # Jinja2 template for configuration files
│   │   └── vars
│   │       └── main.yml  # Variables for the common role
├── inventory
│   └── hosts.ini         # Inventory file for target hosts
└── README.md             # Project documentation
```

## Getting Started

To get started with this project, follow these steps:

1. **Install Ansible**: Ensure that Ansible is installed on your machine. You can install it using pip:

   ```
   pip install ansible
   ```

2. **Configure Inventory**: Update the `inventory/hosts.ini` file with the IP addresses or hostnames of the target machines you want to manage.

3. **Run the Playbook**: Execute the main playbook using the following command:

   ```
   ansible-playbook -i inventory/hosts.ini playbooks/main.yml
   ```

## Roles

This project includes a `common` role that contains tasks, templates, and variables. You can customize the tasks in `roles/common/tasks/main.yml` and define any necessary variables in `roles/common/vars/main.yml`.

## Templates

The `roles/common/templates/example.j2` file is a Jinja2 template that can be used to generate configuration files dynamically based on the variables defined in the role.

## Contributing

Feel free to contribute to this project by submitting issues or pull requests. Your contributions are welcome!