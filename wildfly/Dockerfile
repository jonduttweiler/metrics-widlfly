FROM jboss/wildfly:17.0.1.Final
LABEL maintainer="Jonatan E. Duttweiler <jduttweiler@santafe.gob.ar>"

RUN /opt/jboss/wildfly/bin/add-user.sh admin admin --silent

COPY ./configuration/standalone.xml /opt/jboss/wildfly/standalone/configuration

#Deploy example app
COPY ./test-app.war /opt/jboss/wildfly/standalone/deployments

CMD ["/opt/jboss/wildfly/bin/standalone.sh", "-b", "0.0.0.0", "-bmanagement", "0.0.0.0"]
