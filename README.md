#Download the values file
```
helm show values nats/nats > values.yaml 
```

# Install the Nats Server with helm
## Create Namespace

```
kubectl create namespace nats
```

```
helm install nats nats/nats --values values.yaml --namespace nats
```
