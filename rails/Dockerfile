FROM ruby:2.4.0

ENV LANG C.UTF-8


MAINTAINER YUKI HORITA <y-horita-42t@eagle.sophia.ac.jp>

RUN set -x && \
    apt-get -y update && \
    apt-get install -y postgresql && \
    gem install bootstrap && \
    apt-get install -y vim && \
    mkdir /root/.config &&\
    mkdir /root/.config/nvim &&\
    wget https://raw.githubusercontent.com/yuki-trans-am/init.vim/master/init.vim -P /root/.config/nvim &&\
    /etc/init.d/postgresql start &&\
    apt-get install sudo

WORKDIR /usr/src/rails

VOLUME /usr/src/rails

RUN echo



