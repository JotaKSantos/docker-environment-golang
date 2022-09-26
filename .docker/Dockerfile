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

RUN go install github.com/cweill/gotests/gotests@latest
RUN go install github.com/fatih/gomodifytags@latest
RUN go install github.com/josharian/impl@latest
RUN go install github.com/haya14busa/goplay/cmd/goplay@latest
RUN go install github.com/go-delve/delve/cmd/dlv@latest
RUN go install honnef.co/go/tools/cmd/staticcheck@latest
RUN go install golang.org/x/tools/gopls@latest