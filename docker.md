# Most useful Docker commands

**Connect to a container using sh :**
```linux
docker exec -ti container_id sh
```

**Run an ubuntu container and kill it when you exit**
```linux
docker container run --interactive --tty --rm ubuntu bash
```
* --interactive says you want an interactive session.
* --tty allocates a pseudo-tty.
* --rm tells Docker to go ahead and remove the container when it’s done executing.

**docker container exec** allows you to run a command inside a container.
Example : show the mysql version of a running container :
```linux
 docker exec -it mydb \
 mysql --user=root --password=$MYSQL_ROOT_PASSWORD --version
 ```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTQyMDIwNzIxNV19
-->