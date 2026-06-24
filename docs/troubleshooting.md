# Troubleshooting

## Swap Enabled

```bash
swapoff -a
```

---

## IP Forwarding

```bash
sysctl -w net.ipv4.ip_forward=1
```

---

## containerd

Verify

```bash
systemctl status containerd
```

---

## kubelet

```bash
systemctl status kubelet
```

---

## Nodes NotReady

Verify Flannel

```bash
kubectl get pods -n kube-flannel
```
