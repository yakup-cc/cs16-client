FROM mcr.microsoft.com/devcontainers/base:ubuntu-22.04

ENV DEBIAN_FRONTEND=noninteractive

# CS16-Client ve MainUI derleme bağımlılıkları
RUN apt-get update && apt-get install -y --no-install-recommends \
    build-essential \
    cmake \
    git \
    ninja-build \
    pkg-config \
    ccache \
    clang \
    lldb \
    python3 \
    libfreetype6-dev \
    libfontconfig1-dev \
    libsdl2-dev \
    libgl1-mesa-dev \
    libglu1-mesa-dev \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /workspace