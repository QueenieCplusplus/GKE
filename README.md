# GKE
vm, container, app, registry, cluster, pod, kubectl tool

![gke](https://cdn.qwiklabs.com/ZB%2FLTu%2FfOBuu7svaY0%2Fier%2FSvbJdfF3Lrb%2F5woXeecI%3D)


steps:

(1) create VM

(2) create APP, pack app into Container Image

(3) push Image to Container Registry

(4) create Cluster and Pod

(5) allow External Traffic

(6) scale & update service

(7) using K8s Dashboard


start from step 2:

> create a Nodejs Server 

* 2.1, in cloud shell, edit a js file

        vi server.js
        
* 2.2, using editor

        i
        
* 2.3, js file

       var http = require('http');
       
       var reqHandler = function(req, res){
       
          res.writeHead(200);
          res.end('hi');
       
       }
       
       var www = http.createServer(reqHandler);
       www.listen(8080);

* 2.4, esc the file and save it

       ESC
       
       :wq
       
* 2.5, start server in shell

       node server.js
       
       
  

        
