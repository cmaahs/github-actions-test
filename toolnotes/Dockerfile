FROM debian:stable-slim

ARG USER=cmaahs
ENV HOME /home/$USER

RUN apt-get update \
    && apt-get install -y bash jq net-tools curl wget

# add new user
RUN adduser --disabled-password --gecos "" $USER

USER $USER
WORKDIR $HOME
