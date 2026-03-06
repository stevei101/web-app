FROM nginx:alpine

# Replace default nginx config with Cloud Run-compatible config (port 8080)
COPY nginx.conf /etc/nginx/conf.d/default.conf

# Copy static site
COPY index.html /usr/share/nginx/html/index.html

EXPOSE 8080

CMD ["nginx", "-g", "daemon off;"]
