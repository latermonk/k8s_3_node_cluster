
# 准备代码和Dockerfile

书写Dockerfile & server.js文件    

#  构建dcoker镜像   

##  构建镜像并提交[方法一]
docker build -t ibackchina2018/hello-baby:v1   .    
docker push  ibackchina2018/hello-baby:v1        

##  从dockerhub构建镜像[方法二] 
使用https://github.com/latermonk/k8s_3_node_cluster/的代码
在 docker hub 构建镜像

#  部署单个应用     

kubectl run hello-baby --image=ibackchina2018/hello-baby:v1 --port=8080    


#   应用暴露出来
kubectl expose deployment/hello-baby \
 --type="NodePort"\      
 --port 8080
 
curl访问应用

 
#   scale up App   

kubectl scale deployments/hello-baby  --replicas=2    

curl访问应用  


