# Deploying Node.js Application in Kubernetes


In this file, we will learn how to deploy a Node.js application in Kubernetes.

 First of all,we execute this command to start minikube  
``````
minikube start
``````
Then, we create a docker image for our node js app 
``````
docker build -t asmaeel/nodeimage .
``````

After that, we push the node js image to docker hub accout to use it for deployment
``````
docker push asmaeel/nodeimage:latest
``````

And we create two file one for deployment and one for service of the Node.js application in Kubernetes.
``````
vi deployment.yaml
vim service.yaml
``````
the codefor this two files is available in my github accout 

And Finally we execute this cmd to make the Node.js application available in Kubernetes.
``````
minikube service nodeapp-service
``````

By ASMAE ELAZRAK 

