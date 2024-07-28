FROM ubuntu:20.04

RUN apt-get update && \
    apt-get install nginx -y && \
    echo "\ndaemon off;" >> /etc/nginx/nginx.conf && \
    apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

COPY index.html /var/www/html/index.html

CMD ["nginx"]