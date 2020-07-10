# docker-laravel

## Constitution
* nginx:1.15.6
* php:7.2-fpm
* mysql:8.0
* phpmyadmin/phpmyadmin

## What to do after cloning
1. `docker-compose exec app bash`,`composer create-project --prefer-dist laravel/laravel app`

2. create .env
`DB_NAME=homestead
DB_USER=homestead
DB_PASS=secret
DB_PORT=13306
TZ=Asia/Tokyo`

3. Change mysql authentication(plugin) method
`"caching_sha2_password" -> "mysql_native_password"`

## port
* http://localhost:8000 (Laravel) 
* http://localhost:3000 (phpmyadmin)
