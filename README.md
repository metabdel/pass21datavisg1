# TP visualisation des données avec ggplot

# Specifying an R environment with a runtime.txt file

### Requirements and suggestions

You need to have a `runtime.txt` file that is formatted like:

```
r-<r-version>-<YYYY>-<MM>-<DD>
```

where `<r-version>` is a version of R (like 4.1, 4.0, etc) you want to use,
and `<YYYY>-<MM>-<DD>` is the date for [a snapshot](https://packagemanager.rstudio.com/client/#/repos/1/overview)
from [packagemanager.rstudio.com](https://packagemanager.rstudio.com) that will
be used for installing your R packages.

Try using a date newer than `2022-01-01`, as you'll get faster
package installs thanks to [binary packages](https://www.rstudio.com/blog/package-manager-v1-1-no-interruptions/)
from rstudio.packagemanager.com!

To install R libraries, add `install.package("<package-name>")` calls to
`install.R`. If you want to pin to a specific version of the library, you
can also do `devtools::install_version("<package-name>", "<version>")`.

For some R packages, you might need to install system packages via apt - you can
do so by writing out a list of apt package names in `apt.txt`. You can find
the list of such packages in the page for your package at
[packagemanager.rstudio.com](https://packagemanager.rstudio.com/client/#/). Make sure
to select "Ubuntu 18.04 (Bionic)" in the dropdown on the top right.

Both [RStudio](https://www.rstudio.com/) and [IRKernel](https://irkernel.github.io/)
are installed by default, so you can use either the Jupyter notebook interface or
the RStudio interface.

This repository also contains an example of a [Shiny app](https://github.com/binder-examples/r/tree/master/bus-dashboard).


