Testing elasticsearch + kibana 6.7.1 with opendistro security and proxy authentication.

### Startup
Build and start the containers with `docker-compose up`.  When they are running, exec into the elasticsearch container and initialize the opendistro security plugin with the security configuration


    > docker exec -it elasticsearch bash
    > sh 
    /usr/share/elasticsearch/plugins/opendistro_security/tools/securityadmin.sh \
    -cd plugins/opendistro_security/securityconfig/ -icl -nhnv \
    -cacert config/root-ca.pem \
    -cert config/kirk.pem \
    -key config/kirk-key.pem