# catalog-api-dotnet

docker
docker build -t lordaldi/catalog:v2 .

kubectl create secret generic catalog-secrets --from-literal=mongodb-password='<your-password>'

cd kubernetes
kubectl apply -f ./catalog.yaml
kubectl apply -f ./mongodb.yaml

kubectl get deployment
kubectl get service
kubectl get pods
kubectl get statefulset

-scale kubernetes pods
kubectl scale deployment/catalog-deployment --replicas=3
