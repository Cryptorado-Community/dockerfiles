FROM golang:1.13

ARG nebula_release

RUN git clone https://github.com/slackhq/nebula.git && \
    cd nebula && \
    git checkout "${nebula_release}" && \
    make install

WORKDIR /etc/nebula
