# Qadeer Aslam
### Senior DevOps & Cloud Platform Engineer | SRE & DevSecOps

I design, build, and operate resilient, secure, and observable cloud platforms. My focus is on **production Kubernetes, GitOps continuous delivery, zero-trust infrastructure, and automated platform reliability**. I write custom Kubernetes controllers and automation in Python to eliminate operational bottlenecks and treat infrastructure with software engineering rigor.

📍 **Faisalabad, Pakistan** · 💼 **DevOps / Cloud Engineer at HashX** · 🎓 **BS in Information Technology**  
📬 **Contact:** [qadeeraslam888@gmail.com](mailto:qadeeraslam888@gmail.com) · [LinkedIn](https://linkedin.com/in/qadeer-aslam-devops) · 📄 **[Download Resume (PDF)](./Qadeer_Aslam_DevOps_Resume.pdf)**

---

## 🛠️ Core Competencies

| Domain | Technologies & Standards |
| :--- | :--- |
| **Cloud & Orchestration** | AWS (EKS, VPC, IAM, KMS, S3, CloudWatch), Kubernetes (Custom Controllers, Operators, RBAC, NetworkPolicies), Docker |
| **IaC & GitOps Delivery** | Terraform, Ansible, Helm 3, ArgoCD, Argo Rollouts, GitHub Actions CI/CD |
| **SRE & Observability** | Prometheus, Grafana, Loki, Alertmanager, Google SRE 4 Golden Signals, Multi-Window SLO Burn-Rate Alerting |
| **Security & DevSecOps** | HashiCorp Vault, External Secrets Operator (ESO), Kyverno Policy Engine, Checkov, Trivy, CIS Benchmarks (Level 2) |
| **Automation & Systems** | Python 3.12 (AsyncIO, K8s Informers), Bash / POSIX Shell, PostgreSQL, Redis |

---

## 🚀 Flagship Engineering Projects

Here are my six primary open-source platform implementations, each architected to solve a specific production reliability, delivery, or compliance challenge:

### 1. [enterprise-gitops-argocd-pipeline](https://github.com/qadeeraay/enterprise-gitops-argocd-pipeline)
**Declarative GitOps Continuous Delivery & Automated Canary Analysis**
* **Stack:** ArgoCD, Helm 3, Argo Rollouts, Kyverno, Prometheus
* **Architecture:** Implements an enterprise App-of-Apps deployment topology managing multi-environment workloads from Git as the single source of truth.
* **Impact & Resilience:** Automated metric-driven Canary deployments evaluate Prometheus error rates and P99 latency thresholds, executing an automated rollback in **< 1.8 seconds** if an anomaly is detected. Admission is enforced via Kyverno policies disallowing root privilege escalation.

### 2. [production-observability-golden-signals](https://github.com/qadeeraay/production-observability-golden-signals)
**Production SRE Telemetry & Multi-Window SLO Burn-Rate Alerting**
* **Stack:** Prometheus, Grafana, Loki, Alertmanager, Docker Compose
* **Architecture:** Full observability stack structured around Google SRE's 4 Golden Signals: Latency, Traffic, Errors, and Saturation.
* **Impact & Resilience:** Features multi-window, multi-burn-rate alerting rules (14.4x / 1-hour and 6-hour windows), avoiding transient false positives while instantly paging on catastrophic budget depletion. Correlates metrics directly with Loki logs for sub-minute incident triage.

### 3. [k8s-aiops-self-healing-operator](https://github.com/qadeeraay/k8s-aiops-self-healing-operator)
**Autonomous Kubernetes Remediation Controller**
* **Stack:** Python 3.12, Kubernetes Client / Informers, Prometheus Metrics Engine
* **Architecture:** Custom Kubernetes controller utilizing an event-driven reconciliation loop to watch cluster events and pod lifecycle state transitions.
* **Impact & Resilience:** Detects and remediates `CrashLoopBackOff`, out-of-memory states, and orphaned pods in real time, cutting recovery MTTR from 25+ minutes to **under 5 seconds**. Emits real-time Prometheus metrics tracking self-healing throughput.

### 4. [secure-aws-k8s-compliance-engine](https://github.com/qadeeraay/secure-aws-k8s-compliance-engine)
**Hardened Cloud Infrastructure as Code & DevSecOps Engine**
* **Stack:** Terraform, AWS (VPC, EKS, KMS, S3), Checkov, Trivy
* **Architecture:** Modular Terraform code provisioning an isolated AWS cloud topology with private subnets, KMS customer-managed envelope encryption, and strict IAM permission boundaries.
* **Impact & Resilience:** Zero-trust Kubernetes NetworkPolicies with default-deny traffic isolation. Passing **100% of 213 automated policy-as-code checks** across CIS, SOC 2, and PCI DSS standards with zero security vulnerabilities.

### 5. [enterprise-ansible-vault-secrets](https://github.com/qadeeraay/enterprise-ansible-vault-secrets)
**Zero-Trust Secrets Lifecycle & CIS Operating System Hardening**
* **Stack:** Ansible, HashiCorp Vault, External Secrets Operator (ESO), PostgreSQL
* **Architecture:** Bridges Kubernetes workloads to HashiCorp Vault via ESO and short-lived ServiceAccount JWT tokens, eliminating static cluster credentials.
* **Impact & Resilience:** Dynamically issues ephemeral database credentials with automated 1-hour TTL revocation. Enforces **15 CIS Level 2 Linux benchmark controls** via modular Ansible playbooks.

### 6. [serverless-cost-pipeline](https://github.com/qadeeraay/serverless-cost-pipeline)
**Event-Driven FinOps & Serverless Kubernetes Infrastructure**
* **Stack:** OpenFaaS, NATS JetStream, MinIO S3, Velero, Kubernetes
* **Architecture:** Event-driven pipeline handling async workloads via NATS JetStream with scale-to-zero autoscaling (0 to 5 replicas) to minimize idle cloud spend.
* **Impact & Resilience:** Slashes compute costs by **99.8%** during idle periods; processes objects entirely within a 32MB tmpfs RAM boundary to cut egress by 59%. Includes automated Velero backup and state recovery procedures.

---

## 💡 Engineering Philosophy

* **Reliability is a Feature:** Reliability must be baked into architecture through progressive rollouts, circuit breaking, and clear SLO boundaries, not added as an operational afterthought.
* **Deterministic Automation:** If an operational procedure is performed more than once, it should be codified in Terraform, Ansible, or custom controllers.
* **Actionable Telemetry:** Alerts must reflect user-impacting pain and consumption of error budgets. Every alert sent to an engineer must be unambiguous and immediately actionable.
