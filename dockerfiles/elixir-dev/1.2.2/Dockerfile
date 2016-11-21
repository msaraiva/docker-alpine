FROM msaraiva/elixir:1.2.2
MAINTAINER Marlus Saraiva <marlus.saraiva@gmail.com>

RUN apk --update add erlang-crypto erlang-syntax-tools erlang-parsetools erlang-inets erlang-ssl erlang-public-key erlang-eunit \
    erlang-asn1 erlang-sasl erlang-erl-interface erlang-dev erlang-tools wget git && \
    rm -rf /var/cache/apk/*

RUN mix local.hex --force && \
    mix local.rebar --force

CMD ["/bin/sh"]
