FROM nvidia/cuda:8.0-cudnn5-devel-ubuntu14.04

RUN apt-get update -y && \
    apt-get install -y --no-install-recommends \
    ca-certificates \
    git && \
    rm -rf /var/lib/apt/lists/* /var/cache/apt/archives/*

RUN git clone https://github.com/torch/distro.git ~/torch
RUN cd ~/torch && bash install-deps
