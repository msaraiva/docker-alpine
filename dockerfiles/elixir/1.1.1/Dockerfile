FROM msaraiva/alpine-elixir-base:18.0
MAINTAINER Marlus Saraiva <marlus.saraiva@gmail.com>

ENV ELIXIR_VERSION 1.1.1

RUN apk --update add --virtual build-dependencies wget ca-certificates && \
    wget https://github.com/elixir-lang/elixir/releases/download/v${ELIXIR_VERSION}/Precompiled.zip && \
    mkdir -p /opt/elixir-${ELIXIR_VERSION}/ && \
    unzip Precompiled.zip -d /opt/elixir-${ELIXIR_VERSION}/ && \
    rm Precompiled.zip && \
    apk del build-dependencies && \
    rm -rf /etc/ssl && \    
    rm -rf /var/cache/apk/*

ENV PATH $PATH:/opt/elixir-${ELIXIR_VERSION}/bin

CMD ["/bin/sh"]
