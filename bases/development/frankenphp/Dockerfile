FROM hub.connoisseur-suite.co.uk/production/frankenphp-8.3

RUN mkdir -p /etc/supervisor

COPY supervisor /etc/supervisor

COPY entrypoint.sh /entrypoint.sh

RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]