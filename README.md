# wordpress-as-docker


## Installation

Create '''.env''' File with some project specific values
```
PROJECT_NAME=name which ist used for docker group
PORT=port where wordpress is listening
MYSQL_PASSWORD=<generated password>
```


### Crete certs

```
mkdir certs
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout certs/selfsigned.key -out certs/selfsigned.crt
```


```
docker-compose up -d 
```


