# monitoring

![Photo by Bobby Stevenson on Unsplash](readme-pic.jpg)

k3d cluster create mycluster --agents 3 --api-port 6550
k3d cluster edit mycluster --port-add "30000-32767:30000-32767@server:0"

To install prometheus create user with:
sudo useradd --no-create-home --shell /bin/false prometheus


helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm repo add grafana https://grafana.github.io/helm-charts
helm repo add giantswarm https://giantswarm.github.io/giantswarm-catalog
helm repo add giantswarm-playground https://giantswarm.github.io/giantswarm-playground-catalog
helm repo add teleport https://charts.releases.teleport.dev
 helm repo add robusta https://robusta-charts.storage.googleapis.com && helm repo update
helm repo update