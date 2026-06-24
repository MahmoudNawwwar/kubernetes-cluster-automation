# Kubernetes Cluster Automation

> Automated deployment of a Kubernetes 3-Node Cluster using Ansible, kubeadm, containerd, and Flannel CNI.

## 📌 Project Overview

This project demonstrates how to build a production-style Kubernetes cluster from scratch using kubeadm and automate the worker node configuration with Ansible.

The cluster consists of:

- 1 Control Plane node
- 2 Worker nodes
- containerd as the Container Runtime
- Flannel as the CNI Plugin

---

## 🏗️ Cluster Architecture

```
                   +----------------------+
                   |      Master          |
                   | 192.168.137.128      |
                   | Control Plane        |
                   +----------+-----------+
                              |
              -----------------------------------
              |                                 |
     +--------+--------+               +--------+--------+
     |     Worker1     |               |     Worker2     |
     |192.168.137.133  |               |192.168.137.134  |
     +-----------------+               +-----------------+
```

---

## 🛠️ Technologies Used

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

## 📂 Project Structure

```text
.
├── ansible/
│   ├── inventory
│   └── k8s-workers.yml
│
├── docs/
│   ├── 01-lab-setup.md
│   ├── 02-control-plane.md
│   ├── 03-worker-nodes.md
│   ├── 04-cluster-validation.md
│   └── troubleshooting.md
│
├── manifests/
├── screenshots/
├── README.md
├── LICENSE
└── ansible.cfg
```

---

## ⚙️ Cluster Information

| Node | Role | Operating System | IP Address |
|------|------|------------------|------------|
| master | Control Plane | Ubuntu 24.04 | 192.168.137.128 |
| host1 | Worker | Ubuntu 24.04 | 192.168.137.133 |
| host2 | Worker | Ubuntu 24.04 | 192.168.137.134 |

---

## ✅ Current Status

- Kubernetes Cluster Created
- Control Plane Initialized
- Worker Nodes Joined Successfully
- Flannel CNI Installed
- All Nodes are Ready

---

## 📸 Screenshots

Screenshots will be added after completing the documentation.

---

## 📚 Documentation

Detailed documentation is available in the **docs/** directory.

---

## 🚀 Future Improvements

- Deploy NGINX Application
- Deploy Monitoring Stack
- Deploy Ingress Controller
- Automate Control Plane Installation
- Convert the project into a complete Infrastructure as Code solution
