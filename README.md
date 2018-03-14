
====


#  部署单个应用

kubectl run hello-baby --image=ibackchina2018/hello-baby:v1 --port=8080    


#   应用暴露出来
kubectl expose deployment/hello-baby \
 --type="NodePort"\      
 --port 8080
 
 
#   scale up App

kubectl scale deployments/hello-baby  --replicas=2




