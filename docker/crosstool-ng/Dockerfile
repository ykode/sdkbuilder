FROM ykode/sdkbuilder:latest
LABEL maintainer="Didiet Noor <dnoor@ykode.id>"

RUN useradd -ms /bin/bash ykode
USER ykode
WORKDIR /home/ykode

RUN git clone https://github.com/crosstool-ng/crosstool-ng \
    && cd crosstool-ng && ./bootstrap && ./configure --enable-local && make && cd .. \
    && mkdir ct-build
