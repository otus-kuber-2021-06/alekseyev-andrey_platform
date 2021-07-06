FROM nginx

COPY ./homework.html /app/homework.html
COPY ./web.conf /etc/nginx/conf.d/default.conf
COPY ./nginx.conf /etc/nginx/nginx.conf

RUN useradd -u 1001 -g 101 otus
RUN chown otus: /var/cache/nginx

USER 1001

EXPOSE 8000

CMD ["nginx" , "-g" , "daemon off;"]