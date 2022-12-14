   **VOLUMES**

## Create a volume
   'docker volume create <volume_name>'
   
## Check volumes
   'docker volume ls'
   
## Delete volumes
   'docker volume rm <volume_id>'
   
   
   
   **NETWORKS**
   
## Create a network
   'docker network create <network_name>'
   
## Check networks
   'docker network ls'
   
## Inspect docker network
   'docker network inspect <network_id>'
   
## Change Containers Network
   Disconnect from existing network
   
   'docker network disconnect <network_id> <container_id>'
   
   
   Attach new network
   
   'docker network connect <network_id> <container_id>'
