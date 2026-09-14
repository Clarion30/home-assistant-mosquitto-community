ARG BUILD_VERSION

FROM eclipse-mosquitto:2.1.2-alpine
ARG BUILD_VERSION

LABEL \
  io.hass.name="Mosquitto Community Broker" \
  io.hass.description="Community Home Assistant app using Eclipse Mosquitto 2.1.2" \
  io.hass.type="addon" \
  io.hass.version="${BUILD_VERSION}"

COPY run.sh /run.sh
RUN chmod 755 /run.sh

ENTRYPOINT ["/run.sh"]
