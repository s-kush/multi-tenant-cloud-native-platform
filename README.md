# Multi-Tenant Cloud Native Platform

A hands-on platform engineering project built on K3s to demonstrate modern cloud-native infrastructure, GitOps workflows, multi-tenant application hosting, observability, automation, and operational excellence.

The goal is to build and operate a production-inspired platform capable of hosting isolated tenant workloads while applying real-world platform engineering practices.

---

## Objectives

* Kubernetes Administration
* Multi-Tenant Platform Design
* GitOps with ArgoCD
* Infrastructure Automation
* Monitoring and Observability
* Security and Governance
* Reliability Engineering
* Disaster Recovery and Operations

---

## Current Environment

### Host

* Hostname: `platform.airvault.io`
* OS: Debian 12
* Kubernetes: K3s v1.33.6
* Runtime: containerd

### Installed Components

* CoreDNS
* Metrics Server
* Local Path Provisioner

### Storage

* local-path StorageClass

### Cluster Topology

```text
1 Control Plane Node
```

---

## Platform Vision

The platform provides isolated environments for tenants.

```text
Customer = User = Tenant
```

Each tenant receives:

* Dedicated Namespace
* Resource Quotas
* Limit Ranges
* Persistent Storage
* Secrets and ConfigMaps
* Ingress Access
* Monitoring Access

The platform does not prescribe application architecture.

Tenants may deploy any supported workload within their allocated resources.

---

## Planned Components

### Platform Services

* ingress-nginx
* ArgoCD
* Prometheus
* Grafana
* Loki
* Cert Manager

### Platform Features

* Tenant Isolation
* Resource Governance
* GitOps Deployments
* Backup and Recovery
* Operational Runbooks
* Multi-Node Expansion

---

## Repository Structure

```text
docs/          Project documentation
gitops/        GitOps and ArgoCD resources
k8s/           Kubernetes manifests
monitoring/    Observability stack
notes/         Study notes and operational learnings
platform/      Platform architecture and tenant model
```

---

## Roadmap

### Phase 1

* Documentation
* Architecture
* Tenant Model

### Phase 2

* ingress-nginx

### Phase 3

* Tenant Workloads

### Phase 4

* ArgoCD and GitOps

### Phase 5

* Prometheus, Grafana and Loki

### Phase 6

* Security, Quotas and Governance

### Phase 7

* Backup and Recovery

### Phase 8

* Multi-Node Expansion

---

## Status

Current Phase: **Phase 1 - Foundation**
