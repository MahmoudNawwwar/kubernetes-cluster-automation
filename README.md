# Kubernetes Cluster Automation

Automated deployment of a Kubernetes 3-node cluster using **Ansible**, **kubeadm**, **containerd**, and **Flannel CNI**.

---

## 📖 Project Overview

This project demonstrates how to build a Kubernetes cluster from scratch using Infrastructure as Code (IaC) principles.

The cluster consists of one Control Plane node and two Worker nodes. Ansible is used to automate the worker configuration before joining them to the cluster.

---

## 🛠 Technologies

- Ubuntu 24.04 LTS
- Kubernetes v1.34.9
- kubeadm
- kubelet
- kubectl
- containerd
- Flannel CNI
- Ansible
- VMware Workstation

---

## 🏗 Cluster Topology

| Node | Role | IP Address |
|------|------|------------|
| master | Control Plane | 192.168.137.128 |
| host1 | Worker | 192.168.137.133 |
| host2 | Worker | 192.168.137.134 |

---

## 📂 Project Structure

```text
.
├── ansible/
├── docs/
├── manifests/
├── screenshots/
├── README.md
├── LICENSE
└── ansible.cfg
```

---

## 🚧 Status

Project is under active development.
