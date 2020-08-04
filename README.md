# Kubernetes-BuildBreakFix
## Let's start with Docker
![](https://docs.docker.com/engine/images/architecture.svg | width=50)
### 1. Install Docker
`https://docs.docker.com/get-docker/`

### Docker Hello-world
`PS C:\Users\user1\Lab> docker run hello-world`
```Unable to find image 'hello-world:latest' locally
latest: Pulling from library/hello-world
0e03bdcc26d7: Pull complete
Digest: sha256:49a1c8800c94df04e9658809b006fd8a686cab8028d33cfba2cc049724254202
Status: Downloaded newer image for hello-world:latest

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/
```
### 2. DockerHub 
 Docker Hub  
 `https://hub.docker.com/r/dockercloud/hello-world`

### 3. Build and run from docker file
Clone  
`git clone https://github.com/docker-archive/dockercloud-hello-world.git`<br>
`cd .\dockercloud-hello-world\`  


Build  
`docker build --tag example:1.0 .`  


Run  
`docker run -p 80:80 example:1.0`  

### 4. List, stop and remove existing Containers and Images
`docker ps`  
`docker images`  
`docker image rm <imageid>`  
`docker container ls -a`  
`docker container rm <containerid>`  
## Kubernetes
Kubernets Architecture  
![](https://www.guru99.com/images/1/061419_0430_KubernetesT1.png)

### 5. Configure Kubernetes Cluster
1. Start up 3 VMs 1 Master node and 2 worker nodes)
2. Install Docker, kubectl, kubelet, kubeadm.     
<img src='/images/KubernetesArchitecture_1.png'  width=350/>
3. 


`kubectl exec --stdin --tty shell-demo -- /bin/bash`
