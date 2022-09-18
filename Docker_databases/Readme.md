## Launch a mysql database container
     'docker run -itd -p 6666:3306 --name=myfirst_database --env="MYSQL_ROOT_PASSWORD=test123" --env="MYSQL_DATABASE=user_data" mysql'
   
         --name - Assigning a name to container
         --env - Environment variable to setup database & password
         
         Login to MYSQL Database
          'docker exec -it <container_id> /bin/bash'
         
         Now run mysql command in container to access created database
          'mysql -uroot -p'   - u for user and -p for password, it will promt for password enter password as test123
          
         Now check databses
          'show tables;'
          
          Now select database
           'use <database_name>'
           
          Now check tables
           'show tables'
         
         
## 
