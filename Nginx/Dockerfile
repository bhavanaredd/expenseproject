FROM nginx:latest

# Clean default HTML files
RUN rm -rf /usr/share/nginx/html/*

# ✅ Remove default config to avoid conflict
RUN rm -f /etc/nginx/conf.d/default.conf

# Copy frontend files and custom nginx config
COPY frontend /usr/share/nginx/html
COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
