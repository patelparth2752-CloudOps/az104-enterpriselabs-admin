ENTERPRISE AZ-104 ADMIN PROJECT
Overview

This project demonstrates real-world Azure Administrator (AZ-104) skills by designing, deploying, securing, monitoring, and cleaning up a production-style Azure environment using best practices.

Technologies Used

Azure Virtual Machines (Linux)

Azure Virtual Network & Subnets

Network Security Groups (NSG)

Azure Monitor & Alerts

Recovery Services Vault (Backup)

Azure RBAC (IAM)

GitHub for documentation

Architecture Diagram

(High-level flow of traffic)

User (Browser)
   |
   | HTTP (Port 80)
   v
Public IP
   |
   v
Network Security Group (NSG)
   |
   v
Virtual Network (VNet)
   |
   v
Subnet
   |
   v
Linux VM (Ubuntu)
   |
   v
Nginx Web Server

Project Phases
Phase 1: Resource Group & Networking

Created Resource Group in East US

Designed VNet with custom address space

Configured Subnet and NSG rules

Phase 2: Virtual Machines

Deployed Linux VMs

Selected cost-optimized VM sizes

Configured public IP and NIC

Phase 3: Web Server Configuration

Installed Nginx

Verified web access via browser

Phase 4: Monitoring & Alerts

Enabled Azure Monitor

Created CPU utilization alert

Phase 5: Backup & Recovery

Configured Recovery Services Vault

Enabled VM backup

Verified backup health

Phase 6: Identity & Access Management (IAM)

Created Reader user

Assigned RBAC role

Validated least privilege access

Phase 7: Validation

Stopped one VM and validated service availability

Verified alerts, backup status, and RBAC restrictions

Phase 8: Cleanup

Disabled backups

Deleted Recovery Vault

Deleted all Azure resources to avoid cost

Key Learnings

Azure networking fundamentals

Cost control and governance

Monitoring and operational readiness

Security using RBAC

Proper resource cleanup

Screenshots

Screenshots are stored in the /screenshots folder for validation and evidence.

Author

Parth
AZ-104 Certified | Aspiring Azure Administrator
