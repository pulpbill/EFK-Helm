# EFK
ElasticSearch Fluent Bit and Kibana Helm chart for K8s (and some other things, like Beats/Filebeats) at AWS:

## First steps:
Get yourself a running Kubernetes cluster:
https://github.com/pulpbill/k8s-basics

Create a namespace, I'll use "monitoring" (so do the yamls in this repo):
```
kubectl create namespace monitoring
```

### I created this chart based on other repos / tutorials:
- https://github.com/jswidler/elasticsearch-kubed

- https://medium.com/google-cloud/a-guide-to-deploy-elasticsearch-cluster-on-google-kubernetes-engine-52f67743ee98

- https://github.com/helm/charts/tree/master/stable/fluent-bit


