
```console
az k8sconfiguration create \
        --resource-group AzureArc \
        --cluster-name widebody2 \
        --name rudr-config \
        --operator-instance-name rudr-config \
        --operator-scope namespace \
        --operator-namespace rudr \
        --operator-params '--git-readonly --sync-garbage-collection' \
        --enable-helm-operator true \
        --helm-operator-chart-version 0.6.0 \
        --repository-url git://github.com/slack/rudr-gitops.git
```
