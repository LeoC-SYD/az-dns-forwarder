FROM alpine@sha256:a8560b36e8b8210634f77d9f7f9efd7ffa463e380b75e2e74aff4511df3ef88c

COPY named.conf /etc/bind/

RUN apk add --update-cache --no-cache bind
EXPOSE 53/udp

ENTRYPOINT ["/usr/sbin/named", "-f", "-g"]
