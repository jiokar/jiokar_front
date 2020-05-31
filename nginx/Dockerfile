FROM nginx:latest
MAINTAINER jiokar

RUN echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list
RUN apt-get update
RUN apt-get install certbot python-certbot-nginx -t stretch-backports -y

#COPY ./html /usr/share/nginx/html
COPY ./nginx.conf /etc/nginx/conf.d/