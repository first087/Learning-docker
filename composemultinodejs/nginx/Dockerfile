FROM labdocker/alpine:latest
MAINTAINER Artit Kiuwilai (first087@gmail.com)
LABEL Description="NodeJS/NGINX Build Container" Version="1.0"
RUN apk update && \
    apk add nginx
COPY nginx.conf /etc/nginx/nginx.conf
WORKDIR /usr/sbin
ENTRYPOINT ["nginx","-c","/etc/nginx/nginx.conf"]
EXPOSE 8080