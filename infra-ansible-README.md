# Jenkins Infrastructure as Code

Este repositorio levanta Jenkins usando:

- Ansible (infraestructura)
- Docker (runtime)
- Jenkins Configuration as Code (configuración)

## Requisitos
- Servidor Ubuntu
- Acceso SSH
- Ansible en máquina local

## Despliegue

```bash
ansible-playbook playbooks/site.yml
