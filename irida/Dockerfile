FROM tomcat:9.0-jre11
RUN mkdir -p /etc/irida/plugins /opt/irida/data/sequence /opt/irida/data/reference /opt/irida/data/output
ADD irida.conf /etc/irida/
RUN curl -Lo /usr/local/tomcat/webapps/irida.war https://github.com/phac-nml/irida/releases/download/21.01/irida-21.01.war
EXPOSE 8080
CMD ["/usr/local/tomcat/bin/catalina.sh", "run"]