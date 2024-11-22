FROM mcr.microsoft.com/devcontainers/ruby:2.7

# Set up shell
SHELL ["/bin/bash", "-c"]

# Install Node Version Manager (nvm)
RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash

# Install Node.js 14.18.2
RUN source ~/.bashrc \
    source ~/.nvm/nvm.sh \
    && nvm install 14.18.2 \
    && nvm alias default 14.18.2

# Ensure nvm is available in future RUN commands
ENV PATH="/root/.nvm/versions/node/v14.18.2/bin:${PATH}"
