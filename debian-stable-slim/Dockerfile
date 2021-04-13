FROM debian:stable-slim

RUN useradd -m myuser

COPY hello.sh /home/myuser
RUN chown -R myuser /home/myuser

HEALTHCHECK CMD true
USER myuser:myuser
WORKDIR /home/myuser
ENTRYPOINT ["/home/myuser/hello.sh"]
