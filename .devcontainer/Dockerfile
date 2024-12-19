FROM mcr.microsoft.com/devcontainers/universal:2-linux

# Install necessary packages
RUN apt-get update && apt-get install -y \
    xz-utils \
    curl \
    python3-pip \
    && apt-get clean

# Install Vue.js 
RUN curl -fsSL https://deb.nodesource.com/setup_18.x | bash - && \
    apt-get install -y nodejs && \
    npm install -g @vue/cli

# Install Flask
RUN pip install flask
