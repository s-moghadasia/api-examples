FROM debian:jessie-slim
MAINTAINER Cole Calistra <cole@kairos.com>

RUN apt-get update -qq && apt-get install -qy curl

## Copy working files to container
RUN mkdir -p /app/bin

ADD bin/ /app/bin/
ADD public/ /app/public/
ADD assets/ /app/assets/

WORKDIR /app
ENTRYPOINT ["/app/bin/app"]
