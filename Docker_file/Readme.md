## Dockerfile Basics
  FROM - Imports Base image from docker hub
  COPY - Copies content to docker image 
  ENV - Sets environment variables
  RUN - Runs commands in image
  CMD - Runs commands while creating container 
  Expose - Expose image to particular port
  
  
## Create your first docker file
   Create a file called 'Dockerfile'
   Paste the below content and save it
   
   'FROM centos:centos7
   
    RUN yum update -y
    
    CMD ["echo", "Hello, Welcome to Devops-World"]'

## Build Customized Docker Image from Dockerfile
   'docker build -t myfirstimage .'
   
## Run docker container
   'docker run myfirstimage'
   
## After running container
   It should give below output
   
    Hello, Welcome to Devops-World
