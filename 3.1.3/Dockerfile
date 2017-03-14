FROM alpine:3.5

MAINTAINER "The Ignorant IT Guy" <iitg@gmail.com>

RUN apk update \
  && apk add iperf3 \
  && rm -rf /var/cache/apk/*

ENTRYPOINT ["/usr/bin/iperf3"]
