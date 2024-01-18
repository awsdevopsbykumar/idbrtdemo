FROM tomcat:8.5.47-jdk8-openjdk
#https://tomcat.apache.org/tomcat-8.0-doc/appdev/sample/
COPY ./sample.war /usr/local/tomcat/webapps
EXPOSE 8080
CMD ["/usr/local/tomcat/bin/catalina.sh", "run"]