# Kaan Myumyun

Software Engineering student specializing in DevOps, cloud infrastructure, and backend engineering. I build and automate production-grade systems — from CI/CD pipelines and containerized deployments to Kubernetes clusters and full observability stacks.

## About My Focus

- Completing the SoftUni DevOps and Cloud Programme (March–November 2026): Linux Sysadmin ✓, Azure Essentials ✓, Containerization (in progress), Kubernetes, CI/CD & Monitoring
- Pursuing a Bachelor's in Software Engineering at Trakia University (Expected 2027)
- Building real infrastructure, not just tutorial projects — everything is deployed and running

## Technical Arsenal

- **DevOps & Infrastructure:** Docker, Docker Compose, Kubernetes (k3s), Terraform, GitHub Actions CI/CD, Nginx, Bash scripting, Linux (daily use)
- **Cloud:** AWS EC2, Azure VM, Cloudflare Pages
- **Observability:** Prometheus, Grafana, Grafana Loki, Promtail
- **Backend:** C#, ASP.NET Core Web API, Entity Framework Core, REST APIs, JWT
- **Databases:** PostgreSQL (Neon serverless), SQL Server, MySQL
- **Tools:** Git, Swagger / OpenAPI

## Certifications

- Linux System Administration — March 2026
- Azure Essentials — April 2026

## Featured Projects

### [Hospital Management System](https://github.com/KaanMyumyun/HospitalSystem)
Full-stack hospital platform with a production-grade infrastructure stack:
- **Kubernetes (k3s):** 2 backend + 2 frontend replicas, self-healing pods, Traefik Ingress, automated SSL via cert-manager
- **IaC:** Full Terraform provisioner — one `terraform apply` spins up EC2, installs k3s, provisions the entire stack
- **CI/CD:** GitHub Actions — tests, builds Docker images, pushes to Docker Hub, deploys on merge to main
- **Observability:** Prometheus + Grafana (metrics, alerts) + Loki + Promtail (centralized logging) — dashboards auto-provisioned from GitHub
- **Multi-environment:** Free tier (Cloudflare Pages + Render + Neon) and self-hosted (AWS EC2 + Kubernetes)

### [URL Shortener](https://github.com/KaanMyumyun/UrlShortener)
- Deployed on Azure VM with Docker Compose and GitHub Actions CI/CD
- Free tier: Cloudflare Pages + Render + Neon
- Terraform provisioner for one-command AWS deployment

## Contact

- **Email:** kaan.myumyunn@gmail.com
- **GitHub:** [KaanMyumyun](https://github.com/KaanMyumyun)
- **LinkedIn:** [Kaan-Myumyun](https://linkedin.com/in/Kaan-Myumyun)
