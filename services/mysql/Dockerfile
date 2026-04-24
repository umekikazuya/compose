FROM mysql:8.0.45

# パラメータ指定
ENV LANG=ja_JP.UTF-8
ENV LANGUAGE=ja_JP:ja
ENV TZ=Asia/Tokyo

COPY ./init/*.sql /docker-entrypoint-initdb.d/

# ヘルスチェック
HEALTHCHECK --interval=10s --timeout=5s --retries=10 \
  CMD mysqladmin ping -h localhost -u root -p$$MYSQL_ROOT_PASSWORD >/dev/null || exit 1