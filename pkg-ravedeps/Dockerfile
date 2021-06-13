# designed for RAVE

FROM dipterix/diptools:latest

RUN apt-get update -qq \
  && apt-get install -y --no-install-recommends \
  && Rscript --verbose --no-save -e "remotes::install_github('dipterix/ravepy', upgrade = FALSE, force = TRUE)" \
  && Rscript --verbose --no-save -e "remotes::install_github('beauchamplab/ravebuiltins@migrate2', upgrade = FALSE, force = TRUE)" \
  && Rscript --verbose --no-save -e "remotes::install_github('beauchamplab/rave', upgrade = FALSE, force = TRUE)"
