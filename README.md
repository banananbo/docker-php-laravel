# docker-compose for laravel
## usage
1. set up containers.  
  `docker-compose up -d`
2. create Laravel Project  
`docker-compose exec php laravel new [appname]`
3. edit nginx.conf  
`root /src/sample/public;`
4. restart nginx container  
`docker-compose nginx restart`
5. setting mysql  
`docker-compose exec mysql bash`  
`mysql -u root -p` (enter password 'root')
`GRANT ALL ON [appname].* TO [appname];`
`CREATE DATABASE [appname];`
