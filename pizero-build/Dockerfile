FROM rustembedded/cross:arm-unknown-linux-gnueabihf-0.2.0
ENV DEBIAN_FRONTEND=noninteractive
ENV PKG_CONFIG_PATH=/usr/lib/arm-linux-gnueabihf/pkgconfig
ENV RPI_TOOLS=/rpi_tools
ENV MACHINE=armv6
ENV ARCH=armv6
ENV CC=gcc
ENV OPENSSL_DIR=/openssl
ENV CROSSCOMP_DIR=/rpi_tools/arm-bcm2708/arm-rpi-4.9.3-linux-gnueabihf/bin

# Get Raspberry Pi cross-compiler tools
RUN git -C "/" clone -q --depth=1 https://github.com/raspberrypi/tools.git "${RPI_TOOLS}"

RUN apt update &&\
    apt install -y libraspberrypi-dev
