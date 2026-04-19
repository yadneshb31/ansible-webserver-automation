# Ansible Web Server Automation

## Overview
Automated provisioning of Nginx web servers on AWS EC2 using Ansible with role-based structure.

## Tech
- AWS EC2
- Ansible
- Nginx

## Structure
ansible-webserver-project/
- inventory/hosts.ini
- playbooks/webserver.yml
- roles/nginx/
  - tasks/main.yml
  - files/index.html
  - vars/main.yml
  - handlers/main.yml
- ansible.cfg

## Run
ansible-playbook -i inventory/hosts.ini playbooks/webserver.yml

## Output
Access in browser:
http://<EC2-IP>

## Features
- Nginx install & start
- HTML deployment
- Idempotent execution
- Roles, variables, handlers
