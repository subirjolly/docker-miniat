FROM debian:sid
MAINTAINER Subir Jolly <subirjolly@gmail.com>
VOLUME /root/miniat
VOLUME /root/scripts
WORKDIR /root/miniat

RUN echo 'debconf debconf/frontend select Noninteractive' | debconf-set-selections
RUN apt-get update
RUN apt-get install -y apt-utils
RUN apt-get -y upgrade
RUN apt-get install -y ca-certificates --no-install-recommends

RUN apt-get install -y make \
    procps \
    xtail \
    rsyslog \
    rpm \
    gcc \
    scons \
    python \
    flex \
    libncurses5-dev

RUN apt-get install -y doxygen \
    sqlite3

RUN export PATH=$PATH:~/miniat/out/exe
RUN export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:~/miniat/out/lib
