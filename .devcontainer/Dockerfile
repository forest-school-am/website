# Use a base image
FROM mcr.microsoft.com/devcontainers/base:ubuntu

RUN apt-get update && apt-get install -y build-essential curl inotify-tools

RUN curl https://sh.rustup.rs -sSf | bash -s -- -y
ENV PATH="/root/.cargo/bin:${PATH}"

RUN cargo install --root /usr --locked --git https://github.com/getzola/zola/ --rev 45d3f8d6285f0b47013c5fa31eb405332118af8b
