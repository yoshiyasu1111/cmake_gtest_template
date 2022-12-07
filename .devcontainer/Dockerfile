FROM gcc:12.2-bullseye

RUN adduser -q --gecos "" --disabled-password gccuser \
    && apt-get update \
    && apt-get install -y cmake \
    && rm -fr /var/lib/apt/lists/*
