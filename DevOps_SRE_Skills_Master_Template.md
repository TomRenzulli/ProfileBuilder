# ⚙️ DevOps / SRE / Platform Engineering Skills Master Template

> **Copy-paste reference for GitHub profiles, resumes, and portfolios.**
> Delete what doesn't apply. Add what's missing. Make it yours.

---

## How to Use This Template

1. **DevOps is broad** — Nobody uses all of this. Pick the sections that match your stack and focus.
2. **Tools change, principles don't** — CI/CD, IaC, observability, and automation are forever. The specific tools rotate.
3. **Show your stack** — Employers want to know if you're AWS + Terraform + GitHub Actions or GCP + Pulumi + Cloud Build. Be specific.
4. **Depth over breadth** — "Kubernetes (production clusters, Helm charts, custom operators, 200+ pods)" beats a list of 40 tools you touched once.

---

## 🔵 CI/CD & Build Systems

### CI/CD Platforms

```
GitHub Actions | GitLab CI/CD | Jenkins | CircleCI
Azure DevOps Pipelines | AWS CodePipeline / CodeBuild
Bitbucket Pipelines | TeamCity | Buildkite
Travis CI | Drone CI | Harness | Tekton
Argo Workflows | Concourse CI | Woodpecker CI
Spinnaker (deployment) | Flux (GitOps) | Argo CD (GitOps)
```

### Pipeline Design & Practices

```
Pipeline-as-code (YAML, Groovy, HCL, Jsonnet)
Multi-stage pipelines | Parallel execution | Matrix builds
Branch strategies (trunk-based, GitFlow, GitHub Flow)
Monorepo tooling (Nx, Turborepo, Bazel, Pants)
Artifact management (JFrog Artifactory, Nexus, GitHub Packages, AWS ECR)
Dependency caching | Build optimization | Incremental builds
Pipeline security (secret injection, OIDC tokens, least-privilege runners)
Self-hosted runners / agents | Ephemeral build environments
Deployment strategies: blue-green, canary, rolling, feature flags
Release management | Semantic versioning | Changelog automation
```

### Code Quality & Testing in Pipelines

```
Linting: ESLint, Pylint, Flake8, golangci-lint, ShellCheck, Hadolint
Formatting: Prettier, Black, gofmt, rustfmt
Unit test frameworks: pytest, Jest, Go test, JUnit, RSpec
Integration / E2E testing: Cypress, Playwright, Selenium, k6
Code coverage: Codecov, Coveralls, SonarQube coverage
SAST: Semgrep, SonarQube, CodeQL, Checkmarx, Snyk Code
DAST: OWASP ZAP, Burp Enterprise, Invicti, Nuclei
SCA: Snyk, Dependabot, Renovate, OWASP Dependency-Check
Secret scanning: Gitleaks, truffleHog, detect-secrets, git-secrets
License compliance: FOSSA, Licensee, Scancode
```

---

## 🟢 Containers & Orchestration

### Container Runtimes & Tooling

```
Docker (Dockerfile, multi-stage builds, docker-compose)
Podman | Buildah | Skopeo | containerd | CRI-O
Kaniko (daemonless builds) | BuildKit | Dive (image analysis)
Distroless images | Alpine-based images | Scratch images
Image signing (Cosign, Notary) | SBOM generation (Syft)
Container registries: Docker Hub, ECR, GCR/Artifact Registry, ACR, GHCR, Harbor
```

### Kubernetes

```
Core: Pods, Deployments, Services, ConfigMaps, Secrets, Namespaces
Workloads: StatefulSets, DaemonSets, Jobs, CronJobs, ReplicaSets
Networking: Ingress (Nginx, Traefik, Istio Gateway), NetworkPolicies
           | Service Mesh (Istio, Linkerd, Consul Connect)
           | CoreDNS | MetalLB | Cilium
Storage: PV, PVC, StorageClasses | CSI drivers | Rook-Ceph | Longhorn
Security: RBAC, PodSecurityAdmission, OPA/Gatekeeper, Kyverno
          | Sealed Secrets | External Secrets Operator | Vault integration
Scaling: HPA, VPA, KEDA, Cluster Autoscaler, Karpenter
Helm (charts, repositories, Helmfile) | Kustomize
Operators: Operator SDK, kubebuilder, custom CRDs
Debugging: kubectl, k9s, stern, kubectx/kubens, lens
Multi-cluster: Rancher, Fleet, Liqo, Admiralty
```

### Managed Kubernetes

```
Amazon EKS (Fargate, managed node groups, EKS Anywhere)
Azure AKS (virtual nodes, AGIC, Azure CNI)
Google GKE (Autopilot, Config Sync, Anthos)
DigitalOcean DOKS | Linode LKE | Vultr VKE
Red Hat OpenShift (OCP, OKD) | VMware Tanzu
k3s | k0s | MicroK8s | kind | minikube (dev/lab)
```

### Alternative Orchestration & Compute

```
Docker Swarm | Nomad (HashiCorp)
AWS ECS / Fargate | Azure Container Instances | Cloud Run (GCP)
AWS Lambda | Azure Functions | Google Cloud Functions
Knative (serverless on K8s) | OpenFaaS
Fly.io | Railway | Render
```

---

## 🟠 Infrastructure as Code (IaC)

### Provisioning

```
Terraform (HCL)
— Providers (AWS, Azure, GCP, Cloudflare, Datadog, PagerDuty, etc.)
— State management (remote backends: S3, Azure Blob, GCS, Terraform Cloud)
— Modules (registry, custom, versioned) | Workspaces
— Import | State manipulation (mv, rm, taint)
— Terragrunt (DRY patterns, multi-account)
— Sentinel / OPA (policy-as-code)

Pulumi (TypeScript, Python, Go, C#, YAML)
OpenTofu (open-source Terraform fork)
AWS CloudFormation | CDK (TypeScript, Python)
Azure ARM Templates | Bicep
Google Deployment Manager | Config Connector
Crossplane (Kubernetes-native IaC)
```

### Configuration Management

```
Ansible — playbooks, roles, collections, inventory, AWX/Tower
        | Ansible Vault | Dynamic inventory | Callback plugins
Chef — cookbooks, recipes, Chef Infra, Chef InSpec
Puppet — manifests, modules, Puppet Enterprise, Bolt
SaltStack — states, pillars, grains, Salt Cloud
cloud-init — user-data scripts, cloud-config YAML
```

### Image Building

```
Packer (HCL) — AMIs, Azure images, GCP images, Docker, Vagrant
Vagrant — dev environments, multi-VM labs, provider plugins
Docker (Dockerfile) — application container images
Buildpacks (Cloud Native) | Nixpacks
Golden image pipelines | Image hardening automation
```

---

## 🔴 Cloud Platforms (DevOps Focus)

### Amazon Web Services (AWS)

```
Compute: EC2, ECS, EKS, Lambda, Fargate, App Runner, Lightsail
Storage: S3, EBS, EFS, FSx | Glacier (archival)
Networking: VPC, ALB/NLB, Route 53, CloudFront, API Gateway
           | Transit Gateway, PrivateLink, Direct Connect
Database: RDS, Aurora, DynamoDB, ElastiCache, Redshift
Messaging: SQS, SNS, EventBridge, Kinesis, MSK (Kafka)
CI/CD: CodePipeline, CodeBuild, CodeDeploy, CodeArtifact
Security: IAM, KMS, Secrets Manager, Security Hub, GuardDuty
Monitoring: CloudWatch (Logs, Metrics, Alarms), X-Ray, CloudTrail
IaC: CloudFormation, CDK, SAM | Service Catalog
Organizations, Control Tower, SSO (Identity Center)
Cost: Cost Explorer, Budgets, Savings Plans, Reserved Instances
```

### Microsoft Azure

```
Compute: VMs, App Service, AKS, Functions, Container Apps
Storage: Blob, Files, Disk, Data Lake Storage
Networking: VNets, NSGs, Azure Firewall, Front Door, Application Gateway
           | ExpressRoute, Private Endpoints, Traffic Manager
Database: Azure SQL, Cosmos DB, Cache for Redis, PostgreSQL Flex
Messaging: Service Bus, Event Hubs, Event Grid
CI/CD: Azure DevOps (Repos, Pipelines, Boards, Artifacts)
Identity: Entra ID, Managed Identity, Conditional Access, PIM
Monitoring: Azure Monitor, Log Analytics (KQL), Application Insights
IaC: ARM, Bicep, Terraform AzureRM provider
Cost: Cost Management, Advisor, Reservations
```

### Google Cloud Platform (GCP)

```
Compute: Compute Engine, GKE, Cloud Run, Cloud Functions, App Engine
Storage: Cloud Storage, Persistent Disk, Filestore
Networking: VPC, Cloud Load Balancing, Cloud CDN, Cloud DNS
           | Cloud Interconnect, Cloud NAT, Cloud Armor
Database: Cloud SQL, Firestore, Spanner, Memorystore, BigQuery
Messaging: Pub/Sub, Eventarc, Cloud Tasks
CI/CD: Cloud Build, Artifact Registry, Cloud Deploy
Security: IAM, Secret Manager, Security Command Center
Monitoring: Cloud Monitoring, Cloud Logging, Cloud Trace, Error Reporting
IaC: Deployment Manager, Config Connector, Terraform Google provider
```

### Multi-Cloud & Edge

```
Multi-cloud strategy | Cloud-agnostic IaC (Terraform, Pulumi)
Cloudflare (CDN, Workers, R2, D1, Zero Trust Tunnel)
Fastly | Akamai | AWS CloudFront | Azure CDN
Edge compute: Cloudflare Workers, Lambda@Edge, Deno Deploy
Hybrid: Azure Arc, AWS Outposts, Google Anthos, EKS Anywhere
```

---

## 🟣 Observability & Monitoring

### Metrics

```
Prometheus — PromQL, exporters, recording rules, alerting rules
Grafana — dashboards, alerting, data sources, Grafana Cloud
Datadog — metrics, APM, dashboards, monitors, SLOs
New Relic — APM, Infrastructure, Logs, Synthetics
Victoria Metrics | Thanos | Cortex (long-term Prometheus storage)
StatsD | Telegraf | collectd
CloudWatch Metrics | Azure Monitor Metrics | GCP Cloud Monitoring
```

### Logging

```
ELK Stack (Elasticsearch, Logstash, Kibana) | OpenSearch
Fluentd | Fluent Bit | Vector (Datadog) | Filebeat
Loki + Grafana (LogQL) | Promtail
Datadog Logs | Splunk | Sumo Logic | Papertrail
CloudWatch Logs | Azure Log Analytics (KQL) | GCP Cloud Logging
Structured logging (JSON) | Log levels | Correlation IDs
Log aggregation patterns | Retention & rotation policies
```

### Tracing & APM

```
OpenTelemetry (OTel) — SDK, Collector, auto-instrumentation
Jaeger | Zipkin | Grafana Tempo
Datadog APM | New Relic APM | Dynatrace
AWS X-Ray | Azure Application Insights | GCP Cloud Trace
Distributed tracing | Trace context propagation | Span analysis
Service maps | Dependency visualization | Latency analysis
```

### Alerting & Incident Management

```
PagerDuty | Opsgenie (Atlassian) | VictorOps / Splunk On-Call
Grafana Alerting | Prometheus Alertmanager | Datadog Monitors
Incident.io | FireHydrant | Rootly | Blameless
Statuspage (Atlassian) | Cachet | Instatus
On-call rotation design | Escalation policies
Runbook automation | Alert fatigue reduction
Post-incident reviews / blameless postmortems
```

### Synthetic Monitoring & Testing

```
Grafana Synthetic Monitoring | Datadog Synthetics
Checkly | Uptime Robot | Better Uptime | Pingdom
k6 (load testing) | Locust | Gatling | Artillery
Chaos engineering: Chaos Monkey, Litmus, Gremlin, Chaos Mesh
Health checks | Canary deployments with automated rollback
```

---

## 🟤 Site Reliability Engineering (SRE)

### SRE Principles & Practices

```
SLIs, SLOs, SLA definition & tracking
Error budgets | Error budget policies | Burn rate alerts
Toil identification & reduction | Automation ROI
Capacity planning | Load testing | Performance modeling
Reliability reviews | Production readiness reviews (PRR)
Change management (graduated rollouts, feature flags)
Incident command (IC roles, communication, timelines)
Blameless postmortems | Action item tracking
On-call practices (rotation, handoff, escalation, compensation)
```

### Performance & Scalability

```
Horizontal vs. vertical scaling | Auto-scaling policies
Caching strategies: Redis, Memcached, Varnish, CDN caching
Database optimization: indexing, query optimization, connection pooling
           | Read replicas, sharding, partitioning
Load balancing: L4 vs. L7, health checks, session affinity
Rate limiting | Circuit breakers | Retry with backoff
Queue-based load leveling (SQS, RabbitMQ, Kafka)
Content delivery (CDN configuration, cache invalidation)
Profiling: pprof (Go), cProfile (Python), async-profiler (Java)
```

### Disaster Recovery & Business Continuity

```
RPO / RTO definition | DR tiers (active-active, active-passive, pilot light)
Multi-region / multi-AZ architecture | Failover automation
Backup strategies (snapshots, streaming replication, point-in-time recovery)
DR testing & game days | Chaos engineering
Runbook documentation | Communication plans
Data replication (cross-region, cross-cloud)
```

---

## ⚫ Platform Engineering

### Internal Developer Platforms (IDP)

```
Backstage (Spotify) — service catalog, templates, plugins, TechDocs
Port | Cortex | OpsLevel | Humanitec
Self-service infrastructure provisioning
Golden paths / paved roads | Platform APIs
Developer experience (DX) metrics | DORA metrics
```

### Developer Tooling & Workflows

```
Dev environments: Codespaces (GitHub), Gitpod, DevPod, Coder
Package registries: npm, PyPI, Maven Central, crates.io, Go modules
Internal package registries: Artifactory, Nexus, GitHub Packages, Verdaccio
Documentation: Backstage TechDocs, Confluence, Notion, MkDocs, Docusaurus
API management: Kong, Apigee, AWS API Gateway, Tyk
Service templates | Scaffolding (cookiecutter, Yeoman, Backstage templates)
Feature flags: LaunchDarkly, Unleash, Flagsmith, Split.io, ConfigCat
```

### GitOps

```
Argo CD — Application, ApplicationSet, multi-cluster sync
Flux v2 — GitRepository, Kustomization, HelmRelease
Git as single source of truth | Declarative infrastructure
Drift detection & reconciliation | Automated sync
PR-based deployment workflows | Environment promotion
Image automation (Flux Image Reflector, Argo CD Image Updater)
```

---

## 🟡 Networking & Service Mesh (DevOps Context)

### Service Mesh

```
Istio — VirtualService, DestinationRule, Gateway, mTLS, traffic splitting
Linkerd — lightweight mesh, mTLS, traffic split, multicluster
Consul Connect (HashiCorp) — service discovery, intentions, mesh gateway
Cilium Service Mesh (eBPF-based) | Kuma | Open Service Mesh
Traffic management: canary, A/B, mirroring, fault injection, timeouts
Observability: distributed tracing, access logs, service-level metrics
```

### DNS & Traffic Management

```
External DNS (Kubernetes → Route 53 / CloudFlare / Azure DNS)
cert-manager (Let's Encrypt, Venafi, Vault PKI)
Ingress controllers: Nginx, Traefik, HAProxy, Envoy, Contour
API Gateways: Kong, Ambassador/Emissary, APISIX, AWS API GW
Global load balancing | Geo-DNS | Failover routing
CDN configuration | TLS/SSL management | HSTS
```

### Secrets & Configuration Management

```
HashiCorp Vault — secrets engines, auth methods, dynamic secrets, PKI
                | Vault Agent, CSI provider, Kubernetes integration
AWS Secrets Manager | AWS SSM Parameter Store
Azure Key Vault | GCP Secret Manager
Sealed Secrets (Bitnami) | External Secrets Operator | SOPS
Mozilla SOPS | age encryption | GPG
Environment variable management | .env patterns | 12-factor config
```

---

## 🔧 Programming & Scripting (DevOps Context)

### Core DevOps Languages

```
Python — automation, scripting, Lambda/Cloud Functions, CLI tools, Boto3
Bash / Shell — glue scripts, CI/CD steps, Linux automation, cron
Go — CLI tools, Kubernetes operators, cloud-native tooling, performance
JavaScript / TypeScript — CDK, Pulumi, serverless, tooling scripts
```

### Infrastructure & Config Languages

```
HCL (Terraform, Packer, Nomad, Vault, Consul)
YAML (Kubernetes manifests, Ansible, CI/CD pipelines, Helm, Docker Compose)
JSON / JSONNET (config, CloudFormation, Grafana dashboards)
Bicep (Azure) | Cue | Dhall | Starlark (Bazel)
Jinja2 (Ansible templating) | Go templates (Helm, Hugo)
```

### Query & Domain-Specific Languages

```
PromQL — Prometheus queries, recording rules, alert expressions
LogQL — Loki log queries | Lucene — Elasticsearch/OpenSearch
KQL (Kusto) — Azure Log Analytics, Sentinel
SQL — database ops, migrations, reporting
Rego — OPA/Gatekeeper policy language
CEL — Kubernetes admission, Envoy routing
Regex — log parsing, validation, pattern matching
jq / yq — JSON/YAML processing in pipelines
```

---

## 📦 Source Control & Collaboration

### Git & Platforms

```
Git — branching, merging, rebasing, cherry-pick, bisect, hooks
GitHub — Actions, Packages, Pages, Codespaces, Dependabot, CODEOWNERS
GitLab — CI/CD, Container Registry, Package Registry, GitLab Pages
Bitbucket — Pipelines, mirrors
Azure Repos | AWS CodeCommit (legacy)
```

### Branching & Release Strategies

```
Trunk-based development | GitHub Flow | GitFlow
Conventional Commits | Semantic Release | Changesets
Monorepo management: Nx, Turborepo, Lerna, Bazel, Pants
Git submodules | Git subtree | Sparse checkout
Protected branches | Merge rules | Code review workflows
Signed commits (GPG, SSH) | Commit verification
```

---

## 🛡️ DevSecOps & Supply Chain Security

### Shift-Left Security

```
SAST: Semgrep, CodeQL, SonarQube, Checkmarx, Fortify, Snyk Code
DAST: OWASP ZAP, Burp Enterprise, Invicti, Nuclei
SCA: Snyk, Dependabot, Renovate, Grype, OWASP Dependency-Check
Container scanning: Trivy, Grype, Docker Scout, Anchore, Aqua
IaC scanning: Checkov, tfsec, KICS, Terrascan, Bridgecrew
Secret detection: Gitleaks, truffleHog, detect-secrets, git-secrets
License scanning: FOSSA, Scancode, Licensee
Policy-as-code: OPA/Rego, Sentinel (HashiCorp), Kyverno, Datree
```

### Software Supply Chain

```
SBOM generation: Syft, CycloneDX, SPDX
Image signing: Cosign (Sigstore), Notary v2
Provenance: SLSA framework, in-toto attestations
Artifact verification: Sigstore Rekor (transparency log)
Dependency pinning | Lock files | Reproducible builds
Trusted registries | Admission controllers (image policies)
VEX (Vulnerability Exploitability eXchange) | OpenVEX
```

### Runtime Security

```
Falco — runtime threat detection (Kubernetes, Linux)
Sysdig | Aqua Runtime | NeuVector
eBPF-based security (Cilium Tetragon, Falco with eBPF)
Pod Security Admission | Seccomp profiles | AppArmor / SELinux
Network policies | mTLS enforcement
Runtime vulnerability scanning | Image admission policies
```

---

## 🗄️ Databases & Data (DevOps Context)

### Database Operations

```
Schema migrations: Flyway, Liquibase, Alembic, golang-migrate, Atlas
Database provisioning & IaC (Terraform, CloudFormation)
Backup automation | Point-in-time recovery | Snapshot management
Replication: primary-replica, multi-primary, streaming
Connection pooling: PgBouncer, ProxySQL, RDS Proxy
Performance: slow query analysis, indexing, EXPLAIN plans
Database-as-a-Service: RDS, Aurora, Cloud SQL, Azure SQL, PlanetScale
```

### Data Stores (Common in DevOps)

```
PostgreSQL | MySQL / MariaDB | SQL Server
Redis | Memcached | Valkey
MongoDB | DynamoDB | Cassandra | ScyllaDB
Elasticsearch / OpenSearch | ClickHouse | TimescaleDB
Kafka | RabbitMQ | NATS | Amazon SQS/SNS
etcd | Consul KV | ZooKeeper
MinIO (S3-compatible) | Ceph
```

---

## 🏅 DevOps / SRE / Cloud Certifications

### AWS

```
Cloud Practitioner (CLF-C02)
Solutions Architect Associate (SAA-C03) | Professional (SAP-C02)
SysOps Administrator Associate (SOA-C02)
Developer Associate (DVA-C02)
DevOps Engineer Professional (DOP-C02)
Security Specialty | Advanced Networking Specialty
```

### Azure

```
AZ-900 (Fundamentals) | AZ-104 (Administrator)
AZ-204 (Developer) | AZ-400 (DevOps Engineer Expert)
AZ-305 (Solutions Architect) | AZ-500 (Security)
AZ-700 (Network Engineer) | AZ-140 (Virtual Desktop)
```

### Google Cloud

```
Cloud Digital Leader | Associate Cloud Engineer
Professional Cloud Architect | Professional Cloud DevOps Engineer
Professional Cloud Developer | Professional Cloud Network Engineer
Professional Cloud Security Engineer
```

### Kubernetes & Cloud Native

```
CKA (Certified Kubernetes Administrator)
CKAD (Certified Kubernetes Application Developer)
CKS (Certified Kubernetes Security Specialist)
KCNA (Kubernetes and Cloud Native Associate)
KCSA (Kubernetes and Cloud Native Security Associate)
Prometheus Certified Associate (PCA)
Istio Certified Associate (ICA)
```

### HashiCorp

```
Terraform Associate (003) | Terraform Authoring and Operations Professional
Vault Associate (003) | Vault Operations Professional
Consul Associate (003)
```

### Linux & Foundational

```
LFCS (Linux Foundation Certified Sysadmin)
LFCE (Linux Foundation Certified Engineer)
RHCSA | RHCE | CompTIA Linux+
CompTIA Cloud+ | CompTIA Server+
```

### SRE & Reliability

```
Google Professional Cloud DevOps Engineer (SRE-aligned)
SRE Foundation (DevOps Institute)
Chaos Engineering Practitioner (Gremlin)
```

---

## 📊 How to Display on GitHub

### Option 1: Badge Style (shields.io)

```markdown
![Kubernetes](https://img.shields.io/badge/-Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Terraform](https://img.shields.io/badge/-Terraform-7B42BC?style=flat&logo=terraform&logoColor=white)
![AWS](https://img.shields.io/badge/-AWS-232F3E?style=flat&logo=amazonaws&logoColor=white)
![Azure](https://img.shields.io/badge/-Azure-0078D4?style=flat&logo=microsoftazure&logoColor=white)
![GCP](https://img.shields.io/badge/-GCP-4285F4?style=flat&logo=googlecloud&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![ArgoCD](https://img.shields.io/badge/-Argo_CD-EF7B4D?style=flat&logo=argo&logoColor=white)
![Prometheus](https://img.shields.io/badge/-Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/-Grafana-F46800?style=flat&logo=grafana&logoColor=white)
![Ansible](https://img.shields.io/badge/-Ansible-EE0000?style=flat&logo=ansible&logoColor=white)
![Helm](https://img.shields.io/badge/-Helm-0F1689?style=flat&logo=helm&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/-Go-00ADD8?style=flat&logo=go&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Vault](https://img.shields.io/badge/-Vault-FFEC6E?style=flat&logo=vault&logoColor=black)
```

### Option 2: Grouped Table

```markdown
| Category | Skills |
|----------|--------|
| **Cloud** | AWS, Azure, GCP, Cloudflare, Multi-cloud |
| **Containers** | Docker, Kubernetes (EKS/AKS/GKE), Helm, Kustomize |
| **IaC** | Terraform, Pulumi, Ansible, Packer, CloudFormation, Bicep |
| **CI/CD** | GitHub Actions, GitLab CI, Argo CD, Flux, Jenkins |
| **Observability** | Prometheus, Grafana, Datadog, ELK, OpenTelemetry, PagerDuty |
| **Languages** | Python, Bash, Go, TypeScript, HCL, YAML, PromQL |
| **Security** | Vault, Trivy, Falco, OPA, Cosign, SBOM, SLSA |
| **Databases** | PostgreSQL, Redis, DynamoDB, Kafka, Elasticsearch |
| **Certs** | CKA, AWS SAP, Terraform Associate, AZ-400 |
```

### Option 3: Minimalist List

```markdown
## Skills

**Cloud:** AWS · Azure · GCP · Cloudflare · Multi-region architecture
**Containers:** Docker · Kubernetes · Helm · Istio · containerd · Harbor
**IaC:** Terraform · Ansible · Pulumi · Packer · CDK · Crossplane
**CI/CD:** GitHub Actions · GitLab CI · Argo CD · Flux · Spinnaker
**Observability:** Prometheus · Grafana · Datadog · OTel · Loki · PagerDuty
**Security:** Vault · Trivy · Falco · OPA · Cosign · Gitleaks · Checkov
**Languages:** Python · Go · Bash · TypeScript · HCL · PromQL · SQL
**Certs:** CKA · CKS · AWS DevOps Pro · Terraform Associate · AZ-400
```

---

## 🎯 Role-Specific Starter Packs

### Junior DevOps / Build Engineer

```
Linux administration (Ubuntu/RHEL) | Bash scripting
Git & GitHub/GitLab | CI/CD basics (GitHub Actions or GitLab CI)
Docker (Dockerfile, docker-compose) | Basic Kubernetes (kubectl, pods, services)
Terraform basics (single provider, simple resources)
Python scripting | YAML fluency
AWS or Azure fundamentals | Networking basics (DNS, HTTP, TLS)
Monitoring basics (Prometheus, Grafana, or CloudWatch)
```

### Mid-Level DevOps Engineer

```
Kubernetes (production, Helm, HPA, RBAC, troubleshooting)
Terraform (modules, remote state, multi-environment, Terragrunt)
CI/CD pipeline design (multi-stage, secrets, caching, matrix)
Ansible (playbooks, roles, dynamic inventory)
AWS or Azure (core services, IAM, networking, cost management)
Observability stack (Prometheus + Grafana + Loki or Datadog)
Docker (multi-stage builds, security, registries)
Python + Bash + basic Go | GitOps (Argo CD or Flux)
Incident response | On-call participation | Runbook writing
```

### Senior DevOps / Infrastructure Engineer

```
Multi-cloud or deep single-cloud expertise
Kubernetes at scale (custom operators, service mesh, multi-cluster)
Terraform at scale (custom providers, Sentinel/OPA, state surgery)
Platform engineering (Backstage, golden paths, self-service)
GitOps (Argo CD + ApplicationSets, Flux, environment promotion)
Observability design (SLI/SLO, custom metrics, distributed tracing)
DevSecOps (supply chain security, SBOM, image signing, policy-as-code)
Chaos engineering | DR testing | Capacity planning
Architecture decisions | RFC/ADR writing | Mentoring
Cost optimization | FinOps practices
```

### Site Reliability Engineer (SRE)

```
SLI/SLO/SLA definition & management | Error budgets
Prometheus + Grafana + Alertmanager | OpenTelemetry
Incident command | Blameless postmortems | Runbook automation
Capacity planning | Load testing (k6, Locust, Gatling)
Chaos engineering (Litmus, Gremlin, Chaos Mesh)
Linux internals | Networking deep dive | Performance profiling
Go or Python | Bash | PromQL | SQL
Kubernetes operations | Terraform | Cloud platform expertise
On-call design | Toil reduction | Automation-first mindset
```

### Platform Engineer

```
Backstage / Port / Cortex — internal developer platform
Self-service infrastructure (Terraform modules, Crossplane)
Golden paths & templates (scaffolding, starter kits)
GitOps (Argo CD, Flux) | CI/CD standardization
Developer experience (DX) metrics | DORA metrics
Kubernetes (multi-tenant, namespaces, quotas, RBAC)
API management | Service catalog | TechDocs
Secrets management (Vault, External Secrets Operator)
Cost allocation | Showback/chargeback | FinOps
Go or Python | Internal CLI tooling | SDK development
```

### Cloud Architect (DevOps Background)

```
Multi-cloud architecture | Landing zone design | Well-Architected Framework
Network architecture (hub-spoke, transit gateway, peering, hybrid)
Identity architecture (federation, SSO, cross-account, zero trust)
Cost optimization | Reserved capacity | FinOps strategy
DR/BC architecture (multi-region, RPO/RTO, failover automation)
Security architecture (encryption, key management, compliance)
Migration strategy (6 Rs) | Modernization patterns
Terraform at enterprise scale | Policy-as-code
Executive communication | Architecture decision records (ADRs)
Vendor evaluation | Build vs. buy analysis
```

---

## ✏️ Customization Tips

- **Name your stack:** "AWS + Terraform + GitHub Actions + Argo CD + Prometheus" is a signal, not a list
- **Quantify scale:** "Kubernetes (15 clusters, 3,000 pods, 99.95% uptime SLO)" > "Kubernetes"
- **Show pipeline maturity:** "CI/CD (< 10 min build-to-deploy, automated rollback, canary deploys)" > "CI/CD"
- **Link your repos:** IaC modules, Helm charts, GitHub Actions, CLI tools — working code > bullet points
- **Mention the hard wins:** Zero-downtime migrations, cost reduction percentages, MTTR improvements, toil reduction metrics
- **Include DORA metrics if you track them:** Deployment frequency, lead time, change failure rate, MTTR
- **Don't list what you can't whiteboard:** If someone asked you to diagram it, could you? That's your real skill list

---

*Template maintained by the community. Fork it, customize it, share it.*
*Last updated: March 2026*
