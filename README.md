# Docker Nginx container

[![docker-drupal](https://img.shields.io/badge/spy86-nginx-blue.svg)](https://cloud.docker.com/repository/docker/spy86/nginx) [![Build Status](https://dev.azure.com/DevOpsSysOps/Docker/_apis/build/status/Docker%20Nginx?branchName=main)](https://dev.azure.com/DevOpsSysOps/Docker/_build/latest?definitionId=47&branchName=main)

## What is Nginx
Nginx is an open source reverse proxy server for HTTP/HTTPS/SMTP/POP3/IMAP protocols, we can use this well as a load balancer, HTTP cache, and a web server.

## How to use this image

### Simple use 
```
docker run --name nginx -v /tmp/content:/usr/share/nginx/html:ro -d spy86/nginx:latest
```

### Run with custom configuration
```
docker run --name nginx -v /tmp/nginx.conf:/etc/nginx/nginx.conf:ro -d spy86/nginx:latest
```
