# Use Python 3.12-slim as the base image
FROM python:3.12-slim

FROM nvidia/cuda:12.2.2-base-ubuntu22.04

# Install Miniconda
RUN apt-get update && apt-get install -y wget && \
    wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh && \
    bash Miniconda3-latest-Linux-x86_64.sh -b -p /opt/miniconda3 && \
    rm Miniconda3-latest-Linux-x86_64.sh

# Configure Conda environment
ENV PATH="/opt/miniconda3/bin:$PATH"

WORKDIR /workspace

ENTRYPOINT [ "bash" ]