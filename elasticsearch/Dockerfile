FROM docker.elastic.co/elasticsearch/elasticsearch-oss:6.7.1

COPY . /usr/share/elasticsearch/config/.

RUN bin/elasticsearch-plugin install -b https://d3g5vo6xdbdb9a.cloudfront.net/downloads/elasticsearch-plugins/opendistro-security/opendistro_security-0.9.0.0.zip