FROM resin/rpi-raspbian:jessie
MAINTAINER Patrick Aikens <paikens@gmail.com>

ADD . /bd_build

RUN /bd_build/prepare.sh && \
    /bd_build/system_services.sh && \
    /bd_build/utilities.sh && \
    /bd_build/cleanup.sh

cmd ["/sbin/my_init"]
