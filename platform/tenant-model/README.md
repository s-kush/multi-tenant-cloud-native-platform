# Tenant Model

## Overview

The platform follows the below tenant model:

Customer = User = Tenant

Each tenant receives an isolated environment withtin the Kubernetes cluster.

The Platform is responsible for infrastructure, isolation, governance, storage, networking, and observability.

The tenant is responsible for the applications workload deployed within their allocaed resources.


## Tenant Boundary

A tenant is represented by a dedicated Kubernates namespace.

- Dedicated Namespace
- ResourceQuota
- LimitRange
- ConfigMaps
- Secrets
- PVCs
- Ingress
- Monitoring
- Applications


## Application Model

The platform might provide the application catalogue. A tenant may deploy any supported application within the allocated resources.

Examples:

Tenant A
|
|-- nextcloud 
|-- redis
|-- wordpress

Tenant B
|
|-- n8n
|-- flowise
|-- chatwoot


## Resource Plans

Note: Will be expanded later.

- Plan A
- Plan B
- Plan C


## Storage Model

Persistent storage is allocated through Kubernetes Persistent Volume Claims (PVCs).

Storage belongs to the tenant namespace and is isolated from other tenants.

Examples:
- uploads-data
- backups-data


## DNS Model

Platform services:
- argocd.example.com
- grafana.example.com

Tenant applications:
- tenant-name.apps.example.com

Examples:
- tenant-a.apps.example.com
- tenant-b.apps.example.com


## Future Enhancements

- RBAC
- Multi-user tenants
- Usage Tracking
- Billing integration
- Network Policies
- Backup automation
- Self-service provisioning
- Automated tenant provisioning
