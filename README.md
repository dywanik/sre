# SRE Coding Challenge for Fiscaly

Here you will find my answers to the coding challenge. I start with requirements for all the tools I use. All of them are for mac.

## Requirements

- docker
- iproute2mac

## Docker container

I am using official nginx image for the "Hello world!" part - https://hub.docker.com/_/nginx

### Running container

0. Check your local network IP

```
ip addr show | grep inet
```

1. Copy this repo to your local machine and run:

```
docker build -t my-nginx .
```

2. Run the container and expose required port:

```
docker run -p 8080:80 my-nginx
```

3. Go to http://localhost:8080/ or http://<your.local.ip>:8080/
