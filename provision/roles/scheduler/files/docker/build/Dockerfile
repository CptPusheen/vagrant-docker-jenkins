FROM openjdk:slim

RUN apt-get update && \
    apt-get install -qq -y --no-install-recommends cron && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*


COPY hello-world.xml jenkins-cli.jar /

COPY hello-world /etc/cron.d/        

RUN crontab /etc/cron.d/hello-world

CMD ["sh","-c","cron -f"]

