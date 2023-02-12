FROM linuxserver/wireguard:alpine
COPY --from=mbentley/teamspeak:alpine /opt/teamspeak /opt/teamspeak
COPY --from=mbentley/teamspeak:alpine /entrypoint.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
