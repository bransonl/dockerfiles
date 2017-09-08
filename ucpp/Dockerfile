FROM ubuntu:latest

RUN apt-get update -yq && apt-get upgrade -yq && apt-get install build-essential software-properties-common -yq
RUN add-apt-repository ppa:ubuntu-toolchain-r/test -y && apt-get update -yq && apt-get install gcc-snapshot gcc-6 g++-6 make wget -yq

RUN cd ~ && mkdir ucpp && cd ucpp && wget http://plg.uwaterloo.ca/~usystem/pub/uSystem/u++-7.0.0.sh && sh u++-7.0.0.sh
