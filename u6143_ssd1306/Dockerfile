#ARG BUILD_FROM=ghcr.io/hassio-addons/base/armv7:9.2.0
ARG BUILD_FROM
FROM ${BUILD_FROM}

# Copy root filesystem
COPY rootfs /

# Setup base
RUN apk add --no-cache libc6-compat procps
