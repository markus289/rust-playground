FROM fedora:latest
RUN dnf -y install cargo git rust rust-analyzer rust-src rustfmt sudo \
    && dnf clean all \
    && useradd -m -G users -s /bin/bash vscode \
    && echo vscode ALL=\(root\) NOPASSWD:ALL > /etc/sudoers.d/vscode
