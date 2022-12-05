# Git 2.38.1 for Debian 11-r16 -> https://docs.bitnami.com/tutorials/understand-rolling-tags-containers
FROM bitnami/git:2.38.1-debian-11-r16
LABEL maintainer="sebastian@sommerfeld.io"

RUN groupadd -g 1000 sebastian \
    && useradd -r -u 1000 -g sebastian sebastian \
    && chsh -s /bin/bash sebastian

USER sebastian
COPY assets/.gitconfig /home/sebastian/.gitconfig
