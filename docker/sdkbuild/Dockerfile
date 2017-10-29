FROM ubuntu:xenial

LABEL maintainer="Didiet Noor <dnoor@ykode.id>"
RUN useradd -ms /bin/bash ykode

RUN dpkg --add-architecture i386 \
    && apt-get update -qq \ 
    && apt-get -qq -y install gcc gperf bison flex texinfo help2man make libncurses5-dev \
    build-essential git subversion cvs unzip whois ncurses-dev bc mercurial aptitude \
	python-dev libc6:i386 zlib1g:i386 libstdc++6:i386 \
    && apt-get clean

USER ykode
WORKDIR /home/ykode