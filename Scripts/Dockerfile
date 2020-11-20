# ----------------           Dockerfile for Kustomize   ------------------------------
# Using Base image (Alpine version)
FROM alpine:latest

# Installing curl and kustomize
RUN apk add curl
RUN curl -L --output /tmp/kustomize_v3.8.5_linux_amd64.tar.gz https://github.com/kubernetes-sigs/kustomize/releases/download/kustomize%2Fv3.8.5/kustomize_v3.8.5_linux_amd64.tar.gz && tar -xvzf /tmp/kustomize_v3.8.5_linux_amd64.tar.gz -C /usr/local/bin && chmod +x /usr/local/bin/kustomize

# Setting up work directory as kustomize
WORKDIR /kustomize
