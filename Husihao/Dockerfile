FROM cuhkhaosun/base

RUN apt-get update && apt-get install -y \
    curl \
    bzip2 \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /hsh

RUN curl -L https://github.com/lh3/minimap2/releases/download/v2.28/minimap2-2.28_x64-linux.tar.bz2 | tar -jxvf - \
    && mv minimap2-2.28_x64-linux/minimap2 /usr/local/bin/

ENV PATH="/hsh/minimap2-2.28_x64-linux:${PATH}"

CMD ["minimap2"]