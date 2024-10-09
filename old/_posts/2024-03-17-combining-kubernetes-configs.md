---
layout: post
category: linux
---

Combining kubernetes configs into a single file.

```
KUBECONFIG=~/.kube/config: \
~/k8s-configs/dev.kubeconfig: \
~/k8s-configs/prod.kubeconfig: \
~/k8s-configs/observe.kubeconfig \
kubectl config view --flatten > /tmp/config
```

Enjoy!

