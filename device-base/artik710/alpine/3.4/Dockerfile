FROM resin/armhf-alpine:3.4

LABEL io.resin.device-type="artik710"

RUN apk add --update \
		less \
		nano \
		net-tools \
		ifupdown \		
		usbutils \
		gnupg \
	&& rm -rf /var/cache/apk/*
