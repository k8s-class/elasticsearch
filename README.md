⚡ helm repo add akomljen-charts \
    https://raw.githubusercontent.com/komljen/helm-charts/master/charts/

⚡ helm install --name es-operator \
    --namespace logging \
    akomljen-charts/elasticsearch-operator
  
⚡ kubectl get pods -n logging

⚡ helm install --name efk \
    --namespace logging \
    akomljen-charts/efk
    
⚡ kubectl get pods -n logging
⚡ kubectl port-forward efk-kibana-6cf88598b6-xlkv2 5601 -n logging


Open your web browser at http://localhost:5601 and you should see Kibana dashboard
