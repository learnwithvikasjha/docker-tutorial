# Installing Docker
```
sudo yum install -y docker
```

# Adding our user in Docker Group, so that we can run it without using sudo everytime.
```
sudo usermod -aG docker $USER
newgrp docker
```

# Pulling a Docker Image
```
docker pull nginx
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
docker stop
```
