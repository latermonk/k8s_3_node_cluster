# k8s_3_node_cluster


ip：    
10.1.40.10  
10.1.40.69  
10.1.40.70  

==

Reference:

1.离线安装
https://github.com/Orientsoft/kubekit


2.实际的例子    
原文：     
https://www.sitepoint.com/kubernetes-deploy-node-js-docker-app/     

译文：    
http://blog.csdn.net/mrqingyu/article/details/76855901     




==

##  部署两个httpd节点
kubectl run httpd-app --image=httpd --replicas=2
kubectl run nginx-deployment --image=nginx:1.7.9 --replicas=2

查看部署状况：
kubectl get pod
kubectl get deployment
kubectl describe replicaset







