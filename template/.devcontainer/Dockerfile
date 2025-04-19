FROM mcr.microsoft.com/devcontainers/python:3.12

USER root

### Install Task (https://taskfile.dev/) ###
RUN sh -c "$(curl --location https://taskfile.dev/install.sh)" -- -d -b /usr/local/bin && \
    bash -c "task --completion bash > /etc/bash_completion.d/task"

# hadolint ignore=DL3013
RUN pip install --no-cache-dir --upgrade pip poetry

USER vscode
