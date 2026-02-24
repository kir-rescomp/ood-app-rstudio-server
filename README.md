# RStudio Server app for BMRC OOD 

![GitHub Release](https://img.shields.io/github/release/osc/bc_osc_rstudio_server.svg)
[![GitHub License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)

<p align="center">
<img src="./icon.png" width="300"/>
</p>


# `form.yml.erb` requirements

By one mechanism or another, `form.yml.erb` must supply an RStudio module which can be loaded by this script via the `template/script/sh.erb`. This script will check for the existence of two `context` parameters, `auto_modules_RStudio-Server` and `rstudio_module` (in that order). It will use the first of these which has been defined to load the RStudio-Server module.
