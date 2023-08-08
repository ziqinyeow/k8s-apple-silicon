# Multi-node cluster within a single M1/M2 machines

## Cluster Details
Guide to bootstrapping a highly available Kubernetes cluster with end-to-end encryption between components and RBAC authentication.

VM - VMware Fusion
VM Provisioner - Hashicorp Vagrant
Orchestrater - Kubernetes
Container Runtime - Containerd, Docker
CNI Container Networking - Weave/Flannel/Calico
DNS - CoreDNS
Metadata storage - etcd

## Node configuration

We will be building the following:

1. Two control plane nodes (master-1 and master-2) running the control plane components as operating system services.
2. Two worker nodes (worker-1 and worker-2).
3. One load balancer VM running HAProxy to balance requests between the two API servers.
