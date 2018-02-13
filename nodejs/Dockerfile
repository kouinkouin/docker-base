FROM kouinkouin/debian-base

RUN wget -qO- https://deb.nodesource.com/gpgkey/nodesource.gpg.key | apt-key add - && \
    echo "deb https://deb.nodesource.com/node_8.x stretch main" > /etc/apt/sources.list.d/nodesource.list && \
    apt update && \
    apt install -y nodejs && \
    apt clean && \
    rm -r /var/lib/apt/lists/*

