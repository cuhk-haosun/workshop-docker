# outof cuhkhaosun/base image
FROM cuhkhaosun/base

# Installation dependency
RUN apt-get update && apt-get install -y \
    wget \
    git \
    build-essential \
    zlib1g-dev

# Set working directory
WORKDIR /app

# Installation
RUN git clone https://github.com/lh3/minimap2 && cd minimap2 && make

ENV PATH="/app/minimap2:${PATH}"

CMD ["minimap2"]
