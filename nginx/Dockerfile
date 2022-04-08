FROM nginx:latest

COPY ./conf/* /etc/nginx/conf.d/
COPY ./html/* /usr/share/nginx/html/

RUN mkdir -p /data/nginx