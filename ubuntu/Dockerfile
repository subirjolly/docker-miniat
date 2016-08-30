FROM debian:sid
MAINTAINER Subir Jolly <subirjolly@gmail.com>
VOLUME /root/miniat
WORKDIR /root/miniat

RUN echo 'debconf debconf/frontend select Noninteractive' | debconf-set-selections
RUN apt-get update
RUN apt-get install -y apt-utils
RUN apt-get -y upgrade
RUN apt-get install -y ca-certificates --no-install-recommends

RUN apt-get install -y make \
    rpm \
    gcc \
    scons \
    python \
    flex \
    libncurses5-dev

RUN apt-get install -y doxygen \
    sqlite3
