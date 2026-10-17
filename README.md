# Kaan Myumyun

Aspiring DevOps Engineer and Software Engineering student. I build systems end to end, from an empty AWS account up: Terraform, Kubernetes, CI/CD pipelines, and the scripts and tests that make them safe to run.

## About My Focus

- Completing the SoftUni DevOps and Cloud Programme (March–November 2026): Linux Sysadmin ✓, Azure Essentials ✓, Containerization and Infrastructure ✓, Kubernetes (in progress), CI/CD and Monitoring
- Pursuing a Bachelor's in Software Engineering at Trakia University (Expected 2027)
- Building real infrastructure, not tutorial projects: each one runs on a real cloud account and is torn down when idle

## Technical Arsenal

- **AWS:** EKS, EC2, ECR, RDS (PostgreSQL), VPC, ALB, ACM, IAM with GitHub OIDC, KMS, Secrets Manager, SSM, CloudWatch, SNS
- **DevOps & Infrastructure:** Terraform, Kubernetes (EKS, k3s), Helm, Ansible, Docker, Docker Compose, GitHub Actions, Nginx, Bash, Linux (daily use)
- **Security & Quality:** Trivy, Checkov, TFLint, ShellCheck, kubeconform, ansible-lint, Pod Security, NetworkPolicies
- **Observability:** CloudWatch alarms, Prometheus, Grafana, Grafana Loki, Promtail
- **Cloud & Hosting:** Azure VM, Cloudflare (DNS, Pages), Render
- **Backend:** C#, ASP.NET Core Web API, Entity Framework Core, REST APIs, JWT
- **Databases:** PostgreSQL (RDS, Neon), SQL Server, MySQL
- **Tools:** Git, Swagger / OpenAPI

## Certifications

- Linux System Administration — March 2026
- Azure Essentials — April 2026
- Containerization and Infrastructure — October 2026

## Featured Projects

### [Hospital Management System](https://github.com/KaanMyumyun/HospitalSystem) · [Infrastructure](https://github.com/KaanMyumyun/HospitalSystem-infrastructure)
ASP.NET Core + React/TypeScript hospital platform on Amazon EKS, with every AWS resource in Terraform. Live at [app.hospitalsyst.cc](https://app.hospitalsyst.cc) while the stack is up; always-on demo at [hospitalsystem.pages.dev](https://hospitalsystem.pages.dev/).
- **One command up, one down:** `tf.sh apply` builds the whole stack from an empty AWS account, DNS and data included; `teardown.sh` backs up the database, destroys everything and sweeps every region for leftovers
- **AWS:** EKS in a custom VPC, ALB + ACM for HTTPS, RDS PostgreSQL in private subnets, ECR, KMS encryption for Secrets, logs, images and the database
- **Locked down:** private Kubernetes API reached only through an SSM-managed ops instance; GitHub Actions deploys through OIDC with no stored AWS keys, and admission policies let it change container images and nothing else; restricted Pod Security, read-only root filesystems, NetworkPolicies, a Content-Security-Policy header
- **CI/CD:** tests → Docker build → Trivy scan (a fixable HIGH/CRITICAL blocks the push) → ECR → approval-gated deploy to EKS, with smoke tests and rollback
- **Tested:** about 160 regression tests run the real shell scripts and Ansible playbooks against fake `aws`, `kubectl` and `terraform`; CI runs TFLint, ansible-lint, kubeconform, ShellCheck, Checkov and Trivy
- **Built console-first:** set up by hand in the AWS console, imported with Terracognita, then rewritten into modular Terraform

Earlier versions of the same app: [EC2 + k3s with Traefik and cert-manager](https://github.com/KaanMyumyun/kubeIAchp), and [EC2 configured by Ansible with Prometheus, Grafana and Loki](https://github.com/KaanMyumyun/ansiblehospitalsystem).

### [URL Shortener](https://github.com/KaanMyumyun/UrlShortener)
- Deployed on Azure VM with Docker Compose and GitHub Actions CI/CD
- Free tier: Cloudflare Pages + Render + Neon
- Terraform provisioner for one-command AWS deployment

## Contact

- **Email:** kaan.myumyunn@gmail.com
- **GitHub:** [KaanMyumyun](https://github.com/KaanMyumyun)
- **LinkedIn:** [Kaan-Myumyun](https://linkedin.com/in/Kaan-Myumyun)
