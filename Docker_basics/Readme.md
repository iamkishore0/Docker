## Install Docker in Centos/RHEL/Ubuntu/Debian
    Refer the below link to install Docker https://github.com/iamkishore0/Devops_Tools_Setup/tree/main/Docker
   
## Check Docker version
   'docker --version'
   
## Pull Docker Images
   'docker pull <image_name>'
   
    For Jenkins - 'docker pull jenkins/jenkins:lts'
    For Tomcat - 'docker pull tomcat'
   
## Check docker images
    'docker images'
   
## Create a Docker container from image
    'docker run <image_name>
     For jenkins - 'docker run -itd -p 8080:8080 jenkins/jenkins:lts'
        Arguments 
         i - interactive mode
         t - terminal
         d - detached
         p - port
 
## Check Docker Running Containers
    'docker ps'
   
## Check Docker all containers
    'docker ps -a'
         
## Port mapping
    Run Mutiple jenkins containers in multiple ports
   
    'docker run -itd -p 9000:8080 jenkins/jenkins:lts' - Container will run on 9000 port
   
    'docker run -itd -p 8090:8080 jenkins/jenkins:lts' - Container will run on 8090 port
   
    'docker run -itd -p 8082:8080 jenkins/jenkins:lts' - Container will run on 8082 port
   
    'docker run -itd -p 1234:8080 jenkins/jenkins:lts' - Container will run on 1234 port

## Restart a Docker container
    'docker restart <container_id>'

## Stop a running container
    'docker stop <container_id>'

## Start a stopped container
    'docker start <container_id>

## Remove a stoppped container
    'docker rm <container_id>'
   
## Remove a running container 
    'docker rm -f <container_id>'

## Remove a docker image
    'docker rmi <image_id>'

  
## Login to docker container
    'docker exec -it <container_id> /bin/bash'
   
## Create a docker image from container
    'docker commit <container_id> <new_image_name>' 
