# Installing Redis
Let's pull redis official image

```
docker pull redis
```

```
docker run -d --name my-redis -p 6379:6379 redis
```

# Let's log in to Redis container

```
docker exec -it my-redis /bin/bash
```
