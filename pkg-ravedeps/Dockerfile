# designed for RAVE

FROM dipterix/diptools:latest

RUN apt-get update -qq \
  && apt-get install -y --no-install-recommends \
  && install2.r --error --skipinstalled \
    shinyFiles servr reticulate shinyjs shinydashboard signal \
    colorspace viridisLite RColorBrewer munsell labeling farver scales \
    isoband gtable RcppEigen statmod nloptr minqa progress cellranger \
    zip tidyselect readr hms forcats openxlsx readxl haven sp RcppArmadillo matrixStats \
    conquer MatrixModels SparseM lme4 ggplot2 numDeriv mvtnorm rio \
    maptools quantreg pbkrtest carData shinyFiles shinyjs lmerTest \
    circular car
