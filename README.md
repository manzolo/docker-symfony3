# docker-symfony3

## Add virtualhost to /etc/hosts
```bash
echo "127.0.0.1 symfony3demo.localhost" >> /etc/hosts
```

```bash
git clone https://github.com/manzolo/docker-symfony3.git
cd docker-symfony3/
docker build -t manzolo/docker-symfony3 .
```
##Enter shell
```bash
docker run -it manzolo/docker-symfony3 /bin/bash
```
##Launch web server
```bash
docker run -d -p 8080:80 -p 33060:3306 manzolo/docker-symfony3
```
##test
```
symfony3demo.localhost:8080
```
