# Meson CMake build wrapper

This repository is meant to demonstrate the reliability of the CMake
subprojects implementation in meson. Actually building CMake with
this setup is not recommended.

## Requirements

Meson version 0.51.0 is required to build this project. It can
be installed via pip.

## Usage

To build and test this repository use the following steps:

```bash
git clone https://github.com/mensinda/mesonCMakeBuilder.git
cd mesonCMakeBuilder
git submodule update --init --recursive
/path/to/correct/meson.py build
ninja -C build
ninja -C build test # This will run cmake -h
```

The CMake executable can then be found in `build/subprojects/cmake`.
