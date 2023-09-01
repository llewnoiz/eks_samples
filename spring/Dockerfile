From amazoncorretto:17-alpine3.17-jdk

RUN mkdir /apps
COPY ./ /apps
WORKDIR /apps
RUN chmod 755 ./gradlew
RUN ./gradlew build
COPY ./build/libs/rest-service-0.0.1-SNAPSHOT.jar app.jar
CMD ["java","-jar","app.jar"]