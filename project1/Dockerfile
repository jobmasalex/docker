#Primer BEST PRACTICKS

FROM alpine:3.16.0
#FROM alpine
#FROM debian

#COPY . /opt/

#ENV Nginx_Version 1.22.0-r0

#RUN apk add --no cache --repository https://pkgs.alpinelinux.org/package/edge/main/x86_64/nginx=${Nginx_Version} \
#     && mkdir -p /run/nginx

RUN apk add --no-cache nginx && mkdir -p /run/nginx

#RUN  apt-get update && apt-get install -y \
#     curl \      Alfavitniy poryadok
#     mc \

#      nginx \

#     zsh

#      && rm -rf /var/lib/apt/lists/*

#RUN apt-get update
#RUN apt-get install -y nginx

#COPY custom.conf /etc/nginx/conf.d/

EXPOSE 80

COPY custom.conf /etc/nginx/conf.d/

COPY . /opt/

CMD ["nginx", "-g", "daemon off;"]