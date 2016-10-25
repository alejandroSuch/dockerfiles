FROM alpine:latest

MAINTAINER Alejandro Such, https://github.com/alejandroSuch/

RUN apk update \
    && apk add --no-cache ca-certificates ruby ruby-rdoc ruby-irb ruby-dev build-base zlib-dev \
    && update-ca-certificates \
    && gem update \
    && gem install asciidoctor coderay\ 
    && gem install --pre asciidoctor-pdf asciidoctor-epub3 \
    && apk del ca-certificates ruby-dev build-base zlib-dev \
    && rm -rf /tmp/* /var/cache/apk/*
