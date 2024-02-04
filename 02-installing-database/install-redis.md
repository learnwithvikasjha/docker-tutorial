# 1. Installing Redis
Let's pull redis official image

```
docker pull redis
```

```
docker run -d --name my-redis-db -p 6379:6379 redis
```

# 2. Let's log in to Redis container

```
docker exec -it my-redis-db /bin/bash
```

# 3. Run some docker commands
Let's enter our course_name, objective and deadline

```
redis-cli
set course_name docker-demo
set objective mastering-docker-containers
set deadline mastering-in-3-days
```

# 4. Let's see if these values are saved

```
get course_name
get objective
get deadline
```

# 5. Restart our container and see what happens to the data
```
docker container restart <container_name or container_id>
```

# 6. Remove the current container
```
docker rm my-redis-db
```

# 7. Mount persistence storage to Redis
```
docker run -d --name my-redis-db -p 6379:6379 -v $(pwd)/redis_data:/data redis
```

# 8. Let's repeat steps 2, 3 4 and 5
We shouldn't lose data this time
