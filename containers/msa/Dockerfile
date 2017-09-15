FROM ikuturso/mongo-sites-api

ENV http_proxy 'http://netproxy1.infra.sgdc:8080'
ENV https_proxy 'http://netproxy1.infra.sgdc:8080'

COPY . /root/mongo-sites-api

RUN bash -c 'cd plugins; npm update || echo'

ARG ADDITIONAL_COMMAND
RUN bash -c "$ADDITIONAL_COMMAND"
