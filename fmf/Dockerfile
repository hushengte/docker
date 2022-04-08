FROM disciples/nginx:1.0.0

COPY ./*.conf /etc/nginx/conf.d/

RUN mkdir -p /data/fmf.icu
COPY /usr/share/nginx/html/* /data/fmf.icu/
