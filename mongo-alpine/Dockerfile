FROM alpine:edge

RUN apk add mongodb \
        --update-cache \
        --repository http://dl-4.alpinelinux.org/alpine/edge/testing \
        --allow-untrusted && \
    rm -rf /var/cache/apk/* && rm -rf /tmp/*

VOLUME /data/db

EXPOSE 27017

CMD ["mongod"]
