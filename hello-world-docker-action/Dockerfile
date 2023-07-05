# Container image that runs your code
FROM alpine:3.10

RUN ls -ltr

# Copies your code file from your action repository to the filesystem path `/` of the container
COPY entrypoint.sh /entrypoint.sh

RUN chmod +x entrypoint.sh

RUN ls -ltr

# Code file to execute when the docker container starts up (`entrypoint.sh`)
ENTRYPOINT ["/entrypoint.sh"]
