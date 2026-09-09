# Hi, I'm Qadeer Aslam 👋
### DevOps & Cloud Engineer | SRE & DevSecOps Specialist

I build resilient, secure, and cost-optimized cloud infrastructure. My work focuses on **zero-trust Kubernetes architectures, GitOps progressive delivery, automated incident self-healing, and compliance-first Infrastructure as Code**.

* 📍 Karachi, Pakistan
* 💼 DevOps / Cloud Engineer & COO at **HashX** | DevOps / Cloud Engineer at **Al-Nafi**
* 🎓 BS in Information Technology — The University of Faisalabad
* 📬 Reach me at: [qadeeraslam888@gmail.com](mailto:qadeeraslam888@gmail.com) | [LinkedIn](https://linkedin.com/in/qadeer-aslam-devops)
* 📄 **Resume:** [![Download Resume](https://img.shields.io/badge/Resume-Download_DevOps_PDF-007ACC?style=flat-square&logo=adobeacrobatreader&logoColor=white)](./Qadeer_Aslam_DevOps_Resume.pdf)

---

## 🛠️ Technical Toolkit

* **Cloud & Platforms:** AWS (VPC, EC2, IAM, S3, CloudWatch), Kubernetes, Docker
* **IaC & GitOps Delivery:** Terraform, Ansible, Helm 3, ArgoCD, Argo Rollouts, GitHub Actions
* **SRE & Observability:** Prometheus, Grafana, Loki, Promtail, Alertmanager, Google SRE Golden Signals
* **Security & Compliance:** HashiCorp Vault, External Secrets Operator, PCI DSS v4, ISO 27001, CIS Benchmarks, Checkov, Trivy, Cosign
* **Scripting & Linux:** Python 3.12, Bash, Linux Server Administration (Ubuntu, RHEL), Network Security

---

## 🚀 Featured Enterprise Projects (Pinned Showcase)

| Repository | Domain | Core Tech | Reliability & Business Impact |
| :--- | :--- | :--- | :--- |
| **[enterprise-gitops-argocd-pipeline](https://github.com/qadeeraay/enterprise-gitops-argocd-pipeline)** | GitOps & Progressive Delivery | ArgoCD, Helm 3, Argo Rollouts, Kyverno | Pull-based zero-trust release platform with metric-driven Canary analysis & auto-rollback in **< 1.8s**. |
| **[production-observability-golden-signals](https://github.com/qadeeraay/production-observability-golden-signals)** | Observability & SRE | Prometheus, Grafana, Loki, Alertmanager | Google SRE 4 Golden Signals stack with multi-window **14.4x SLO error budget burn rate alerting**. |
| **[enterprise-ansible-vault-secrets](https://github.com/qadeeraay/enterprise-ansible-vault-secrets)** | Config Mgmt & Secret-Zero | Ansible, HashiCorp Vault, K8s ESO | **100% compliance** across 15 CIS Level 2 Linux controls & 1-hour dynamic database credential leasing. |
| **[k8s-aiops-self-healing-operator](https://github.com/qadeeraay/k8s-aiops-self-healing-operator)** | K8s Internals & AIOps | Python 3.12, K8s API, Informers, Prometheus | Autonomous operator slashing MTTR by **99.2% (<5s vs 25-45m)** for OOMKilled & CrashLoopBackOff. |
| **[secure-aws-k8s-compliance-engine](https://github.com/qadeeraay/secure-aws-k8s-compliance-engine)** | DevSecOps & Cloud IaC | Terraform, AWS KMS/VPC/S3, Checkov, Trivy | Production AWS & K8s infrastructure passing **100.0% of 213 automated policy controls** (NIST/ISO/PCI DSS). |
| **[serverless-cost-pipeline](https://github.com/qadeeraay/serverless-cost-pipeline)** | FinOps & Serverless | OpenFaaS, NATS JetStream, MinIO, Cosign | Event-driven pipeline cutting compute costs by **99.8%** and egress bandwidth by **59%** in a 32MB tmpfs RAM. |

---

## 📈 Engineering Philosophy
1. **Security by Default, Not an Afterthought:** Everything runs as non-root with dropped Linux capabilities, immutable root filesystems, and dynamic rotated secrets.
2. **Deterministic Automation:** If a task has to be performed twice, it belongs in Ansible, Terraform, or a custom Kubernetes controller.
3. **Actionable Observability:** Dashboards must track user experience (the 4 Golden Signals). Alerts must be symptom-based and strictly tied to customer-impacting SLO burn rates.
