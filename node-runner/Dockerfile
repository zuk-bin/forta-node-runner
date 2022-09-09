# syntax=docker/dockerfile:1
FROM debian

RUN apt update \
    && apt install -y curl \
    && rm -rf /var/lib/apt/lists/*

RUN curl https://dist.forta.network/artifacts/forta -o /bin/forta \
    && chmod +x /bin/forta

ENTRYPOINT ["/bin/forta"]
CMD ["run"]
