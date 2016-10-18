FROM alpine:3.4

RUN apk add --update nginx && \
    rm -rf /var/cache/apk/* && \
    rm -rf /tmp/* && \
    adduser -D -g '' -G www-data www-data

ADD nginx.conf /etc/nginx/
ADD symfony.conf /etc/nginx/conf.d/

CMD ["nginx"]

EXPOSE 80
EXPOSE 443
