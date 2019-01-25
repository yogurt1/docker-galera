# docker-galera

Docker image for MariaDB Galera cluster
Based on [serveralnines/galera-docker-mariadb](https://github.com/severalnines/galera-docker-mariadb)

Entrypoint modified to support secrets:

+ MYSQL_ROOT_PASSWORD_FILE -> MYSQL_ROOT_PASSWORD
+ XTRABACKUP_PASSWORD_FILE -> XTRABACKUP_PASSWORD

And you can run `garbd`, check `Swarm` example

## Examples

+ [Swarm](examples/swarm/)

## PS



Thanks @severalnines

Check base repo for more info