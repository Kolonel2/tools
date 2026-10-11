FROM ubuntu:26.04

RUN apt-get update \
 && apt-get install -y --no-install-recommends \
      ca-certificates \
      curl \
      iputils-ping \
      openssh-client \
      iproute2 \
      dnsutils \
      netcat-openbsd \
 && rm -rf /var/lib/apt/lists/*

# Keep the container alive so you can exec/console into it
CMD ["sleep", "infinity"]
