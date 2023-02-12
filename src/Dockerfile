FROM linuxserver/wireguard:alpine
RUN apk add --no-cache bzip2 ca-certificates coreutils libstdc++ su-exec tini w3m
COPY --from=mbentley/teamspeak:alpine /opt/teamspeak /opt/teamspeak
COPY --from=mbentley/teamspeak:alpine /entrypoint.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
