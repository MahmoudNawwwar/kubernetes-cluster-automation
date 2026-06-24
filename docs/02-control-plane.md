# Control Plane Installation

## Steps

- Install containerd
- Configure SystemdCgroup
- Enable CRI
- Install kubeadm
- Install kubelet
- Install kubectl
- Initialize the cluster

```bash
sudo kubeadm init --pod-network-cidr=10.244.0.0/16
```

Copy kubeconfig

```bash
mkdir -p ~/.kube
sudo cp /etc/kubernetes/admin.conf ~/.kube/config
sudo chown $(id -u):$(id -g) ~/.kube/config
```

Install Flannel

```bash
kubectl apply -f https://github.com/flannel-io/flannel/releases/latest/download/kube-flannel.yml
```
