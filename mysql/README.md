# Quick start

## Building The Image:

Access the project's root folder and build the image MySQL :

```
  docker build -t mysql-image -f ./mysql/db/Dockerfile 
```
## Running The Container Mysql:

In the root folder of the project, run :

```
  docker run -d -v $(pwd)/mysql/db/data:/var/lib/mysql -p 3306:3306 --rm --name TestMysql mysql-image
```

## Now Do Your Database:

```
  docker exec -i TestMysql mysql -uroot -proot < ./mysql/db/script.sql
```
