FROM hub.connoisseur-suite.co.uk/bases/frankenphp-8.3:latest

RUN apt-get update && apt-get install -y supervisor \
    && mkdir -p /var/log/supervisor

RUN mkdir -p /etc/supervisor

COPY supervisor /etc/supervisor

COPY entrypoint.sh /entrypoint.sh

RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]