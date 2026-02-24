# Batch Connect - OSC RStudio Server

![GitHub Release](https://img.shields.io/github/release/osc/bc_osc_rstudio_server.svg)
[![GitHub License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)

# Usage

This repository provides a basic RStudio app for use with OnDemand.

*IMPORTANT* This RStudio app is intentionally incomplete and must be completed by adding local files for `form.yml.erb` and `submit.yml.erb`. Generic versions of these files cannot be provided because they depend on the local OnDemand setup.

# `form.yml.erb` requirements

By one mechanism or another, `form.yml.erb` must supply an RStudio module which can be loaded by this script via the `template/script/sh.erb`. This script will check for the existence of two `context` parameters, `auto_modules_RStudio-Server` and `rstudio_module` (in that order). It will use the first of these which has been defined to load the RStudio-Server module.
