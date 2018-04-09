# docker-ubuntu16.04-postgresql9.6-nginx

## Description

This is a repository containing Dockerfile to create a Docker image consisting of:
1. Base Image: Ubuntu 16.04
2. Database: PostgreSQL 9.6
3. Web Server: Nginx 1.10.3

## Commands

### 1. Command to build the Docker image
```
sudo docker build -t docker-ubuntu16.04-postgresql9.6-nginx:1.0 .
```
### 2. Command to run the Docker image
```
sudo docker run -it -p 23001:5432 -p 23002:80 -p 23003:443 docker-ubuntu16.04-postgresql9.6-nginx:1.0
```
## Additional Information

### PostgreSQL credential information:
```
Username: sa

Password: 123
```

### Exposed Port:
1. 5432, for PostgreSQL
2. 80, for Nginx
3. 443, for Nginx

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details