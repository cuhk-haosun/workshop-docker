FROM cuhkhaosun/base:latest

LABEL image.author.name "Yifang Qi"
LABEL image.author.email "223050049@link.cuhk.edu.cn"

WORKDIR /app

RUN curl -L https://github.com/lh3/minimap2/releases/download/v2.27/minimap2-2.27_x64-linux.tar.bz2 | tar -jxvf -

ENV PATH=$PATH:/app/minimap2-2.27_x64-linux
