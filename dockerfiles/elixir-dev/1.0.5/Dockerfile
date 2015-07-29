FROM msaraiva/elixir:1.0.5
MAINTAINER Marlus Saraiva <marlus.saraiva@gmail.com>

RUN apk --update add erlang-inets erlang-ssl erlang-public-key erlang-eunit \
    erlang-asn1 erlang-sasl erlang-erl-interface erlang-dev wget git && \
    rm -rf /var/cache/apk/*

RUN mix local.hex --force && \
    mix local.rebar --force

CMD ["/bin/sh"]
