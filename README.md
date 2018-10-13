## About 

This repo gives you out of the box set of docker container to start local php-mysql-nginx project on your local machine. Nothing else needed, except docker installed on your mac/windows/linux. 

### Contains

+ PHP 7.2 with many modules, incl.
  + gd
  + mbstring
  + pdo_mysql
  + addtionaly in container: zip, vim, yarn
+ MySQL 5.7
+ NGINX 1.13.8
  + Confiured to show /public folder on the project



## To start

Clone the repo, then run  ` docker-compose up -d`
and visit http://127.0.0.1 in your browser
Other useful commands:
+ `docker-compose ps` - shows you status of your containers (by nqinx "demon off" doesn't mean is not working)
+ `docker-compose stop`
+ `docker-compose build --no-cahe` when you need to rebuild without cached images (for ex. when php dockerfile was modified)

