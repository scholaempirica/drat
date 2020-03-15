## Repository of R packages for [Schola Empirica](https://scholaempirica.org)

Install packages from this repository like so (example for the `reschola` package):

``` r
install.packages("reschola", repos = "https://scholaempirica.github.io/drat/")
```

Or, to gain more direct access to this package repository, put this in your .Rprofile:

```r
local({r <- getOption("repos")
# add drat repo
r["scholaempirica"] <- "scholaempirica.github.io/drat"
options(repos=r)})
```

...then you will be able to do just

``` r
install.packages("reschola")
```

even though the `reschola` package is not on CRAN.

This may be preferable to using e.g. `remotes::install_github("scholaempirica/reschola")` since you

- always get a release, rather than the latest snapshot, which may be broken.
- get a binary package if available
- get a package with the vignettes built by default

Currently the repository contains the following packages:

- [reschola](https://github.com/scholaempirica/reschola) for reproducible research at Schola Empirica
- [redoc](https://github.com/scholaempirica/reschola), a [custom patch](https://github.com/petrbouchal/redoc/commit/69cbc91be1ea699360bfa7d6e86429abae8f842b) of [noamross/redoc](https://github.com/noamross/redoc) fixing documentatio and an RStudio addin

Source code for all the packages is hosted on [Github](https://github.com/scholaempirica).

The repository has been created using the `drat` package by @eddelbuettel; see more at <http://dirk.eddelbuettel.com/code/drat.html>
