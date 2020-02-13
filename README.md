
```console
az k8sconfiguration create \
        --resource-group AzureArc \
        --cluster-name widebody \
        --name rudr \
        --enable-helm-operator true \
        --helm-operator-chart-version 0.6.0 \
        --operator-instance-name rudr \
        --operator-params read-only \
        --operator-scope namespace \
        --repository-url git://github.com/slack/gitops-rudr

```
