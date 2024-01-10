FROM gitpod/workspace-base:latest

USER gitpod
SHELL ["/bin/bash", "-o", "pipefail", "-c"]

# Install Pants
RUN curl --proto '=https' --tlsv1.2 -fsSL https://static.pantsbuild.org/setup/get-pants.sh | bash
