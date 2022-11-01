# Kustomize-k8s

# Ref Doc Link
https://www.densify.com/kubernetes-tools/kustomize

# Install Kustomize
step1: curl -s "https://raw.githubusercontent.com/kubernetes-sigs/kustomize/master/hack/install_kustomize.sh"  | bash

Step2: sudo mv kustomize /usr/local/bin

step3: kustomize -h

# Deploy Application

Lets see if production values are being applied by running
-> kustomize build overlays/prod

Once you have reviewed, apply your overlays to the cluster with 
-> kubectl apply -k overlays/prod
