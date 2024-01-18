FROM centos:7
  
RUN mkdir /opt/tomcat/

WORKDIR /opt/tomcat
RUN yum update -y
RUN yum install java-11-openjdk -y
RUN java -version

RUN curl -O https://downloads.apache.org/tomcat/tomcat-8/v8.5.93/bin/apache-tomcat-8.5.93.tar.gz
RUN tar xvfz apache*.tar.gz
RUN mv apache-tomcat-8.5.93/* /opt/tomcat/.

#https://tomcat.apache.org/tomcat-8.0-doc/appdev/sample/
COPY ./sample.war /opt/tomcat/webapps

EXPOSE 8080

CMD ["/opt/tomcat/bin/catalina.sh", "run"]
