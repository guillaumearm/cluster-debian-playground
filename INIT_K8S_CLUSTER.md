# Controller

### Init k8s cluster

```bash
kubeadm init --apiserver-advertise-address=192.168.122.10 --node-name $HOSTNAME --pod-network-cidr=10.244.0.0/16
```

### Install flannel

```bash
kubectl apply -f https://raw.githubusercontent.com/coreos/flannel/master/Documentation/kube-flannel.yml
```

### Check pods

```bash
kubectl get pod -A
```

### Check nodes

```bash
kubectl get nodes
```

# Workers
