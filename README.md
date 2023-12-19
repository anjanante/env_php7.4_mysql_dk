# This is a development environment for php 7.4.

After extracting the repository, run
`docker-compose up -d`

We find:
* mysql/phpmyadmin in 127.0.0.1:8080
* maildev in 127.0.0.1:8081
* www directory in 127.0.0.1:8741

## If you want to install symfony, for example
`docker exec www_docker_sf composer create-project symfony/website-skeleton project`

Configuring the database in the .env file

`DATABASE_URL=mysql://root:@db_mysql_sf:3306/db_name?serverVersion=5.7`

Configuring Maildev in the .env file

`MAILER_DSN=smtp://maildev_docker_sf:25`

![Symfony project](https://raw.githubusercontent.com/anjanante/env_php7.4_mysql_dk/main/sf5.4.33.png)

