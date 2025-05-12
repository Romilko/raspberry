FROM gradle:8.13-jdk17 AS builder

WORKDIR /source

COPY . .

RUN gradle compileJava bootJar -x test

FROM alpine:latest

RUN apk add --no-cache openjdk17-jre

WORKDIR /app

COPY --from=builder /source/build/libs/*.jar app.jar

EXPOSE 5050

ENTRYPOINT ["java", "-jar", "app.jar"]
