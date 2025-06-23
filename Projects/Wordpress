Deploy WordPress on Kubernetes with Nginx and MySQL

git clone https://github.com/techiescamp/kubernetes-projects.git

cd kubernetes-projects
CD into 04-WordPress-deployment
CD into the Docker
docker build -t monudocker334/wordpress-nginx-k8s:latest .
docker push monudocker334/wordpress-nginx-k8s:latest
docker rmi ImageID
******************************************************************************************
kubectl create ns wordpress

Run the following command to set the WordPress namespace as the default namespace.
kubectl config set-context --current --namespace=wordpress

echo -n '<data>' | base64
echo -n 'admin@123' | base64
kubectl apply -f secret.yaml
kubectl get secret

kubectl apply -f nginx-cm.yaml
kubectl apply -f mysql-cm.yaml
kubectl get cm

kubectl apply -f pvc.yaml
kubectl get pvc

kubectl apply -f mysql.yaml
kubectl get sts
kubectl get svc

kubectl apply -f wordpress.yaml
kubectl get deploy
kubectl get svc
kubectl get pvc
kubectl get pv

kubectl apply -f networkpolicy.yaml
kubectl get networkpolicy

Once every object has been created, try to access WordPress on the browser by searching on the 
browser as {node-IP:nodeport} or if you have configured the Ingress Controller, search the Domain 
name on the browser.
kubectl delete -f .
**********************************************************************************************************
kubectl delete all --all -n wordpress
This will delete:

All Pods
All Services
All Deployments
All ReplicaSets
Everything managed by kubectl get all
