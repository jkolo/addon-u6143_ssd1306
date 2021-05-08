#ARG BUILD_FROM=ghcr.io/hassio-addons/base/armv7:9.2.0
ARG BUILD_FROM
FROM ${BUILD_FROM}

# Copy root filesystem
COPY rootfs /
RUN ln -sfv libwiringPi.so.2.60 \
      /usr/local/lib/libwiringPi.so && \
	ln -sfv libwiringPiDev.so.2.60 \
	  /usr/local/lib/libwiringPiDev.so

# Setup base
RUN apk add --no-cache libc6-compat procps
