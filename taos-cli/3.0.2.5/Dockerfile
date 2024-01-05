FROM alextinng/java:8_with_arthas
LABEL authors="alextinng"

WORKDIR /taos

RUN set -eux \
    && yum -y install tar \
    && yum -y install gzip \
    && curl -O https://www.taosdata.com/assets-download/3.0/TDengine-client-3.0.2.5-Linux-x64-Lite.tar.gz \
    && tar xvf TDengine-client-3.0.2.5-Linux-x64-Lite.tar.gz \
    && cd TDengine-client-3.0.2.5 \
    && sh install_client.sh \
    && rm -rf TDengine-client-3.0.2.5-Linux-x64-Lite.tar.gz \
    && rm -rf TDengine-client-3.0.2.5