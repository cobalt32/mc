FROM alpine
WORKDIR /srv/minecraft
RUN apk update
RUN apk add openjdk8-jre-base
RUN wget https://launcher.mojang.com/v1/objects/1b557e7b033b583cd9f66746b7a9ab1ec1673ced/server.jar
COPY . .
EXPOSE 25565
ENTRYPOINT ["java"]
CMD ["-Xms2G", "-Xmx4G", "-jar", "server.jar", "nogui"]
