FROM mcr.microsoft.com/devcontainers/cpp:dev-debian

RUN apt-get update \
  && apt-get install --no-install-recommends -y \
    # compiler tools
    catch2 \
    clang-tidy \
    clangd \
    ccache \
    libboost-all-dev \
    # python3 support
    python3-pip \
    # testing
    lcov

# Add ./bin to PATH
ENV PATH="./bin:${PATH}"
