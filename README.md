### testing flannel with kind.

Grab the kube-flannel manifest and put it in /tmp/

```
curl -L https://git.io/kube-flannel.yaml > /tmp/kube-flannel.yaml
```

Then start a new kind cluster with the config in [./kind](./kind/config)

This will bring up a 6 node cluster with flannel as the cni.

3 cp node and 3 worker nodes.
