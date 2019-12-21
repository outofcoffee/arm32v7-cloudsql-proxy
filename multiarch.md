# Building for non amd64 architectures

## Prerequisites

Build on the target architecture, e.g. arm32v7, aarch64 etc.

## Image build

Docker uses the values of `GOARCH` to determine the architecture, so for arm32v7 the value would be `arm`, for aarch64 it would be `arm64` etc.

Override the architecture:

    docker build --rm \
        --build-arg GOARCH=arm \
        --tag outofcoffee/cloudsql-gce-proxy:1.17-arm32v7 .
