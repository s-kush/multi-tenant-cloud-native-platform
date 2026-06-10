# ADR-001

Decision:
Use K3s instead of kubeadm.

Reason:
Lower operational overhead and faster deployment.

Tradeoff:
Less granular control of control-plane components.

---

# ADR-002

Decision:
Use the existing K3s cluster on platform.airvault.io.

Reason:
The cluster is already clean and operational.

Tradeoff:
Some bootstrap decisions predate the project.

---

# ADR-003

Decision:
Use local-path storage initially.

Reason:
Simple and sufficient for learning and platform development.

Tradeoff:
Not suitable for highly available storage.

---

# ADR-004

Decision:
Customer, User, and Tenant are treated as the same entity in Platform.

Reason:
Simplifies namespace ownership, quota management, storage allocation, and workload isolation.

Tradeoffs:
Does not support multi-user organizations initially.

Future:
RBAC can be introduced to support multiple users within a tenant.
