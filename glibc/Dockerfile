# Copyright (c) 2016-2018 Accupara Inc. All rights reserved
FROM accupara/ubuntu:16.04
MAINTAINER Accupara Inc. "contact@accupara.com"

RUN sudo apt-get update \
 && sudo apt-get install -y \
        gawk \
        autoconf \
        automake \
        bzip2 \
        flex \
        gettext \
        gperf \
        gzip \
        libgmp-dev \
        libisl-dev \
        libmpc-dev \
        libmpfr-dev \
        zip \
 && sudo apt-get build-dep -y gcc

# Use bash explicitely instead of the ubuntu default of dash
# Required for libtool to function properly
RUN sudo update-alternatives --install /bin/sh sh /bin/bash 100
