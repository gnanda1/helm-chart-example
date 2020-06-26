# helm-chart-example
Helm Charts for NodeJS Sample Weather App 

Commands:

```

helm install gnanda1 .

````

````

export SAMPLE_NODE_PORT=$(kubectl get --namespace default -o jsonpath="{.spec.ports[0].nodePort}" services gnanda1-service)

export SAMPLE_NODE_IP=$(kubectl get nodes --namespace default -o jsonpath="{.items[0].status.addresses[0].address}")

And then open your web browser to http://${SAMPLE_NODE_IP}:${SAMPLE_NODE_PORT}" from the command line, eg:

open http://${SAMPLE_NODE_IP}:${SAMPLE_NODE_PORT}

```

# Delete helm chart.

helm uninstall gnanda1
