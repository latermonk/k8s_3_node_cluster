




==

##  部署两个httpd节点

###  kubectl 命令行创建节点     
kubectl run httpd-app --image=httpd --replicas=2    
kubectl run nginx-deployment --image=nginx:1.7.9 --replicas=2    

###  kubectl通过yaml文件创建
kubectl apply -f App1.yaml


查看部署状况：    
kubectl get pod     
kubectl get deployment     
kubectl describe replicaset      


部署流程：    
1.kubectl create a deployment    
2.deployment create a replicaSet    
3.replicaSet 创建pod     






Reference:

1.离线安装
https://github.com/Orientsoft/kubekit


2.实际的例子    
原文：     
https://www.sitepoint.com/kubernetes-deploy-node-js-docker-app/     

译文：    
http://blog.csdn.net/mrqingyu/article/details/76855901     

