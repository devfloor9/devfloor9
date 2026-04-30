**Cloud Native Architect & Agentic AI Platform Engineer**

- 📍 Seoul, Korea
- 💼 LinkedIn: [@youngjoonjeong](https://www.linkedin.com/in/youngjoonjeong/)
- 🌐 Engineering Playbook: [devfloor9.github.io/engineering-playbook](https://devfloor9.github.io/engineering-playbook/)
- 🐙 GitHub: [@devfloor9](https://github.com/devfloor9)

## Summary

Building production-grade cloud native platforms at the intersection of Kubernetes and Generative AI. I specialize in Amazon EKS architecture optimization, GPU infrastructure for large-scale model serving, and designing end-to-end Agentic AI platforms that actually work in production.

My work focuses on turning complex infrastructure challenges into battle-tested engineering patterns — from Cilium networking and Karpenter autoscaling to vLLM/llm-d distributed inference, AWS Neuron/Trainium2 serving, and MCP-based agent orchestration. Beyond infrastructure, I am open-sourcing the **AIDLC (AI Development Lifecycle) × AgenticOps** methodology itself — so the design → construction → operations loop can be closed by agents, not humans at every step. Everything I build gets documented in the [Engineering Playbook](https://devfloor9.github.io/engineering-playbook/), an open knowledge base for the cloud native community.

## Key Skills

### Cloud Native Infrastructure
* Deep expertise in **Amazon EKS** — cluster architecture, networking (Cilium, Gateway API), autoscaling (Karpenter), and operational excellence
* Node strategy across **EKS Auto Mode / Karpenter / Managed Node Groups + DRA** — including the DRA ↔ Karpenter/Auto Mode incompatibility and MNG-based fallbacks
* Production experience with **hybrid infrastructure** — EKS Hybrid Nodes, SR-IOV with DGX H200, on-prem/cloud bridging
* **GitOps-driven operations** with Argo CD, infrastructure as code, and automated deployment pipelines
* Performance optimization — CNI benchmarking, East-West traffic tuning, CoreDNS optimization

### Agentic AI & GPU Platform Engineering
* End-to-end **Agentic AI platform** design on Kubernetes — from GPU resource management to agent observability
* Model serving at scale with **vLLM, llm-d, NVIDIA Dynamo, NeMo Framework**, and MoE architectures
* **AWS Neuron / Trainium2 / Inferentia2** serving via vLLM + optimum-neuron (Llama 4 Scout/Maverick, BF16)
* **Inference Gateway** routing, KV Cache-aware scheduling, disaggregated serving, LWS multi-node, Bifrost → Bedrock fallback
* **Cascade Routing** tuning and **semantic caching** across 3 layers (KV / Prompt / Semantic)
* **Self-Improving Agent Loop** + continuous training pipeline (Langfuse trace → Ragas/LLM-as-a-Judge → GRPO/DPO → kgateway canary)
* **Multi-Agent Collaboration** patterns (LangGraph / CrewAI / AutoGen / Strands, Orchestrator/Voting/Debate/Supervisor)
* RAG pipelines with **Milvus / Qdrant** vector databases, evaluation with **RAGAS + Langfuse Custom Evaluators**
* **Amazon Bedrock AgentCore** and **MCP (Model Context Protocol)** integration for enterprise agent deployments

### Enterprise AI Platform
* **AIDLC × AgenticOps**: open-source methodology for closed-loop agentic delivery — design, construction, and operations automated end-to-end (see `oh-my-aidlcops`)
* **Regulatory Compliance**: EU AI Act, NIST AI RMF 1.1, ISO/IEC 42001, Korean AI Basic Act, ISMS-P, and financial supervisory regulations
* **Agent Versioning**: prompt registry, Shadow / Canary / A-B / Blue-Green release patterns
* **AI Gateway Guardrails**: input/output guards with Guardrails AI, NeMo Guardrails, Llama Guard 3, Bedrock Guardrails

### Security & Governance
* **Identity-First Security** with EKS Pod Identity, IRSA, and Keycloak OIDC + OAuth2-Proxy two-tier flows
* Runtime threat detection with **GuardDuty Extended Threat Detection**
* Policy-as-code with **Kyverno**, supply chain security, and compliance automation

### Workshop & Technical Writing
* Lead author on the **AWS Workshop Studio** EKS GenAI workshop (LLMs → scalable agent systems) and maintainer of the upstream starter kit it runs on

## Tech Stack

**Container & Orchestration:** Amazon EKS, EKS Auto Mode, Karpenter, MNG + DRA, Helm, Argo CD

**Networking:** Cilium, Gateway API, kgateway, CoreDNS, ALB/NLB, CloudFront + WAF + Shield

**AI/ML Serving:** vLLM, SGLang, llm-d, NVIDIA Dynamo, NeMo Framework, AWS Neuron / Trainium2 / Inferentia2, Amazon Bedrock AgentCore

**AI Gateway:** kgateway + agentgateway, Bifrost, LiteLLM (with Team RBAC), OpenClaw

**AI Agents:** Kagent, MCP (Model Context Protocol), LangGraph, CrewAI, AutoGen, Strands

**Auth & Identity:** Keycloak, OAuth2-Proxy (OIDC), EKS Pod Identity, IRSA, External Secrets Operator

**GPU Management:** NVIDIA GPU Operator, DCGM, DRA, MIG, KAI Scheduler, NIXL, CRIU (experimental)

**MLOps:** Kubeflow, MLflow, KServe, SageMaker

**Observability:** Prometheus, Grafana, AMP/AMG + ADOT, Langfuse, Hubble, OpenTelemetry

**Security:** Kyverno, GuardDuty, EKS Pod Identity, Harbor

**Vector DB & Evaluation:** Milvus, Qdrant, RAGAS, LLM-as-a-Judge, Langfuse Custom Evaluators

**IaC & GitOps:** CDK, Terraform, Argo CD, GitHub Actions

## Featured Projects

### [`oh-my-aidlcops`](https://github.com/devfloor9/oh-my-aidlcops) — AIDLC × AgenticOps plugin marketplace
Sibling project to [oh-my-claudecode](https://github.com/Yeachan-Heo/oh-my-claudecode). A Claude Code / Kiro compatible marketplace that layers **AgenticOps** (self-improving loop, autopilot-deploy, incident response, continuous evaluation, cost governance) on top of the [AWS-official AIDLC workflows](https://github.com/awslabs/aidlc-workflows), so the Inception → Construction → Operations lifecycle closes itself. Ships four plugins — `agentic-platform`, `agenticops`, `aidlc-inception`, `aidlc-construction` — and five Tier-0 workflows (`/oma:autopilot`, `/oma:aidlc-loop`, `/oma:agenticops`, `/oma:self-improving`, `/oma:platform-bootstrap`). Built on `awslabs/mcp` hosted MCP servers. *Phase 1 MVP.*

### [`engineering-playbook`](https://github.com/devfloor9/engineering-playbook) — Cloud Native & Agentic AI engineering reference
77+ production-tested guides across 7 tracks, spanning Agentic AI platforms, EKS best practices, AIDLC/AgenticOps, hybrid infrastructure, security governance, ROSA, and quantitative benchmark reports. Trilingual (Korean / English / Chinese), Docusaurus 3.9.2. The April 2026 restructure introduced a 3-tier hierarchy (foundations / platform-selection / advanced-patterns), the Self-Improving Loop ADR, Continuous Training Pipeline, CRIU GPU Migration, Cascade Routing Tuning, AI Gateway Guardrails, and AWS Neuron Stack documents. Live at [devfloor9.github.io/engineering-playbook](https://devfloor9.github.io/engineering-playbook/).

### [`aws-samples/sample-genai-on-eks-starter-kit`](https://github.com/aws-samples/sample-genai-on-eks-starter-kit) — core maintainer (MEMBER)
The starter kit that powers the EKS GenAI workshop. Recent contributions:
- **PR #131** *(in review)* — full demo stack: Code Review MCP (RAG with TEI + Qdrant) + Keycloak OIDC + OAuth2-Proxy + kGateway 2-tier ingress with TLS + LiteLLM Team RBAC + per-user Langfuse tracing via OpenWebUI forward-user-info headers
- **PR #141** — restore Langfuse `session_id` / `tags` on LangChain traces (Langfuse Python SDK v3 moved these out of `RunnableConfig["tags"]` into `config["metadata"]`), unblocking Module 4 Custom Evaluators
- **PR #127 / #126** — External Secrets Operator + Amazon Managed Prometheus & Grafana (AMP/AMG) with ADOT collector
- **PR #87** — OpenClaw AI Agent Orchestrator component, new AI Agent category + DevOps and Doc Writer example agents

### [`awslabs/ai-on-eks`](https://github.com/awslabs/ai-on-eks) + [`ai-on-eks-charts`](https://github.com/awslabs/ai-on-eks-charts) — upstream contributor
AWS official AI on EKS guides and Helm charts. Contributed the **Llama 4 (Scout & Maverick) on Trainium2 vLLM deployment guide** ([ai-on-eks#276](https://github.com/awslabs/ai-on-eks/pull/276)) and matching Helm values ([ai-on-eks-charts#12](https://github.com/awslabs/ai-on-eks-charts/pull/12)): Karpenter-provisioned `trn2.48xlarge`, AWS Neuron DLC (optimum-neuron 0.4.5, Neuron SDK 2.26.1), `tensor-parallel-size 16` across all 16 Trainium chips, BF16 inference without quantization, ~20 min end-to-end deploy.

## Engineering Playbook Topics

📘 **EKS Best Practices** — Cilium ENI, Gateway API, CoreDNS, Karpenter, cost management, control plane scaling, Pod Identity

📗 **Operations & Observability** — GitOps (Argo CD), node monitoring, EKS debugging & resiliency, Pod health lifecycle

📙 **Agentic AI Platform** — EKS GPU node strategy (Auto Mode / Karpenter / MNG / DRA), vLLM, llm-d, NVIDIA Dynamo, MoE serving, AWS Neuron stack, Inference Optimization (KV Cache-aware / disaggregated serving / LWS multi-node / Bifrost → Bedrock fallback), LLM Gateway 2-tier (kgateway + agentgateway + Bifrost), Kagent, Milvus, RAGAS

📔 **AIDLC & AgenticOps** — AIDLC framework principles, Ontology × Harness, Built-in/Org/Domain extensions, evaluation framework, multi-agent collaboration, agent versioning, regulatory compliance (EU AI Act / NIST AI RMF / ISO 42001 / Korean AI Basic Act), AgenticOps observability and DevOps Guru predictive operations

📕 **Hybrid Infrastructure** — EKS Hybrid Nodes, SR-IOV with DGX H200, file storage strategy, Harbor registry integration

📓 **Security & Governance** — Identity-First Security, GuardDuty Extended Threat Detection, Kyverno, supply chain security, AI Gateway guardrails

📗 **ROSA** — Red Hat OpenShift on AWS installation, security, and compliance

📒 **Benchmark Reports** — CNI performance (VPC CNI vs Cilium), Gateway API implementation, AI/ML workloads, AgentCore vs EKS self-hosted inference, NVIDIA Dynamo, hybrid infrastructure, security operations
