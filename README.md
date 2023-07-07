### nginx
docker build -t disciples/nginx:1.0.0 ./nginx
docker run -v /data/nginx/conf/:/etc/nginx/conf.d -v /data/nginx/certs/:/etc/nginx/certs -v /data/nginx/logs/:/var/log/nginx -v /data/www/:/data/www -p 80:80 -p 443:443 -d disciples/nginx:1.0.0

### mysql
docker build -t disciples/mysql:1.0.0 ./mysql
###### -e MYSQL_ROOT_PASSWORD=[password]
docker run -v /data/mysql/:/var/lib/mysql -p 33066:3306 -d disciples/mysql:1.0.0

### redis
docker build -t disciples/redis:1.0.0 ./redis
docker run -v /data/redis/:/data -p 16379:6379 -d disciples/redis:1.0.0
