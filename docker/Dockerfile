# Specifies which underlying mirror is based
FROM java:8

# Author information
MAINTAINER wwj

# Mount point statement
VOLUME /tmp

# Copy a local file or directory to the file or directory of the container
ADD /target/jenkin-mongodb-rest-0.0.1.jar springboot.jar

#shell script
RUN bash -c 'touch /springboot.jar'

# Expose the 2233 port of the container to external access.
EXPOSE 2233

# When the container is running, execute the instructions to run jar
ENTRYPOINT ["java", "-jar", "springboot.jar"]