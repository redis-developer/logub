FROM openjdk:11-jdk-slim
ENV PORT 8081
ENV CLASSPATH /opt/lib
EXPOSE 8081

COPY pom.xml target/lib* /opt/lib/


COPY target/*.jar /opt/app.jar
WORKDIR /opt
CMD ["java", "-XX:+UnlockExperimentalVMOptions", "-jar", "app.jar"]
