## About 

This repo gives you out of the box set of docker containers to run php-mysql-nginx project on your local machine. Nothing else needed, except docker installed on your mac/windows/linux. 

### Contains

+ PHP 7.4 with many modules, incl.
  + mbstring
  + bcmath
  + pdo_mysql
  + additionally in container: zip, vim, yarn
+ MySQL 5.7
+ NGINX 1.13.8
  + Configured to show /public folder 



## To start

Clone the repo, then run  ` docker-compose up -d`
and visit http://127.0.0.1 in your browser

Other useful commands:
+ `docker-compose ps` - shows you status of your containers (by nqinx "demon off" doesn't mean is not working)
+ `docker-compose stop`
+ `docker-compose build --no-cache` when you need to rebuild without cached images (for ex. when php dockerfile was modified)
+ `docker exec -it YOUR_PHP_CONTAINER_NAME bash` to enter bash in your php container, name of wich you can check using `docker-compose ps`

### To access db via sequel pro/workbench/dbver
+ port: `3306`
+ user: `dbuser`
+ password: `secret`
+ database: `website`

### Contribution
Welcome :) please do it by PR.