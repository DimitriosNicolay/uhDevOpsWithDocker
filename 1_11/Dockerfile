FROM amazoncorretto:8u504-alpine3.24

EXPOSE 8080

WORKDIR /usr/src/app

COPY . .

RUN chmod +x mvnw

RUN ./mvnw package

CMD [ "java", "-jar", "./target/docker-example-1.1.3.jar" ]