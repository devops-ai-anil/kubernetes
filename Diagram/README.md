# 🚀 AI DevOps Kubernetes Architecture

## 📌 Overview
This architecture represents an AI-powered DevOps system that performs log analysis and auto-healing using Kubernetes and LLM (Claude).

---

## 🏗 Architecture Diagram

```mermaid
graph TD

    User --> LoadBalancer
    LoadBalancer --> Ingress
    Ingress --> Service

    Service --> Pod1
    Service --> Pod2

    Pod1 --> Logs
    Pod2 --> Logs

    Logs --> AIEngine
    AIEngine --> Analysis

    Analysis --> DecisionEngine
    DecisionEngine --> AutoHealing

    AutoHealing --> Kubernetes

    Prometheus --> Pod1
    Prometheus --> Pod2
    Grafana --> Prometheus

    GitHubActions --> CI
    CI --> CD
    CD --> Kubernetes

    Terraform --> Infrastructure
    Infrastructure --> Kubernetes
