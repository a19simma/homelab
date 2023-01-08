# Cluster configuration using Argo-CD

## Install CNI

apply the calico helm chart with the provided values file in .\cni

```
kubectl create ns tigera-operator
helm install calico  projectcalico/tigera-operator -n tigera-operator
kubectl apply -f .\calico-ippoll.yml
```

Calico may have issues uninstalling some of its Service account and be stuck in the cluster

```
kubectl patch -n calico-system ServiceAccount/calico-node --type json --patch='[{"op":"remove","path":"/metadata/finalizers"}]'
```
