## Execute your first docker file
  Create a File called docker-compose.yml & edit that file paste the below yaml configuration file and save it
  
version: "3"

services:
  wordpress_website:
    image: wordpress:latest
    ports:
      - "8090:80"
    depends_on:
      - mysql
    environment:
      WORDPRESS_DB_HOST: mysql
      WORDPRESS_DB_USER: root
      WORDPRESS_DB_PASSWORD: "password"
      WORDPRESS_DB_NAME: wordpress
    networks:
      mynetwork:
        

  mysql:
    image: "mysql:5.7"
    environment:
      MYSQL_DATABASE: wordpress
      MYSQL_ROOT_PASSWORD: "password"
    volumes:
      - ./mysql:/var/lib/mysql
    networks:
      mynetwork:
        

networks:
  mynetwork:
    ipam:
      driver: default
      
      
## Execute Docker compose file
    'docker compose up -d'
    
## Check Docker compose containers status
    'docker compose ls'
    
## Down docker compose containers
    'docker compose down'
    
## Down docker compose containers including volumes
    'docker compose down -v'

