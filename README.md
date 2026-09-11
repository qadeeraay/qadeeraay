# Hi, I'm Qadeer Aslam 👋

### DevOps & Cloud Platform Engineer | SRE & DevSecOps

I design and operate reliable, secure, and cost-efficient cloud platforms. My background spans **production Kubernetes, GitOps delivery pipelines, zero-trust secrets management, and automated platform reliability**. Beyond infrastructure automation, I write custom Kubernetes controllers and backend services in Python, treating platform operations with software engineering discipline.

* 📍 **Location:** Karachi, Pakistan
* 💼 **Current:** DevOps / Cloud Engineer & COO at **HashX** | Previously DevOps Engineer at **Al-Nafi**
* 🎓 **Education:** BS in Information Technology — The University of Faisalabad
* 📬 **Contact:** [qadeeraslam888@gmail.com](mailto:qadeeraslam888@gmail.com) | [LinkedIn](https://linkedin.com/in/qadeer-aslam-devops)
* 📄 **Resume:** [![Download Resume](https://img.shields.io/badge/Resume-Download_DevOps_PDF-007ACC?style=flat-square&logo=adobeacrobatreader&logoColor=white)](./Qadeer_Aslam_DevOps_Resume.pdf)

---

## 🛠️ Technical Focus

* **Cloud & Orchestration:** AWS (EKS, VPC, IAM, KMS, S3, CloudWatch), Kubernetes (Custom Controllers, Operators, RBAC, NetworkPolicies), Docker
* **IaC & GitOps Delivery:** Terraform, Ansible, Helm 3, ArgoCD, Argo Rollouts, GitHub Actions CI/CD
* **Reliability & Observability:** Prometheus, Grafana, Loki, Alertmanager, Google SRE 4 Golden Signals, Multi-Window SLO Burn-Rate Alerting
* **Security & Governance:** HashiCorp Vault, External Secrets Operator (ESO), Kyverno Policy Engine, Checkov, Trivy, CIS Benchmarks Hardening
* **Languages & Systems:** Python 3.12 (AsyncIO, K8s Informers), Bash/Shell, PostgreSQL, Redis

---

## 🚀 Featured Platform Projects (Top 6)

The following six projects highlight my work across cloud infrastructure, progressive delivery, platform automation, and production reliability:

### 1. [enterprise-gitops-argocd-pipeline](https://github.com/qadeeraay/enterprise-gitops-argocd-pipeline)
**Domain:** GitOps Delivery & Progressive Rollouts  
**Stack:** ArgoCD, Helm 3, Argo Rollouts, Kyverno, Prometheus  
* Declarative App-of-Apps delivery platform managing multi-environment Kubernetes deployments from a single source of truth.
* Metric-driven Canary deployments that analyze Prometheus error rates and P99 latencies, automatically rolling back failed releases in **< 1.8s**.
* Cluster-wide Kyverno admission policies enforcing zero-trust pod security (non-root execution, dropped capabilities, read-only root filesystems).

### 2. [production-observability-golden-signals](https://github.com/qadeeraay/production-observability-golden-signals)
**Domain:** Site Reliability Engineering (SRE) & Observability  
**Stack:** Prometheus, Grafana, Loki, Alertmanager, Docker Compose  
* Production monitoring stack implementing the Google SRE 4 Golden Signals: Latency, Traffic, Errors, and Saturation.
* Configured with **multi-window, multi-burn-rate SLO alerting** (14.4x / 1-hour and 6-hour burn rates), eliminating transient alert noise while catching rapid error budget depletion.
* Pre-configured Grafana dashboards with correlated Loki log queries for instant incident triage.

### 3. [k8s-aiops-self-healing-operator](https://github.com/qadeeraay/k8s-aiops-self-healing-operator)
**Domain:** Kubernetes Platform Automation & Controllers  
**Stack:** Python 3.12, Kubernetes Client / Informers, Prometheus Metrics  
* Autonomous Kubernetes controller running an event-driven reconciliation loop to detect and resolve pod failure states in real time.
* Mitigates `CrashLoopBackOff`, memory pressure, and zombie pods autonomously, reducing mean time to recovery (MTTR) from 25+ minutes to **under 5 seconds**.
* Emits custom Prometheus metrics tracking remediation velocity and cluster self-healing success rates.

### 4. [secure-aws-k8s-compliance-engine](https://github.com/qadeeraay/secure-aws-k8s-compliance-engine)
**Domain:** Cloud Infrastructure as Code & DevSecOps  
**Stack:** Terraform, AWS (VPC, EKS, KMS, S3), Checkov, Trivy  
* Production-grade Terraform modules provisioning secure AWS cloud topology with isolated subnets, KMS customer-managed encryption keys, and strict IAM boundaries.
* Zero-trust Kubernetes NetworkPolicies with default-deny ingress/egress.
* Automated CI pipeline verifying **100% compliance across 213 policy-as-code controls** with zero security alerts.

### 5. [enterprise-ansible-vault-secrets](https://github.com/qadeeraay/enterprise-ansible-vault-secrets)
**Domain:** Secrets Lifecycle Management & OS Hardening  
**Stack:** Ansible, HashiCorp Vault, External Secrets Operator (ESO), PostgreSQL  
* Solves the "secret-zero" dilemma by integrating HashiCorp Vault with Kubernetes via ESO and ServiceAccount tokens.
* Provisions short-lived, dynamic database credentials with automated 1-hour TTL lease expirations and revocation.
* Automated Ansible playbooks enforcing **15 CIS Level 2 Linux benchmark controls** (SSH hardening, auditd rules, file permissions).

### 6. [serverless-cost-pipeline](https://github.com/qadeeraay/serverless-cost-pipeline)
**Domain:** FinOps & Event-Driven Serverless Infrastructure  
**Stack:** OpenFaaS, NATS JetStream, MinIO S3, Velero, Kubernetes  
* Event-driven processing pipeline that scales functions from 0 to 5 replicas based on traffic bursts, cutting idle compute costs by **99.8%**.
* In-memory image processing within a 32MB tmpfs boundary, reducing egress bandwidth consumption by 59%.
* Automated disaster recovery workflows with Velero backing up state and MinIO object storage.

---

## ⚡ Systems & Backend Engineering

When I'm not writing Terraform or tuning alert thresholds, I build high-performance backend systems in Python:
* **[distributed-rate-limiter](https://github.com/qadeeraay/distributed-rate-limiter)** — Atomic Token Bucket & Sliding Window rate limiter built with Redis Lua scripting, RFC 6585 compliance, and fail-open resilience.
* **[distributed-url-shortener](https://github.com/qadeeraay/distributed-url-shortener)** — High-throughput URL redirection service with sub-5ms latency, Base62 encoding, and a Redis Bitset Bloom filter for anti-cache penetration.
* **[mini-search-engine](https://github.com/qadeeraay/mini-search-engine)** — In-memory full-text search engine featuring Okapi BM25 ranking, positional inverted indexes, and prefix autocomplete.

---

## 💡 Engineering Principles

* **Code Standards for Infrastructure:** Platform and IaC code should be held to the same software engineering standards as customer-facing applications: modular structure, deterministic testing, and clear failure domains.
* **Actionable Alerts Only:** Alerts must be tied directly to customer-facing SLOs and error budgets. If an alert doesn't require immediate human action, it belongs in a dashboard, not an on-call pager.
* **Automate Repetitive Operations:** Any manual maintenance task performed more than once is a candidate for automation via Terraform, Ansible, or custom Kubernetes controllers.
