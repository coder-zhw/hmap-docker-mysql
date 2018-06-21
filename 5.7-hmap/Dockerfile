FROM mysql:5.7

LABEL maintainer="zhw <coder.zhw@qq.com>"

ENV TZ Asia/Shanghai

COPY 5.7-hmap/hmap.cnf /etc/mysql/conf.d/

RUN set -x \
    && echo "Asia/Shanghai" > /etc/timezone \
    && dpkg-reconfigure -f noninteractive tzdata
