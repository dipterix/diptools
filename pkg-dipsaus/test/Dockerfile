# Test file

FROM rocker/r-base:latest

LABEL maintainer="Zhengjia Wang <zhengjia.wang@rice.edu>" \
  org.label-schema.license="GPL-3.0" \
  org.label-schema.vcs-url="https://github.com/dipterix/diptools" \
  org.label-schema.vendor="Dipterix"

RUN apt-get update -qq \
  && apt-get install -y --no-install-recommends \
    file \
    git \
    libcairo2-dev \
    libclang-dev \
    libcurl4-openssl-dev \
    libedit2 \
    libfftw3-dev \
    libgit2-dev \
    libhdf5-dev \
    libssl-dev \
    libssh2-1-dev \
    libv8-dev \
    libxml2-dev \
    psmisc \
    procps \
    sudo \
    unixodbc-dev \
    wget \
    zlib1g-dev \
  && install2.r --error --skipinstalled --deps TRUE \
    devtools fftwtools hdf5r fst

# docker build --tag diptools:test ./pkg-dipsaus/test

