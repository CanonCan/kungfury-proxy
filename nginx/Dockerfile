FROM docker.io/nginx:alpine

ADD config/nginx.conf /etc/nginx/nginx.conf
ADD config/kungfury.cert /etc/ssl/kungfury.cert
ADD config/kungfury.key /etc/ssl/kungfury.key
ADD config/proxy.conf /etc/nginx/proxy.conf

EXPOSE 80 443

STOPSIGNAL SIGQUIT

CMD ["nginx", "-g", "daemon off;"]
