---
layout: post
category: linux
---

In this example, we combine 3 environments into one configuration file.

```
KUBECONFIG=~/.kube/config: \
~/k8s-configs/dev.kubeconfig: \
~/k8s-configs/prod.kubeconfig: \
~/k8s-configs/observe.kubeconfig \
kubectl config view --flatten > /tmp/config
```

Enjoy!

