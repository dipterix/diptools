FROM rocker/r-base:latest

LABEL maintainer="Zhengjia Wang <zhengjia.wang@rice.edu>"

RUN apt-get update -qq \
  && apt-get install -y --no-install-recommends \
    file \
    git \
    libapparmor1 \
    libclang-dev \
    libcurl4-openssl-dev \
    libedit2 \
    libssl-dev \
    lsb-release \
    psmisc \
    procps \
    python-setuptools \
    sudo \
    wget \
    libxml2-dev \
    libcairo2-dev \
    libsqlite-dev \
    libmariadbd-dev \
    libmariadbclient-dev \
    libpq-dev \
    libssh2-1-dev \
    unixodbc-dev \
    libsasl2-dev \
    zlib1g-dev \
    libgit2-dev \
    libfftw3-dev \
    libv8-dev \
    libhdf5-dev \
  && install2.r --error \
    --deps TRUE \
    devtools \
    fftwtools \
    hdf5r \
    fst \
    dipsaus \
    lazyarray \
    threeBrain \
  && Rscript --verbose --vanilla -e "devtools::install_github('beauchamplab/raveio', upgrade = FALSE, force = TRUE)" \
  && Rscript --verbose --vanilla -e "devtools::install_github('dipterix/rutabaga', upgrade = FALSE, force = TRUE)"

