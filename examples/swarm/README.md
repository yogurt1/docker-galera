# Swarm example

## Deployment

1. Create overlay network

```sh
docker network create --driver overlay galera
```

2. Create secrets

```sh
echo ... | docker secret create mysql_root_password -
echo ... | docker secret create xtrabackup_password -
```

3. Deploy stack

```sh
docker stack deploy galera -c docker-stack.yml
```

Now you can access Galera on `galera` network by `galera` hostname
