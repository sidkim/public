FROM ubuntu:20.04
RUN \
  apt update && apt install nginx -y && \
  rm -rf /var/lib/apt/lists/* && \
  echo "\ndaemon off;" >> /etc/nginx/nginx.conf && \
  chown -R www-data:www-data /var/lib/nginx
EXPOSE 80
WORKDIR /etc/nginx
CMD ["nginx"]
