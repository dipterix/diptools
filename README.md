[![license](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://opensource.org/licenses/GPL-3.0)
[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
[![Docker Layers](https://images.microbadger.com/badges/image/dipterix/diptools.svg)](https://microbadger.com/images/dipterix/diptools "Get your own image badge on microbadger.com")

Visit [github](https://github.com/dipterix) for more about available Dipterix's R packages.


## Diptools: Dipterix's personal toolbox

### Overview

This repository contains Dockerfiles for Docker containers of R packages
* `dipsaus`: provides add-ons to R popular packages [[github](https://github.com/dipterix/dipsaus)], [[CRAN](https://cran.r-project.org/package=dipsaus)]
* `lazyarray`: fast read and write GB-level arrays within seconds [[github](https://github.com/dipterix/lazyarray)], [[CRAN](https://cran.r-project.org/package=lazyarray)]
* `threeBrain`: 3D FreeSurfer & SUMA brain viewer in web browsers 
[[github](https://github.com/dipterix/threeBrain)], [[CRAN](https://cran.r-project.org/package=threeBrain)]
* `fst`: fast data frame IO [[github](https://github.com/fstpackage/fst)], [[CRAN](https://cran.r-project.org/package=fst)]
* `hdf5r`: R HDF5 file IO [[github](https://github.com/hhoeflin/hdf5r)], [[CRAN](https://cran.r-project.org/package=hdf5r)]
* `fftwtools`: FFT library [[CRAN](https://cran.r-project.org/package=fftwtools)]

> This container image is built with `rocker/r-base:latest`

### Installation

```
docker pull dipterix/diptools
```

### Dev-version

Dev-version contains github version of `dipsaus`, `lazyarray`, and `threeBrain`

```
docker pull dipterix/diptools:devel
```

### License
The Dockerfiles in this repository are licensed under GPL-3 or later. 


