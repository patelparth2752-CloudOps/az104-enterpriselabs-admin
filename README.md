name: Enterprise AZ-104 Admin Project Validation

on:
  push:
    branches:
      - main
  workflow_dispatch:

jobs:
  project-overview:
    name: Project Overview
    runs-on: ubuntu-latest
    steps:
      - name: Display project summary
        run: |
          echo "ENTERPRISE AZ-104 ADMIN PROJECT"
          echo "--------------------------------"
          echo "This project demonstrates hands-on Azure Administrator (AZ-104) skills."
          echo "Focus areas: compute, networking, security, monitoring, backup, and cleanup."

  technologies:
    name: Technologies Used
    runs-on: ubuntu-latest
    steps:
      - name: List technologies
        run: |
          echo "Azure Virtual Machines (Linux / Ubuntu)"
          echo "Azure Virtual Network (VNet) and Subnets"
          echo "Network Security Groups (NSG)"
          echo "Azure Monitor and Alerts"
          echo "Recovery Services Vault (Azure Backup)"
          echo "Azure RBAC (IAM)"
          echo "GitHub for documentation"

  architecture:
    name: Architecture Overview
    runs-on: ubuntu-latest
    steps:
      - name: Display architecture flow
        run: |
          echo "User (Browser)"
          echo "  -> HTTP (Port 80)"
          echo "  -> Public IP"
          echo "  -> Network Security Group (NSG)"
          echo "  -> Virtual Network (VNet)"
          echo "  -> Subnet"
          echo "  -> Linux VM (Ubuntu)"
          echo "  -> Nginx Web Server"

  project-phases:
    name: Project Phases
    runs-on: ubuntu-latest
    steps:
      - name: Phase 1 - Resource Group and Networking
        run: |
          echo "Created Resource Group in East US"
          echo "Designed VNet with custom address space"
          echo "Configured subnets and NSG rules"

      - name: Phase 2 - Virtual Machines
        run: |
          echo "Deployed Linux VMs"
          echo "Selected cost-optimized VM sizes"
          echo "Configured NICs and public IPs"

      - name: Phase 3 - Web Server Configuration
        run: |
          echo "Installed and configured Nginx"
          echo "Verified web access via browser"

      - name: Phase 4 - Monitoring and Alerts
        run: |
          echo "Enabled Azure Monitor"
          echo "Created CPU utilization alerts"
          echo "Validated alerts using simulated CPU load"

      - name: Phase 5 - Backup and Recovery
        run: |
          echo "Configured Recovery Services Vault"
          echo "Enabled VM backups"
          echo "Verified backup health"

      - name: Phase 6 - Identity and Access Management
        run: |
          echo "Created Reader user"
          echo "Assigned RBAC roles"
          echo "Validated least-privilege access"

      - name: Phase 7 - Validation
        run: |
          echo "Stopped one VM to validate service behavior"
          echo "Verified alerts, backups, and RBAC restrictions"

      - name: Phase 8 - Cleanup
        run: |
          echo "Disabled VM backups"
          echo "Deleted Recovery Services Vault"
          echo "Removed all Azure resources to prevent cost"

  summary:
    name: Key Learnings and Author
    runs-on: ubuntu-latest
    steps:
      - name: Display key learnings
        run: |
          echo "Key Learnings:"
          echo "- Azure networking and security fundamentals"
          echo "- Cost control and governance"
          echo "- Monitoring and alerting strategies"
          echo "- RBAC and identity management"
          echo "- Resource lifecycle management"

      - name: Author
        run: |
          echo "Author: Parth"
          echo "AZ-104 Certified | Aspiring Azure Administrator"
