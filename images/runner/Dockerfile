FROM ghcr.io/actions/actions-runner:2.337.0
USER root
RUN apt-get update \
  && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends ca-certificates curl git jq unzip \
  && rm -rf /var/lib/apt/lists/*
USER runner
