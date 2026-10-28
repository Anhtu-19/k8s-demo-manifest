<<<<<<< HEAD
# k8s-demo-manifest
=======
#Báo cáo
>>>>>>> 174cf9f (add kubernetes manifests)
# Kubernetes Demo Manifest

Repo chứa Kubernetes manifest phục vụ thực hành GitOps với ArgoCD.

## Thành phần

- deployment.yaml: Triển khai 2 Pod Nginx.
- service.yaml: Cung cấp truy cập nội bộ tới các Pod.
- ingress.yaml: Khai báo định tuyến HTTP tới Service.

## Luồng GitOps

GitHub Manifest -> ArgoCD Application -> Sync -> Kubernetes Cluster

Deployment -> Pod
Service -> Truy cập Pod
Ingress -> Định tuyến HTTP tới Service

## Kiểm tra

kubectl get deployment
kubectl get pods
kubectl get svc
kubectl get ingress
