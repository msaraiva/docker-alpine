FROM alpine:3.2
MAINTAINER Marlus Saraiva <marlus.saraiva@gmail.com>

RUN apk --update add ncurses-libs && rm -rf /var/cache/apk/*

RUN echo 'http://dl-4.alpinelinux.org/alpine/edge/main' >> /etc/apk/repositories

CMD ["/bin/sh"]
