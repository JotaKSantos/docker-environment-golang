FROM golang:1.19.1

ARG user
ARG uid

RUN apt update && apt install --no-install-recommends -y \
        git gpg gnupg gpg-agent socat

ENV GOPATH=

RUN groupadd --gid $uid $user \
    && useradd --uid $uid --gid $uid -m $user

# WORKDIR /var/www

USER $user