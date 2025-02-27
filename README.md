# GitHub Actions Pipeline with Azure Key Vault

This repository contains an example of how to configure a GitHub Actions pipeline to retrieve secrets from Azure Key Vault and use them to run an Ansible playbook.

## Repository Structure

```
.
├── .github
│ └── workflows
│ └── azure-keyvault-pipeline.yml # GitHub Actions pipeline file
├── README.md # This file with the documentation
└── playbook.yml # Ansible Playbook
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

### Final Notes

- **`azure-keyvault-pipeline.yml`**: This file defines the GitHub Actions workflow and is located inside `.github/workflows/`.
- **`playbook.yml`**: This file contains the Ansible playbook that will be executed in the pipeline. You must adapt it according to your needs.
