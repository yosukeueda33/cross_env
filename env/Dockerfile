FROM multiarch/ubuntu-core:arm64-bionic

WORKDIR /app

RUN sed -i.bak -e "s%http://archive.ubuntu.com/ubuntu/%http://ftp.iij.ad.jp/pub/linux/ubuntu/archive/%g" /etc/apt/sources.list

RUN apt update
RUN apt install -y gcc
RUN apt install -y g++
RUN apt install -y make
RUN apt install -y cmake
RUN apt install -y zip
RUN apt install -y python3
RUN apt install -y vim
RUN apt install -y tmux

RUN apt install -y libssl-dev
RUN apt install -y libcurl4-openssl-dev
RUN apt install -y zlib1g-dev

RUN apt install -y git
RUN apt install -y curl

ENTRYPOINT ["tail", "-f", "/dev/null"]
