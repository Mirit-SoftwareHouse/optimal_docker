## Table of contents
* [General info](#general-info)
* [Setup](#setup)

## General info
This project is docker for laravel projects. Clone it somewhere and copy into existing project
	
## Setup

If you want other database name than `database` change 
```- MYSQL_DATABASE=database```
in `docker-compose.yml`

To run this:

```
$ docker-compose up -d
```
to enter into container with laravel
```
$ docker exec -it -u 1000:www-data laravel /bin/bash
```

Your laravel project is available on `project.localhost` if you want to change this 
edit `dockerfiles/local.conf` file

In your .env file set config:
`DB_HOST=mariadb`