FROM docker.io/alpine:latest

USER root
RUN apk add curl
RUN curl -sSfL -o /tmp/whoami.tar.gz https://github.com/traefik/whoami/releases/download/v1.10.1/whoami_v1.10.1_linux_amd64.tar.gz
RUN tar -C /usr/local/bin -xf /tmp/whoami.tar.gz whoami

ENV WHOAMI_PORT_NUMBER=3000
CMD ["/usr/local/bin/whoami"]
