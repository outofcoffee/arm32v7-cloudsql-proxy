# Building for ARM

## Prerequisites

Build on the target architecture, e.g. arm32v7

## Image build

Override the architecture:

    docker build --rm \
        --build-arg GOARCH=arm \
        --tag outofcoffee/cloudsql-gce-proxy:1.16-arm32v7 .
