FROM msaraiva/elixir:1.1.1
MAINTAINER Marlus Saraiva <marlus.saraiva@gmail.com>

RUN echo 'http://dl-4.alpinelinux.org/alpine/edge/community' >> /etc/apk/repositories

RUN apk --update upgrade && apk --update add erlang-inets erlang-ssl erlang-public-key erlang-eunit \
    erlang-asn1 erlang-sasl erlang-erl-interface erlang-dev wget git && \
    rm -rf /var/cache/apk/*

RUN mix local.hex --force && \
    mix local.rebar --force

CMD ["/bin/sh"]
