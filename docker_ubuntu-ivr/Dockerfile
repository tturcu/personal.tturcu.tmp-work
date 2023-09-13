# This is a test docker image
# Get the GCC preinstalled image from Docker Hub
FROM ubuntu:22.04

RUN apt-get update \
    && apt-get install -y --no-install-recommends gcc libc6-dev

WORKDIR /workspace

COPY test.c /workspace

RUN gcc test.c -o test
