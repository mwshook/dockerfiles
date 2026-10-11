FROM alpine:3.24@sha256:294b683cb724975bec92580e1e685676bd4b50bda910ddb8c51d4cabeaec77e6

LABEL org.opencontainers.image.source=https://github.com/hairyhenderson/dockerfiles

ENV PAGER /usr/bin/moor
ENV EDITOR /usr/bin/micro
ENV VISUAL /usr/bin/micro

RUN apk add --no-cache mandoc man-pages util-linux-doc e2fsprogs-doc moor micro openssh
RUN rc-update add sshd

USER 42000:42000

ENTRYPOINT ["man"]
