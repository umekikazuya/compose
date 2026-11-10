FROM floci/floci:latest-aws
ENV FLOCI_HOSTNAME=floci

COPY --chmod=755 init/01.sh /etc/floci/init/start.d/01.sh
COPY --chmod=755 init/02.sh /etc/floci/init/start.d/02.sh
COPY --chmod=755 init/03.sh /etc/floci/init/start.d/03.sh