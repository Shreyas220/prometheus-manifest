# prometheus-manifest

### steps 
```
kubectl create -f https://raw.githubusercontent.com/prometheus-operator/prometheus-operator/master/bundle.yaml
kubectl create namespace monitoring
kubectl apply -f ./manifests-1.23.0/prometheus/
kubectl apply -f ./manifests-1.23.0/grafana/
kubectl port-forward pod/prometheus 9090
kubectl port-forward pod/grafana 3000
```
