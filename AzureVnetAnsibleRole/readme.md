# Ansible - Azure Virtual Network (VNet)

This repository contains an Ansible role to provision an Azure Virtual Network (VNet) along with a subnet. It uses the `azure.azcollection` and is ideal for automating Azure networking in a repeatable and declarative manner.


## 📌 Components Created
- Azure Resource Group (if not existing)
- Azure Virtual Network (VNet)
- Subnet inside the VNet


## 📁 Directory Structure
AzureVnetAnsibleRole/
    ├── defaults/
    │   └── main.yml
    └── tasks/
        └── main.yml


## 🚀 How to Run
az login
ansible-playbook playbook.yml -i localhost


## ✅ Prerequisites
1. Ansible installed (pip install ansible)
2. Azure CLI installed and authenticated (az login)


## Install Azure collection for Ansible:
1. ansible-galaxy collection install azure.azcollection
2. Python packages:
   pip install azure-cli-core msrest azure-mgmt-network


## 🔐 Authentication
This role uses the credentials from Azure CLI (az login). For other auth methods, set AZURE_CLIENT_ID, AZURE_SECRET, AZURE_SUBSCRIPTION_ID, and AZURE_TENANT.