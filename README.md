# EFK
EasticSearch Fluent Bit and Kibana for K8s (and some other things, like Beats/Filebeats) at AWS:

## First steps:
Get yourself a running Kubernetes cluster:
https://github.com/pulpbill/k8s-basics


### ElasticSearch cluster:

We are going to focus first on an ES cluster:

1. Create a Storage Class on your cluster:

```
kind: StorageClass
apiVersion: storage.k8s.io/v1
metadata:
  name: standard
provisioner: kubernetes.io/aws-ebs
parameters:
  type: gp2
reclaimPolicy: Retain
mountOptions:
  - debug
volumeBindingMode: Immediate
```


