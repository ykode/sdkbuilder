FROM ykode/sdkbuilder:latest
LABEL maintainer="Didiet Noor <dnoor@ykode.id>"

RUN useradd -ms /bin/bash ykode
USER ykode
WORKDIR /home/ykode

ADD ./arm-yk-linux-gnueabihf.linux-host.tar.gz /home/terra 
ADD ./buildroot-2017.08.1.tar.gz /home/terra