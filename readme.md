# Docker Nginx/PHP/MariaDB setup

This is configured using images available on DockerHub.

Everything is still customisable.

In this setup you get:
- NGINX 1.9.1
- PHP-fpm 7.4.9
- MariaDB 10.5.4 (2 instances)
- MariaDB 5.5.46
- phpmyadmin 5.0.2

I used these guides to set up PHP and NGINX:
- http://geekyplatypus.com/dockerise-your-php-application-with-nginx-and-php7-fpm/
- http://geekyplatypus.com/making-your-dockerised-php-application-even-better/

## Setup

Clone this repo.

To start up:

1. open terminal
2. in terminal, navigate to the directory where you cloned this repo
3. run the following command
```
docker-compose up
```

From your favorite browser you can access:
- NGINX server on localhost:8080
- PhpMyAdmin on localhost:7000

You can change the exposed ports in the `docker-compose.yml`-file.

Place your PHP-code in the `/src/site` directory.