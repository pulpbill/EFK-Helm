# EFK
EasticSearch Fluent Bit and Kibana for K8s (and some other things, like Beats/Filebeats) at AWS:

## First steps:
Get yourself a running Kubernetes cluster:
https://github.com/pulpbill/k8s-basics

Create a namespace, I'll use "monitoring":
```
kubectl create namespace monitoring
```

### ElasticSearch cluster:

We are going to focus first on an ES cluster:

1. Create a Storage Class on your cluster:



