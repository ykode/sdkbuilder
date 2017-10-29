FROM ykode/sdkbuilder:latest
LABEL maintainer="Didiet Noor <dnoor@ykode.id>"

RUN useradd -ms /bin/bash ykode
USER ykode
WORKDIR /home/ykode

ADD ./arm-yk-linux-gnueabihf.linux-host.tar.gz /home/ykode
ADD ./buildroot-2017.08.1.tar.gz /home/ykode

# This is to be able to share directory with the host
RUN mkdir -p /home/ykode/buildroot-2017.08.1/output
