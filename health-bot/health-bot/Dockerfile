FROM openjdk:8
WORKDIR /
ADD target/health-bot-0.0.1-SNAPSHOT.jar app.jar
RUN useradd -m myuser
USER myuser
EXPOSE 8090
CMD java -jar -Dspring.profiles.active=prod app.jar