FROM jboss/wildfly:15.0.1.Final
RUN /opt/jboss/wildfly/bin/add-user.sh admin admin --silent

#Copiar el management.properties y listo, a eso lo ponemos en el gitignore y dejamos la linea anterior comentada


CMD ["/opt/jboss/wildfly/bin/standalone.sh", "-b", "0.0.0.0", "-bmanagement", "0.0.0.0"]