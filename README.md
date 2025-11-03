Ansible Assignments Project

This repository contains the assignments for the Ansible course, separated into two parts.

Part 1: User Management (Vault)

This part of the project manages user creation and uses Ansible Vault to protect sensitive information.

Execution

To run Part 1, first change into the directory:

cd parte1


Then, run the users.yml playbook. This playbook uses a vault, so it will ask for a password:

ansible-playbook users.yml --vault-password-file vault-pass


The playbook should run without any issues, creating the specified users.





Part 2: Web Server Deployment (Roles)

This part of the project deploys a complete Apache web server (httpd), including vhost configuration, firewall. It uses a roles structure for better organization.

The main site.yml playbook orchestrates everything, importing the deployment playbook (dev_deploy.yml) and the test playbook (get_web_content.yml).

Execution

To run Part 2, first change into the directory:

cd parte2

To launch the full deployment and tests, simply run the main site.yml playbook:

ansible-playbook site.yml


To launch the full deployment and tests, simply run the main site.yml playbook:

ansible-playbook site.
