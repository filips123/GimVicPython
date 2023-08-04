# GimVičPython

Pre-compiled Python distributions for GimVičUrnik.

## About

This repository contains pre-compiled Python distributions for usage in [GimVičUrnik](https://github.com/filips123/GimVicUrnik). Versions can be built with GitHub Actions and accessed from the production server with `pyenv` plugin.

Although this repository is public, it is intended only for usage in GimVičUrnik.

## Structure

* Branch `main` - Contains GitHub workflows that manage building and uploading Python versions.
* Branch `plugin` - Contains a pyenv plugin that installs pre-built Python versions.
* Releases - Store pre-built Python versions.

## Usage

1. Trigger [a workflow dispatch](https://github.com/filips123/GimVicPython/actions/workflows/build.yml) with a specific Python version.
2. Wait around 20 minutes so the build completes and the version is released.
3. Plugin will be updated and a new version with `-bin` suffix will be added.
4. Update the plugin on the server and switch to the correct Python version.
