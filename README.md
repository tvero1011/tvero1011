# Hi, I'm Rovert Pangan 👋

**AWS Certified Solutions Architect – Associate (SAA-C03)** • **HashiCorp Certified: Terraform Associate (004)**

**Cloud Engineer • DevOps & Cloud Automation**

I build cloud infrastructure and automation using **AWS, Azure, Terraform, Ansible, Python, Docker, Kubernetes and CI/CD**. My projects focus on Infrastructure as Code, secure access without stored keys, monitoring, and finding what breaks before users do.

Before moving into cloud, I spent 15+ years in business operations and team leadership, so I care about the same things in infrastructure that I did in operations: repeatable processes, clear ownership, and honest reporting of limits.

Every project below has an interview-style write-up of what works, what broke, and what I would change for production. All are learning and portfolio projects with sample data, not client systems.

---

## 🚀 Featured Projects

| Project | What it shows | Technologies |
| --- | --- | --- |
| ☁️ **[ShopFast Infrastructure](https://github.com/tvero1011/shopfast-terraform)** | 3-tier AWS stack in Terraform (7 modules): public ALB, ECS Fargate in private subnets across 2 AZs with CPU autoscaling, encrypted private RDS PostgreSQL, Secrets Manager, VPC endpoints instead of a NAT gateway, CloudWatch alarms, and remote state with native S3 locking. GitHub Actions deploys through OIDC (no stored keys). Deployed and tested on AWS, then destroyed to avoid charges. | Terraform • AWS • ECS • Docker • GitHub Actions |
| 🔐 **[Azure Lead-Intake API](https://github.com/tvero1011/azure-lead-intake-api)** | Serverless Python API on Azure Functions. Entra ID app-role authentication (401, 403, 422 handled separately), managed identity to Table Storage and Key Vault, storage shared keys disabled, secrets kept out of Terraform state. Terraform with Azure Policy and monitoring, deployed by GitHub Actions through OIDC behind a protected environment. 26 automated tests, CodeQL, Gitleaks. Tested live, then destroyed between sessions. | Azure • Terraform • Python • Entra ID • GitHub Actions |
| ☸️ **[Kubernetes Health Monitor](https://github.com/tvero1011/k8s-health-monitor)** | Flask service containerized with Docker (non-root, Gunicorn) and deployed to Kubernetes (kind) with a Helm chart, liveness and readiness probes, and a CPU autoscaler load-tested from 2 to 5 replicas. GitHub Actions builds a commit-SHA image and deploys to a temporary cluster. Prometheus and Grafana monitor it. | Kubernetes • Helm • Docker • Prometheus • Grafana |
| 🖼️ **[Serverless Image API](https://github.com/tvero1011/serverless-image-api)** | Image upload and gallery on AWS (S3, API Gateway, Lambda, DynamoDB), 32 resources in Terraform, with a separate least-privilege IAM role per function. I reviewed my own code, found and fixed a stored XSS bug and a file-validation gap, and proved both fixes on the live stack. | Terraform • AWS • Lambda • API Gateway |
| 🛡️ **[Ansible Server Hardening](https://github.com/tvero1011/ansible-server-hardening)** | Ansible role that hardens Ubuntu servers (SSH, UFW, Fail2ban, auditd, unattended upgrades), plus a compliance check that reads the effective SSH settings and a drift check that fails on a mismatch. Tested on local VMs, then run once on a temporary AWS environment built with Terraform and reached through a jump host. CI runs ansible-lint. | Ansible • Terraform • Linux • GitHub Actions |
| 🐍 **[DevOps Automation Toolkit](https://github.com/tvero1011/automation_toolkit)** | Python (boto3) monitoring toolkit: EC2 health, application log checks over SSH with a checkpoint, API health checks with retries, S3 security audit, one combined alert email, and JSON/CSV reports. 44 mocked tests, plus a real run against AWS in a Terraform test environment that found a bug the tests missed. Designed to run on Lambda and EventBridge. | Python • boto3 • pytest • Terraform • AWS |
| 🤖 **[Workflow Automation (n8n, Zapier, Make)](https://github.com/tvero1011/lead-to-crm-n8n)** | Seven workflows on three platforms, including an AI lead-to-CRM flow: secured webhook, input validation, HubSpot upsert with no duplicates, AI lead scoring and reply drafting using company documents (RAG), and human approval in Slack before any email is sent. Also invoice processing with OCR and AI extraction, and AI customer-message triage with Slack escalation. More: [Lead Enrichment and Scoring (Zapier)](https://github.com/tvero1011/lead-enrichment-intelligent-scoring). | n8n • OpenAI • HubSpot • Supabase • Slack • Zapier • Make.com |

---

## 🛠 Technical Skills

### Cloud
* AWS: VPC • ALB • VPC Endpoints • ECS / Fargate • ECR • RDS • DynamoDB • Lambda • API Gateway • EventBridge • S3 • EC2 • CloudWatch • SNS • IAM • Secrets Manager
* Azure: Functions • Entra ID (app roles, managed identity) • Key Vault • Table Storage • Azure Policy • RBAC • Application Insights

### Infrastructure as Code & Configuration
* Terraform (modules, remote state with native S3 locking)
* Ansible (roles, playbooks, Vault)

### DevOps & Automation
* GitHub Actions (CI/CD, OIDC, CodeQL, Gitleaks)
* Docker • Kubernetes (kind) • Helm
* Prometheus • Grafana
* n8n • Zapier • Make.com
* Linux (Ubuntu / WSL2)

### Programming
* Python (boto3, Flask, Pydantic, pytest)
* JavaScript / Node.js

### Version Control
* Git • GitHub

---

## 📜 Certifications

* ✅ AWS Certified Solutions Architect – Associate (SAA-C03) — [Verify on Credly](https://credly.com/badges/9868d43b-4956-4a8c-8ce8-6dacccd4f9b0)
* ✅ HashiCorp Certified: Terraform Associate (004) — [Verify on Credly](https://credly.com/badges/5b20f04f-97ec-4caa-888e-c9c536254019)

---

## 🌱 Currently Learning

* Python for cloud automation and DevOps tooling
* Microsoft Azure, going deeper after the Lead-Intake project
* Keeping secrets out of Terraform state (RDS-managed passwords)
* HTTPS, Multi-AZ databases, and tighter least-privilege networking for my AWS projects

---

## 🌐 Connect with Me

* 🌍 Portfolio: https://rovportfolio.vercel.app
* 💼 LinkedIn: https://www.linkedin.com/in/rovert-pangan-b720b13b
* 📧 Email: [rovert101179@gmail.com](mailto:rovert101179@gmail.com)

---

> *I enjoy building practical cloud infrastructure and automation solutions, and I say the limits of each project first.*
