FROM eclipse-temurin:21-jre-jammy

WORKDIR / app

COPY build/libs/*.jar app.jar


RUN useradd -m springuser && chown -R springuser /app


EXPOSE 80

ENTRYPOINT [ "java", "jar", "app.jar" ]