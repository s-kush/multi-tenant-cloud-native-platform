# Tenant Model

Each tenant receives:

- Namespace
- ResourceQuota
- LimitRange
- ConfigMap
- Secret
- Service
- Ingress
- Persistent Volume

Example:

tenant-a
├── frontend
├── backend
└── postgres

tenant-b
├── frontend
├── backend
└── postgres

TODO: Map tenants to actual users on the platform? Helps in sepration at user level.
