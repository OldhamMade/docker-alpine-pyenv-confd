FROM oldhammade/alpine-pyenv-py3.4.5:0.2

MAINTAINER Phillip B Oldham <info@oldhammade.net>

LABEL name="Alpine + pyenv + py3.4.5 + confd" \
      distribution="alpine" \
      licence="MIT"

RUN apk add --no-cache wget && \
    wget https://github.com/kelseyhightower/confd/releases/download/v0.11.0/confd-0.11.0-linux-amd64 -O /usr/bin/confd && \
    chmod o+x /usr/bin/confd && \
    apk del wget && \
    pip install virtualenv
