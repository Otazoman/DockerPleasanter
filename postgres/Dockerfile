FROM postgres:13-alpine
ENV LANG ja_JP.utf8

# バックアップ用のディレクトリを生成しておく
RUN mkdir -p /var/lib/postgresql/arclog/ &&\
    chmod 777 /var/lib/postgresql/arclog/

# timezone setting
RUN apk --no-cache add tzdata && \
    cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime && \
    apk del tzdata
