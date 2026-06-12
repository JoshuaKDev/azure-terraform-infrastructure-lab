# Azure Infrastructure as Code Lab

## Overview

This project demonstrates the deployment and management of Azure infrastructure using Terraform and Infrastructure as Code (IaC) principles. The goal is to create a repeatable, scalable, and secure Azure environment entirely through code rather than manual portal configuration.

The lab focuses on foundational cloud infrastructure, security best practices, monitoring, and automation to simulate real-world cloud engineering and cloud operations workflows.

## Objectives

- Deploy Azure infrastructure using Terraform
- Implement Infrastructure as Code (IaC) best practices
- Create reusable Terraform modules
- Secure cloud resources using Azure security controls
- Enable monitoring and logging
- Practice cloud automation and version control workflows
- Document cloud architecture and deployment processes

---

## Technologies Used

### Cloud Platform
- Microsoft Azure

### Infrastructure as Code
- Terraform

### Development Tools
- Visual Studio Code
- Git
- GitHub
- Azure CLI

### Azure Services
- Resource Groups
- Virtual Networks (VNets)
- Subnets
- Network Security Groups (NSGs)
- Virtual Machines
- Public IP Addresses
- Azure Key Vault
- Azure Bastion
- Azure Monitor
- Log Analytics Workspace

---

## Project Architecture

```text
Resource Group
│
├── Virtual Network
│   └── Subnet
│
├── Network Security Group
│
├── Linux Virtual Machine
│
├── Windows Virtual Machine
│
├── Azure Key Vault
│
├── Azure Bastion
│
└── Azure Monitor
```

---

## Project Phases

### Phase 1 – Core Infrastructure

Deploy foundational Azure resources using Terraform:

- Resource Group
- Virtual Network
- Subnet
- Network Security Group
- Linux Virtual Machine
- Windows Virtual Machine
- Public IP Address

#### Goals

- Build a functional Azure environment
- Deploy infrastructure through code
- Verify successful provisioning using Terraform

---

### Phase 2 – Security Hardening

Implement security controls and best practices:

- Restrict inbound network access
- Configure Network Security Groups
- Deploy Azure Bastion
- Configure Managed Identities
- Store secrets in Azure Key Vault

#### Goals

- Reduce attack surface
- Follow least privilege principles
- Improve cloud security posture

---

### Phase 3 – Monitoring and Logging

Enable visibility into deployed resources:

- Azure Monitor
- Log Analytics Workspace
- VM Insights
- Performance monitoring

#### Goals

- Collect operational telemetry
- Monitor system health
- Practice cloud monitoring workflows

---

### Phase 4 – Terraform Modularization

Refactor infrastructure into reusable Terraform modules.

Example structure:

```text
terraform/
│
├── modules/
│   ├── network/
│   ├── vm/
│   └── monitoring/
│
├── main.tf
├── variables.tf
├── outputs.tf
└── providers.tf
```

#### Goals

- Improve code organization
- Increase reusability
- Follow Infrastructure as Code best practices

---

### Phase 5 – CI/CD Automation

Integrate GitHub Actions to automate Terraform workflows.

Pipeline:

```text
Git Push
   ↓
Terraform Format
   ↓
Terraform Validate
   ↓
Terraform Plan
   ↓
Terraform Apply
```

#### Goals

- Automate deployments
- Implement Infrastructure as Code pipelines
- Practice DevOps workflows

---

## Security Controls Implemented

- Network Security Groups (NSGs)
- Least Privilege Access
- Azure Bastion Administration
- Managed Identities
- Azure Key Vault Secret Storage
- Infrastructure as Code Change Tracking
- Version Control Through GitHub

---

## Screenshots

### Terraform Deployment

*Add screenshot of successful Terraform deployment.*

---

### Azure Resource Group

*Add screenshot showing deployed resources.*

---

### Virtual Network Configuration

*Add screenshot of VNet and subnet configuration.*

---

### Azure Key Vault

*Add screenshot showing deployed Key Vault.*

---

### Azure Monitor

*Add screenshot of monitoring dashboard.*

---

### GitHub Actions Pipeline

*Add screenshot of successful workflow execution.*

---

## Lessons Learned

- Infrastructure can be deployed consistently and repeatedly through code.
- Terraform simplifies Azure resource management.
- Security should be integrated during deployment rather than added later.
- Monitoring and observability are critical components of cloud operations.
- Version control improves infrastructure reliability and change management.

---

## Future Improvements

- Azure Firewall
- Private Endpoints
- Azure Policy
- Azure Defender for Cloud
- Hub-and-Spoke Networking
- Multi-Environment Deployments (Dev/Test/Prod)
- Automated Security Scanning
- Terraform Remote State Storage

---

## Author

Joshua Kitchen

GitHub: https://github.com/JoshuaKDev

Website: https://www.jkcloudsecurity.com
