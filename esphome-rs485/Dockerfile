ARG BUILD_FROM=esphome/esphome-hassio-aarch64:cache-dev
FROM ${BUILD_FROM}

# Copy root filesystem
COPY rootfs /

RUN pip3 install --no-cache-dir https://github.com/coalcooker/esphome/archive/master.zip

# Build arguments
ARG BUILD_VERSION=master

# Labels
LABEL \
    io.hass.type="addon" \
    io.hass.version=master
