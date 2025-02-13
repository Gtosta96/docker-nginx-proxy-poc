FROM nginx:1.22
RUN apt update && apt-get -y install vim htop curl wget

COPY ./proxy.nginx /etc/nginx/nginx.conf