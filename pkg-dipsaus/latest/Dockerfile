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
    libcurl4-openssl-dev \
    libfftw3-dev \
    libfreetype6-dev \
    libfribidi-dev \
    libgit2-dev \
    libhdf5-dev \
    libharfbuzz-dev \
    libjpeg-dev \
    libpng-dev \
    libssl-dev \
    libssh2-1-dev \
    libtiff5-dev \
    libv8-dev \
    libxml2-dev \
    psmisc \
    procps \
    sudo \
    wget \
    zlib1g-dev \
  && install2.r --error --skipinstalled --deps TRUE \
    devtools fftwtools hdf5r fst \
    dipsaus lazyarray threeBrain raveio \
  && Rscript --verbose --vanilla -e "devtools::install_github('dipterix/rutabaga', upgrade = FALSE, force = TRUE)"

