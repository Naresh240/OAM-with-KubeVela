# OAM-with-KubeVela

# Minikube Installation
  [minikube Installation](https://github.com/Naresh240/kubernetes/tree/main/minikube-setup)
# Enable minikube ingress
  minikube addons enable ingress
# Install Kubevela
  curl -fsSl https://kubevela.io/script/install.sh | bash -s 1.3.4
  vela install
  
  Helm:
  
  helm repo add kubevela https://charts.kubevela.net/core
  helm repo update
  helm install --create-namespace -n vela-system kubevela kubevela/vela-core --version 1.3.4 --wait
# Run Application
  vela up -f oam-springboot.yml
