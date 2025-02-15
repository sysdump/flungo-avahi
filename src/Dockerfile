FROM alpine

RUN apk add --no-cache avahi avahi-tools dbus augeas

RUN mkdir -p /run/dbus && chmod 755 /run/dbus

COPY entrypoint.sh /opt/entrypoint.sh
RUN chmod +x /opt/entrypoint.sh

ENTRYPOINT ["/opt/entrypoint.sh"]
