# Installing Docker
```
sudo yum install -y docker
```

# Adding our user in Docker Group, so that we can run it without using sudo every time.
```
sudo usermod -aG docker $USER
newgrp docker
```

# Pulling a Docker Image
```
docker pull nginx
```

# Seeing list of Docker Images
```
docker images
```

# Running Nginx
```
docker run -d -p 80:80 --name my-web-server nginx
```

# Checking Running Docker Containers
```
docker ps
```

# Stopping Docker 
```
docker stop <container_name or container_id>
```

# Starting a stopped container
```
docker start <container_name or container_id>
```

# Removing a container
```
docker rm <container_name or container_id>
```
