ARG UPSTREAM_VERSION

FROM thorax/erigon:${UPSTREAM_VERSION}

USER root

COPY /security /security
COPY entrypoint.sh /usr/local/bin/entrypoint.sh
RUN chmod u+x /usr/local/bin/entrypoint.sh

ENV DATADIR="/home/erigon/.local/share"

ENTRYPOINT [ "/usr/local/bin/entrypoint.sh" ]
