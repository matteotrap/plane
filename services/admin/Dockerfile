FROM makeplane/plane-admin:v1.4.3

# The stock nginx config listens on IPv4 only; Fly's private network is IPv6-only.
RUN sed -i 's/listen 3000;/listen 3000;\n    listen [::]:3000;/' /etc/nginx/nginx.conf
