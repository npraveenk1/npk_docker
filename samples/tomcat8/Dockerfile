FROM java:8-jre

ENV CATALINA_HOME /usr/local/tomcat
ENV PATH $CATALINA_HOME/bin:$PATH



RUN  cd /usr/local/ \
     && wget http://www-us.apache.org/dist/tomcat/tomcat-8/v8.5.12/bin/apache-tomcat-8.5.12.zip \
     && unzip apache-tomcat-8.5.12.zip \
     && mv apache-tomcat-8.5.12/ tomcat/

EXPOSE 8080

CMD ["/usr/local/tomcat/bin/catalina.sh", "run"]
