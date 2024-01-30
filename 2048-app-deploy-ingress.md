# 2048 App

## Create Fargate profile

```
eksctl create fargateprofile \
    --cluster eks-cluster-2048 \
    --region <REGION> \
    --name alb-sample-app \
    --namespace game-2048
```

## Deploy the deployment, service and Ingress

```
kubectl apply -f deploy.yml
kubectl apply -f service.yml

```