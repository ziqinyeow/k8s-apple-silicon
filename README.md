# Multi-node cluster within a single M1/M2 machine

## Cluster Details
Guide to bootstrapping a highly available Kubernetes cluster with end-to-end encryption between components and RBAC authentication w/o Helm.

VM - [VMware Fusion](https://customerconnect.vmware.com/en/evalcenter?p=fusion-player-personal-13) \
VM Provisioner - [Hashicorp Vagrant](https://developer.hashicorp.com/vagrant/tutorials/getting-started/getting-started-index) \
Orchestrater - [Kubernetes](https://kubernetes.io/) \
Orchestrater Installer - [Kubeadm](https://kubernetes.io/docs/setup/production-environment/tools/kubeadm/create-cluster-kubeadm/) \
Container Runtime - [Containerd](https://containerd.io/), [Docker](https://www.docker.com/) \
CNI Container Networking - [Weave](https://github.com/weaveworks/weave), [Flannel](https://github.com/flannel-io/flannel), [Calico](https://github.com/projectcalico/calico) \
DNS - [CoreDNS](https://github.com/coredns/coredns) \
Metadata storage - [Etcd](https://github.com/etcd-io/etcd)

## Node configuration

We will be building the following:

1. Two control plane nodes (master-1 and master-2) running the control plane components as operating system services.
2. Two worker nodes (worker-1 and worker-2).
3. One load balancer VM running HAProxy to balance requests between the two API servers.


🚀 in progress
