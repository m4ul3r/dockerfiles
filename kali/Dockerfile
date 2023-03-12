FROM kalilinux/kali-rolling

WORKDIR /root

ENV DEBIAN_FRONTEND=noninteractive

RUN apt update -y && apt dist-upgrade -y && apt autoremove -y && apt clean

RUN apt -y install \
    kali-linux-headless \
    zsh

ENTRYPOINT ["/bin/zsh"]
