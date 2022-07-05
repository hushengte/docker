FROM nginx:latest

COPY ./conf/nginx.conf /etc/nginx/nginx.conf
COPY ./conf/proxy.conf /etc/nginx/proxy.conf

COPY ./html/* /usr/share/nginx/html/