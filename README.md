
# Automação do Gerenciamento de Servidores com Ansible

> Trabalho de Conclusão de Curso (TCC) – Tecnólogo em Redes de Computadores  
> **Faculdade de Tecnologia de Osasco – FATEC Osasco**  
> **Autoras:** Evellyn Patricia Adolfo & Marcos Donato  
> **Orientador:** Prof. Dr. Francisco Eugenio Barrella  
> **Ano:** 2026

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Ansible](https://img.shields.io/badge/Ansible-12+-red.svg)](https://docs.ansible.com/)
[![Python](https://img.shields.io/badge/Python-3.12+-blue.svg)](https://www.python.org/)

## 📌 Sobre o Projeto

Este repositório contém os playbooks, inventários, roles e scripts desenvolvidos para o TCC *"Automação do Gerenciamento de Servidores com Ansible"*. O objetivo é demonstrar a aplicação prática de Infraestrutura como Código (IaC) para padronizar, automatizar e escalar a administração de servidores Linux (Debian/Ubuntu e Red Hat/Rocky) e Windows em ambientes heterogêneos.

### ✨ Principais Funcionalidades
- ✅ Automação de configuração base (SSH, usuários, firewall)
- ✅ Provisionamento de serviços: DNS (Bind9), Web (Nginx), DHCP
- ✅ Suporte multi-distribuição com roles parametrizadas
- ✅ Estrutura modular seguindo [Best Practices do Ansible](https://docs.ansible.com/projects/ansible/2.9/user_guide/playbooks_best_practices.html)
- ✅ Script de geração automática de estrutura de projetos (`ansible_project_v4.sh`)

## 🚀 Pré-requisitos

- **Control Node:** Linux (Fedora 40 recomendado)
- **Ansible:** ≥ 12
- **Python:** ≥ 3.12
- **Acesso SSH** aos hosts gerenciados (Linux) ou **WinRM** (Windows)
- **Privilégios** sudo (Linux) / Admin (Windows)

## 📁 Estrutura do Projeto

```bash
TCC_Ansible/
    │
    ├── ansible01_v3
    │   │
    │   ├── ansible.cfg        # Configurações globais
    │   ├── inventory/         # Inventários
    │   │   │
    │   │   ├── group_vars/        # Variáveis por grupo de hosts
    │   │   ├── host_vars/         # Variáveis por host específico
    │   │   ├── testing            # Inventário de teste
    │   │   └── production         # Inventário de produção
    │   │
    │   ├── playbooks/         # Playbooks de orquestração
    │   ├── roles/             # Roles modulares (common, dns, web, windows_dc)
    │   └── vars/
    │
    ├── scripts/           # Scripts auxiliares (ansible_project_v4.sh)
    └── README.md
```


> 🎓 *Projeto desenvolvido como requisito parcial para obtenção do título de Tecnólogo em Redes de Computadores pela FATEC Osasco.*
