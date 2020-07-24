FROM dipsaus:latest

RUN apt-get update -qq \
	&& apt-get install -t unstable -y --no-install-recommends \
	&& Rscript --verbose --vanilla -e "devtools::install_github('dipterix/dipsaus')" \\
	&& Rscript --verbose --vanilla -e "devtools::install_github('dipterix/lazyarray')" \\
	&& Rscript --verbose --vanilla -e "devtools::install_github('dipterix/threeBrain')"

# docker build --tag dipsaus:devel ./pkg-dipsaus/devel
