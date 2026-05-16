# Ahmad Asmar

**Staff DevOps / Platform Lead** · Open to opportunities

**6+ years scaling cloud-native infrastructure across AWS, GCP, and Azure.** The last three of those owning a SaaS-scale AWS-native platform: 20 EKS clusters across 4 regions, 25+ microservices, 20+ government customers — built from a hybrid Azure+AWS estate, with the first 18 months as the **sole DevOps engineer**. Open-source maintainer of a Terraform Registry module powering self-service GitLab runner fleets (3,767 downloads) and a 158★ Claude Code skills marketplace.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-ahmadasmar-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ahmadasmar)
[![Medium](https://img.shields.io/badge/Medium-@ahmed.asmar-12100E?logo=medium&logoColor=white)](https://medium.com/@ahmed.asmar)
[![Portfolio](https://img.shields.io/badge/Portfolio-ahmedasmar.github.io-24292e?logo=github&logoColor=white)](https://ahmedasmar.github.io)
[![CKA](https://img.shields.io/badge/CNCF-Certified%20Kubernetes%20Administrator-326CE5?logo=kubernetes&logoColor=white)](https://www.cncf.io/training/certification/cka/)

---

## 🌟 Featured open source

| Project | Highlight |
|---|---|
| [**terraform-aws-gitlab-docker-autoscaler-runner**](https://github.com/ahmedasmar/terraform-aws-gitlab-docker-autoscaler-runner) | **3,767 downloads** on the Terraform Registry. Scale-to-zero GitLab runner platform on AWS Fleeting + 100% spot + attribute-based instance selection. 2 years of maintenance · v0.6.8. |
| [**devops-claude-skills**](https://github.com/ahmedasmar/devops-claude-skills) | **158 ★ · 32 forks**. A Claude Code Skills marketplace for DevOps workflows — onboarding ArgoCD clusters, migrating Helm charts to GitOps, AWS SSO auth recovery, and more. |
| [**godaddy-webhook**](https://github.com/ahmedasmar/godaddy-webhook) | Cert-manager DNS-01 webhook for GoDaddy (Go). ACME automation for domains that don't fit the standard providers. |
| [**terraform-aws-sftp**](https://github.com/ahmedasmar/terraform-aws-sftp) | AWS Transfer Family SFTP module on top of S3. |
| [**platform-engineering-project**](https://github.com/ahmedasmar/platform-engineering-project) | kagent AI agents + MCP servers (Datadog) + Ollama on k8s — a working sandbox for AI-on-platform patterns. |

---

## ✍️ Published writing

- **["Automating Pod Disruption Budgets with Kyverno"](https://medium.com/zencity-engineering/automating-pod-disruption-budgets-with-kyverno-0a6bee7bbcca)** — *Zencity Engineering*, Dec 2, 2025. How Zencity auto-generated PDBs for every microservice missing one, preventing service downtime when Karpenter consolidates nodes.
- **["Building a Local Dev Platform with Kubernetes, Tilt, and local GitLab pipelines"](https://medium.com/@ahmed.asmar/building-a-local-dev-platform-with-kubernetes-tilt-and-local-gitlab-pipelines-ab534d428c82)** — *Medium*, Apr 9, 2026. A local dev platform mirroring prod via k3d + Traefik + Kustomize + Tilt + GitLab CI.

More at [`@ahmed.asmar` on Medium](https://medium.com/@ahmed.asmar).

---

## 💼 Career

| When | Role | Where |
|---|---|---|
| **May 2023 – present** · 3 yr | Senior DevOps Engineer | **Zencity** (via [ASAL Technologies](https://www.asaltech.com/)) — full platform ownership |
| **Jun 2021 – May 2023** · 2 yr | DevOps Engineer L2 | **Freightos** — GCP, Kubernetes, ArgoCD, CI/CD |
| **Jul 2020 – Jul 2021** · 1 yr | DevOps Engineer | **PDF Solutions** — cloud IaC, configuration management |
| **May 2019 – Jul 2020** | IT Support Technician | **Partners for Sustainable Development** |
| **Dec 2017 – Dec 2018** | IT Support Technician | **Palestine Telecommunications (Paltel) Group** |

---

## What I do

- **Multi-account AWS at scale** — 20 SSO-managed accounts, 4 regions (us-east-1, eu-west-1, ca-central-1, eu-west-2), 20 EKS clusters, 25+ microservices.
- **GitOps platform owner** — 3-month epic standing up dedicated ArgoCD devops clusters on shared-staging-devops + shared-prod-devops. Authored ~70% of the `zc-gitops` repo. ApplicationSet pattern for multi-cluster fan-out. Cluster onboarding via cross-account IAM (Pod Identity + AssumeRole) — no bearer tokens.
- **Service mesh + Gateway API migration** — designed the 12-phase rollout plan for Istio Ambient (sidecar-less). Shipped Phases 0/1/2.0/2.1/2.2 to all 6 staging clusters in a 2-week sprint (125 commits across 8 repos). Validated the cross-account `TargetGroupBinding` pattern that removes the NLB hop between ALB and pods.
- **EKS fleet operations** — 6 major Kubernetes upgrades over 3 years (1.22 → 1.34). Last upgrade across ~10 production clusters in **2 working days**. Fleet-wide migrations to Bottlerocket, Kyverno, VPA, and Pod Identity — zero rollbacks.
- **Modern Terraform CI/CD** — replaced "push-to-staging-and-hope" with validate → Checkov → plan-in-MR → Infracost → auto-apply. **37% faster pipelines (8:52 → 5:36)** fleet-wide.
- **Open-source maintainer** — Terraform Registry module powering Zencity's runner fleet (also adopted beyond it), and a Claude Code skills marketplace people actually star and fork.

---

## Tech stack

| Layer | Tools |
|---|---|
| **Cloud** | AWS (multi-account, multi-region) · GCP (integration) · IAM Identity Center · Transit Gateway · Route 53 · CloudFront · Bedrock |
| **Kubernetes** | EKS 1.34 · Karpenter 1.12 · Bottlerocket 1.59 · Pod Identity · AWS LBC v3 · VPA · Kyverno · Istio Ambient · Gateway API · cert-manager · external-secrets · external-dns |
| **GitOps / Helm** | ArgoCD (ApplicationSets, Server-Side Diff, Pod Identity cluster onboard) · Helm · Crossplane v2 (Upbound) · monochart |
| **IaC** | Terraform · Terragrunt · Checkov · Infracost · `tfmv` |
| **CI/CD** | GitLab CI (Premium) · `services-release` unified template · self-hosted EC2 spot runners · ARM64 · GitHub Actions |
| **Observability** | Datadog (APM, Logs, Synthetics, Operator) · CloudWatch · Zenduty |
| **Security** | SCPs · WAF · KMS · External Secrets · SOC 2 auditee · ISO 27001 lead responder · SAST / SCA / gitleaks / Trivy in CI |
| **Languages** | Bash · HCL · YAML · Python · Go (read) · GraphQL |

---

## Certifications

- **CKA — Certified Kubernetes Administrator** (CNCF)

---

## Contact

- **LinkedIn:** [linkedin.com/in/ahmadasmar](https://www.linkedin.com/in/ahmadasmar)
- **Portfolio:** [ahmedasmar.github.io](https://ahmedasmar.github.io) — projects, writing, full tech stack
- **Medium:** [`@ahmed.asmar`](https://medium.com/@ahmed.asmar)
- **GitHub:** here · Commonplace contributions live at [`ahmad-asmar`](https://github.com/ahmad-asmar)

> Open to Staff / Senior DevOps · Platform Engineering · SRE roles. Remote-friendly · GMT+3.
