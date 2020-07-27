#-------------------------------------------------------------------------------------------------------------
# Copyright (c) Microsoft Corporation. All rights reserved.
# Licensed under the MIT License. See https://go.microsoft.com/fwlink/?linkid=2090316 for license information.
#-------------------------------------------------------------------------------------------------------------

# To fully customize the contents of this image, use the following Dockerfile instead:
# https://github.com/microsoft/vscode-dev-containers/tree/v0.128.0/containers/codespaces-linux/.devcontainer/Dockerfile
FROM mcr.microsoft.com/vscode/devcontainers/universal:0-linux

# ** [Optional] Uncomment this section to install additional packages. **
#
ENV DEBIAN_FRONTEND=noninteractive
RUN sudo apt-get update -qqy \
    && sudo apt-get -qqy install --no-install-recommends wget
# Install PowerShell 7
RUN sudo wget https://packages.microsoft.com/config/debian/10/packages-microsoft-prod.deb \
    && sudo dpkg -i packages-microsoft-prod.deb \
    && sudo rm packages-microsoft-prod.deb \
    && sudo apt-get -qqy update \
    && sudo apt-get -qqy install powershell

# RUN wget -q https://packages.microsoft.com/config/ubuntu/18.04/packages-microsoft-prod.deb \
#     && sudo dpkg -i packages-microsoft-prod.deb && sudo apt-get -qqy update \
#     && sudo apt-get install -y powershell

# Update the list of products
# RUN sudo apt-get update

# Enable the "universe" repositories
# RUN sudo add-apt-repository universe
