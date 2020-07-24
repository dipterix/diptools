FROM rocker/r-base:latest

LABEL org.label-schema.license="GPL-3.0" \
      org.label-schema.vcs-url="https://github.com/dipterix/diptools" \
      org.label-schema.vendor="Dipterix's personal repositories" \
      maintainer="Zhengjia Wang <zhengjia.wang@rice.edu>"

RUN apt-get update -qq \
	&& apt-get install -t unstable -y --no-install-recommends \
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
	&& install2.r --error \
    --deps TRUE \
    BiocManager \
    devtools \
    dipsaus \
    lazyarray \
    threeBrain

# docker build --tag dipsaus:latest ./pkg-dipsaus/latest
