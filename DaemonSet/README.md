# DaemonSet

A DaemonSet in Kubernetes ensures that a copy of a Pod runs on all (or some) nodes in a cluster. It’s mainly used for deploying system-level services that need to be present on every node — such as log collectors, monitoring agents, or network plugins.

🧩 Definition

A DaemonSet is a Kubernetes workload resource that automatically runs and manages Pods across all nodes that match its selector.
When new nodes are added, the DaemonSet automatically schedules Pods onto them.
When nodes are removed, their DaemonSet Pods are also deleted.

🛠 Common Use Cases

Log collection: e.g. Fluentd, Logstash
Monitoring: e.g. Prometheus Node Exporter
Networking: e.g. Calico, Cilium agents
Storage: e.g. Ceph or GlusterFS agents running on each node
