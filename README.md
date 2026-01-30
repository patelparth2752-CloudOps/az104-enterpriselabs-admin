project:
  name: ENTERPRISE AZ-104 ADMIN PROJECT

  overview: >
    This project demonstrates hands-on Azure Administrator (AZ-104) skills by
    designing, deploying, securing, monitoring, and cleaning up a
    production-style Azure environment using Azure best practices.
    The environment simulates an enterprise Linux-based web workload.

  technologies_used:
    - Azure Virtual Machines (Linux / Ubuntu)
    - Azure Virtual Network (VNet) and Subnets
    - Network Security Groups (NSG)
    - Azure Monitor and Alerts
    - Recovery Services Vault (Azure Backup)
    - Azure RBAC (IAM)
    - GitHub for documentation

  architecture:
    description: High-level traffic flow
    flow:
      - User (Browser)
      - HTTP (Port 80)
      - Public IP
      - Network Security Group (NSG)
      - Virtual Network (VNet)
      - Subnet
      - Linux VM (Ubuntu)
      - Nginx Web Server

  project_phases:
    - phase: Phase 1 - Resource Group & Networking
      tasks:
        - Created a Resource Group in East US
        - Designed a VNet with custom address space
        - Configured subnets and NSG rules

    - phase: Phase 2 - Virtual Machines
      tasks:
        - Deployed Linux virtual machines
        - Selected cost-optimized VM sizes
        - Configured NICs and public IPs

    - phase: Phase 3 - Web Server Configuration
      tasks:
        - Installed and configured Nginx
        - Verified web access via browser

    - phase: Phase 4 - Monitoring & Alerts
      tasks:
        - Enabled Azure Monitor
        - Created CPU utilization alerts
        - Validated alerts using simulated CPU load

    - phase: Phase 5 - Backup & Recovery
      tasks:
        - Configured Recovery Services Vault
        - Enabled VM backups
        - Verified backup health and status

    - phase: Phase 6 - Identity & Access Management (IAM)
      tasks:
        - Created a Reader user
        - Assigned RBAC roles
        - Validated least-privilege access

    - phase: Phase 7 - Validation
      tasks:
        - Stopped one VM to validate service behavior
        - Verified alerts, backup configuration, and RBAC restrictions

    - phase: Phase 8 - Cleanup
      tasks:
        - Disabled VM backups
        - Deleted Recovery Services Vault
        - Removed all Azure resources to prevent ongoing costs

  key_learnings:
    - Azure networking and security fundamentals
    - Cost control and governance
    - Monitoring and alerting strategies
    - Role-based access control (RBAC)
    - End-to-end resource lifecycle management

  screenshots:
    location: /screenshots
    description: Validation screenshots and evidence

  author:
    name: Parth
    title: AZ-104 Certified | Aspiring Azure Administrator
