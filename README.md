# 🚀 Infrastructure Platform

Production-ready Azure platform using Terraform, CI/CD, security best practices, and infrastructure automation.

---

## 📋 Project Overview

This project demonstrates a realistic Azure infrastructure setup designed and operated the way modern platform engineering teams manage cloud infrastructure. The focus is on **automation**, **security**, **observability**, and **operational excellence**.

---

## 👥 Team & Roles

| Name | Role | Responsibilities |
|------|------|------------------|
| **Nikhil Mhatre** | Platform Lead | Architecture decisions, PR reviews, production approvals, governance oversight |
| **Karan Parab** | Platform Engineer | Infrastructure development, Terraform coding, feature implementation, dev deployments |

---

## 🏗️ Architecture Components

### Infrastructure Services
- **Networking:** Azure VNet, Subnets, NSGs, Private Endpoints
- **Compute:** VM Scale Set with autoscaling
- **Traffic Management:** Application Gateway (L7 with WAF)
- **Data:** PostgreSQL Flexible Server (private endpoint)
- **Storage:** Azure Blob Storage (private endpoint)

### Security & Identity
- **Azure Entra ID** - User identity and RBAC
- **Managed Identity** - Passwordless authentication
- **Azure Key Vault** - Secrets management
- **RBAC** - Least privilege access control

### Observability & Governance
- **Azure Monitor** - Metrics and alerts
- **Log Analytics Workspace** - Centralized logging
- **Cost Management** - Budget alerts and tracking
- **Mandatory Tagging** - Cost allocation and governance

---

## 📁 Project Structure
```
platform-infrastructure/
├── .azuredevops/
│ └── pipelines/ # CI/CD pipeline definitions
│ ├── terraform-plan.yml
│ ├── terraform-apply.yml
│ └── pr-validation.yml
├── environments/
│ ├── dev/ # Development environment configs
│ │ ├── terraform.tfvars
│ │ └── backend.tf
│ └── prod/ # Production environment configs
│ ├── terraform.tfvars
│ └── backend.tf
├── modules/
│ ├── networking/ # VNet, subnets, NSGs
│ ├── compute/ # VMSS, Bastion
│ ├── security/ # Key Vault, Managed Identity
│ ├── data/ # PostgreSQL, Storage
│ └── monitoring/ # Azure Monitor, Log Analytics
├── docs/
│ ├── runbooks/ # Operational procedures
│ ├── architecture/ # Architecture diagrams
│ └── decisions/ # Architecture Decision Records (ADRs)
├── main.tf # Root module orchestration
├── variables.tf # Input variables
├── outputs.tf # Output values
├── providers.tf # Provider configuration
└── README.md # This file
```

---
# 📞 Contact & Support
- **Platform Lead**: Nikhil Mhatre
- **Platform Engineer**: Karan Parab

- **Repository**: [github.com/Nikhil-Mhatre/platform-infrastructure](https://github.com/Nikhil-Mhatre/platform-infrastructure.git)

- **Last Updated**: January 2, 2026
- **Updated By**: Karan Parab (Platform Engineer)