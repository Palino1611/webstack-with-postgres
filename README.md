# webstack
postgres + nginx + php + redis

1. docker-compose starts postgres from alraedy created image named postgres:11
2. nginx and php use website data which we have stored on local server in /www/web
example of the index.php:
root@server:~# cat /www/web/index.php
<?php
echo phpinfo();
3. creadeDB/init.sql file - you can set what users or databases can be created at the time when the container is started

how to run it:
docker-compose up -d
