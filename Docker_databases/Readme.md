## Launch a mysql database container
     'docker run -itd -p 6666:3306 --name=myfirst_database --env="MYSQL_ROOT_PASSWORD=test123" mysql'
   
         --name - Assigning a name to container
         --env - Environment variable to setup database & password
         
       Login to MYSQL Database
          'docker exec -it <container_id> /bin/bash'
         
       Now run mysql command in container to access created database
          'mysql -uroot -p'   - u for user and -p for password, it will promt for password enter password as test123
          
       Now check databses
          'show databses;'
          
       Create a Database
          'create database <database_name>;'
          
       Now select database
           'use <database_name>;'
           
       Now check tables
           'show tables;'
           
       Create a table called employees
           'create table employees (id int not null, name text );'
           
       Insert some data in to employees table
           'insert into employees (id,name) values (1, 'kishore');'
           'insert into employees (id,name) values (2, 'yaswanth');'
           
       Run a Simple SQL Query to see data in tables
            'select * from employees;'           
           
         
