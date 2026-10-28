FROM nginx:1.27-alpine
COPY index.html /usr/share/nginx/html/
HEALTHCHECK CMD wget -q0-http://localhost/ || exit 1
EXPOSE 80