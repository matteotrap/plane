FROM makeplane/plane-backend:v1.4.3

# The stock entrypoint binds gunicorn to IPv4 only; Fly's private network is IPv6-only.
RUN sed -i 's/--bind 0.0.0.0:/--bind [::]:/' ./bin/docker-entrypoint-api.sh
