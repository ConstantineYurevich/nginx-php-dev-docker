# Nginx-PHP-Dev Docker Image

Docker Image with Nginx+PHP+XDebug that has everything you may need for integration with PHPStorm

# Intallation

To make this image work with your local source code you should have the following folder structure:

```
<your project dir>
  /config
    nginx-app.conf
    php-app.conf
  /http
  /logs
    /profiler
  /secure
```

# Running image

```
docker run -v <full path to your project dir>:/data -p 80 yurevichcv/nginx-php-dev:latest
```


# PHPStorm Deployment Config Setup

- Type: `SFTP`
- SFTP Host: `<Docker VM Host>`
- Port: `<Docker Container Mapped Port>`
- User name: `root`
- Auth type: `password`
- Password: `root`
