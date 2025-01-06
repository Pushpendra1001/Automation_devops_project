https://aws.amazon.com/
https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html

# aws configure

https://github.com/eksctl-io/eksctl/releases

# eksctl create cluster --name devopsproject

https://kubernetes.io/docs/tasks/tools/install-kubectl-windows/


################################ manual way ##################################
kubectl apply -f https://raw.githubusercontent.com/vimallinuxworld13/eks_istio_bookinfo_app/refs/heads/master/bookinfo.yaml

kubectl port-forward   svc  productpage  80:9080

kubectl delete all --all

##########################################################################


####################### GitOps ##########################################

kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml



kubectl config set-context --current --namespace=argocd


https://github.com/argoproj/argo-cd/releases

argocd login --core
or
cd Downloads
./argocd-windows-amd64.exe  login --core



argocd admin initial-password -n argocd
or
./argocd-windows-amd64.exe admin initial-password -n argocd


kubectl port-forward svc/argocd-server -n argocd 8080:443



https://github.com/
https://git-scm.com/downloads

echo "# devops_project_based_learning_2025_batch1" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M master
git remote add origin https://github.com/vimallinuxworld13/devops_project_based_learning_2025_batch1.git
git push -u origin master


curl https://raw.githubusercontent.com/vimallinuxworld13/eks_istio_bookinfo_app/refs/heads/master/bookinfo.yaml  -o bookinfo.yaml



git add .
git commit -m first .
git push


kubectl get pods -n default

kubectl port-forward  svc/productpage  -n default  80:9080


http://127.0.0.1/productpage








https://github.com/istio/istio/releases/tag/1.24.2


istioctl  install --set profile=demo


kubectl get pods -n istio-system

kubectl get svc  -n istio-system

kubectl label namespace default  istio-injection=enabled



kubectl delete pods  --all -n default


kubectl get pods -n default






kubectl apply -f bookinfo-gateway.yaml

or

curl https://raw.githubusercontent.com/vimallinuxworld13/devops_project_based_learning_2025_batch1/refs/heads/master/bookinfo-gateway.yaml -o bookinfo-gateway.yaml

git add .
git commit -m first .
git push



cd "C:\Users\Vimal Daga\Downloads\istio-1.24.2-win-amd64\istio-1.24.2\samples"

# kubectl.exe  apply -f addons/

istioctl  dashboard kiali















