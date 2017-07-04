# docker-nginx-rdns

Nginx + [https rdns](https://github.com/flant/nginx-http-rdns) module

## Example 
```
server {
    listen        80;
    rdns double;

    location / {
        rdns_allow         google.* # accepts only connections from google domains
    }
}
```
