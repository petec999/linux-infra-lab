# Linux Infrastructure Lab

Hands-on Linux infrastructure and DevOps engineering lab.

## Environment

- Rocky Linux 10.1
- Oracle VirtualBox
- Python 3.12
- Ansible Core
- Git

## Current Features

### System Information Playbook

Collects Linux system information using Ansible facts.

Reports:
- Hostname
- OS distribution and version
- Kernel version
- Available system memory

Run:

    ansible-playbook -i localhost, playbooks/system-info.yml

## Project Structure

- playbooks/ - Ansible automation playbooks

## Roadmap

- [x] Ansible system facts collection
- [ ] Ansible roles and inventory
- [ ] Linux service management
- [ ] Docker containers
- [ ] CI/CD pipelines
- [ ] Infrastructure monitoring
- [ ] Terraform
- [ ] Kubernetes

## Related Project

OpenMind AI - AI-powered Linux infrastructure diagnostics.

## Author

Independent Linux / Infrastructure / Platform Engineering lab.
