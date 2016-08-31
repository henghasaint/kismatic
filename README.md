# Kismatic Platform

[![Build Status](https://snap-ci.com/On8xdVQV0xY5VXICf0Fx0Vq7fVMDUAfU6JFc8Wtt94A/build_image)](https://snap-ci.com/apprenda/kismatic-platform/branch/master)

## Developer notes
### Pre-requisites
- Go installed
- Glide for vendoring (https://glide.sh)
- Docker (required for building)

### Build using make
We use `make` to clean, build, and produce our distribution package. Take a look at the Makefile for more details.

In order to build the Go binaries (e.g. Kismatic CLI):
```
make build
```

In order to clean:
```
make clean
```

In order to produce the distribution package:
```
make dist
```
This will produce an `./out` directory, which contains the bits, and a tarball.

You may pass build options as necessary:
```
GOOS=linux make build 
```


