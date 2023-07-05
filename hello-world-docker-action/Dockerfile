# Container image that runs your code
FROM alpine:3.10

RUN ls -ltr

# Copies your code file from your action repository to the filesystem path `/` of the container
COPY ./hello-world-docker-action/entrypoint.sh /entrypoint.sh

RUN chmod -R 777 /entrypoint.sh

RUN ls -ltr

# Code file to execute when the docker container starts up (`entrypoint.sh`)
ENTRYPOINT ["/entrypoint.sh"]
