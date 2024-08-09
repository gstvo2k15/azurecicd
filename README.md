# GitHub Actions Pipeline con Azure Key Vault

Este repositorio contiene un ejemplo de cómo configurar un pipeline de GitHub Actions para recuperar secretos desde Azure Key Vault y utilizarlos en la ejecución de un playbook de Ansible.

## Estructura del Repositorio

```
.
├── .github
│   └── workflows
│       └── azure-keyvault-pipeline.yml  # Archivo del pipeline de GitHub Actions
├── README.md  # Este archivo con la documentación
└── playbook.yml  # Playbook de Ansible
```

## GitHub Actions Workflow:

```
|
|--- Checkout code
|
|--- Azure Login
|
|--- Fetch secrets from Azure Key Vault
|
|--- Install Ansible
|
|--- Execute Ansible playbook
```

### Notas Finales

- **`azure-keyvault-pipeline.yml`**: Este archivo define el workflow de GitHub Actions y se ubica dentro de `.github/workflows/`.
- **`playbook.yml`**: Este archivo contiene el playbook de Ansible que se ejecutará en el pipeline. Debes adaptarlo según tus necesidades.
