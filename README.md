**Cloud Native Architect & Agentic AI Platform Engineer**

- 📍 Seoul, Korea
- 💼 LinkedIn: [@youngjoonjeong](https://www.linkedin.com/in/youngjoonjeong/)
- 🌐 Engineering Playbook: [devfloor9.github.io/engineering-playbook](https://devfloor9.github.io/engineering-playbook/)
- 🐙 GitHub: [@devfloor9](https://github.com/devfloor9)

## Summary

Building production-grade cloud native platforms at the intersection of Kubernetes and Generative AI. I specialize in Amazon EKS architecture optimization, GPU infrastructure for large-scale model serving, and designing end-to-end Agentic AI platforms that actually work in production.

My work focuses on turning complex infrastructure challenges into battle-tested engineering patterns — from Cilium networking and Karpenter autoscaling to vLLM/llm-d distributed inference and MCP-based agent orchestration. Everything I build gets documented in the [Engineering Playbook](https://devfloor9.github.io/engineering-playbook/), an open knowledge base for the cloud native community.

## Key Skills

### Cloud Native Infrastructure
* Deep expertise in **Amazon EKS** — cluster architecture, networking (Cilium, Gateway API), autoscaling (Karpenter), and operational excellence
* Production experience with **hybrid infrastructure** — EKS Hybrid Nodes, SR-IOV with DGX H200, on-prem/cloud bridging
* **GitOps-driven operations** with Argo CD, infrastructure as code, and automated deployment pipelines
* Performance optimization — CNI benchmarking, East-West traffic tuning, CoreDNS optimization

### Agentic AI & GPU Platform Engineering
* End-to-end **Agentic AI platform** design on Kubernetes — from GPU resource management to agent observability
* Model serving at scale with **vLLM, llm-d, NeMo Framework**, and MoE architectures
* **Inference Gateway** routing, KV Cache-aware scheduling, and distributed inference optimization
* RAG pipelines with **Milvus** vector database, evaluation with **RAGAS**, monitoring with **Langfuse**
* **Amazon Bedrock AgentCore** and **MCP (Model Context Protocol)** integration for enterprise agent deployments

### Security & Governance
* **Identity-First Security** with EKS Pod Identity and IRSA
* Runtime threat detection with **GuardDuty Extended Threat Detection**
* Policy-as-code with **Kyverno**, supply chain security, and compliance automation

## Tech Stack

**Container & Orchestration:** Amazon EKS, EKS Auto Mode, Karpenter, Helm, Argo CD

**Networking:** Cilium, Gateway API, CoreDNS, ALB/NLB

**AI/ML Serving:** vLLM, llm-d, NeMo Framework, Amazon Bedrock AgentCore

**AI Agents:** Kagent, MCP (Model Context Protocol), Inference Gateway

**Observability:** Prometheus, Grafana, Langfuse, Hubble, OpenTelemetry

**Security:** Kyverno, GuardDuty, EKS Pod Identity, Harbor

**Vector DB & Evaluation:** Milvus, RAGAS

**IaC & GitOps:** CDK, Terraform, Argo CD, GitHub Actions

## Featured Projects

### [Engineering Playbook](https://github.com/devfloor9/engineering-playbook)
Comprehensive documentation site covering cloud native architecture and Agentic AI best practices. 40+ technical guides across infrastructure optimization, operations, AI platform engineering, hybrid infrastructure, security, and ROSA. Built with Docusaurus, dual-language (Korean/English).

### [genai-on-eks](https://github.com/devfloor9/genai-on-eks)
Building scalable GenAI platforms on Amazon EKS — reference architectures and deployment patterns for production AI workloads.

## Engineering Playbook Topics

📘 **Infrastructure Optimization** — Cilium ENI, Gateway API, CoreDNS, Karpenter, cost management

📗 **Operations & Observability** — GitOps, node monitoring, EKS debugging & resiliency guides

📙 **Agentic AI Platform** — vLLM, llm-d, MoE serving, Inference Gateway, Milvus, Kagent, Bedrock AgentCore, RAGAS

📕 **Hybrid Infrastructure** — Hybrid Nodes, SR-IOV DGX H200, Harbor registry integration

📓 **Security & Governance** — Identity-First Security, GuardDuty, Kyverno, supply chain security

📒 **Benchmark Reports** — CNI performance, AI/ML workloads, hybrid infrastructure, security operations
PROFILE_EOF
echo "Done"
