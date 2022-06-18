FROM alpine:latest

# Install packages and remove default server definition
RUN apk --no-cache add \
  curl \
  supervisor \
  bind

RUN mkdir -p /etc/bind/zone
RUN mkdir -p /run/named
RUN chown named.named -Rf /run/named

WORKDIR /