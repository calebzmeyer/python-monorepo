FROM gitpod/workspace-base:latest

USER gitpod
SHELL ["/bin/bash", "-o", "pipefail", "-c"]

ENV PYENV_ROOT="${HOME}/.pyenv"
ENV PYTHON_VERSION="3.11.7"

ENV PATH="${PYENV_ROOT}/bin:${PYENV_ROOT}/shims:${PATH}"

# Install Python Versions
RUN curl https://pyenv.run | bash && \
    pyenv install ${PYTHON_VERSION} && \
    pyenv global ${PYTHON_VERSION}

# Install Pants
RUN curl --proto '=https' --tlsv1.2 -fsSL https://static.pantsbuild.org/setup/get-pants.sh | bash
