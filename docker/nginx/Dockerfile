FROM nginx:latest

COPY uwsgi_nginx.conf /etc/nginx/conf.d/default.conf

CMD ["nginx", "-g", "daemon off;","-c","/etc/nginx/nginx.conf"]