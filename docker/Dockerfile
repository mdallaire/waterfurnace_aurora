FROM ruby:2.7
ENV WATERFURNACE_AURORA_VERSION 1.4.5
ENV TTY=/dev/ttyUSB0
ENV MQTT=mqtt://localhost
RUN gem install waterfurnace_aurora -v ${WATERFURNACE_AURORA_VERSION}
WORKDIR /usr/local/bundle/bin/
CMD ruby aurora_mqtt_bridge $TTY $MQTT
