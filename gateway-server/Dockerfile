FROM maven:3.9.6-eclipse-temurin-21
WORKDIR /app
COPY . .
RUN mvn clean package -DskipTests
WORKDIR /app/target
ENTRYPOINT ["java", "-jar", "gateway-server.jar"]

