FROM ubuntu:latest

RUN apt-get update -yq && \
    apt-get upgrade -yq && \
    apt-get install -yq build-essential \
                        software-properties-common

RUN add-apt-repository ppa:ubuntu-toolchain-r/test -y && \
    apt-get update -yq && \
    apt-get install -yq gcc-snapshot \
                        gcc-6 \
                        g++-6 \
                        make \
                        wget

WORKDIR /root/ucpp

RUN wget http://plg.uwaterloo.ca/~usystem/pub/uSystem/u++-7.0.0.sh && \
    sh u++-7.0.0.sh
