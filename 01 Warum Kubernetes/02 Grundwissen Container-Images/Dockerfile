FROM openjdk:11-jdk-slim AS builder
WORKDIR /tmp
COPY HelloWorld.java .
RUN javac HelloWorld.java

FROM openjdk:11-jre-slim AS final
RUN mkdir -p /opt/HelloWorld
WORKDIR /opt/HelloWorld
COPY --from=builder /tmp/HelloWorld.class .
CMD [ "java", "HelloWorld" ]