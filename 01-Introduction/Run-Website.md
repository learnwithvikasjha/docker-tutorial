# Create a website
Let's create a demo website. I am going to use this HTML.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Website</title>
</head>
<body>
    <header>
        <h1>Welcome to My Website</h1>
    </header>
    <div>
        <p>This is a sample HTML website. You can replace this text with your own content.</p>
    </div>
</body>
</html>

```

# Map local directory to docker container's volume

```
docker run -d -p 80:80 -v /path/to/your/local/directory:/usr/share/nginx/html --name my-web-server nginx
```
