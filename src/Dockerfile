FROM linuxserver/wireguard:alpine
RUN apk add --no-cache bash su-exec ca-certificates tini
COPY --from=mbentley/teamspeak:alpine /opt/teamspeak /opt/teamspeak
COPY --from=mbentley/teamspeak:alpine /entrypoint.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
