# Lab Setup

## Environment

- VMware Workstation
- Ubuntu 24.04 LTS

## Virtual Machines

| Node | vCPU | RAM | Role |
|------|------|-----|------|
| master | 2 | 4 GB | Control Plane |
| host1 | 2 | 4 GB | Worker |
| host2 | 2 | 2 GB | Worker |

## Network

| Node | IP |
|------|-------------|
| master | 192.168.137.128 |
| host1 | 192.168.137.133 |
| host2 | 192.168.137.134 |

## Software

- Kubernetes v1.34.9
- containerd
- Flannel CNI
- Ansible
