# Youngjoon Jeong

Cloud native architect working on Amazon EKS and AI platforms.

[Engineering Playbook](https://devfloor9.github.io/engineering-playbook/)

I work on Kubernetes platform design, model serving, and day-2 operations for AI workloads. Much of my recent work sits at the boundary between infrastructure and application teams: accelerator capacity, traffic routing, identity, observability, evaluation, and release safety.

I also write implementation notes and architecture guides. I try to separate measured results from calculated examples and proposed designs, and to document the conditions behind each recommendation.

## Current work

### [Engineering Playbook](https://github.com/devfloor9/engineering-playbook)

A bilingual reference for AWS, Kubernetes, and AI platform engineering. As of October 2026, it contains 318 Korean source documents with corresponding English pages across EKS, AI platform architecture, model serving, hybrid infrastructure, security, AIDLC, and benchmarks.

Recent updates include:

- repository-wide document audits, correction ledgers, and offline checks for published examples;
- guidance for reasoning and tool-call output integrity;
- model-serving coverage for vLLM, llm-d, NVIDIA Dynamo, AWS Neuron, inference routing, and cache-aware scheduling; and
- terminology and style reviews across the Korean and English AIDLC and model-serving sections.

The site also publishes [`llms.txt`](https://devfloor9.github.io/engineering-playbook/llms.txt), a combined text export, and a per-page Markdown manifest for documentation tools.

### [sample-oh-my-aidlcops](https://github.com/aws-samples/sample-oh-my-aidlcops)

I contribute to this AWS Samples project for applying the AI Development Lifecycle (AIDLC) to agent-assisted software delivery. It provides installable workflows and plugins for inception, construction, operations, evaluation, and platform setup in Claude Code and Kiro.

The project began as `oh-my-aidlcops` and now lives in the `aws-samples` organization. My recent work has included plugin packaging, ontology injection, opt-in observability, documentation localization, and CI/link reliability.

### GenAI on Amazon EKS

I contribute examples and documentation to the EKS GenAI workshop ecosystem:

- [sample-genai-on-eks-starter-kit](https://github.com/aws-samples/sample-genai-on-eks-starter-kit): merged work includes [Langfuse session and tag propagation](https://github.com/aws-samples/sample-genai-on-eks-starter-kit/pull/141) and [OpenClaw orchestrator examples](https://github.com/aws-samples/sample-genai-on-eks-starter-kit/pull/87).
- [awslabs/ai-on-eks](https://github.com/awslabs/ai-on-eks) and [ai-on-eks-charts](https://github.com/awslabs/ai-on-eks-charts): contributed the [Llama 4 on Trainium2 deployment guide](https://github.com/awslabs/ai-on-eks/pull/276) and its [vLLM Helm values](https://github.com/awslabs/ai-on-eks-charts/pull/12).

## Areas I work in

- **EKS platform architecture:** cluster and node design, Cilium and Gateway API networking, Karpenter, EKS Auto Mode, hybrid nodes, and GitOps.
- **Model serving:** vLLM, llm-d, NVIDIA Dynamo, GPU scheduling, AWS Neuron on Trainium and Inferentia, distributed inference, and request routing.
- **AI platform operations:** observability, evaluation, prompt and agent versioning, release strategies, and incident response.
- **Security and governance:** workload identity, policy as code, supply-chain controls, guardrails, and regulatory requirements.

Tools I use regularly include Kubernetes, Helm, Argo CD, Terraform, AWS CDK, Prometheus, OpenTelemetry, Langfuse, Milvus, Qdrant, LangGraph, Strands, and the Model Context Protocol (MCP).

## Writing and workshops

I write for engineers who need to make or operate a system, not just evaluate a product. My preferred format is a concrete problem, explicit constraints, an implementation path, and a note about what has and has not been verified.

I am also a lead author of an AWS Workshop Studio course on building generative AI workloads on Amazon EKS and help maintain the starter kit used by the workshop.

## Contact

The best place to reach me is [LinkedIn](https://www.linkedin.com/in/youngjoonjeong/). For corrections or questions about a guide, please open an issue in the relevant repository.
