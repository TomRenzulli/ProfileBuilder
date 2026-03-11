# 🖥️ Information Technology Skills Master Template

> **Copy-paste reference for GitHub profiles, resumes, and portfolios.**
> Delete what doesn't apply. Add what's missing. Make it yours.

---

## How to Use This Template

1. **Pick your tier** — Skills are organized from foundational (Helpdesk) through advanced (Architecture). Start where you are.
2. **Be honest** — List what you actually administer, not what you've seen once in a lab.
3. **Show depth** — Star (⭐) or bold your strongest skills. "Active Directory (GPO design, tiered admin, 5,000+ users)" hits harder than just "Active Directory."
4. **Keep it current** — Microsoft renames things every 6 months. Review quarterly.

---

## 🟢 Helpdesk / Desktop Support (Tier 1)

### Ticketing & Service Management

```
ServiceNow | Jira Service Management | Zendesk
Freshdesk / Freshservice | ConnectWise Manage
ManageEngine ServiceDesk Plus | Spiceworks
SLA tracking | Ticket triage | Escalation procedures
Knowledge base creation & maintenance
```

### Endpoint Support

```
Windows 10/11 troubleshooting | macOS support | ChromeOS
Driver installation & management | Blue screen (BSOD) diagnosis
Printer setup & troubleshooting (local, network, print servers)
Peripheral configuration (monitors, docking stations, KVM)
Imaging & deployment (MDT, WDS, USB boot media)
Software installation & licensing | MSI / EXE deployment
Browser troubleshooting (Chrome, Edge, Firefox)
```

### Account & Access Management

```
Active Directory — password resets, account unlocks, group membership
Azure AD / Entra ID — basic user management, MFA resets
Microsoft 365 — mailbox access, license assignment, distribution lists
Google Workspace — account provisioning, password resets
Shared drive / folder permissions (NTFS basics)
VPN client setup & troubleshooting
```

### Hardware

```
Desktop / laptop setup & deployment | Asset tagging & tracking
RAM / SSD / HDD replacement | Cable management
Monitor configuration (multi-display, resolution, refresh rate)
Docking station troubleshooting (USB-C, Thunderbolt)
Mobile device setup (iOS, Android) | MDM enrollment
Warranty processing & RMA coordination
```

### Networking Basics

```
IP addressing (static, DHCP) | DNS concepts (A, CNAME, MX)
Wi-Fi troubleshooting | Ethernet connectivity
VPN connectivity issues | Proxy configuration
Basic ping / tracert / ipconfig / nslookup
Network printer mapping | Drive mapping (UNC paths)
```

### Remote Support Tools

```
Remote Desktop (RDP / MSTSC) | Quick Assist
TeamViewer | AnyDesk | Splashtop
Dameware | BeyondTrust Remote Support
ConnectWise ScreenConnect | LogMeIn
```

---

## 🟡 Helpdesk / Technical Support (Tier 2)

### Active Directory Administration

```
User & group management (OUs, security groups, distribution lists)
Group Policy — applying, linking, troubleshooting (gpresult, rsop.msc)
Computer object management | Domain join / unjoin
DHCP scope management | DNS record creation & modification
Account provisioning & deprovisioning workflows
Service accounts | Managed Service Accounts (gMSA)
Delegation of control | LDAP queries
```

### Microsoft 365 / Exchange Administration

```
Exchange Online — mailbox management, shared mailboxes, aliases
Mail flow troubleshooting (message trace, NDR analysis)
Distribution lists / Microsoft 365 Groups / shared calendars
OneDrive / SharePoint permissions | Teams administration
Retention policies | Litigation hold basics
License management & optimization
Conditional Access policy troubleshooting
Intune — device enrollment, compliance policies, app deployment
```

### Endpoint Management & Deployment

```
SCCM / MECM (Microsoft Endpoint Configuration Manager)
Intune / Microsoft Endpoint Manager | Autopilot
PDQ Deploy / PDQ Inventory | WSUS (Windows Server Update Services)
MDT (Microsoft Deployment Toolkit) | WDS
Group Policy software deployment | PowerShell remoting
Patch management | Software packaging (MSI, MSIX, AppX)
Application compatibility troubleshooting
```

### Networking (Intermediate)

```
VLAN concepts | Switch port configuration basics
DHCP troubleshooting (scope, reservations, relay)
DNS troubleshooting (forward/reverse lookup, conditional forwarders)
Firewall rule requests & basic troubleshooting
Wi-Fi — AP management, SSIDs, authentication (WPA2/3 Enterprise)
Certificate-based authentication (802.1X basics)
VPN configuration (client & site-to-site concepts)
Packet capture basics (Wireshark)
```

### Scripting & Automation (Intermediate)

```
PowerShell — bulk AD operations, user provisioning, reporting
Batch scripting | Task Scheduler
Basic Python scripting for automation
Registry editing | GPO preference items
CSV/Excel report generation from system data
```

### Monitoring & Troubleshooting

```
Event Viewer (Windows) | syslog basics (Linux)
Performance Monitor (perfmon) | Resource Monitor
Sysinternals Suite (Process Explorer, Autoruns, ProcMon, TCPView)
Disk management (Disk Management, diskpart, Storage Spaces)
Windows Recovery Environment (WinRE) | Safe Mode
Service management (services.msc, sc.exe, systemctl)
```

---

## 🟠 Helpdesk / Senior Technical Support (Tier 3)

### Advanced Active Directory & Identity

```
AD Sites & Services | AD Replication troubleshooting (repadmin)
FSMO roles — identification, transfer, seizure
AD Certificate Services (AD CS) — certificate templates, enrollment
AD Federation Services (AD FS) | Azure AD Connect / Cloud Sync
Hybrid identity (on-prem + Azure AD) | Pass-through authentication
Kerberos troubleshooting | NTLM relay awareness
Trust relationships (forest, external, shortcut)
Fine-grained password policies | AD recycle bin
Schema extensions | tombstone lifetime & lingering objects
```

### Advanced Networking & Infrastructure

```
Routing & switching (VLANs, trunking, spanning tree, OSPF/BGP basics)
Firewall administration (Palo Alto, Cisco ASA, Fortinet, pfSense)
Load balancers (F5, HAProxy, Azure LB, AWS ALB/NLB)
NAC (Network Access Control) | 802.1X (RADIUS / NPS)
SD-WAN concepts | MPLS basics | Site-to-site VPN management
Network segmentation | DMZ design
Packet analysis (Wireshark, tcpdump) | NetFlow analysis
```

### Server Administration

```
Windows Server 2016/2019/2022/2025
— Roles: AD DS, DNS, DHCP, File Server, Print Server, NPS, WSUS
— Failover Clustering | Storage Spaces Direct (S2D)
— Windows Admin Center | Server Manager | RSAT
— DFS (Distributed File System) — namespaces & replication

Linux Server (RHEL/CentOS, Ubuntu, Debian)
— systemd service management | cron jobs
— SSH hardening | firewalld / iptables / nftables
— NFS / Samba | Apache / Nginx | Package management (apt, yum, dnf)
— LVM | RAID configuration | Log management (journalctl, rsyslog)
```

### Virtualization & Hypervisors

```
VMware vSphere / ESXi / vCenter — VM lifecycle, snapshots, vMotion
Hyper-V — VM management, checkpoints, replication, live migration
Proxmox VE | KVM/QEMU | Citrix Hypervisor (XenServer)
Resource allocation & capacity planning
Template creation | VM cloning | OVA/OVF management
Virtual networking (vSwitch, distributed switch, port groups)
Storage: vSAN, iSCSI, NFS datastores, FC SAN basics
```

### Storage & Backup

```
SAN / NAS concepts | iSCSI | Fibre Channel basics
NetApp | Dell EMC (PowerStore, Unity) | Pure Storage
Synology / QNAP (SMB/NFS)
Veeam Backup & Replication | Commvault | Rubrik
Acronis | Nakivo | Azure Backup | AWS Backup
Backup strategies (3-2-1 rule, RPO, RTO)
Disaster recovery planning & testing
DFS-R | DFSR troubleshooting | Robocopy / rsync
```

### Database Basics (IT Operations)

```
SQL Server — basic administration, backup/restore, maintenance plans
MySQL / MariaDB — installation, user management, backups
PostgreSQL — basic ops, pg_dump, replication concepts
MongoDB basics | Redis basics
Database connectivity troubleshooting (ODBC, connection strings)
```

### Advanced Scripting & Automation

```
PowerShell Advanced — modules, functions, error handling, remoting
— Active Directory module | Exchange Online module
— Microsoft Graph API via PowerShell
— Desired State Configuration (DSC)
Python — system administration scripts, API integration
Bash — Linux automation, cron, log parsing
Ansible — playbooks, roles, inventory management
Terraform basics | ARM templates | Bicep
REST API interaction (Invoke-RestMethod, curl, Postman)
```

---

## 🔴 Systems Administrator / Infrastructure Engineer

### Infrastructure Design & Management

```
Server lifecycle management (procurement → deployment → decommission)
Capacity planning | Performance tuning | Availability design
High availability (HA) & fault tolerance | Load balancing
Disaster recovery (DR) — runbooks, failover testing, site recovery
Change management | Maintenance windows | Rollback procedures
Documentation — network diagrams, runbooks, SOPs, as-built docs
```

### Cloud Administration

```
Microsoft Azure
— Azure AD / Entra ID | Conditional Access | PIM
— Virtual Machines | App Services | Azure SQL
— Virtual Networks (VNets) | NSGs | Azure Firewall | Front Door
— Azure Storage (Blob, Files, Tables) | Azure Backup
— Azure Monitor | Log Analytics | Application Insights
— Azure DevOps | ARM / Bicep templates

Amazon Web Services (AWS)
— EC2 | S3 | RDS | Lambda | CloudFormation
— VPC | Security Groups | IAM | Route 53
— CloudWatch | CloudTrail | Systems Manager
— AWS Organizations | Control Tower basics

Google Cloud Platform (GCP)
— Compute Engine | Cloud Storage | Cloud SQL
— VPC | IAM | Cloud Monitoring
```

### Configuration Management & IaC

```
Ansible — playbooks, roles, inventories, Ansible Tower/AWX
Terraform — providers, state management, modules, workspaces
Puppet | Chef | SaltStack
Docker — containerization, Dockerfile, docker-compose
Kubernetes — pods, services, deployments, namespaces, Helm
CI/CD pipelines (GitHub Actions, Azure DevOps, Jenkins, GitLab CI)
GitOps workflows | Infrastructure as Code best practices
```

### Email & Collaboration Infrastructure

```
Exchange Server (on-prem) — DAGs, transport rules, certificates
Exchange Online / Microsoft 365 — hybrid configuration
SMTP relay | Mail flow connectors | SPF / DKIM / DMARC
Microsoft Teams (telephony, meeting rooms, policies)
SharePoint Online / On-Prem | OneDrive for Business
Zoom / Webex administration | Slack administration
```

### Print & Peripheral Infrastructure

```
Print server management | Universal Print (Azure)
Printer fleet management (PaperCut, PrinterLogic, Equitrac)
Large-scale driver management | GPO printer deployment
Multifunction device (MFD) configuration & security
```

### Monitoring & Observability

```
Nagios / Icinga | Zabbix | PRTG | Datadog
SolarWinds (NPM, SAM, NCM) | ManageEngine OpManager
Grafana + Prometheus | ELK Stack (Elasticsearch, Logstash, Kibana)
Azure Monitor | AWS CloudWatch | GCP Cloud Monitoring
SNMP | WMI | Syslog | Windows Event Forwarding (WEF)
Uptime monitoring | Alerting & escalation | Dashboarding
Capacity trending | Performance baselining
```

### Telephony & Unified Communications

```
VoIP — SIP, RTP, codecs | Microsoft Teams Phone System
Cisco Unified Communications Manager (CUCM) | Webex Calling
Zoom Phone | RingCentral | 8x8
PBX concepts | SBC (Session Border Controller)
Call quality troubleshooting (MOS, jitter, packet loss)
Contact center basics (Genesys, Five9, NICE)
```

---

## 🟣 IT Management & Architecture

### ITSM & Governance Frameworks

```
ITIL 4 (Service Value System, practices, continual improvement)
ITIL v3 (Incident, Problem, Change, Service Level, CMDB)
COBIT | MOF (Microsoft Operations Framework)
Change Advisory Board (CAB) | Change management process
Incident management | Problem management (root cause analysis)
Service catalog design | SLA / OLA / UC management
CMDB — CI relationships, asset management, discovery tools
Capacity management | Availability management
```

### IT Project & Vendor Management

```
Project planning & execution | Gantt charts | WBS
Agile / Scrum / Kanban (IT context) | Waterfall
Vendor evaluation & selection | RFP / RFI process
Contract negotiation | SLA enforcement
Budget planning & tracking | TCO / ROI analysis
Procurement workflows | License management (SAM / ITAM)
ServiceNow ITAM | Flexera | Snow Software
```

### Architecture & Design

```
Enterprise architecture frameworks (TOGAF, Zachman)
Network architecture — campus, data center, WAN, SD-WAN
Identity architecture — Zero Trust, tiered AD model, PAM
Cloud architecture — landing zones, hub-spoke, multi-cloud
Hybrid cloud design — connectivity, identity sync, workload placement
Migration planning — P2V, V2V, on-prem to cloud
Reference architectures (Microsoft, AWS, Google)
High availability design patterns | DR architecture
```

### Compliance & Security (IT Ops Perspective)

```
CIS Benchmarks (Windows, Linux, cloud) | STIG hardening
Patch management strategy & SLAs | Vulnerability remediation
Audit log management | Retention policies
Data classification | DLP policies (Microsoft Purview, etc.)
Encryption at rest & in transit | Certificate management (PKI)
Endpoint hardening | USB device control | BitLocker / FileVault
Security awareness training administration (KnowBe4, Proofpoint)
```

---

## 🟤 Specialty Domains

### Physical Infrastructure & Data Center

```
Rack & stack | Cable management (structured cabling, fiber, Cat6/6a)
UPS / PDU management | Generator coordination
HVAC & environmental monitoring | Hot/cold aisle containment
KVM switches | Out-of-band management (iLO, iDRAC, IPMI)
Data center standards (TIA-942, Uptime Institute tiers)
Colocation management | Vendor escort procedures
Asset lifecycle — procurement, deployment, decommission, disposal (NIST 800-88)
```

### Mobile Device Management (MDM / UEM)

```
Microsoft Intune | Jamf Pro (macOS/iOS) | VMware Workspace ONE
MobileIron / Ivanti | SOTI | Kandji
Device enrollment (DEP, Autopilot, Zero-Touch)
Compliance policies | App protection policies
BYOD vs. corporate-owned device strategies
Remote wipe | Conditional Access integration
```

### Directory Services (Deep Dive)

```
Active Directory Domain Services (AD DS)
— Forest / domain design | Trust relationships
— OU structure & delegation | GPO design & inheritance
— AD replication topology | Sites & subnets
— SYSVOL & NETLOGON troubleshooting
— Tiered administration model (Tier 0/1/2)
— AD hardening (AdminSDHolder, Protected Users, LAPS)

Azure AD / Entra ID
— Hybrid identity (Azure AD Connect, Cloud Sync)
— Conditional Access | PIM | Identity Protection
— App registrations | Enterprise applications | SSO (SAML, OIDC)
— B2B / B2C | Tenant management
— License management | Dynamic groups

LDAP | Kerberos | NTLM | RADIUS / NPS
FreeIPA | JumpCloud | Okta Universal Directory
```

### Group Policy (Deep Dive)

```
GPO design — naming conventions, layering strategy, WMI filters
Security settings — password policy, audit policy, user rights
Software restriction / AppLocker / WDAC
Folder redirection | Drive mapping | Printer deployment
Administrative templates (ADMX/ADML) — custom & Microsoft
GPO preferences vs. policies | Item-level targeting
Loopback processing (merge vs. replace)
Starter GPOs | GPO backup & restore | GPO migration
Resultant Set of Policy (RSoP) | gpresult /H | GPMC reporting
Security filtering | Block inheritance | Enforced GPOs
Slow link detection | GPO caching
```

### DNS (Deep Dive)

```
Record types: A, AAAA, CNAME, MX, TXT, SRV, PTR, NS, SOA, CAA
Forward & reverse lookup zones | Zone delegation
Conditional forwarders | Stub zones
AD-integrated DNS | DNS scavenging & aging
Split-brain / split-horizon DNS
DNSSEC concepts | DNS over HTTPS (DoH) / DNS over TLS (DoT)
External DNS providers (Cloudflare, Route 53, Azure DNS, GoDaddy)
DNS troubleshooting (nslookup, dig, Resolve-DnsName)
DNS security — cache poisoning, DNS tunneling awareness
Internal vs. external namespace design
```

### DHCP (Deep Dive)

```
Scope design — subnets, exclusions, reservations
DHCP options (router, DNS, domain name, NTP, PXE/TFTP)
DHCP relay agents | IP Helper addresses
Failover — hot standby vs. load balance
Superscopes | Multicast scopes
Lease management | Conflict detection
DHCP database backup & restore | Audit logging
IPv6 DHCPv6 | SLAAC
Migration between DHCP servers
```

---

## 🟡 Programming & Scripting (IT Context)

### Core IT Scripting

```
PowerShell — AD management, M365 automation, server admin, DSC
Bash / Shell — Linux admin, cron jobs, log parsing, system health checks
Python — API integrations, data manipulation, automation frameworks
Batch / CMD — legacy Windows scripting, login scripts
VBScript — legacy (GPO logon scripts, SCCM) — declining but still exists
```

### Infrastructure as Code

```
Terraform (HCL) | Pulumi | CloudFormation (YAML/JSON)
ARM Templates | Bicep (Azure)
Ansible (YAML) | Puppet (Ruby DSL) | Chef (Ruby)
Docker (Dockerfile) | Kubernetes (YAML manifests, Helm charts)
Vagrant (Ruby) | Packer (HCL/JSON)
```

### Query Languages (IT Ops)

```
SQL — reporting, asset queries, CMDB queries
KQL (Kusto) — Azure Monitor, Log Analytics, Sentinel
SPL — Splunk log analysis
WMI Query Language (WQL) — SCCM, GPO WMI filters
LDAP queries — AD search filters
PowerShell pipeline — Where-Object, Select-Object, etc.
Regex — log parsing, pattern matching
```

---

## 🏅 IT Certifications

### Microsoft

```
Fundamentals: AZ-900 | SC-900 | MS-900 | AI-900
Associate: AZ-104 (Azure Admin) | AZ-204 (Developer)
         | AZ-500 (Security) | AZ-700 (Networking)
         | MS-102 (M365 Admin) | MD-102 (Endpoint Admin)
Expert: AZ-305 (Solutions Architect) | AZ-400 (DevOps)
Legacy (still valued): MCSA | MCSE
```

### CompTIA

```
Core: A+ | Network+ | Security+
Infrastructure: Server+ | Cloud+ | Linux+
Cybersecurity: CySA+ | PenTest+ | CASP+
Data/Analytics: Data+ | DataSys+
Project: Project+
```

### Cisco

```
CCNA (200-301) | CCNP Enterprise | CCNP Security
CCNP Data Center | CCNP Collaboration
DevNet Associate | DevNet Professional | CDE
CCIE (Enterprise, Security, Data Center, Collaboration)
```

### Cloud Vendor

```
AWS: Cloud Practitioner | SAA | SAP | SysOps | DevOps | Security Specialty
Azure: AZ-900 → AZ-104 → AZ-305 (architect track)
GCP: Cloud Digital Leader | Associate Cloud Engineer | Professional Cloud Architect
```

### Linux

```
CompTIA Linux+ | LPIC-1 | LPIC-2 | LPIC-3
RHCSA (Red Hat Certified System Administrator)
RHCE (Red Hat Certified Engineer)
LFCS | LFCE (Linux Foundation)
```

### ITSM & Governance

```
ITIL 4 Foundation | ITIL 4 Managing Professional
ITIL 4 Strategic Leader | ITIL 4 Practice Manager
HDI Desktop Support Technician | HDI Support Center Analyst
COBIT 2019 Foundation
```

### Virtualization & Storage

```
VMware: VCA | VCP-DCV | VCAP-DCV | VCDX
VCP-NV (Network Virtualization)
NetApp NCDA | Dell EMC (DECA, DECS)
Veeam VMCE | VMCA
```

### Project & Management

```
PMP | CAPM | PMI-ACP
Scrum Master (CSM, PSM I/II)
PRINCE2 Foundation / Practitioner
Lean Six Sigma (Yellow, Green, Black Belt)
```

---

## 📊 How to Display on GitHub

### Option 1: Badge Style (shields.io)

```markdown
![Windows Server](https://img.shields.io/badge/-Windows_Server-0078D6?style=flat&logo=windows&logoColor=white)
![Active Directory](https://img.shields.io/badge/-Active_Directory-0078D6?style=flat&logo=windows&logoColor=white)
![Azure](https://img.shields.io/badge/-Azure-0078D4?style=flat&logo=microsoftazure&logoColor=white)
![PowerShell](https://img.shields.io/badge/-PowerShell-5391FE?style=flat&logo=powershell&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat&logo=linux&logoColor=black)
![VMware](https://img.shields.io/badge/-VMware-607078?style=flat&logo=vmware&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Terraform](https://img.shields.io/badge/-Terraform-7B42BC?style=flat&logo=terraform&logoColor=white)
![Ansible](https://img.shields.io/badge/-Ansible-EE0000?style=flat&logo=ansible&logoColor=white)
![AWS](https://img.shields.io/badge/-AWS-232F3E?style=flat&logo=amazonaws&logoColor=white)
![Cisco](https://img.shields.io/badge/-Cisco-1BA0D7?style=flat&logo=cisco&logoColor=white)
![Splunk](https://img.shields.io/badge/-Splunk-000000?style=flat&logo=splunk&logoColor=white)
```

### Option 2: Grouped Table

```markdown
| Category | Skills |
|----------|--------|
| **Identity** | Active Directory, Azure AD / Entra ID, GPO, LDAP, Okta |
| **Infrastructure** | Windows Server, Linux (RHEL, Ubuntu), VMware, Hyper-V |
| **Cloud** | Azure (AZ-104), AWS, GCP, Terraform, ARM/Bicep |
| **Networking** | Cisco, Palo Alto, DNS, DHCP, VPN, VLAN, 802.1X |
| **Automation** | PowerShell, Bash, Python, Ansible, Docker, CI/CD |
| **Monitoring** | Splunk, Grafana, Zabbix, Azure Monitor, PRTG |
| **ITSM** | ITIL 4, ServiceNow, Jira, Change/Incident/Problem Mgmt |
| **Backup/DR** | Veeam, Azure Backup, DFS-R, 3-2-1 strategy, DR testing |
```

### Option 3: Minimalist List

```markdown
## Skills

**Identity:** Active Directory · Azure AD · GPO · LDAP · Kerberos · MFA · PAM
**Servers:** Windows Server · Linux (RHEL, Ubuntu) · VMware · Hyper-V · Proxmox
**Cloud:** Azure · AWS · Terraform · Docker · Kubernetes · CI/CD
**Networking:** Cisco · Palo Alto · DNS · DHCP · VPN · VLAN · Suricata
**Automation:** PowerShell · Bash · Python · Ansible · DSC · REST APIs
**ITSM:** ITIL 4 · ServiceNow · Change Mgmt · Incident Response · CMDB
**Certs:** AZ-104 · CCNA · Security+ · VCP-DCV · ITIL 4
```

---

## 🎯 Role-Specific Starter Packs

### Helpdesk / Desktop Support (Tier 1)

```
Windows 10/11 | macOS | Active Directory (password resets, account mgmt)
Microsoft 365 (Outlook, Teams, OneDrive) | Printer troubleshooting
RDP / Quick Assist / TeamViewer | ServiceNow / Jira
Hardware setup & imaging | Basic networking (IP, DNS, Wi-Fi)
Customer service | Ticket documentation | SLA awareness
```

### IT Support Specialist (Tier 2)

```
Active Directory (users, groups, GPO troubleshooting)
Microsoft 365 Admin (Exchange Online, Teams, Intune basics)
SCCM / Intune — deployment, patching | WSUS
PowerShell scripting (bulk operations, reporting)
Networking (VLAN, DHCP, DNS records, firewall rule requests)
Endpoint management | Software packaging | MDT/Autopilot
```

### Systems Administrator

```
Windows Server (AD DS, DNS, DHCP, GPO, DFS, NPS, WSUS)
Linux (RHEL/Ubuntu — systemd, SSH, firewalld, Apache/Nginx)
VMware vSphere / Hyper-V | Veeam | Storage (SAN/NAS)
Azure / AWS administration | Terraform | Ansible
PowerShell & Bash automation | Monitoring (Zabbix, PRTG, Grafana)
ITIL (Change, Incident, Problem) | Documentation & runbooks
```

### Network Administrator

```
Cisco IOS / NX-OS | Palo Alto PAN-OS | Fortinet FortiOS
Routing: OSPF, BGP, static | Switching: VLANs, STP, trunking
VPN (IPSec, SSL, WireGuard) | SD-WAN | MPLS
Wireless: Cisco Meraki, Aruba, Ubiquiti | 802.1X / RADIUS
Monitoring: SolarWinds, PRTG, Grafana | NetFlow / sFlow
Firewall policy management | Network segmentation | ACLs
```

### Cloud Engineer / Administrator

```
Azure: VMs, VNets, NSGs, Azure AD, Storage, Azure DevOps
AWS: EC2, S3, VPC, IAM, RDS, CloudFormation, CloudWatch
Terraform | Ansible | Docker | Kubernetes | Helm
CI/CD (GitHub Actions, Azure DevOps, Jenkins)
Identity: Azure AD, Conditional Access, SSO, PIM
Cost management | Tagging strategy | Landing zone design
Python | Bash | PowerShell | YAML | HCL
```

### IT Manager / Director

```
ITIL 4 | Budget planning & TCO/ROI | Vendor management
ServiceNow (ITSM, ITAM, CMDB) | SLA management
Team leadership | Hiring & mentoring | Performance reviews
Project management (PMP, Agile/Scrum) | Change Advisory Board
Architecture review | Technology roadmapping | Risk assessment
Compliance (CIS, SOC 2, HIPAA, PCI) | Audit coordination
Executive communication | Business continuity planning
```

---

## ✏️ Customization Tips

- **Specify scale:** "Active Directory (3 forests, 12,000 users, hybrid Azure AD)" > "Active Directory"
- **Show progression:** "Helpdesk Tier 1 → Tier 2 → Sysadmin → Cloud Engineer" tells a story
- **Include environment context:** "VMware vSphere 8.0 (40 hosts, 600+ VMs)" > "VMware"
- **Mention the hard stuff:** Migrations, disaster recovery tests, and large-scale rollouts stand out
- **Link to projects:** Automation scripts, monitoring dashboards, and IaC repos show real work
- **ITIL matters:** If you run change management or maintain a CMDB, say so — it signals maturity
- **Don't sleep on soft skills:** Documentation, vendor management, mentoring, and cross-team collaboration are differentiators at senior levels

---

*Template maintained by the community. Fork it, customize it, share it.*
*Last updated: March 2026*
