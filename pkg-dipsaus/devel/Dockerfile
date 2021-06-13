FROM dipterix/diptools:latest

RUN apt-get update -qq \
	&& apt-get install -t unstable -y --no-install-recommends \
	libsodium-dev \
	&& install2.r --error fastmap dipsaus \
	&& Rscript --verbose --no-save -e "devtools::install_github('dipterix/restbatch', upgrade = FALSE, force = TRUE)"
#	&& Rscript --verbose --no-save -e "devtools::install_github('dipterix/dipsaus', upgrade = FALSE, force = TRUE)" \
#	&& Rscript --verbose --no-save -e "devtools::install_github('dipterix/farray', upgrade = FALSE, force = TRUE)" \
#	&& Rscript --verbose --no-save -e "devtools::install_github('dipterix/threeBrain', upgrade = FALSE, force = TRUE)"

# docker build --tag diptools:latest ./pkg-dipsaus/latest
# docker build --tag diptools:devel ./pkg-dipsaus/devel

# docker tag diptools:latest dipterix/diptools:20200724
# docker push dipterix/diptools:20200724
# docker tag diptools:latest dipterix/diptools:latest
# docker push dipterix/diptools:latest

# docker run -p 8787:8787 -d --name rave --mount type=bind,source="/Volumes/OneDrive/data",target=/data/ext -e ROOT=TRUE -e PASSWORD=password dipterix/rave:latest
# docker exec -ti rave addraveuser beauchamplab ...

