FROM alpine:3.14
#Alpine container installs and updates java and all the basic dependencies
RUN  apk update \
  && apk upgrade \
  && apk add --update openjdk11 tzdata curl unzip bash \
  && rm -rf /var/cache/apk/*
## Installing Java Jre with alpine if there is no JRE for java 11
# RUN apk update \
#   && apk upgrade \
#   && apk add openjdk11-jre


##Maven dependency installation
## apk add mvn



## Spring boot app for java 11
##WORKDIR /app
##COPY .mvn/ .mvn
##COPY mvnw pom.xml ./
##COPY src ./src
##CMD ["./mvnw", "spring-boot:run"] 
