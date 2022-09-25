FROM golang:1.19.1

RUN apt update && apt install --no-install-recommends -y \
        git gpg gnupg gpg-agent socat

ENV GOPATH=
RUN go install golang.org/x/tools/gopls@latest
RUN go install github.com/go-delve/delve/cmd/dlv@latest