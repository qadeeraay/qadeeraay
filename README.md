# Hi, I'm Qadeer Aslam 👋

## DevOps & Cloud Platform Engineer | SRE & DevSecOps

I design and operate reliable, secure, and cost-efficient cloud platforms. My background spans **production Kubernetes, GitOps delivery pipelines, zero-trust secrets management, and automated platform reliability**. Beyond infrastructure automation, I build high-throughput backend services and custom Kubernetes controllers in Python, bridging the gap between infrastructure operations and software engineering.

* 📍 Karachi, Pakistan
* 💼 DevOps / Cloud Engineer & COO at **HashX** | DevOps / Cloud Engineer at **Al-Nafi**
* 🎓 BS in Information Technology — The University of Faisalabad
* 📬 Contact: [qadeeraslam888@gmail.com](mailto:qadeeraslam888@gmail.com) | [LinkedIn](https://linkedin.com/in/qadeer-aslam-devops)
* 📄 **Resume:** [![Download Resume](https://img.shields.io/badge/Resume-Download_DevOps_PDF-007ACC?style=flat-square&logo=adobeacrobatreader&logoColor=white)](./Qadeer_Aslam_DevOps_Resume.pdf)

---

## 🛠️ Technical Stack & Tooling

* **Container Orchestration & Cloud:** Kubernetes (Custom Controllers, Operators, RBAC, NetworkPolicies), AWS (VPC, EKS, IAM, S3, CloudWatch), Docker
* **IaC & GitOps Delivery:** Terraform, Ansible, Helm 3, ArgoCD, Argo Rollouts, GitHub Actions CI/CD
* **SRE & Observability:** Prometheus, Grafana, Loki, Alertmanager, SLO/SLI Multi-Window Burn Rate Alerting
* **Security & DevSecOps:** HashiCorp Vault, External Secrets Operator, Cosign, Trivy, Checkov, CIS Hardening, PCI DSS v4
* **Backend Systems & Languages:** Python 3.12, Bash/Shell, PostgreSQL, Redis (Streams, Lua scripting, Bloom filters)

---

## 🚀 Cloud Infrastructure & Platform Engineering

| Platform Project | Focus Domain | Architecture & Technologies | Reliability & Production Impact |
| :--- | :--- | :--- | :--- |
| **[enterprise-gitops-argocd-pipeline](https://github.com/qadeeraay/enterprise-gitops-argocd-pipeline)** | GitOps & Progressive Delivery | ArgoCD, Helm 3, Argo Rollouts, Kyverno | Pull-based release platform with metric-driven Canary analysis and automated rollback in **< 1.8s**. |
| **[production-observability-golden-signals](https://github.com/qadeeraay/production-observability-golden-signals)** | Observability & SRE | Prometheus, Grafana, Loki, Alertmanager | Google SRE 4 Golden Signals stack with multi-window **14.4x SLO error budget burn rate alerting**. |
| **[k8s-aiops-self-healing-operator](https://github.com/qadeeraay/k8s-aiops-self-healing-operator)** | Kubernetes Controllers | Python, K8s Client & Informers, Prometheus | Custom Kubernetes controller slashing crash recovery MTTR by **99.2% (<5s vs 25-45m)**. |
| **[enterprise-ansible-vault-secrets](https://github.com/qadeeraay/enterprise-ansible-vault-secrets)** | Config & Secret Lifecycle | Ansible, HashiCorp Vault, External Secrets | **100% compliance** across 15 CIS Level 2 Linux controls with 1-hour dynamic secret leasing. |
| **[secure-aws-k8s-compliance-engine](https://github.com/qadeeraay/secure-aws-k8s-compliance-engine)** | DevSecOps & Cloud IaC | Terraform, AWS KMS/VPC/S3, Checkov, Trivy | Production AWS & K8s infrastructure passing **100% of 213 automated compliance controls**. |
| **[serverless-cost-pipeline](https://github.com/qadeeraay/serverless-cost-pipeline)** | FinOps & Serverless | OpenFaaS, NATS JetStream, MinIO, Cosign | Event-driven pipeline cutting compute costs by **99.8%** and egress bandwidth by **59%** in a 32MB tmpfs. |

---

## ⚡ Distributed Systems & Backend Services

Engineering high-throughput, low-latency microservices with native telemetry and resilience:

| Service | Architecture & Algorithms | Technologies | Key Highlights |
| :--- | :--- | :--- | :--- |
| **[distributed-url-shortener](https://github.com/qadeeraay/distributed-url-shortener)** | Bijective Base62 over monotonic sequences, Redis Bitset Bloom filter, Async clickstream worker | FastAPI, PostgreSQL, Redis Streams, Docker | **Sub-5ms p99 redirect hot-path**, anti-cache penetration defense, and asynchronous stream analytics. |
| **[distributed-rate-limiter](https://github.com/qadeeraay/distributed-rate-limiter)** | Atomic Token Bucket & Sliding Window via Redis `EVALSHA`, multi-tier policies | FastAPI ASGI, Redis Lua, Prometheus | **Zero race-condition over-quota leaks**, RFC 6585 & IETF header compliance, and fail-open resilience. |
| **[mini-search-engine](https://github.com/qadeeraay/mini-search-engine)** | Positional Inverted Index, Okapi BM25 ranking, Prefix Trie, Damerau-Levenshtein typo correction | Python 3.12, FastAPI, Modern Web UI | **44x faster query execution** than linear scans, exact phrase matching, and search-as-you-type autocomplete. |

---

## 💡 Engineering Principles

1. **Production Parity in Code:** Infrastructure and platform tooling should follow the same software engineering standards as customer-facing applications: modular code, targeted error handling, and robust test suites.
2. **Deterministic Automation:** If an operational procedure is performed more than once, automate it via Terraform, Ansible, or custom Kubernetes controllers.
3. **Actionable Observability:** Alerts must be symptom-based and tied directly to user-impacting SLOs, avoiding alert fatigue and reducing MTTR.
