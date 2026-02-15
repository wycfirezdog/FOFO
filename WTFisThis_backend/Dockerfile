FROM eclipse-temurin:25-jdk-alpine
WORKDIR /app

RUN apk add --no-cache maven

COPY . .
RUN mvn clean package -DskipTests -B

EXPOSE 8080
CMD ["java", "-jar", "target/demo-0.0.1-SNAPSHOT.jar"]
