# docker-nginx-rdns

Nginx + [https rdns](https://github.com/flant/nginx-http-rdns) module

## usage

`docker pull quay.io/buildo/nginx-rdns`

## example conf file
```
server {
    listen        80;
    rdns double;

    location / {
        rdns_allow         google.* # accepts only connections from google domains
    }
}
```
