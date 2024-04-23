#install
kubectl create -f node-exporter.yaml 
kubectl create -f prometheus/rbac-setup.yaml
kubectl create -f prometheus/configmap.yaml
kubectl create -f prometheus/prometheus.deploy.yml
kubectl create -f prometheus/prometheus.svc.yml
kubectl create -f grafana/grafana-deploy.yaml
kubectl create -f grafana/grafana-svc.yaml
kubectl create -f grafana/grafana-ing.yaml
