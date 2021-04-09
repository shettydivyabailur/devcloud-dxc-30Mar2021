# Ingress Cantroller required the following clusterroles bindings to be applied.
```
kubectl create clusterrolebinding add-on-cluster-admin   --clusterrole=cluster-admin   --serviceaccount=kube-system:default
kubectl create clusterrolebinding add-on-cluster-admin-1   --clusterrole=cluster-admin   --serviceaccount=default:default
```

```
kubectl get svc
kubectl get pods -o wide
curl 192.168.77.143
kubectl get rc
kubectl expose rc nginx-ingress-controller --type=NodePort
kubectl get svc
kubectl get pods -o wide
curl 172.42.42.102:31097
curl 172.42.42.102:31097 -H 'Host: helloworld-v1.example.com'
curl 172.42.42.102:31097 -H 'Host: helloworld-v2.example.com'
```

