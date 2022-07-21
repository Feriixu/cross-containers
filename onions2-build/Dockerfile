FROM ghcr.io/cross-rs/mips-unknown-linux-musl:latest

RUN apt update && apt install -y git wget subversion build-essential libncurses5-dev zlib1g-dev gawk flex quilt git-core unzip libssl-dev python-dev python-pip libxml-parser-perl time
RUN git clone https://github.com/OnionIoT/source.git
