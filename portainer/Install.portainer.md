helm repo add portainer https://portainer.github.io/k8s/
helm repo update
helm install --create-namespace -n portainer portainer portainer/portainer --set enterpriseEdition.enabled=true --set service.type=ClusterIP --set tls.force=true