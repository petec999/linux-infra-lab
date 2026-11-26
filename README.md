# Linux Infrastructure Lab

Hands-on infrastructure automation lab using Rocky Linux and Ansible.

## Environment

Rocky Linux 10.1 in VirtualBox, Ansible Core, Python and Git. The exercises run locally with an explicit localhost inventory.

## Implemented

| Playbook | Purpose | Effect |
| --- | --- | --- |
| [system-info.yml](playbooks/system-info.yml) | Hostname, OS, kernel and memory facts | Writes `~/system-report.txt` |
| [service-audit.yml](playbooks/service-audit.yml) | Inspect SSH and NetworkManager systemd services | Read-only |

```bash
ansible-playbook -i localhost, playbooks/system-info.yml
ansible-playbook -i localhost, playbooks/service-audit.yml
```

Check syntax before executing:

```bash
ansible-playbook -i localhost, --syntax-check playbooks/system-info.yml
ansible-playbook -i localhost, --syntax-check playbooks/service-audit.yml
```

## Learning roadmap

- [x] Ansible facts and local reporting
- [x] Service inventory and audit
- [ ] Variables, templates and roles
- [ ] Idempotent service configuration
- [ ] Containers and CI/CD
- [ ] Monitoring, Terraform and Kubernetes

This repository is a personal learning lab, not a production platform. Only committed exercises are described as implemented. Never commit secrets, machine-specific reports or private inventory data.
