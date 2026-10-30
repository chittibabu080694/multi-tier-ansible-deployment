# Multi-Tier Application Deployment with Ansible

An automated, modular Ansible project for deploying a 3-tier architecture (Load Balancer, Web/Application servers, and Database server) across cloud instances.

## Project Architecture
- **Load Balancer Tier (`lb`):** Nginx reverse proxy routing traffic across backend nodes.
- **Application Tier (`app`):** Node.js runtime and application environment configured via templates.
- **Database Tier (`db`):** PostgreSQL server with automated database and user creation.

## Directory Structure
```text
multi-tier-ansible-deployment/
├── ansible.cfg
├── site.yml
├── group_vars/
│   └── all.yml
├── inventory/
│   └── hosts.ini
└── roles/
    ├── common/
    ├── database/
    ├── backend/
    └── frontend/
